---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 30119dbd92c3a1b8552f19857225d868d50dd03b
ms.sourcegitcommit: 0ae140eafaca2dddc4584930cc0ac27fb1731c61
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2022
ms.locfileid: "65017110"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Recursos, incluindo APIs e ferramentas, no status de _visualização_ podem mudar sem aviso prévio e alguns podem nunca ser promovidos ao status de disponibilidade geral (GA). Não utilize recursos de visualização em aplicativos de produção.


## <a name="march-2022-new-and-generally-available"></a>Março de 2022: Novo e disponível para o público geral

### <a name="files"></a>Arquivos
Use um [pacote](/graph/api/resources/bundle) para compartilhar vários arquivos ao mesmo tempo, assim como outros recursos [driveItem](/graph/api/resources/driveitem). Você pode aplicar operações CRUD em um pacote e [adicionar](/graph/api/bundle-additem) um item ou [remover](/graph/api/bundle-removeitem) um item de um pacote.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
Use a [permissão específica de recurso](/graph/api/resources/resourcespecificpermission) para autorizar um aplicativo do Teams a acessar diretamente os dados de uma instância específica de um chat ou equipe. Por exemplo, a permissão específica do recurso ChannelMessage.Read.Group permite que um aplicativo do Teams leia as mensagens de canal de uma única equipe.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
[Obter](/graph/api/approval-get)decisões de [aprovação](/graph/api/resources/approval) associadas a uma [solicitação de atribuição de pacote de acesso](/graph/api/resources/accesspackageassignmentrequest).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
Especifique a [inclusão ou exclusão de aplicativos cliente](/graph/api/resources/conditionalaccessclientapplications) como um [conjunto de condições](/graph/api/resources/conditionalAccessConditionSet) para aplicar uma [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy).


## <a name="march-2022-new-in-preview-only"></a>Março de 2022: novo somente para visualização

### <a name="cloud-communications--online-meeting"></a>Comunicações na nuvem | Reunião online
Especifique um ou [participantes da reunião](/graph/api/resources/meetingParticipants?view=graph-rest-beta&preserve-view=true) como co-organizador.

### <a name="device-and-app-management--cloud-pc"></a>Gerenciamento de dispositivos e aplicativos | PC na nuvem
- Use permissões delegadas ou de aplicativo de `RoleManagement.Read.CloudPC` para as operações de leitura do recurso [unifiedRoleDefinition](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true).
- Use permissões delegadas ou de aplicativo de `RoleManagement.ReadWrite.CloudPC` para as operações de leitura e gravação do recurso [unifiedRoleDefinition](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true).
- Especifique a ID e o nome de exibição de uma assinatura do Azure como parte das informações de uma [imagem de origem de um dispositivo](/graph/api/resources/cloudPcSourceDeviceImage?view=graph-rest-beta&preserve-view=true).
- Especifique [configurações do Windows](/graph/api/resources/cloudpcwindowssettings?view=graph-rest-beta&preserve-view=true) para definir ao criar PCs na nuvem para uma [política de provisionamento](/graph/api/resources/cloudPcProvisioningPolicy?view=graph-rest-beta&preserve-view=true).

### <a name="device-and-app-management--corporate-management"></a>Gerenciamento de dispositivos e aplicativos | Gerenciamento corporativo
- As atualizações de março do Intune para a versão beta.

### <a name="device-and-app-management--multi-tenant-management"></a>Gerenciamento de dispositivos e aplicativos | Gerenciamento multilocatário
[Listar](/graph/api/managedtenants-managedtenant-list-auditevents?view=graph-rest-beta&preserve-view=true) e [obter](/graph/api/managedtenants-auditevent-get?view=graph-rest-beta&preserve-view=true) eventos de auditoria para locatários gerenciados no Microsoft 365 Lighthouse.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
[Listar](/graph/api/organizationsettings-list-microsoftapplicationdataaccess?view=graph-rest-beta&preserve-view=true) ou [atualizar](/graph/api/microsoftapplicationdataaccesssettings-update?view=graph-rest-beta&preserve-view=true) as [configurações](/graph/api/resources/microsoftapplicationdataaccesssettings?view=graph-rest-beta&preserve-view=true) que especificam o acesso de aplicativos da Microsoft aos dados do Microsoft 365 pertencentes a usuários em uma organização. Por exemplo, dada a autorização adequada, se apenas aplicativos Microsoft 365 (como Word e Excel) podem acessar os dados do Microsoft 365 dos usuários ou se outros aplicativos da Microsoft (como o Windows) também podem acessar os dados. Por padrão, todos os usuários em uma organização podem acessar em um aplicativo da Microsoft quaisquer dados do Microsoft 365 que o usuário tenha sido autorizado a acessar. 

