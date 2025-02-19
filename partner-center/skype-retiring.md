---
title: Migrar as assinaturas do Skype for Business Online Plano 1 para versões mais recentes do Office 365 | Partner Center
ms.topic: article
ms.date: 03/15/2019
Description: A transição de clientes com o Skype prestes a expirar para assinaturas de negócios Online plano 1 para uma opção de SKU com suporte. É recomendável mover os clientes para novas assinaturas antes da data de término da assinatura anual.
author: LauraBrenner
ms.author: labrenne
keywords: Planos do Skype for Business, Skype desativado, Office 365
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e71e6b05b5ea489b2b6b486f388f5c575dfd02c5
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62133906"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migrar assinaturas do Skype for Business Online Plano 1 para versões mais novas do Office 365

**Aplica-se a**

- Partner Center

O Skype for Business Online Plano 1 será desativado a partir de 1º de agosto de 2018. Após essa data, os clientes não poderão mais adquirir novas assinaturas do Skype for Business Plano 1. As assinaturas existentes não serão renovadas automaticamente quando expirarem, e não haverá uma opção de renovação. Na página de detalhes da assinatura, o status da assinatura do Skype for Business Online Plano 1 foi alterado para "Expira em [data]" de "Renovação automática em [data]".  

Para garantir a continuidade dos clientes, você deve fazer a transição de clientes com assinaturas do Skype for Business Online Plano 1 que vão expirar para uma opção de SKU com suporte, listada abaixo. É recomendável mover os clientes para as novas assinaturas antes da data de término da assinatura anual, para evitar possíveis interrupções de serviço. 

>[!NOTE]
>As SKUs do Skype for Business Online Plano 1 comerciais e governamentais estão sendo desativadas.

Se você usar a API (CREST ou Partner Center), encontre as assinaturas que vão expirar avaliando a data de término da assinatura juntamente com a propriedade de renovação automática = Falso. As assinaturas do Skype for Business Online Plano 1 serão definidas como renovação automática=Falso em 1º de setembro de 2018. Você pode mover os clientes para um novo plano a qualquer momento. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Planos de substituição do Skype for Business Online Plano 1

Com os novos planos, seus os clientes podem aproveitar novos recursos e funcionalidades no Office 365. Detalhes de preço são encontrados na lista de preços e oferecem a matriz de lista no Partner Center. 

- Opção 1: Office 365 Enterprise F1
- Opção 2: Microsoft 365 Enterprise F1
- Opção 3: Outros planos do Office 365

|**Recurso**    |**Opção 1**   |**Opção 2**   |**Opção 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Obtenha todos os recursos incluídos no Skype for Business Online Plano 1|Sim   |Sim   |Sim   |
|Mensagens Instantâneas e presença |Sim   |Sim   |Sim   |
|Áudio e vídeo ponto a ponto sobre IP|Sim   |Sim   |Sim   
|Participar de reuniões como um usuário autenticado| Sim   |Sim   |Sim   |

## <a name="transition-customers-to-new-product-plans"></a>Transição dos clientes para novos planos do produto

A Microsoft oferece continuamente novos produtos e serviços para nossos parceiros. Nesses casos, você pode precisar fazer o upgrade dos clientes para novos serviços ou migrar as assinaturas de SKUs que serão encerradas em breve. A migração dos clientes de SKUs desativadas para as mais recentes requer as seguintes etapas:

- Comprar a nova assinatura
- Reatribuir as licenças de usuário atuais
- Cancelar a assinatura antiga

### <a name="migrate-your-customers-to-new-plans"></a>Migrar seus clientes para novos planos

1. Para adquirir a nova assinatura, do **menu do Partner Center**, selecione **clientes**, selecione o cliente que você deseja mover e, em seguida, selecione **adicionar assinaturas**.

2. Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**. 

Agora seu cliente deve ter assinaturas antigas e novas: a assinatura antiga do Skype for Business Online Plano 1 e a nova "de destino", por exemplo, Opção 1 - Office 365 Enterprise F1.

3. Para reatribuir as licenças de usuários do cliente, do **Partner Center** menu, selecione **clientes**, selecione o cliente estiver movendo e, em seguida, selecione **usuários e licenças** . A página Usuários e Licenças do cliente será aberta.

4. Para reatribuir a licença do usuário, selecione o usuário a ser reatribuído e selecione **Gerenciar licenças**.

5. Na página **Gerenciar licenças**, desmarque a caixa de seleção da licença do Skype for Business Online Plano 1 e selecione um novo plano de serviço para a assinatura para a qual o cliente está mudando.

6. Selecione **Enviar**. Uma página de confirmação lista as novas atribuições de licença. Continue esse mesmo processo para outros usuários que precisam de atribuições de licença.

Depois de migrar a licença do usuário para o novo serviço, você pode cancelar com segurança a assinatura desativada no nível do cliente.

7. Dos **Partner Center** menu, selecione **clientes**. Selecione o cliente cuja assinatura você está cancelando.

8. Na página de detalhe da assinatura, defina o status da assinatura como **Suspensa**.

9. Selecione **Enviar**.

A assinatura antiga será suspensa e a nova assinatura será ativada. A assinatura suspensa será desprovisionada automaticamente após 120 dias. O cliente não pagará custos adicionais pela assinatura antiga.

