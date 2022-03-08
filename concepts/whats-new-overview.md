---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 79d281a04cf4ae1dc683efa93da394e59bdc9149
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333831"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Recursos, incluindo APIs e ferramentas, no status de _visualização_ podem mudar sem aviso prévio e alguns podem nunca ser promovidos ao status de disponibilidade geral (GA). Não utilize recursos de visualização em aplicativos de produção.


## <a name="february-2022-new-and-generally-available"></a>Janeiro de 2022: Novo e disponível ao público em geral

### <a name="teamwork"></a>Trabalho em equipe
Obtenha [detalhes sobre uma reunião online](/graph/api/resources/teamworkOnlineMeetingInfo) associada a um [chat](/graph/api/resources/chat) através da propriedade **onlineMeetingInfo**.

## <a name="february-2022-new-in-preview-only"></a>Fevereiro de 2022: novo somente para visualização

### <a name="change-notifications"></a>Notificações de alteração
Assine para alterações de contatos, eventos ou mensagens do Outlook e receba notificações que incluem dados de recursos na carga. Para obter mais informações, confira [Alterar notificações para recursos do Outlook no Microsoft Graph](outlook-change-notifications-overview.md).

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
Use as permissões de aplicativo `CustomSecAttributeAssignment.Read.All` para ler [definições de atributo de segurança personalizadas](/graph/api/resources/customsecurityattributedefinition?view=graph-rest-beta&preserve-view=true) para uma organização sem um usuário conectado.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- Defina as [configurações](/graph/api/resources/accessreviewstagesettings?view=graph-rest-beta&preserve-view=true) para cada [estágio](/graph/api/resources/accessreviewstage?view=graph-rest-beta&preserve-view=true) em uma revisão de acesso em vários estágios. Além de [obter](/graph/api/accessreviewstage-get?view=graph-rest-beta&preserve-view=true) ou [atualizar](/graph/api/accessreviewstage-update?view=graph-rest-beta&preserve-view=true) um estágio de revisão de acesso, você pode fazer o seguinte: 
  - [Interrompa](/graph/api/accessreviewstage-stop?view=graph-rest-beta&preserve-view=true) os revisores de dar mais entrada a um estágio e prossiga para o próximo estágio, se aplicável. 
  - [Filtre](/graph/api/accessreviewstage-filterbycurrentuser?view=graph-rest-beta&preserve-view=true) e obtenha todos os estágios em uma [instância de revisão de acesso](/graph/api/resources/accessreviewinstance?view=graph-rest-beta&preserve-view=true) para a qual o usuário da chamada é um revisor
  - [Liste decisões](/graph/api/accessreviewstage-list-decisions?view=graph-rest-beta&preserve-view=true) de uma revisão de acesso em vários estágios.