### <a name="security--attack-simulation-and-training"></a>Segurança | Treinamento e simulação de ataque
- [Listar automações de simulação](/graph/api/attacksimulationroot-list-simulationautomations?view=graph-rest-beta&preserve-view=true) para um locatário.
- [Listar execuções](/graph/api/resources/simulationautomationrun?view=graph-rest-beta&preserve-view=true) de automações de simulação para um locatário.

### <a name="search"></a>Pesquisar
- Especifique em uma [ solicitação de pesquisa](/graph/api/resources/searchrequest?view=graph-rest-beta&preserve-view=true) se os arquivos duplicados do SharePoint devem ser cortados dos resultados da pesquisa. O padrão é false.
- Qualifique uma cadeia de caracteres de [consulta de pesquisa](/graph/api/resources/searchquery?view=graph-rest-beta&preserve-view=true) com um modelo, que dá suporte a KQL e variáveis de consulta.

### <a name="sites-and-lists"></a>Sites e listas
Para uma [coluna](/graph/api/resources/columnDefinition?view=graph-rest-beta&preserve-view=true) que contém dados de taxonomia especifique o [termo](/graph/api/resources/termstore-term?view=graph-rest-beta&preserve-view=true) pai e o [conjunto de termos](/graph/api/resources/termstore-set?view=graph-rest-beta&preserve-view=true) para os quais os termos filho podem ser selecionados como valores de coluna.

### <a name="tasks-and-plans"></a>Tarefas e planos
Identifique se um plano do Planner destinado a experiências fora do Planner (como o Microsoft Teams) pode acompanhar o trabalho nesse contexto, verificando os **detalhes** da relação do recurso [plannerPlan](/graph/api/resources/plannerPlan?view=graph-rest-beta&preserve-view=true) correspondente.

### <a name="teamwork"></a>Trabalho em equipe
- Obtenha ou defina [informações de resumo](/graph/api/resources/teamSummary?view=graph-rest-beta&preserve-view=true) sobre uma [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true), incluindo a contagem de proprietários, membros e convidados.
- Classifique mensagens em ordem decrescente ao [listar mensagens em um chat](/graph/api/chat-list-messages?view=graph-rest-beta&preserve-view=true).


## <a name="february-2022-new-and-generally-available"></a>Janeiro de 2022: Novo e disponível ao público em geral

### <a name="teamwork"></a>Trabalho em equipe
Obtenha [detalhes sobre uma reunião online](/graph/api/resources/teamworkOnlineMeetingInfo) associada a um [chat](/graph/api/resources/chat) através da propriedade **onlineMeetingInfo**.

## <a name="february-2022-new-in-preview-only"></a>Fevereiro de 2022: novo somente para visualização

### <a name="applications"></a>Aplicativos
- Use uma nova opção de política de [autenticação de aplicativo](/graph/api/resources/applicationauthenticationmethodpolicy?view=graph-rest-beta&preserve-view=true) para restringir um segredo de senha personalizado em um aplicativo ou entidade de serviço.
- Especifique as [configurações](/graph/api/resources/windowsApplication?view=graph-rest-beta&preserve-view=true) para aplicativos que executam o Windows e publicados na Microsoft Store ou na loja de jogos do Xbox.

### <a name="change-notifications"></a>Notificações de alteração
Assine para alterações de contatos, eventos ou mensagens do Outlook e receba notificações que incluem dados de recursos na carga. Para obter mais informações, confira [Alterar notificações para recursos do Outlook no Microsoft Graph](outlook-change-notifications-overview.md).

### <a name="device-and-app-management--cloud-pc"></a>Gerenciamento de dispositivos e aplicativos | PC na nuvem 
- Defina as [configurações de ponto de restauração](/graph/api/resources/cloudpcrestorepointsetting?view=graph-rest-beta&preserve-view=true), que incluem a frequência para criar um ponto de restauração e se os usuários podem restaurar seu próprio PC na nuvem com base em um backup de ponto de restauração.
- [Restaurar](/graph/api/manageddevice-restorecloudpc?view=graph-rest-beta&preserve-view=true) um PC na nuvem com base em um instantâneo anterior.
- [Restaurar vários PCs na nuvem](/graph/api/manageddevice-bulkrestorecloudpc?view=graph-rest-beta&preserve-view=true) em uma única solicitação especificando suas IDs de dispositivo gerenciado e um intervalo de data/hora (por exemplo, antes, depois) de um ponto de restauração.

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

### <a name="search"></a>Pesquisar
Configure [acrônimo](/graph/api/resources/search-acronym?view=graph-rest-beta&preserve-view=true), [indicador](/graph/api/resources/search-bookmark?view=graph-rest-beta&preserve-view=true) e recursos [QnA](/graph/api/resources/search-qna?view=graph-rest-beta&preserve-view=true) como [respostas de pesquisa administrativa para usuários em uma organização](search-concept-answers.md).


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
