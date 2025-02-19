---
title: Consolidação de locatários de autorização regional do CSP | Partner Center
ms.topic: article
ms.date: 03/15/2019
description: Use estas instruções para consolidar locatários para países/regiões diferentes.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.author: evansma
keywords: migrar provedores, provisionamento, conta de locatário, consolidar locatários
ms.localizationpriority: medium
robots: noindex,nofollow
ms.openlocfilehash: 5e83b9720393356268f59d42b4210c427a3b3bc6
ms.sourcegitcommit: 5e67a2540b0ff9eb248e5dc41b9d9ad1fc900b36
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2019
ms.locfileid: "66819940"
---
# <a name="csp-regional-authorization-tenant-consolidation"></a>Consolidação de locatários de autorização regional do CSP

**Aplica-se a**

-  Partner Center
-  Partner Center para Microsoft Cloud for US Government


\[Algumas informações se relacionam ao produto de pré-lançamento que pode ser substancialmente modificado antes do lançamento comercial. Microsoft não oferece garantias, expressas ou implícitas, quanto às informações fornecidas aqui.\]

Use estas instruções para consolidar locatários para países/regiões diferentes.

**Observação**  Você deve estar ciente de todas as assinaturas e números de estações para seus clientes provisionados nas contas de transição. Você reprovisionará exatamente as mesmas assinaturas com o mesmo número de estações sob a nova conta de CSP Central como parte do processo de migração. Use o recurso de lista de exportação para ajudar a criar uma lista de clientes para mover para o locatário centralizado. Os parceiros optam por consolidar seus locatários. Quando consolidação for concluída, os parceiros não poderão reverter para seu estado anterior. Observe que a ação do cliente talvez seja necessária.



## <a name="prepare-for-migration"></a>Preparar para a migração


-   Entrar no seu **Partner Center** com o **a transição** (existente) conta (o farão a transição) e take anotação de todos os clientes e todos os serviços provisionados para os clientes.

