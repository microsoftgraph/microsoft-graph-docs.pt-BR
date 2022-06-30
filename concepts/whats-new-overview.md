---
title: Novidades do Microsoft Graph
description: Exiba os destaques das novidades Microsoft Graph nos últimos dois meses, o que foi adicionado em versões anteriores e como você pode compartilhar suas ideias.
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 56b50679f230dfc3dd656baf4fdb9bd9a4220b6e
ms.sourcegitcommit: 175dda9b51aaa94fa00d0e4b7101c771b6315f05
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66557157"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Recursos, incluindo APIs e ferramentas, no status de _visualização_ podem mudar sem aviso prévio e alguns podem nunca ser promovidos ao status de disponibilidade geral (GA). Não utilize recursos de visualização em aplicativos de produção.

## <a name="june-2022-new-and-generally-available"></a>Junho de 2022: novo e disponível para o público geral

### <a name="cloud-communications--call-records"></a>Comunicações na nuvem | Registros de chamadas
Obtenha informações sobre o codec de áudio, codec de vídeo, protocolo de transporte de rede e saltos de rota de rastreamento para um [fluxo de mídia](/graph/api/resources/callrecords-mediastream) ao [obter um registro de chamada](/graph/api/callrecords-callrecord-get) e expandir cada [segmento](/graph/api/resources/callrecords-segment) de uma [sessão](/graph/api/resources/callrecords-session).

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- [Liste as unidades administrativas ](/graph/api/device-list-memberOf) que um [dispositivo](/graph/api/resources/device) é membro.
- Gerenciar dispositivos como membros em uma [unidade administrativa](/graph/api/resources/administrativeunit): [listar membros](/graph/api/administrativeunit-list-members) incluindo dispositivos, e [obter](/graph/api/administrativeunit-get-members), [adicionar](/graph/api/administrativeunit-post-members), e [remover](/graph/api/administrativeunit-delete-members) um dispositivo como membro. 
- [Obtenha](/graph/api/application-get) o status e outros detalhes de [certificação de segurança e conformidade](/graph/api/resources/certification) de um [programa](/graph/api/resources/application) para proteger os dados do cliente. Para obter mais informações, consulte [Certificação Microsoft 365](/microsoft-365-app-certification/docs/enterprise-app-certification-guide).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
 Configure e gerencie as [configurações da política de métodos de autenticação de Passagem de Acesso Temporário](/graph/api/resources/temporaryAccessPassAuthenticationMethodConfiguration) no seu locatário.

### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
- Encontre novas colunas nos relatórios do Teams gerados pelos seguintes métodos:
  - [getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts)
  - [getTeamsUserActivityUserDetail](/graph/api/reportroot-getTeamsUserActivityUserDetail)
  - [getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getTeamsDeviceUsageUserDetail)
  - [getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts)
  - [getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getTeamsDeviceUsageDistributionUserCounts)
- A coluna Windows Phone nos relatórios do Teams gerados pelos seguintes métodos:
  - [getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts)
  - [getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getTeamsDeviceUsageDistributionUserCounts)


### <a name="teamwork"></a>Trabalho em equipe
Assine as notificações de alteração do seguinte no Teams:
- [equipe e canal](teams-changenotifications-team-and-channel.md)
- [associação de equipe e canal](teams-changenotifications-teammembership.md)
- [chat](teams-changenotifications-chat.md)
- [associação do chat](teams-changenotifications-chatmembership.md)

## <a name="june-2022-new-in-preview-only"></a>Junho de 2022: novo somente na visualização

### <a name="compliance--ediscovery"></a>Conformidade | Descoberta eletrônica
Acesse a [API de Descoberta Eletrônica](/graph/api/resources/security-ediscoverycase?view=graph-rest-beta&preserve-view=true) do namespace de [segurança](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true) no futuro, em vez do namespace de conformidade.

