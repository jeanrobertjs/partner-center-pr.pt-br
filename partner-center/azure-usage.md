---
title: Microsoft Azure o dimensionamento da VM para uso máximo de reserva | Centro de parceiros
ms.topic: article
ms.date: 08/05/2019
Description: Ao comprar reservas do Microsoft Azure em nome dos seus clientes, você precisará escolher uma máquina virtual (VM) dimensionada para atender às necessidades de computação do cliente.
author: LauraBrenner
ms.author: labrenne
keywords: azure, reservas, vm, gerenciar, uso, dimensionamento
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 1c1c0170c5efd8abf2e1afb7bb6ef1dfac2b7e5b
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820197"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Dimensionamento de VM do Microsoft Azure para uso máximo de reserva do Azure

**Aplica-se a**

- Partner Center
- Portal do Azure
- Parceiros no CSP

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Determinar o tamanho da VM para reserva do Azure do cliente 

Ao comprar reservas do Microsoft Azure em nome dos seus clientes, você precisará escolher uma máquina virtual (VM) dimensionada para atender às necessidades de computação do cliente. Você pode encontrar essas informações usando um destes métodos:

- API de utilização do Azure
- O portal do Azure
- Azure PowerShell
- A API do Azure Resource Manager (ARM)

As instruções para o uso de cada um desses métodos estão listadas a seguir. Depois que você comprar uma reserva, o desconto da reserva será aplicado automaticamente em máquinas virtuais que correspondam aos atributos e à quantidade da reserva. Você não precisa atribuir a reserva a uma VM.

>[!NOTE]
>Os descontos da reserva não se aplicam a VMs clássicas ou promocionais.

>[!IMPORTANT]
>Para identificar o tipo e o tamanho da VM a ser comprada em nome de seu cliente, você deverá usar um dos métodos descritos abaixo já que o tipo de série de VM não é exibido corretamente nos arquivos de reconciliação do Partner Center.

**Obter informações de dimensionamento de VM usando a API de utilização do Azure**

