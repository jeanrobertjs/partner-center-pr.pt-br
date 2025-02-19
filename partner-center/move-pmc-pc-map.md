---
title: Migração do PMC para o Partner Center | Partner Center
ms.topic: article
ms.date: 06/14/2019
description: Entenda as diferenças e semelhanças entre o PMC e o Partner Center
author: LauraBrenner
ms.author: labrenne
keywords: PMC, migração, mover para o Partner Center
ms.localizationpriority: medium
ms.openlocfilehash: b7cc7104d648eff3a5461d950345c283a307ea6c
ms.sourcegitcommit: 7b66b159e8fd37a30ddd7065881a83497aa433b0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2019
ms.locfileid: "70921472"
---
# <a name="moving-from-pmc-to-partner-center"></a>Migração do PMC para o Partner Center

Estamos tornando mais fácil para você fazer negócios conosco, introduzindo um único site (Partner Center) que serve como um ponto central de envolvimento. Você descobrirá que tudo o que fazia no PMC (Partner Membership Center) pode ser realizado em seu painel no Partner Center. 

Você também pode fazer muito mais, tudo sem sair de um único site da Web. No entanto, alguns dos recursos e a terminologia podem parecer diferentes. Para reduzir as preocupações iniciais sobre onde e quais são as coisas, certifique-se de fazer o Tour do site do seu painel.

Esta tabela apresenta algumas das diferenças entre o PMC e o Partner Center.

## <a name="renewing-your-microsoft-partner-network--membership"></a>Renovação da associação ao Microsoft Partner Network

|**PMC**   |**Partner Center**|
|----------------------|:-----------------------------|
|As renovações começaram 90 dias antes do aniversário e precisam ser concluídas até a data do aniversário| Os parceiros podem renovar a partir do dia após o aniversário e até 30 dias após o aniversário.|

## <a name="account-structure"></a>Estrutura da conta