### <a name="device-and-app-management--multi-tenant-management"></a>Gerenciamento de dispositivos e aplicativos | Gerenciamento multilocatário
[Obtenha](/graph/api/managedtenants-managedtenant-list-myroles?view=graph-rest-beta&preserve-view=true) a coleção de [funções atribuídas a um usuário conectado](/graph/api/resources/managedtenants-myRole?view=graph-rest-beta&preserve-view=true) para um [locatário gerenciado](/graph/api/resources/managedtenants-managedTenant?view=graph-rest-beta&preserve-view=true).

### <a name="education"></a>Educação
- [Crie](/graph/api/educationassignment-setupfeedbackresourcesfolder?view=graph-rest-beta&preserve-view=true) uma pasta do SharePoint em uma [atribuição](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) para carregar documentos de comentários.
- [Crie](/graph/api/educationfeedbackresourceoutcome-post-outcomes?view=graph-rest-beta&preserve-view=true) um [documento de comentários](/graph/api/resources/educationFeedbackResourceOutcome?view=graph-rest-beta&preserve-view=true) em um [envio](/graph/api/resources/educationsubmission?view=graph-rest-beta&preserve-view=true) na pasta de comentários associada à atribuição.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- [Promover](/graph/api/domain-promote?view=graph-rest-beta&preserve-view=true) um subdomínio verificado no domínio raiz.
- [Obtenha](/graph/api/application-get?view=graph-rest-beta&preserve-view=true) a URL para os metadados do SAML para federação de um [programa](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) de locatário único.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
Ocultar links de redefinição de senha de autoatendimento (SSPR) nas [configurações de visibilidade de texto da página de logon](/graph/api/resources/loginpagetextvisibilitysettings?view=graph-rest-beta&preserve-view=true) na página de entrada de um locatário. 


## <a name="may-2022-new-and-generally-available"></a>Maio de 2022: novos e geralmente disponíveis

### <a name="education"></a>Educação
- [Controlar Alterações dos recursos de atribuição.](/graph/api/educationassignment-delta)
- [Controlar Alterações dos recursos da categoria de atribuição.](/graph/api/educationcategory-delta)

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
Um [aplicativo](/graph/api/resources/application) registrado no Azure Active Directory (Microsoft Azure AD) pode especificar as informações de contato do aplicativo ou serviço de um banco de dados de Gerenciamento de Ativos ou Serviços.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
Permitir que um locatário do Azure Active Directory (Azure AD) defina uma [federação com outra organização cujo provedor de identidade (IdP) ofereça suporte ao protocolo SAML ou WS-Fed](/graph/api/resources/samlOrWsFedExternalDomainFederation). Isso permite que o locatário do Azure AD dê acesso aos seus recursos para usuários convidados.

### <a name="search"></a>Pesquisar
Você pode especificar até 1000 resultados de pesquisa por página para uma [solicitação de pesquisa](/graph/api/resources/searchrequest).

### <a name="sites-and-lists"></a>Sites e listas
- Obtenha uma coleção de recursos de [tipo de conteúdo](/graph/api/resources/contentType) do hub de tipo de conteúdo que são compatíveis usando a ação [getCompatibleHubContentTypes](/graph/api/contenttype-getcompatiblehubcontenttypes). 
- Adicione ou sincronize um tipo de conteúdo do hub de tipo de conteúdo para um [site](/graph/api/resources/site) ou [lista](/graph/api/resources/list), usando a ação [addCopyFromContentTypeHub](/graph/api/contenttype-addcopyfromcontenttypehub). Isso torna um tipo de conteúdo ou sua atualização disponível para um site ou lista específica onde é necessário. Essa é uma melhoria da infraestrutura de sincronização herdada que envia o tipo de conteúdo para todos os sites de uma organização, reduzindo os tempos de espera para a propagação da publicação. 
- Obtenha uma ou mais [operações avançadas e de longa duração](/graph/api/resources/richlongrunningoperation) ocorrendo em um site ou lista, o que pode acontecer ao adicionar um tipo de conteúdo de forma síncrona.