- Os aplicativos podem usar a permissão de aplicativo `EntitlementManagement.ReadWrite.All` para [criar uma solicitação de recurso do pacote de acesso](/graph/api/entitlementmanagement-post-accesspackageresourcerequests?view=graph-rest-beta&preserve-view=true) para adicionar ou remover um recurso de um [catálogo de pacotes de acesso](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
- Use uma série de novas propriedades para configurar a [identidade visual de uma organização](/graph/api/resources/organizationalbrandingproperties?view=graph-rest-beta&preserve-view=true). Por exemplo, uma versão de banner do logotipo da empresa para a página de entrada, um favicon personalizado com URL baseado em CDN e algumas outras propriedades personalizadas para que os usuários gerenciem contas.
- Inclua ou exclua o Linux como uma das [condições da plataforma](/graph/api/resources/conditionalaccessplatforms?view=graph-rest-beta&preserve-view=true) em uma [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- Identifique [entidades de serviço em risco](/graph/api/resources/riskyserviceprincipal?view=graph-rest-beta&preserve-view=true) de uma organização com o Azure AD, que continuamente [detecta e avalia os riscos](/graph/api/resources/serviceprincipalriskdetection?view=graph-rest-beta&preserve-view=true) com base em vários sinais e aprendizado de máquina. Você pode [confirmar](/graph/api/riskyserviceprincipal-confirmcompromised?view=graph-rest-beta&preserve-view=true) se uma entidade de serviço em risco está realmente comprometida, na qual a Microsoft desabilitará esse objeto de entidade do serviço. Você pode [descartar](/graph/api/riskyserviceprincipal-dismiss?view=graph-rest-beta&preserve-view=true) o risco de uma entidade de serviço em risco. E você pode [listar o histórico de risco](/graph/api/riskyserviceprincipal-list-history?view=graph-rest-beta&preserve-view=true) de uma entidade de serviço.
- Use [configurações de acesso entre locatários](/graph/api/resources/crosstenantaccesspolicy-overview?view=graph-rest-beta&preserve-view=true) para controlar e gerenciar a colaboração entre usuários de sua organização e de outras organizações. Eles são granulares para permitir que você determine os usuários, grupos e aplicativos, tanto da sua organização quanto de organizações externas, que podem participar da colaboração do Azure AD B2B e da conexão direta do Azure AD B2B. 
- Habilite ou desabilite usuários e grupos em uma organização para usar o [CBA (autenticação baseada em certificado) nativo do Azure AD](/graph/api/resources/x509CertificateAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true).

## <a name="january-2022-new-and-generally-available"></a>Janeiro de 2022: Novo e disponível ao público em geral

### <a name="devices-and-apps--service-health-and-communications"></a>Dispositivos e aplicativos | Integridade do serviço e comunicações
Obtenha um [anexo de anúncio de serviço](/graph/api/resources/serviceAnnouncementAttachment) a uma [mensagem de atualização de serviço](/graph/api/resources/serviceupdatemessage).

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- Obtenha uma coleção de recursos de [revisão de acesso](/graph/api/resources/accessreviewreviewer) que é usada para definir revisores contatados para uma [instância de revisores de acesso](/graph/api/resources/accessReviewInstance).
- Diferencie 3 tipos de recursos cujo acesso é representado por meio de uma [decisão de revisão de acesso](/graph/api/resources/accessreviewinstancedecisionitem):
  - Uma [política de atribuição de pacote de acesso](/graph/api/resources/accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource) para a qual o acesso é determinado por uma decisão de revisão de acesso.
  - Uma [função de recurso do Azure](/graph/api/resources/accessReviewInstanceDecisionItemAzureRoleResource) para a qual o acesso é determinado por uma decisão de revisão de acesso.
  - Uma [entidade de serviço](/graph/api/resources/accessReviewInstanceDecisionItemServicePrincipalResource) cujo acesso a um recurso é determinado por uma decisão de revisão de acesso.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
Imponha um [controle de sessão](/graph/api/resources/conditionalAccessSessionControls) (definindo a propriedade **disableResilienceDefaults**) para determinar se o Microsoft Azure AD deve estender as sessões existentes com base nas informações coletadas antes de uma interrupção.

### <a name="teamwork"></a>Trabalho em equipe
[Criar um chat](/graph/api/chat-post) usando as permissões do aplicativo.

## <a name="january-2022-new-in-preview-only"></a>Janeiro de 2022: Novo somente na pré-visualização

### <a name="compliance--ediscovery"></a>Conformidade | Descoberta eletrônica
Obtenha a URL do site OneDrive for Business de um custodiante (propriedade **siteWebUrl** de [userSource](/graph/api/resources/ediscovery-userSource?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
- Obtenha ou atualize as [configurações de uma organização](/graph/api/resources/cloudpcorganizationsettings?view=graph-rest-beta&preserve-view=true), que incluem a versão do sistema operacional Windows para provisionar em PCs na nuvem e o tipo de conta de usuário nos PCs na nuvem provisionados.
- [Altere o tipo de conta de usuário](/graph/api/cloudPC-changeUserAccountType?view=graph-rest-beta&preserve-view=true) em um PC na nuvem especificado.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- Os revisores de uma revisão de acesso podem [registrar](/graph/api/accessreviewinstancedecisionitem-recordalldecisions?view=graph-rest-beta&preserve-view=true) as decisões para as quais o usuário atual é o revisor.
- Configure [a data e hora do último login de um usuário como um insight](/graph/api/resources/userLastSignInRecommendationInsightSetting?view=graph-rest-beta&preserve-view=true) para ajudar os revisores na tomada de decisões para uma [definição de cronograma de revisão de acesso](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true).
- Configure [a data e hora da última entrada de um usuário como um insight](/graph/api/resources/userSignInInsight?view=graph-rest-beta&preserve-view=true) para uma [decisão sobre o acesso de um usuário ou entidade de segurança em uma instância de uma revisão de acesso](/graph/api/resources/accessreviewinstancedecisionitem?view=graph-rest-beta&preserve-view=true).
- O solicitante de um pacote de acesso pode fornecer informações personalizadas como parte de um [recurso de pacote de acesso](/graph/api/resources/accesspackageresource?view=graph-rest-beta&preserve-view=true) que pode ser usado para tomar decisões de aprovação do pacote de acesso.
- Um solicitante pode editar a resposta para a uma [pergunta](/graph/api/resources/accessPackageQuestion?view=graph-rest-beta&preserve-view=true) em uma [política de atribuição de pacote de acesso](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true).

### <a name="reports--identity-and-access-reports"></a>Relatórios | Relatórios de identidade e acesso
- Obtenha detalhes dos [métodos de autenticação registrados para um usuário](/graph/api/resources/userRegistrationDetails?view=graph-rest-beta&preserve-view=true), como autenticação multifator, redefinição de senha de autoatendimento e autenticação sem senha.
- Obtenha as seguintes propriedades para um evento de [entrada](/graph/api/resources/signIn?view=graph-rest-beta&preserve-view=true) de um usuário ou aplicativo em uma organização: 
  - Qualquer contexto de autenticação de [acesso condicional](/graph/api/resources/authenticationContext?view=graph-rest-beta&preserve-view=true).
  - Qualquer [política de duração da sessão](/graph/api/resources/sessionLifetimePolicy?view=graph-rest-beta&preserve-view=true) de acesso condicional.
  - A ID de um recurso do Azure acessada durante a entrada.
  - O identificador da credencial de identidade federada de um aplicativo, caso tenha sido usado para entrar.
  - O identificador da entidade de serviço que representa o recurso de destino no evento de entrada.

### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
Obtenha relatórios de uso do Outlook, OneDrive e SharePoint para o Microsoft Cloud for US Government. Confira o resumo sobre [implantações na nuvem](/graph/api/resources/report?view=graph-rest-beta&preserve-view=true#cloud-deployments).

### <a name="sites-and-lists"></a>Sites e listas
- Adicione ou sincronize um tipo de conteúdo do hub de tipo de conteúdo para um [site](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) ou [lista](/graph/api/resources/list?view=graph-rest-beta&preserve-view=true), usando a ação [addCopyFromContentTypeHub](/graph/api/contenttype-addcopyfromcontenttypehub?view=graph-rest-beta&preserve-view=true). Isso torna um tipo de conteúdo ou sua atualização disponível para um site ou lista específica onde é necessário. Essa é uma melhoria da infraestrutura de sincronização herdada que envia o tipo de conteúdo para todos os sites de uma organização, reduzindo os tempos de espera para a propagação da publicação. 
- Obtenha uma ou mais [operações avançadas e de longa duração](/graph/api/resources/richlongrunningoperation?view=graph-rest-beta&preserve-view=true) ocorrendo em um site ou lista, o que pode acontecer ao adicionar um tipo de conteúdo de forma síncrona.
- Obtenha uma coleção de recursos de [tipo de conteúdo](/graph/api/resources/contentType?view=graph-rest-beta&preserve-view=true) do hub de tipo de conteúdo que são compatíveis usando a ação [getCompatibleHubContentTypes](/graph/api/contenttype-getcompatiblehubcontenttypes?view=graph-rest-beta&preserve-view=true). 

### <a name="teamwork"></a>Trabalho em equipe
- Permita que os usuários escolham **LastModifiedDateTime** ou **CreatedDateTime** como a ordem de classificação ao [listar mensagens em um chat](/graph/api/chat-list-messages?view=graph-rest-beta&preserve-view=true).
- Especifique a atribuição do usuário (na propriedade **onBehalfOf**) quando um bot envia uma [mensagem de chat](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) em nome de um usuário.
- Adicione os seguintes tipos de membros a um [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true):
  - [Convidado anônimo](/graph/api/resources/anonymousGuestConversationMember?view=graph-rest-beta&preserve-view=true)
  - [Usuário da conta Microsoft](/graph/api/resources/microsoftAccountUserConversationMember?view=graph-rest-beta&preserve-view=true)
  - [Usuário do Skype for Business](/graph/api/resources/skypeForBusinessUserConversationMember?view=graph-rest-beta&preserve-view=true)
  - [Skype usuário](/graph/api/resources/skypeUserConversationMember?view=graph-rest-beta&preserve-view=true)
- Use a permissão delegada `TeamworkTag.Read` para ler [marcas](/graph/api/resources/teamworktag?view=graph-rest-beta&preserve-view=true) e [membros de marcas](/graph/api/resources/teamworktagmember?view=graph-rest-beta&preserve-view=true) no Teams, em nome do usuário conectado.

## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote nos novos recursos na [Comunidade Microsoft Tech](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de **_visualização_**. Todas as atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de **_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/office/dev-program), ganhe uma assinatura gratuita do Microsoft 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](https://developer.microsoft.com/graph/changelog/).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).