1. Use o valor do atributo ServiceType desde additionalInfo na resposta da API para identificar o tamanho da VM a ser comprada.
2. Para obter mais informações, consulte [Obter registros de utilização de um cliente do Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) na [API do Partner Center](https://docs.microsoft.com/partner-center/develop/).

**Obter informações de dimensionamento de VM usando o portal do Microsoft Azure**

1. No Partner Center, vá para a página de seus **clientes** .
2. Encontre o cliente que deseja comprar reservas de VM do Azure e então selecione a seta para baixo para expandir as informações do cliente. Selecione **Portal de Gerenciamento do Microsoft Azure** para abrir o registro do cliente no portal do Azure.
3. Selecione **Máquinas virtuais** no menu do portal e então selecione a VM para a qual você deseja comprar uma reserva.
4. Na página de detalhes da VM, encontre as informações de tamanho e região, como ilustrado abaixo, e use essas informações para comprar a reserva no Partner Center.  

    ![Informações de tamanho e região na página de detalhes](images/usage1.png)

**Obter informações de dimensionamento de VM usando Microsoft Azure PowerShell**

Use as informações na imagem abaixo para obter a localização e o tamanho da VM para a qual você deseja comprar uma reserva. 

![Local e tamanho da VM](images/usage2.png)

**Obter informações de dimensionamento de VM usando a API de Azure Resource Manager (ARM)**

1. Usando o ARMClient ou as APIs ARM, chame o cliente ARM para a VM para a qual você deseja comprar uma reserva.

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. A chamada retorna os valores de **vmSize** e **location**, como ilustrado abaixo.

    ![valor de](images/usage3.png) local do valor ![de vmSize](images/usage4.png)

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Verificar o desconto de uso e de reserva de VM do Azure

Depois de você comprar uma Instância de VM Reservada do Azure em nome de um cliente, o desconto para pagamento antecipado pelo espaço de VM será automaticamente aplicado às máquinas virtuais que correspondem aos atributos e à quantidade de reservas do cliente.

Você pode verificar o uso de reservas do cliente e ver para quais máquinas virtuais os descontos de reserva são aplicados usando um dos seguintes métodos:

- O portal do Azure
- API de utilização do Azure

As instruções para o uso de cada um desses métodos estão listadas a seguir.

>[!NOTE]
>Somente a API de utilização do Azure mostra a qual máquina virtual o desconto está sendo aplicado.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Verificar o uso de reserva do cliente no portal do Microsoft Azure

1. No Partner Center, vá para a página de seus **clientes** .

2. Encontre o cliente cujo desconto e uso de reserva você deseja verificar e então selecione a seta para baixo para expandir as informações do cliente. Selecione **Portal de Gerenciamento do Microsoft Azure** para abrir o registro do cliente no portal do Azure.
3. Selecione **Reservas** no menu do portal e então selecione a reserva cujo uso você deseja verificar.
4. Na página **Visão geral**, verifique o gráfico de utilização da reserva, que mostra o quanto da reserva foi aplicado às máquinas virtuais.

    >[!NOTE]
    >Os dados de utilização podem ser atrasados em até 8 horas.

    a. Se a utilização da reserva for de 100%, o cliente estará recebendo toda a economia possível que a compra de reserva pode fornecer.
    b. Se o uso da reserva for 0%, o desconto não estará sendo aplicado a nenhuma máquina virtual.
    c. Se o uso da reserva estiver entre 1% e 99%, há benefícios não utilizados.

5. Para evitar essa situação, determine a VM de tamanho correto para dar suporte às necessidades de computação do cliente antes de fazer a compra.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Verificar o uso de reserva do cliente com a API de utilização do Azure

>[!NOTE]
>Somente a API de utilização do Azure mostra a qual máquina virtual o desconto está sendo aplicado.  

Você pode obter dados de uso da reserva com a API de utilização do Azure para verificar se o cliente está recebendo o desconto da reserva e para ver a quais VMs (máquinas virtuais) o desconto é aplicado. Compare o Exemplo A ao Exemplo B para saber como verificar o uso da reserva de um cliente.

![Exemplos de uso de reserva](images/usage5.png)

- A reservationId identifica a reserva do Azure que foi usada para aplicar o desconto à VM.
- consumptionMeter é a MeterId para a VM que tem o desconto da reserva aplicado a ela.
- O ReservationMeter mostra o custo de US$ 0 desde que o desconto da reserva foi aplicado.

Para obter mais informações, consulte [Obter registros de utilização de um cliente do Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) na [API do Partner Center](https://docs.microsoft.com/partner-center/develop/).

>[!IMPORTANT]
>Os custos de software, como o Microsoft Windows Server, não estão incluídos no preço de uma reserva de VM e aparecerão como itens de linha separados no registro do pedido e em sua fatura. No entanto, se um cliente tiver o Benefício de Uso Híbrido do Azure, os custos de software não serão aplicados. Para obter mais informações, consulte [Custos de software do Windows não incluídos com Instâncias Reservadas](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Recursos de reservas do Azure

|**Para obter informações sobre**   |**Leia este**    |
|:-----------------------------|:-----------------|
|Reservas do Azure na visão geral do CSP  | [Vender Microsoft Azure instâncias de VM reservadas](azure-reservations.md)
|Comprando reservas do Azure para seus clientes no Partner Center   |[Comprar reservas do Azure](azure-reservations-buying.md)
|Gerenciando reservas do Azure no Partner Center | [Gerenciando reservas do Azure no Partner Center](azure-reservations-manage.md)
|Como comprar reservas do Azure no portal do Azure | [Pagar antecipadamente por máquinas virtuais com Instâncias de VM Reservadas do Azure](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) na Ajuda do Azure |
|Como gerenciar reservas do Azure no portal do Azure   |[Gerenciar instâncias de VM reservadas](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) na Ajuda do Azure  |
|Como comprar reservas do Azure usando a API do Partner Center | [Comprar Instâncias de VM Reservadas do Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) na documentação do desenvolvedor do Partner Center