### <a name="tasks-and-plans"></a>Tarefas e planos
- [Obtenha](/graph/api/plannerplandetails-get) ou [atualize](/graph/api/plannerplandetails-update) as descrições das categorias como parte dos [detalhes](/graph/api/resources/plannerplandetails) de um [plano](/graph/api/resources/plannerplan).
- Em vez da propriedade do **proprietário** de um **plano**, use o **tipo** de propriedade de um [contêiner de plano](/graph/api/resources/plannerplancontainer) para especificar as regras de autorização e a vida útil de um **plano**.
- Obtenha a prioridade de uma [tarefa](/graph/api/resources/plannerTask).

### <a name="teamwork"></a>Trabalho em equipe
[Receba mensagens em um canal](/graph/api/channel-list-messages) e [inclua todas as respostas](/graph/api/channel-list-messages#example-3-request-with-top-and-expand-query-options-on-replies) à mensagem.

### <a name="to-do-tasks"></a>Tarefas pendentes
- Dividir uma [tarefa pendentes](/graph/api/resources/todotask) complexa em tarefas mais acionáveis e menores, cada uma delas como um [item de lista de verificação](/graph/api/resources/checklistitem).
- Rotular uma tarefa pendente com uma [categoria](/graph/api/resources/outlookcategory) definida pelo usuário para agrupar contatos do Outlook, eventos, mensagens, postagens de grupo e tarefas pendentes.


## <a name="may-2022-new-in-preview-only"></a>Maio de 2022: novo apenas na versão prévia

### <a name="application"></a>Aplicativo
Ao configurar o Proxy de Aplicativo do Azure AD para aplicativos locais para acesso remoto seguro, use a propriedade **isStateSessionEnabled** no recurso [onPremisesPublishing](/graph/api/resources/onPremisesPublishing?view=graph-rest-beta&preserve-view=true) para especificar se deve validar o parâmetro de estado se o aplicativo usar o fluxo de concessão do código de autorização OAuth 2.0. Definir essa propriedade ajuda os administradores a proteger o aplicativo contra solicitação intersite forjada (CSRF).

### <a name="compliance--subject-rights-requests"></a>Conformidade | Solicitações de direitos de entidade
- Especifique ou obtenha os locais que devem ser pesquisados em uma [solicitação de direitos de assunto](/graph/api/resources/subjectRightsRequest?view=graph-rest-beta&preserve-view=true), como [caixas de correio](/graph/api/resources/subjectRightsRequestAllMailboxLocation?view=graph-rest-beta&preserve-view=true), [canais do SharePoint, OneDrive ou Teams](/graph/api/resources/subjectRightsRequestAllSiteLocation?view=graph-rest-beta&preserve-view=true).
- Especifique ou obtenha uma consulta de conteúdo baseada em KQL que deve ser usada para pesquisa em uma solicitação de direitos de entidade.

### <a name="device-and-app-management--cloud-pc"></a>Gerenciamento de dispositivos e aplicativos | PC na nuvem
- Obtenha um [resultado](/graph/api/resources/cloudpcbulkremoteactionresult?view=graph-rest-beta&preserve-view=true) claramente definido no [reprovisionamento em massa de dispositivos Cloud PC](/graph/api/manageddevice-bulkReprovisionCloudPc?view=graph-rest-beta&preserve-view=true).
- [Obtenha](/graph/api/manageddevice-getcloudpcreviewstatus?view=graph-rest-beta&preserve-view=true) ou [defina](/graph/api/manageddevice-setcloudpcreviewstatus?view=graph-rest-beta&preserve-view=true) um [status de revisão do Cloud PC](/graph/api/resources/cloudpcreviewstatus?view=graph-rest-beta&preserve-view=true) ou defina o [status de revisão do Cloud PC](/graph/api/manageddevice-bulksetcloudpcreviewstatus?view=graph-rest-beta&preserve-view=true) em massa para vários dispositivos.

### <a name="device-and-app-management--multi-tenant-management"></a>Gerenciamento de dispositivos e aplicativos | Gerenciamento multilocatário
[Obtenha](/graph/api/managedtenants-managedtenant-list-tenantusage?view=graph-rest-beta&preserve-view=true) o número de usuários ativos mensais para cada serviço em um locatário gerenciado.

### <a name="education"></a>Educação
Use um [recurso de aplicativo Teams](/graph/api/resources/educationteamsappresource?view=graph-rest-beta&preserve-view=true) que corresponda a um aplicativo instalado do Microsoft Teams, para permitir que os usuários do serviço de educação criem e compartilhem atribuições com aplicativos do Teams inseridos, como o YouTube ou o FlipGrid.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
A ativação de um serviço [para uma organização](/graph/api/organization-activateService?view=graph-rest-beta&preserve-view=true) e [para um usuário](/graph/api/user-activateServicePlan?view=graph-rest-beta&preserve-view=true) foi preterida e deixará de retornar dados em 30 de junho de 2022.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
Como parte da [função de usuário padrão](/graph/api/resources/defaultuserrolepermissions?view=graph-rest-beta&preserve-view=true) de uma [ política de autorização ](/graph/api/resources/authorizationPolicy?view=graph-rest-beta&preserve-view=true), especifique se o proprietário registrado de um dispositivo pode ler suas próprias chaves de recuperação do BitLocker.

### <a name="reports--identity-and-access-reports"></a>Relatórios | Relatórios de identidade e acesso
Obtenha um [relatório de uso para os métodos de autenticação registrados de um usuário](/graph/api/resources/userregistrationdetails?view=graph-rest-beta&preserve-view=true) que inclui o método padrão para autenticação de multi-fatores.

### <a name="search--index"></a>Pesquisa | Índice
[Obtenha](/graph/api/externalconnectors-connectionquota-get?view=graph-rest-beta&preserve-view=true) as [informações de cota](/graph/api/resources/externalconnectors-connectionQuota?view=graph-rest-beta&preserve-view=true) de uma [conexão](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true). Essas informações incluem o número de itens que você pode ingerir na conexão, levando em consideração os itens restantes na conexão e a cota restante no nível do locatário de todas as suas conexões.

### <a name="sites-and-lists"></a>Sites e listas
[Controlar alterações para o item de lista do SharePoint recursos.](/graph/api/listitem-delta?view=graph-rest-beta&preserve-view=true)

### <a name="teamwork"></a>Trabalho em equipe
- Use permissões de aplicativo para [obter todos os chats](/graph/api/chat-list?view=graph-rest-beta&preserve-view=true) em que um usuário especificado está envolvido sem que o usuário esteja presente.
- [Enviar notificações do feed de atividades para vários usuários em massa](/graph/api/teamwork-sendActivityNotificationToRecipients?view=graph-rest-beta&preserve-view=true), até 100 usuários de cada vez.

### <a name="to-do-tasks"></a>Tarefas pendentes
A partir de 31 de maio de 2022, o [conjunto de API de tarefas pendentes que é compilado sobre a baseTask](/graph/api/resources/tasks-overview?view=graph-rest-beta&preserve-view=true) está preterido. Esse conjunto de API deixará de retornar dados em 31 de agosto de 2022. Em vez disso, use o [conjunto de API de tarefas pendentes compilado o todoTask](/graph/api/resources/todo-overview?view=graph-rest-beta&preserve-view=true).


## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote nos novos recursos na [Comunidade Microsoft Tech](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de visualização **_prévia_**. As atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de **_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/m365-dev-call) da chamada semanal da comunidade da plataforma Microsoft 365.
- Inscreva-se no [programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/office/dev-program), ganhe uma assinatura gratuita do Microsoft 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](https://developer.microsoft.com/graph/changelog/).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).