![lista de clientes regionais](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a>Migrar contas de clientes


1.  Entrar no seu **Partner Center** com o **a transição** (novo) conta (aquele estão fazendo a transição para) e navegue até a lista de clientes da **clientes**.

2.  Selecione Clientes.

3.  Clique em **Solicitar uma relação de revendedor**. Será exibida uma mensagem de email padrão para apresentar aos seus clientes. Essa mensagem contém uma URL com a ID da organização exclusiva para sua nova conta do Partner Center.

4.  **Ação do cliente:** Certifique-se de que cada um dos clientes ativos que você deseja migrar visita esta URL. Ao abrir a URL, o cliente será solicitado a entrar no portal do Office 365. O cliente entra usando a mesma ID da organização que ele usa para acessar os portais de administrador do Azure e do Office 365.

5.  Ao entrar, o Administrador Global da conta do cliente será solicitado a enviar um contrato para conceder privilégios de administrador delegado à nova conta CSP. Se concordar, o cliente marca a caixa de seleção e concorda em autorizar o relacionamento.

Os clientes aparecerão na lista de clientes do parceiro após o envio do contrato, um por um.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrando assinaturas baseadas em uso do Office 365 e não Azure


1.  Depois que o cliente assinar o contrato, você poderá recriar as assinaturas dele em seu locatário parceiro centralizado.

2.  Dos **Partner Center** selecionar **clientes**.

3.  Abra o nome da empresa do cliente que você deseja migrar.

4.  Clique em **Adicionar assinatura**.

5.  Adicione as assinaturas corretas e os números de estações do catálogo. Verificar com as informações fornecidas nas contas de parceiro de **origem da transição**.

![lista de clientes](images/regionalcustomer2.png)

6.  Clique em **Enviar**.

Agora os serviços serão fornecidos para o cliente da conta de parceiro de **destino da transição**.

Repita essas etapas para migrar assinaturas para todos os outros clientes.

Antes de prosseguir para a próxima seção, certifique-se de que todas as assinaturas de cliente existentes nas contas de parceiros de **origem da transição** sejam reprovisionadas sob a conta de parceiro de **destino da transição**.

**Observação**  Os parceiros devem suspender as assinaturas na conta de locatário parceiro de **origem da transição** no Partner Center no mesmo dia que essas assinaturas são transmitidas e configuradas na conta de locatário parceiro de **destino da transição** no Partner Center para garantir que não haja cobrança dupla. As solicitações de suporte serão negadas para créditos decorrentes de alguma sobreposição de cobranças que ocorra devido à não configuração das assinaturas de **origem da transição** como desabilitadas.



## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Desabilitando as assinaturas do Office 365 na conta de parceiro de origem da transição


Desabilitar a assinatura de CSP sob as contas de parceiros de **destino da transição** impede qualquer cobrança futura. Você não precisa desabilitar manualmente as assinaturas do Azure, elas são desativadas automaticamente durante o processo de migração.

1.  Entrar para o **Partner Center** com o **fazendo a transição do** CSP de conta e navegue até a lista de clientes.

2.  Abra o cliente com assinaturas para desabilitar e, em seguida, selecione a primeira oferta a ser desabilitada.
3.  Defina a assinatura como **suspensa** e clique em **enviar**.

 >[! **Observação**] suspendendo a assinatura garante a cobrança dupla não ocorrerá.



~~~
The Subscription shows **suspended** on the subscriptions list.
~~~

4.  Repita essas etapas para todas as assinaturas sob o cliente. Verifique se todas são exibidas como **suspensas**.

5.  Selecione o próximo cliente na lista e repita o processo para desabilitar todas as assinaturas.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrando assinaturas baseadas em uso do Azure


Observe que assinaturas de CSP baseadas em uso do Azure não precisam ser migradas manualmente como no caso das assinaturas de CSP do Office 365. O suporte do Microsoft Azure pode migrar as assinaturas do Azure, bem como todos os serviços ou recursos implantados, das contas de revendedor CSP de **origem da transição** para a conta de revendedor CSP de **destino da transição**. Não haverá qualquer interrupção do serviço para o cliente durante a transição.

1.  Certifique-se de que as contas de clientes que precisam de assinaturas do Azure migradas aceitem o contrato para serem associadas à nova conta CSP de **destino da transição**.
2.  Os parceiros notificam a Microsoft quais contas de clientes que têm assinaturas do Azure estão prontas para migrar, fornecendo também os nomes de empresa do cliente.
3.  A Microsoft migra as assinaturas baseadas em uso do Azure e notifica o parceiro quando a migração é concluída.
4.  O parceiro confirma se agora a assinatura do Azure sob a conta de revendedor CSP de **origem da transição** é exibida como suspensa no Partner Center, na seção de assinaturas de cliente.
5.  O parceiro confirma se agora a assinatura do Azure sob a conta de revendedor CSP de **destino da transição** mostra o status de **ativa** no Partner Center, na seção de assinaturas de cliente.

>[! **Observação**] desabilitar as assinaturas em que o cliente não altera a aparência do cliente na lista de clientes. Atualmente, não há uma opção para remover clientes da lista. Os parceiros devem evitar readicionar assinaturas para esses clientes a partir da conta de **destino da transição** no futuro.



6.  Repita essas etapas para todas as assinaturas em todos os seus clientes para impedir encargos futuros nas contas de **origem da transição**. O parceiro receberá uma fatura final com um crédito pelo número de dias não utilizados entre o dia de cancelamento e o último dia do período de cobrança. Nenhuma fatura futura será gerada após esse período de cobrança final.

### <a name="notes"></a>Observações

-   Desabilitar a assinatura da conta CSP de **origem da transição** não afeta o serviço do cliente final contanto que o serviço tenha sido provisionado pela conta CSP de **destino da transição** antes de desabilitar.

-   A assinaturas não podem ser usadas pelo cliente e não geram encargos quando são suspensas ou canceladas.

-   Atualmente, não há uma maneira de remover completamente um cliente da Lista de clientes.

-   **Observação**  Os parceiros devem suspender as assinaturas na conta de locatário parceiro de **origem da transição** no Partner Center no mesmo dia que essas assinaturas são transmitidas e configuradas na conta de locatário parceiro de **destino da transição** no Partner Center para garantir que não haja cobrança dupla. A Microsoft não dará suporte para solicitações de créditos decorrentes de alguma sobreposição de cobranças que ocorra devido à não configuração das assinaturas de **origem da transição** como suspensas.



### <a name="simplify-migration-using-export"></a>Simplificar a migração usando Exportar

Usando a **função Exportar**, você pode capturar as assinaturas que serão usadas em sua nova estrutura consolidada:

1.  Clique em **clientes** no Partner Center para ver a lista de clientes em sua estrutura existente.

2.  Abra o nome do cliente desejado.

3.  Na página **Assinaturas**, clique em **Exportar Assinaturas** para exportar os detalhes das assinaturas para um arquivo do Excel.

4.  Use essa lista para recriar as assinaturas em seu novo locatário consolidado.

### <a name="api-registration"></a>Registro de API

Para obter mais informações sobre o registro de API [consulte esta página](https://go.microsoft.com/fwlink/?linkid=847990).