|**PMC**   |**Partner Center**|
|----------------------|:-----------------------------|
|Sede mais localizações – cada uma avaliada separadamente. A avaliação de competências foi feita no nível local|Uma empresa global, sua PGA (conta global do parceiro), incluindo locais, avaliada como um todo; dados de desempenho e habilidades agregados no nível de PGA; inclui várias exibições de perfil para programas como Perfil de parceiro e perfil de negócios para referências e marketing. Para obter mais informações, veja [A estrutura de conta no Partner Center](https://docs.microsoft.com/partner-center/account-structure.md).|

## <a name="sign-in"></a>Entre

|**PMC**   |**Partner Center**|
|----------------------|:-----------------------------|
|Era possível usar suas credenciais de MSA (conta Microsoft) ou de conta pessoal (joe@outlook.com)|Você precisa usar suas credenciais de conta corporativa, (joe@joescompany.com). Para obter mais informações, confira [Sua conta corporativa e o Partner Center](https://docs.microsoft.com/partner-center/azure-active-directory-tenants-and-partner-center.md).|

## <a name="user-roles"></a>Funções de usuário

|**PMC**   |**Partner Center**|
|----------------------|:-----------------------------|
|Muitas funções no PMC não são usadas no Partner Center|O administrador que realiza a migração para o Partner Center recebe automaticamente as funções de Administrador do MPN, Administrador da Conta e Administrador de Referências. Em seguida, eles podem atribuir outros usuários a funções de usuário.|
|Os usuários eram gerenciados no nível de local|Os usuários são gerenciados no nível da empresa (PGA) em vez de no nível de local. A exceção é o Administrador de incentivos, que funciona no nível de local.|
|   |O Partner Center tem dois amplos conjuntos de funções: as funções que administram o locatário do Azure AD e as funções que administram os negócios da empresa. Organize as funções da maneira que faz sentido para sua empresa. Uma pessoa pode fazer tudo ou várias pessoas podem receber funções e permissões separadas. Para obter mais informações, confira [Atribuir funções e permissões de usuário](https://docs.microsoft.com/partner-center/permissions-overview). 

## <a name="how-competencies-and-benefits-are-accounted-for"></a>Como as competências e os benefícios são contabilizados

|**PMC**   |**Partner Center**|
|----------------------|:-----------------------------|
|Acumulado por local e administrado por local|Os benefícios são para toda a empresa, incluindo benefícios para a administração; no entanto, você pode gerenciar os benefícios da maneira mais adequada para a empresa |
|Podia ter outros ABTKs (kits de ferramentas de benefícios adicionais) até que eles foram desativados em outubro de 2018.|Sem ABTKs; um MAPS por empresa; uma competência prata por empresa; uma competência ouro por empresa|
||Contanto que ainda não tenha o MAPS, você pode comprá-lo. A propriedade do MAPS não está vinculada a competências.  
|Os benefícios foram acessados no PDD (Download Digital do Parceiro) |Todos os benefícios são acessados no Partner Center|
|Competências e benefícios espalhados e divididos entre vários locais|Suas competências e seus benefícios de todos os seus locais são consolidados no nível da empresa (PGA) e ficarão retidos até sua data de aniversário. Nesse momento, será necessário comprar ou renovar no nível da empresa. Desempenho e habilidades, bem como competências, são agregados globalmente|
|As declarações de comprovante do Software Assurance são feitas na ferramenta VRR (Voucher Validation and Redemption)|Agora você pode acessar e gerenciar os SAVTs (comprovantes de treinamento do Software Assurance) e/ou os DPSs (serviços de planejamento implantados) no Partner Center.  A ferramenta VVR herdada será desativada em 1º de outubro de 2019.  |

## <a name="associating-mcp-ids-to-partner-center"></a>Associar IDs do MCP ao Partner Center

|**PMC**   |**Partner Center**   |
|-------------------------|:-------------------|
|Você pode associar a mesma ID do MCP a várias empresas.| Somente uma ID do MCP pode ser associada a uma única conta do Partner Center. Você deve fazer a associação manualmente. No painel do Partner Center, selecione o ícone **Sua conta** no canto direito do painel e, em seguida, selecione **Meu perfil**. Em **Seu aprendizado**, será possível associar sua conta do Microsoft Learning e também conectar sua conta Microsoft à Partner University.

## <a name="visual-studio-benefits-and-msa"></a>Benefícios do Visual Studio e MSA

|**PMC**   |**Partner Center**   |
|-----------------|:-----------------|
|Alocação de benefícios do Visual Studio para o MSA|Os benefícios do Visual Studio alocados para o MSAs serão respeitados e mantidos.|
||As alocações do Visual Studio no MSA serão preservadas após a renovação no Partner Center.|
||No Partner Center, um parceiro pode adicionar contas corporativas e contas de usuário convidado que são MSA por meio do mesmo locatário em que o parceiro é administrador MPN no locatário do Azure AD. Se o parceiro for um administrador global em vários locatários do Azure AD e todos esses locatários estiverem associados à mesma conta do Partner Center, o parceiro poderá adicionar usuários em todos esses locatários aos benefícios do Visual Studio e às alocações baseadas em uso do Azure. Embora os usuários convidados possam receber assinaturas baseadas em uso do Visual Studio pelo administrador do MPN ou pelo administrador global, os usuários convidados não podem entrar no Partner Center usando as respectivas MSAs. No entanto, os usuários convidados podem entrar no Azure e no Visual Studio para validar e usar os respectivos benefícios atribuídos. |

## <a name="programs-now-located-and-managed-in-partner-center"></a>Programas agora localizados e gerenciados no Partner Center 

|**PMC**   |**Partner Center**|
|----------------------|:-----------------------------|
|PDD  |Benefícios|
|CHIP, ICP, PIE | Incentivos|
||Indicações|
|Insights do Parceiro| Análises|
|Ferramenta de Validação e Resgate de Comprovante| Ferramenta de Validação e Resgate de Comprovante|
|           |Programas de Provedor de Soluções na Nuvem|

Os benefícios do Visual Studio alocados para o MSAs serão respeitados e mantidos. Eles também serão preservados após a renovação no Partner Center. No entanto, se você remover uma alocação de MSA uma vez que ela já tenha sido migrada no Partner Center, ela não poderá ser adicionada novamente ao Partner Center.

No Partner Center, um parceiro pode adicionar contas corporativas e contas de usuário convidado, que são MSA, por meio do mesmo locatário em que o parceiro é administrador MPN no locatário do Azure AD. Se o parceiro for um administrador global em vários locatários do Azure AD e todos esses locatários estiverem associados à mesma conta do Partner Center, o parceiro poderá adicionar usuários em todos esses locatários aos benefícios do Visual Studio e às alocações baseadas em uso do Azure.

Embora os usuários convidados possam receber assinaturas baseadas em uso do Visual Studio pelo administrador do MPN ou pelo administrador global, os usuários convidados não podem entrar no Partner Center usando as respectivas MSAs. No entanto, os usuários convidados podem entrar no Azure e no Visual Studio para validar e usar os respectivos benefícios atribuídos.
