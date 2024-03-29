---
title: Destaques de versões anteriores no Microsoft Graph
description: O que havia de novo no Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 99c5e8144f1994b6c4a8cba02476c0fcef4561e4
ms.sourcegitcommit: 005e9d483d03ed048611ffd180a92930afff4e42
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66646154"
---
# <a name="highlights-of-earlier-releases"></a>Destaques de versões anteriores

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


## <a name="april-2022-new-and-generally-available"></a>Abril de 2022: novo e com disponibilidade geral

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Use a [Gestão de Identidade Privilegiada (PIM)](/graph/api/resources/privilegedidentitymanagementv3-overview) em aplicativos de produção para gerenciar, controlar e monitorar o acesso a recursos importantes na sua organização. O acesso é habilitado por meio de funções privilegiadas e do controle de acesso baseado em função (RBAC) e pode ser concedido a usuários, grupos ou entidades de serviço. Os recursos podem estar no Microsoft Azure AD, no Azure e em outros serviços de nuvem da Microsoft, tais como o Microsoft 365 ou o Microsoft Intune.

### <a name="search--index"></a>Pesquisa | Índice
- Use as permissões do aplicativo `ExternalConnection.Read.All` e `ExternalConnection.ReadWrite.All` para ler ou gravar todas as conexões externas sem a presença de um usuário conectado.
- Use a permissão do aplicativo `ExternalItem.Read.All` para ler todos os itens externos sem a presença de um usuário conectado.
- Use a permissão delegada `ExternalConnection.ReadWrite.OwnedBy` para ler e gravar conexões externas em nome de um usuário conectado ao qual seu aplicativo está autorizado.
- Use a permissão delegada `ExternalConnection.Read.All` ou `ExternalConnection.ReadWrite.All` para ler ou gravar todas as conexões externas em nome de um usuário conectado.
- Use a permissão delegada `ExternalItem.ReadWrite.OwnedBy` para ler e gravar itens externos em nome de um usuário conectado, para o qual seu aplicativo está autorizado.
- Use a permissão delegada `ExternalItem.Read.All` ou `ExternalItem.ReadWrite.All` para ler ou gravar todos os itens externos em nome de um usuário conectado.


## <a name="april-2022-new-in-preview-only"></a>Abril de 2022: novo somente para visualização

### <a name="customer-bookings"></a>Reservas do Cliente
- [Obtenha informações de disponibilidade](/graph/api/bookingbusiness-getstaffavailability?view=graph-rest-beta&preserve-view=true) para recursos de um [membro da equipe](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true) em uma [empresa](/graph/api/resources/bookingbusiness?view=graph-rest-beta&preserve-view=true).
- Use a permissão de aplicativo `Bookings.Read.All` em operações de leitura para recursos de[empresas](/graph/api/resources/bookingbusiness?view=graph-rest-beta&preserve-view=true), [membro da equipe](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true), [serviço](/graph/api/resources/bookingservice?view=graph-rest-beta&preserve-view=true), [cliente](/graph/api/resources/bookingcustomer?view=graph-rest-beta&preserve-view=true) e [compromisso](/graph/api/resources/bookingappointment?view=graph-rest-beta&preserve-view=true).
- Use a permissão de aplicativo `BookingsAppointment.ReadWrite.All` para operações de leitura/gravação para recursos de cliente e compromisso.

### <a name="device-and-app-management--cloud-pc"></a>Gerenciamento de dispositivos e aplicativos | PC na nuvem
- Especifique [Configurações do Windows](/graph/api/resources/cloudpcwindowssettings?view=graph-rest-beta&preserve-view=true) como parte das [configurações da organização do PC na nuvem](/graph/api/resources/cloudPcOrganizationSettings?view=graph-rest-beta&preserve-view=true) para um locatário.
- [Obtenha](/graph/api/user-list-cloudpcs?view=graph-rest-beta&preserve-view=true) os dispositivos de PC na nuvem atribuídos ao usuário conectado.
- [Obter informações para iniciar um dispositivo de PC na nuvem](/graph/api/cloudpc-getcloudpclaunchinfo?view=graph-rest-beta&preserve-view=true) para o usuário conectado.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
Configure [ configurações de federação](/graph/api/resources/internalDomainFederation?view=graph-rest-beta&preserve-view=true) para federar domínios com o Azure Active Directory.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
[Obtenha atribuições](/graph/api/accesspackageassignment-additionalaccess?view=graph-rest-beta&preserve-view=true) para as quais o usuário correspondente tem pacotes de acesso incompatíveis. 

### <a name="reports--identity-and-access-reports"></a>Relatórios | Relatórios de identidade e acesso
Confirme se um evento é [de alto risco e está comprometido](/graph/api/signin-confirmCompromised?view=graph-rest-beta&preserve-view=true) ou é [seguro](/graph/api/signin-confirmSafe?view=graph-rest-beta&preserve-view=true) marcando o evento nos logs de entrada Azure Active Directory correspondentes.

### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
- [Obtenha um relatório de distribuição total](/graph/api/reportroot-getTeamsUserActivityTotalDistributionCounts?view=graph-rest-beta&preserve-view=true) para a contagem de atividades específicas do Teams em um período especificado. As contagens de atividades do Teams incluem mensagens de chat da equipe, chamadas, reuniões, duração do áudio, postagem de mensagens e assim por diante.
- Obtenha tipos de atividade adicionais em relatórios que [obtém detalhes do usuário](/graph/api/reportroot-getTeamsUserActivityUserDetail?view=graph-rest-beta&preserve-view=true), [obtém contagens de atividades ](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-beta&preserve-view=true)e [obtém contagens de total de atividade](/graph/api/reportroot-getteamsuseractivitytotalcounts?view=graph-rest-beta&preserve-view=true).

### <a name="teamwork"></a>Trabalho em equipe
Compartilhar um canal com uma ou mais equipes:
- [Liste os canais que são compartilhados com uma equipe](/graph/api/team-list-incomingchannels?view=graph-rest-beta&preserve-view=true).
- [Liste todos os canais em uma equipe](/graph/api/team-list-allchannels?view=graph-rest-beta&preserve-view=true) incluindo aqueles hospedados em uma equipe ou compartilhados com ela.
- [Liste membros da equipe que podem acessar um canal compartilhado especificado](/graph/api/sharedwithchannelteaminfo-list-allowedmembers?view=graph-rest-beta&preserve-view=true).
- [Remova um canal compartilhado com uma equipe](/graph/api/team-delete-incomingchannels?view=graph-rest-beta&preserve-view=true).
- [Liste as equipes que compartilharam um canal especificado](/graph/api/sharedwithchannelteaminfo-list?view=graph-rest-beta&preserve-view=true).
- [ Deixe de compartilhar um canal com uma equipe](/graph/api/sharedwithchannelteaminfo-delete?view=graph-rest-beta&preserve-view=true).


## <a name="march-2022-new-and-generally-available"></a>Março de 2022: Novo e disponível para o público geral

### <a name="files"></a>Arquivos
Use um [pacote](/graph/api/resources/bundle) para compartilhar vários arquivos ao mesmo tempo, assim como outros recursos [driveItem](/graph/api/resources/driveitem). Você pode aplicar operações CRUD em um pacote e [adicionar](/graph/api/bundle-additem) um item ou [remover](/graph/api/bundle-removeitem) um item de um pacote.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
Use a [permissão específica de recurso](/graph/api/resources/resourcespecificpermission) para autorizar um aplicativo do Teams a acessar diretamente os dados de uma instância específica de um chat ou equipe. Por exemplo, a permissão específica do recurso ChannelMessage.Read.Group permite que um aplicativo do Teams leia as mensagens de canal de uma única equipe.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- [Obter](/graph/api/approval-get)decisões de [aprovação](/graph/api/resources/approval) associadas a uma [solicitação de atribuição de pacote de acesso](/graph/api/resources/accesspackageassignmentrequest).
- Como parte do[Gerenciamento de direitos do Azure Active Directory (Azure AD)](/graph/api/resources/entitlementmanagement-overview), use uma [política de atribuição de pacote de acesso](/graph/api/resources/accesspackageassignmentpolicy) para gerenciar uma solicitação, aprovação, atribuição ou revisão regular para um [pacote de acesso](/graph/api/resources/accesspackage). Você pode controlar o acesso de usuários internos e externos a grupos, aplicativos e sites do SharePoint Online de uma organização.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
Especifique a [inclusão ou exclusão de aplicativos cliente](/graph/api/resources/conditionalaccessclientapplications) como um [conjunto de condições](/graph/api/resources/conditionalAccessConditionSet) para aplicar uma [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy).

### <a name="use-the-toolkit"></a>Usar o kit de ferramentas
Celebre o verdadeiro trabalho em equipe com as contribuições da comunidade e experimente os novos recursos do [Kit de ferramentas do Microsoft Graph v2.4.0](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases/tag/v2.4.0):
- Otimize a atualização de imagens de pessoas no componente [pessoa](/graph/toolkit/components/person) usando o atributo `disable-image-fetch`para controlar a busca desnecessária.
- Evite o carregamento desnecessário de imagens de pessoas no componente [seletor de pessoas](/graph/toolkit/components/people-picker) usando o atributo `disable-images`. 
- Filtre por usuários, grupos e lista de pessoas disponíveis no componente [seletor de pessoas](/graph/toolkit/components/people-picker) usando os atributos `user-filters`, `group-filters` e `people-filters`.


## <a name="march-2022-new-in-preview-only"></a>Março de 2022: novo somente para visualização

### <a name="cloud-communications--online-meeting"></a>Comunicações na nuvem | Reunião online
Especifique um ou [participantes da reunião](/graph/api/resources/meetingParticipants?view=graph-rest-beta&preserve-view=true) como co-organizador.

### <a name="compliance--ediscovery"></a>Conformidade | Descoberta Eletrônica
[Limpe dados](/graph/api/ediscovery-sourcecollection-purgeData?view=graph-rest-beta&preserve-view=true) e exclua permanentemente mensagens do Microsoft Teams de uma [coleção de origem](/graph/api/resources/ediscovery-sourcecollection?view=graph-rest-beta&preserve-view=true) de descoberta eletrônica.

### <a name="device-and-app-management--cloud-pc"></a>Gerenciamento de dispositivos e aplicativos | PC na nuvem
- Use permissões delegadas ou de aplicativo de `RoleManagement.Read.CloudPC` para as operações de leitura do recurso [unifiedRoleDefinition](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true).
- Use permissões delegadas ou de aplicativo de `RoleManagement.ReadWrite.CloudPC` para as operações de leitura e gravação do recurso [unifiedRoleDefinition](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true).
- Especifique a ID e o nome de exibição de uma assinatura do Azure como parte das informações de uma [imagem de origem de um dispositivo](/graph/api/resources/cloudPcSourceDeviceImage?view=graph-rest-beta&preserve-view=true).
- Especifique e configure as[configurações do Windows](/graph/api/resources/cloudpcwindowssettings?view=graph-rest-beta&preserve-view=true) ao criar PCs na nuvem para uma [política de provisionamento](/graph/api/resources/cloudPcProvisioningPolicy?view=graph-rest-beta&preserve-view=true).

### <a name="device-and-app-management--corporate-management"></a>Gerenciamento de dispositivos e aplicativos | Gerenciamento corporativo
- As atualizações de março do Intune para a versão beta.

### <a name="device-and-app-management--multi-tenant-management"></a>Gerenciamento de dispositivos e aplicativos | Gerenciamento multilocatário
[Listar](/graph/api/managedtenants-managedtenant-list-auditevents?view=graph-rest-beta&preserve-view=true) e [obter](/graph/api/managedtenants-auditevent-get?view=graph-rest-beta&preserve-view=true) eventos de auditoria para locatários gerenciados no Microsoft 365 Lighthouse.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- [Listar](/graph/api/organizationsettings-list-microsoftapplicationdataaccess?view=graph-rest-beta&preserve-view=true) ou [atualizar](/graph/api/microsoftapplicationdataaccesssettings-update?view=graph-rest-beta&preserve-view=true) as [configurações](/graph/api/resources/microsoftapplicationdataaccesssettings?view=graph-rest-beta&preserve-view=true) que especificam o acesso de aplicativos da Microsoft aos dados do Microsoft 365 pertencentes a usuários em uma organização. Por exemplo, dada a autorização adequada, se apenas aplicativos Microsoft 365 (como Word e Excel) podem acessar os dados do Microsoft 365 dos usuários ou se outros aplicativos da Microsoft (como o Windows) também podem acessar os dados. Por padrão, todos os usuários em uma organização podem acessar em um aplicativo da Microsoft quaisquer dados do Microsoft 365 que o usuário tenha sido autorizado a acessar. 
- Seguindo o modelo de segurança cibernética de Confiança Zero, os parceiros da Microsoft podem usar [GDAP (privilégios de administrador delegado granular)](/graph/api/resources/delegatedadminrelationships-api-overview?view=graph-rest-beta&preserve-view=true) para executar tarefas administrativas com acesso menos privilegiado aos locatários dos clientes, a fim de evitar possíveis exposições de segurança. Em vez de solicitar a função de Administrador Global como no passado, os parceiros solicitam funções específicas para a administração de locatários do cliente por um período definido, e seus clientes devem conceder explicitamente acesso menos privilegiado a eles.

### <a name="security--attack-simulation-and-training"></a>Segurança | Treinamento e simulação de ataque
- [Listar automações de simulação](/graph/api/attacksimulationroot-list-simulationautomations?view=graph-rest-beta&preserve-view=true) para um locatário.
- [Listar execuções](/graph/api/resources/simulationautomationrun?view=graph-rest-beta&preserve-view=true) de automações de simulação para um locatário.

### <a name="search"></a>Pesquisar
- Especifique em uma [solicitação de pesquisa](/graph/api/resources/searchrequest?view=graph-rest-beta&preserve-view=true) se os arquivos duplicados do SharePoint devem ser cortados dos resultados da pesquisa. O padrão é false. 
- Qualifique uma cadeia de caracteres de [consulta de pesquisa](/graph/api/resources/searchquery?view=graph-rest-beta&preserve-view=true) com um modelo, que dá suporte a KQL e variáveis de consulta.

### <a name="sites-and-lists"></a>Sites e listas
- Para uma [coluna](/graph/api/resources/columnDefinition?view=graph-rest-beta&preserve-view=true) que contém dados de taxonomia especifique o [termo](/graph/api/resources/termstore-term?view=graph-rest-beta&preserve-view=true) pai e o [conjunto de termos](/graph/api/resources/termstore-set?view=graph-rest-beta&preserve-view=true) para os quais os termos filho podem ser selecionados como valores de coluna.
- Obtenha as configurações de um [site](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true), incluindo seu idioma e fuso horário.

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


## <a name="december-2021-new-and-generally-available"></a>Dezembro de 2021: novo e disponível ao público geral

### <a name="cloud-communications--presence"></a>Comunicações na nuvem | Presença
[Inscreva-se nas notificações de alterações](/graph/api/subscription-post-subscriptions) no status de [presença](/graph/api/resources/presence) de um usuário especificado. Sempre especifique um certificado de criptografia na solicitação de assinatura, pois são [notificações avançadas que incluem dados de recursos criptografados](webhooks-with-resource-data.md).


### <a name="compliance--subject-rights-requests"></a>Conformidade | Solicitações de direitos de entidade
Como parte do [gerenciamento de privacidade no Microsoft 365](/privacy/solutions/privacymanagement/privacy-management?view=o365-worldwide&preserve-view=true), a [API de solicitações de direitos do sujeito](/graph/api/resources/subjectrightsrequest) estreia nos pontos de extremidade v1 e beta do Microsoft Graph. A API permite que os usuários façam solicitações para revisar ou gerenciar seus dados pessoais em suas organizações. Ele também permite que as organizações automatizem e dimensionem o gerenciamento dessas solicitações, ajudando-as a atender às regulamentações do setor com mais eficiência.

### <a name="customer-booking"></a>Reserva de clientes
Use a API do Microsoft Bookings em aplicativos de produção e aproveite os seguintes novos recursos e atualizações:
- Notifique seus clientes nos EUA ou Canadá por SMS para um [compromisso](/graph/api/resources/bookingappointment) ou serviço [ específico ](/graph/api/resources/bookingservice) associado a um compromisso.
- Habilite a reunião online para um serviço e gere automaticamente um link de reunião do Microsoft Teams para o compromisso.
- Permita um ou mais clientes em um compromisso de grupo, definindo uma contagem máxima de participantes para um serviço e para um compromisso e acompanhando a contagem real de participantes em um compromisso.
- Crie uma [pergunta personalizada](/graph/api/resources/bookingcustomquestion) para uma [empresa](/graph/api/resources/bookingbusiness), associe uma pergunta a uma opção para especificá-la como obrigatória para um serviço e acompanhe perguntas e respostas em um compromisso.
- Obter ou definir o fuso horário de um cliente em um compromisso ou [membro da equipe](/graph/api/resources/bookingstaffmember).
- Obtenha ou defina o local e o número de telefone de um [cliente](/graph/api/resources/bookingcustomer).
- Acesse a API v1 do novo ponto de extremidade `https://graph.microsoft.com/v1.0/solutions/`. Observe que a API beta permanece no `https://graph.microsoft.com/beta` ponto de extremidade.

### <a name="education"></a>Educação
- Especifique [tarefa](/graph/api/resources/educationassignment) ser adicionada somente aos calendários dos alunos usando a propriedade **addToCalendarAction**.
- [Reatribuir](/graph/api/educationsubmission-reassign) uma [tarefa enviada](/graph/api/resources/educationsubmission) a um aluno com feedback para revisão.
- [Listar atribuições](/graph/api/educationuser-list-assignments) para [um educationUser](/graph/api/resources/educationuser). 

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
[Atualizar](/graph/api/accessreviewinstance-update) revisores e revisores de fallback para uma instância [de uma análise de acesso](/graph/api/resources/accessreviewinstance).

### <a name="teamwork"></a>Trabalho em equipe
- Identifique um [chat](/graph/api/resources/chat) no Microsoft Teams por sua URL da Web (por meio da propriedade **webUrl** ).
- Obtenha detalhes de um evento que aconteceu em um chat, canal ou equipe, acessando [eventMessageDetail](/graph/api/resources/EventMessageDetail) de um [chatMessage](/graph/api/resources/chatmessage) ou [chat](/graph/api/resources/chat). Por exemplo, membros adicionados a um canal ou chat, e a descrição da equipe atualizada.

## <a name="december-2021-new-in-preview-only"></a>Dezembro de 2021: novo apenas na visualização

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões online
Habilite o registro para uma [reunião online](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) usando um sistema de [registro externo](/graph/api/resources/externalmeetingregistration?view=graph-rest-beta&preserve-view=true). 

### <a name="cloud-communications--presence"></a>Comunicações na nuvem | Presença
- Use a ação [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true) para definir o status de disponibilidade e atividade preferencial de um usuário. A presença do usuário se torna a presença preferencial.
- Use a ação [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true) para limpar os status de disponibilidade e atividade preferencial de um usuário.
- Use `Presence.ReadWrite` como permissão delegada com [setPresence](/graph/api/presence-setpresence?view=graph-rest-beta&preserve-view=true), [clearPresence](/graph/api/presence-clearpresence?view=graph-rest-beta&preserve-view=true), [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true)ou [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true).
- Use `Presence.ReadWrite.All` como permissão de aplicativo com [setPresence](/graph/api/presence-setpresence?view=graph-rest-beta&preserve-view=true), [clearPresence](/graph/api/presence-clearpresence?view=graph-rest-beta&preserve-view=true), [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true)ou [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
- Os administradores podem habilitar o [Microsoft Managed Desktop](/graph/api/resources/microsoftmanageddesktop?view=graph-rest-beta&preserve-view=true) especificando as configurações em uma [política de provisionamento de PC na nuvem](/graph/api/resources/cloudpcprovisioningpolicy?view=graph-rest-beta&preserve-view=true) e configurando uma experiência de dispositivo gerenciado para um PC na nuvem.
- [Reinicializar](/graph/api/cloudpc-reboot?view=graph-rest-beta&preserve-view=true) um [PC na nuvem](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true).
- [Renomear](/graph/api/cloudpc-rename?view=graph-rest-beta&preserve-view=true) para atualizar o nome de exibição de um PC na nuvem.
- [Solução](/graph/api/cloudpc-troubleshoot?view=graph-rest-beta&preserve-view=true) para verificar o status de integridade de um PC na nuvem e do host da sessão.
- Acompanhe o último resultado da ação remota em um PC na nuvem, incluindo reinicialização, renomeação, reprovisionamento, solução de problemas, pela propriedade **lastRemoteActionResult**.
- Acompanhe o último carimbo de data/hora de logon de um PC na nuvem pela propriedade **lastLoginResult**.
- Rastreie a data em que uma [imagem de dispositivo PC na nuvem](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) se torna indisponível pela propriedade **expireDate**.
- Acompanhe o status do sistema operacional em uma [imagem de dispositivo de PC na nuvem](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) pela propriedade **osStatus**.
- [Crie](/graph/api/rbacapplication-post-roledefinitions?view=graph-rest-beta&preserve-view=true), [atualize](/graph/api/unifiedroledefinition-update?view=graph-rest-beta&preserve-view=true) e [exclua](/graph/api/unifiedroledefinition-delete?view=graph-rest-beta&preserve-view=true)um objeto[unifiedRoleDefinition](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true) para um provedor RBAC do PC na nuvem.

### <a name="education"></a>Educação
- [Acompanhe as alterações](delta-query-overview.md) nos recursos [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true) e [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta&preserve-view=true).
- Especifique [tarefa](/graph/api/resources/educationassignment) ser adicionada somente aos calendários dos alunos usando a propriedade **addToCalendarAction**.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- [Obter](/graph/api/application-get?view=graph-rest-beta&preserve-view=true) os detalhes de certificação de um [aplicativo](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) pela propriedade de **certificação**. A propriedade é definida apenas quando o aplicativo é certificado pelo [Programa de Conformidade do Aplicativo do Microsoft 365](/microsoft-365-app-certification/docs/enterprise-app-certification-guide).  
- [Inclua](/graph/api/permissiongrantpolicy-post-includes?view=graph-rest-beta&preserve-view=true) ou [exclua](/graph/api/permissiongrantpolicy-post-excludes?view=graph-rest-beta&preserve-view=true) a certificação como uma [condição](/graph/api/resources/permissionGrantConditionSet?view=graph-rest-beta&preserve-view=true) em uma [política de concessão de permissão](/graph/api/resources/permissiongrantpolicy?view=graph-rest-beta&preserve-view=true) pela propriedade **certifiedClientApplicationsOnly** de [permissionGrantConditionSet](/graph/api/resources/permissionGrantConditionSet?view=graph-rest-beta&preserve-view=true).

### <a name="search--index"></a>Pesquisa | Índice
Use a operação [atualizar](/graph/api/externalconnectors-schema-update?view=graph-rest-beta&preserve-view=true) para atualizar as propriedades dos itens em um esquema de [conexão](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true), incluindo seus aliases e rótulos.

### <a name="teamwork"></a>Trabalho em equipe
- [Liste](/graph/api/teams-list?view=graph-rest-beta&preserve-view=true) todas as equipes em uma organização.

### <a name="to-do-tasks"></a>Tarefas pendentes
- Para prever a capacidade de gerenciar em um único lugar todas as tarefas de várias fontes (como mensagens do Outlook, chats do Teams, documentos do OneDrive):
  - Use a [Api de Tarefas Pendentes](/graph/api/resources/tasks-overview?view=graph-rest-beta&preserve-view=true) e acesse-o no novo ponto de extremidade `https://graph.microsoft.com/beta/me/tasks/`.
  - Use o segmento `allTasks` para obter todas as tarefas de um usuário: `https://graph.microsoft.com/beta/me/tasks/alltasks`.
  - Diferencie entre uma lista de tarefas interna (como **Email sinalizado** ou **Tarefas**) e uma lista de tarefas definida pelo usuário. Uma lista de tarefas integrada é representada pelo recurso [wellKnownTaskList](/graph/api/resources/wellknowntasklist?view=graph-rest-beta&preserve-view=true) e uma lista de tarefas definida pelo usuário é representada pelo recurso [taskList](/graph/api/resources/tasklist?view=graph-rest-beta&preserve-view=true).
  - Diferencie entre o tipo de tarefas atualmente definido, [tarefa](/graph/api/resources/task?view=graph-rest-beta&preserve-view=true), de um tipo base [baseTask](/graph/api/resources/basetask?view=graph-rest-beta&preserve-view=true).
- Divida uma tarefa mais [tarefa](/graph/api/resources/task?view=graph-rest-beta&preserve-view=true) em subtarefas menores e mais acionáveis. Cada subtarefa é representada por um [checklistItem](/graph/api/resources/checklistitem?view=graph-rest-beta&preserve-view=true) recurso.
- [Mover](/graph/api/basetask-move?view=graph-rest-beta&preserve-view=true) uma tarefa entre listas.
- Consulte esta [ postagem do blog ](https://devblogs.microsoft.com/microsoft365dev/announcing-the-public-preview-of-to-do-tasks-api/) para obter mais detalhes e migre todos os aplicativos existentes que usam a [API To Do anterior](/graph/api/resources/todo-overview?view=graph-rest-beta&preserve-view=true) para a [API To Do mais recente](/graph/api/resources/tasks-overview?view=graph-rest-beta&preserve-view=true).


## <a name="november-2021-new-and-generally-available"></a>Novembro de 2021: Novo e geralmente disponível ao público

### <a name="files"></a>Arquivos
Obtenha o estado de uma unidade a partir de um horário específico definindo o carimbo de data/hora codificado no URL codificado. Confira um [exemplo](/graph/api/driveitem-delta#example-4-retrieving-delta-results-using-a-timestamp).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
- Execute [campanhas](/graph/api/resources/authenticationMethodsRegistrationCampaign) e [imponha os usuários a se registrarem](/graph/api/resources/registrationEnforcement) no momento da entrada para configurar os métodos de autenticação direcionados.
-  Configurar um [provedor de identidade Apple](/graph/api/resources/applemanagedidentityprovider) em um locatário do Azure AD B2C.

## <a name="november-2021-new-in-preview-only"></a>Novembro de 2021: Novo somente na pré-visualização

### <a name="cloud-communications--online-meeting"></a>Comunicações na nuvem | Reunião online
Admita automaticamente novos tipos de participantes em uma reunião online e ignore o lobby da reunião:
- Somente pessoas convidadas pelo organizador.
- Somente os participantes da mesma empresa.

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
- Defina uma [configuração](/graph/api/resources/cloudPcDomainJoinConfiguration?view=graph-rest-beta&preserve-view=true) de como um dispositivo de PC na nuvem provisionado pode ingressar no Azure Active Directory (Microsoft Azure AD): somente nuvem e ingressar somente no Microsoft Azure AD, ou híbrido e ingressar no Active Directory local e no Microsoft Azure AD.
- Obtenha o [recurso de imagem da galeria](/graph/api/resources/cloudPcGalleryImage?view=graph-rest-beta&preserve-view=true) da organização atual que pode ser usado para provisionar um PC na nuvem.

### <a name="devices-and-apps--device-updates"></a>Dispositivos e aplicativos | Atualizações do dispositivo
- Use as [configurações de salvaguarda](/graph/api/resources/windowsupdates-safeguardSettings?view=graph-rest-beta&preserve-view=true) para recusar as proteções contra prováveis problemas em uma implantação.
- Suporte para um [estado de implantação](/graph/api/resources/windowsupdates-deploymentState?view=graph-rest-beta&preserve-view=true) em que uma implantação está com defeito devido ao conteúdo não ser mais implantável, por exemplo, no fim do serviço.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- Defina e atribua [atributos de segurança personalizado ](/graph/api/resources/custom-security-attributes-overview?view=graph-rest-beta&preserve-view=true) aos objetos do Microsoft Azure AD. Use esses atributos para armazenar informações, categorizar objetos ou impor um controle de acesso refinado sobre recursos específicos do Azure. Use esses atributos com o [Controle de acesso baseado em atributo do Azure](/azure/role-based-access-control/conditions-overview) (Azure ABAC).
- [Crie um grupo dentro de uma unidade administrativa](/graph/api/administrativeunit-post-members?view=graph-rest-beta&preserve-view=true).

### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
[Os relatórios de uso do Microsoft 365](/graph/api/resources/report?view=graph-rest-beta&preserve-view=true) no tipo de saída JSON não são mais fortemente tipados e são do tipo `Edm.Stream`. Para obter mais informações, consulte [Alterações da propriedade OData na API de relatórios de uso do Microsoft 365 no Microsoft Graph](https://devblogs.microsoft.com/microsoft365dev/odata-property-changes-to-microsoft-365-usage-reports-api-in-microsoft-graph/).

### <a name="teamwork"></a>Trabalho em equipe
Marque um chat como [lido](/graph/api/chat-markChatReadForUser?view=graph-rest-beta&preserve-view=true) ou [não lido](/graph/api/chat-markchatunreadforuser?view=graph-rest-beta&preserve-view=true) para um usuário.


## <a name="october-2021-new-and-generally-available"></a>Outubro de 2021: novo e em disponibilidade geral

### <a name="cloud-communications--calls"></a>Comunicações na nuvem | Chamadas
- [Transferir](/graph/api/call-transfer) uma chamada ponto a ponto ativa.
- Transferir uma chamada em grupo para um determinado participante (beneficiário).

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões online
Oferece suporte a vários números de chamada tarifada e de chamada gratuita para acesso telefônico ([audioconferência](/graph/api/resources/audioConferencing)) de uma [reunião online](/graph/api/resources/onlinemeeting).

### <a name="education"></a>Educação
Suporta um arquivo de [mídia](/graph/api/resources/educationMediaResource) ou algum outro [recurso genérico externo](/graph/api/resources/educationExternalResource) como um [recurso de atribuição](/graph/api/resources/educationassignmentresource).

### <a name="identity-and-access--applications"></a>Identidade e acesso | Aplicativos
- Para direcionar a experiência de consentimento de um [aplicativo](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true), especifique os [recursos do que o aplicativo precisa para acessar](/graph/api/resources/requiredresourceaccess?view=graph-rest-beta&preserve-view=true), incluindo o conjunto de permissões delegadas do OAuth 2.0 e funções de aplicativo que o aplicativo exige.
- Limite o número de APIs necessárias a 50 e as permissões necessárias a 400 por aplicativo.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- Defina os [atributos de extensão](/graph/api/resources/onpremisesextensionattributes) para um [dispositivo](/graph/api/resources/device) e gerencie-os no Azure Active Directory na [criação](/graph/api/device-post-devices) ou [atualização](/graph/api/device-update) do dispositivo.
- [Obtenha uma chave de recuperação do BitLocker](/graph/api/bitlockerrecoverykey-get) em nome do usuário conectado que é o proprietário do dispositivo ou em uma função adequada. Obter uma chave de recuperação gera um [log de auditoria](/azure/active-directory/reports-monitoring/concept-audit-logs), em paridade com a experiência do usuário final.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Especifique uma lista de usuários adicionais ou membros do grupo a serem notificados sobre o andamento da análise de acesso, na propriedade **additionalNotificationRecipients** de um [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
Especifique os dispositivos em uma [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy), como parte das [condições](/graph/api/resources/conditionalAccessConditionSet) que regem quando a política se aplica.

### <a name="personal-contacts"></a>Contatos pessoais
Habilite o suporte para permissões delegadas (`Contacts.Read` ou `Contacts.ReadWrite`) para recursos de [profilePhoto](/graph/api/resources/profilephoto?view=graph-rest-beta&preserve-view=true) em contas Microsoft pessoais.

### <a name="teamwork"></a>Trabalho em equipe
- [Obtenha todas as mensagens de chat em todos os canais](/graph/api/channel-getallmessages) em uma [equipe](/graph/api/resources/team).
- [Obtenha todas mensagens de todos os chats](/graph/api/chats-getallmessages) em que um usuário participa, incluindo chats individuais, chats em grupo e chats de reunião.
- Confira os [modelos de licenciamento e pagamento](teams-licenses.md) que se aplicam às APIs do Microsoft Teams no Microsoft Graph.

### <a name="users"></a>Usuários
As licenças de usuário dos serviços Azure Active Directory (Azure AD) agora suportam um data/hora para quando o [estado da atribuição de licença](/graph/api/resources/licenseassignmentstate) for atualizado pela última vez. 

## <a name="october-2021-new-in-preview-only"></a>Outubro de 2021: novo apenas na pré-visualização

### <a name="applications"></a>Aplicativos
Use [credenciais de identidade federada](/graph/api/resources/federatedidentitycredential?view=graph-rest-beta&preserve-view=true) para gerenciar as credenciais de um aplicativo e permitir que os aplicativos de nuvem de uma organização acessem o Azure AD sem usar segredos e certificados.

### <a name="cloud-communications--calls"></a>Comunicações na nuvem | Chamadas
Identifique um [participante](/graph/api/resources/participantInfo?view=graph-rest-beta&preserve-view=true) da chamada, usando a propriedade **participantId** do tipo de recurso [participantInfo](/graph/api/resources/participantInfo?view=graph-rest-beta&preserve-view=true).

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões online
Habilite o [registro de reunião](/graph/api/resources/meetingregistration?view=graph-rest-beta&preserve-view=true) e organize reuniões online como um [webinar](/office/get-started-with-teams-webinars-42f3f874-22dc-4289-b53f-bbc1a69013e3). Associe a reunião a uma página de registro e escolha inscrever todos ou apenas os membros da organização como [inscritos da reunião](/graph/api/resources/meetingregistrant?view=graph-rest-beta&preserve-view=true). 

### <a name="customer-booking"></a>Reserva de clientes
- Oferece suporte aos seguintes atributos para um [serviço de reserva](/graph/api/resources/bookingService?view=graph-rest-beta&preserve-view=true):
  - Habilite o envio de notificações por SMS aos clientes para os compromissos (propriedade **smsNotificationsEnabled**).
  - A URL que os clientes podem usar para acessar o serviço (propriedade **webUrl**).
- Reserve um [compromisso](/graph/api/resources/bookingappointment?view=graph-rest-beta&preserve-view=true) com um ou mais dos seguintes atributos:
  - Especifique o fuso horário do cliente (propriedade **customerTimeZone**).
  - Especifique a URL para um compromisso online (propriedade **joinWebUrl**).
  - Habilite as notificações por SMS para o cliente para o compromisso (propriedade **smsNotificationsEnabled**).
- Especifique um ou mais endereços e números de telefone para um [cliente](/graph/api/resources/bookingcustomer?view=graph-rest-beta&preserve-view=true).
- Especifique o fuso horário para um [membro da equipe](/graph/api/resources/bookingStaffMember?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Cloud PC
[Liste](/graph/api/virtualendpoint-list-serviceplans?view=graph-rest-beta&preserve-view=true) os [planos de serviço do Windows 365](/graph/api/resources/cloudPcServicePlan?view=graph-rest-beta&preserve-view=true) que uma organização assina para seus PCs na nuvem. Em cada [tipo de plano de serviço](/graph/api/resources/cloudPcServicePlan?view=graph-rest-beta&preserve-view=true#cloudpcserviceplantype-values) (business ou enterprise), uma organização pode optar por assinar de uma variedade de configurações de plano que variam de acordo com atributos como vCPU, RAM e armazenamento.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
Especifique as [principais definições de configuração de credenciais](/graph/api/resources/keycredentialconfiguration?view=graph-rest-beta&preserve-view=true) que podem ser [configuradas para permitir restrições a um aplicativo ou entidade de serviço](/graph/api/resources/appmanagementconfiguration?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Habilite as seguintes [configurações](/graph/api/resources/assignmentReviewSettings?view=graph-rest-beta&preserve-view=true) adicionais para revisar uma [política de atribuição de pacote de acesso](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true):
- Comportamento padrão se a solicitação não for revisada em uma determinado período (propriedade **accessReviewTimeoutBehavior**).
- Exibir recomendações ao revisor (propriedade **isAccessRecommendationEnabled**).
- Exigir que o revisor forneça justificativa para a aprovação (propriedade **isApprovalJustificationRequired** ).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- Especifique se as configurações de [política de avaliação de acesso contínuo](/graph/api/resources/continuousAccessEvaluationPolicy?view=graph-rest-beta&preserve-view=true) devem ser ou foram migradas para a [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- Como parte de um [acesso condicional](/azure/active-directory/conditional-access/overview) do Azure Active Directory, use um novo controle de sessão, [continuousAccessEvaluationSessionControl](/graph/api/resources/continuousAccessEvaluationSessionControl?view=graph-rest-beta&preserve-view=true), para avaliar continuamente o acesso e tomar decisões de acesso. 

### <a name="search--index"></a>Pesquisa | Índice
- Especifique as [configurações](/graph/api/resources/externalconnectors-searchsettings?view=graph-rest-beta&preserve-view=true) para a experiência de pesquisa de conteúdo em uma [conexão externa](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true). Por exemplo, um [modelo de exibição](/graph/api/resources/externalconnectors-displaytemplate?view=graph-rest-beta&preserve-view=true) para resultados de pesquisa e uma [regra](/graph/api/resources/externalconnectors-propertyRule?view=graph-rest-beta&preserve-view=true) para selecionar o modelo de exibição.
- Relacione um ou mais [grupos externos](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-beta&preserve-view=true) para uma [conexão externa](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true). Por exemplo, um grupo externo, como uma unidade de negócio ou uma equipe de trabalho, pode determinar as permissões para o conteúdo na fonte de dados representada pela conexão externa.
- Opcionalmente, pode especificar a ID de um aplicativo do Teams em uma [conexão externa](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true) na propriedade **connectorId**.

### <a name="users"></a>Usuários
[Valide uma senha](/graph/api/user-validatePassword?view=graph-rest-beta&preserve-view=true) em tempo real em relação à política de validação de senha de uma organização, à medida que um usuário digita a senha. Obtenha [informações detalhadas da validação](/graph/api/resources/passwordValidationInformation?view=graph-rest-beta&preserve-view=true) de acordo com as regras da política.


## <a name="september-2021-new-and-generally-available"></a>Setembro de 2021: novo e disponível para o público em geral

### <a name="cloud-communications--calls"></a>Comunicações na nuvem | Chamadas
- Colocar um [participante](/graph/api/resources/participant) em espera e tocar música em segundo plano usando a ação [startHoldMusic](/graph/api/participant-startHoldMusic).
- Reincorporar um participante colocado em espera em uma chamada anteriormente usando a ação [stopHoldMusic](/graph/api/participant-stopHoldMusic).

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões on-line
- Obtenha o fluxo de conteúdos de um relatório de participante de um [evento ao vivo do Teams](/microsoftteams/teams-live-events/what-are-teams-live-events).
- Obtenha ou defina a opção para gravar automaticamente uma [reunião online](/graph/api/resources/onlineMeeting).
- Use `OnlineMeetingArtifact.Read.All` como delegada ou permissão de aplicativo para ler artefatos de reuniões on-line. Para obter mais informações, consulte [permissões de reuniões on-line](permissions-reference.md#online-meetings-permissions).

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
O status da impressora em nuvem inclui todos os valores padrão [Internet Printing Protocol (IPP)](https://www.iana.org/assignments/ipp-registrations/ipp-registrations.xhtml).

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações mensais do Intune para a versão v1.0. No [changelog](https://developer.microsoft.com/graph/changelog), defina o filtro **Data** para setembro de 2021 e procure uma seção com esse mesmo título.

### <a name="files"></a>Arquivos
- Obtenha os detalhes de qualquer vírus detectado em um [driveItem](/graph/api/resources/driveItem) por meio de uma propriedade de **malware**.
- Use a função [delta](/graph/api/driveitem-delta) para acompanhar as alterações não apenas no diretório raiz, mas também em outras pastas dentro de uma unidade.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
Os provedores de controle de acesso baseado em função (RBAC) podem [gerenciar funções](/graph/api/resources/rolemanagement) do Azure Active Directory, [definindo ações de funções](/graph/api/resources/unifiedroledefinition)que podem ser realizadas em recursos específicos e [atribuindo funções](/graph/api/resources/unifiedroleassignment) aos usuários com base em tais definições de função, fornecendo o acesso correspondente a esses recursos.

### <a name="search--query"></a>Pesquisa | Consulta
- Agregue os resultados de pesquisa do tipo numéricos ou cadeia de caracteres que são importados pelos [Conectores do Microsoft Graph](/microsoftsearch/connectors-overview) e que estão definidos para serem refináveis no [esquema](/graph/api/resources/schema). Veja mais informações sobre o [refinamento dos resultados de pesquisa usando agregações](search-concept-aggregation.md).
- [Classifique](/graph/api/resources/search-api-overview#sort-search-results) os resultados de pesquisa do OneDrive e do SharePoint em qualquer propriedade classificável. Para obter mais informações, consulte [Uso da API de Pesquisa da Microsoft para classificar resultados da pesquisa](search-concept-sort.md).

### <a name="teamwork"></a>Trabalho em equipe
Usar uma única ação [provisionEmail](/graph/api/channel-provisionemail) para obter o endereço de email de um [canal](/graph/api/resources/channel), se houver, ou criar um, se não houver. Usar a ação [removeEmail](/graph/api/channel-removeemail) para remover o endereço de email.

### <a name="workbooks-and-charts"></a>Pastas de trabalho e gráficos
Criar linhas de tabela de forma assíncrona. Para um melhor desempenho, uma boa prática para criar várias linhas de tabela é agrupá-las em uma operação do tipo [criar tableRow](/graph/api/table-post-rows) e realizar a operação de forma assíncrona. Prossiga com a operação [GET workbookOperation](/graph/api/workbookoperation-get) e a função [tableRowOperationResult](/graph/api/workbook-tableRowOperationResult) para obter o novo recurso [workbookTableRow](/graph/api/resources/workbooktablerow).


## <a name="september-2021-new-in-preview-only"></a>Setembro de 2021: novos somente em versão prévia

### <a name="applications"></a>Aplicativos
Os aplicativos que usam fluxos de logon único do Security Assertion Markup Language (SAML) podem especificar um URI de redirecionamento padrão (propriedade **defaultRedirectUri** do [aplicativo](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)) ou identificar um URI de redirecionamento específico no qual os usuários são enviados para fazer logon (propriedade **redirectUriSettings** do [webApplication](/graph/api/resources/webapplication?view=graph-rest-beta&preserve-view=true)). 

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões on-line
Obter o número total de participantes em um [relatório de presença de reunião](/graph/api/resources/meetingattendancereport?view=graph-rest-beta&preserve-view=true) de uma [reunião on-line](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true).

### <a name="compliance--ediscovery"></a>Conformidade | Descoberta eletrônica
A operação [criar caso](/graph/api/ediscovery-case-post?view=graph-rest-beta&preserve-view=true) sempre cria casos em formato grande. Isso expande o limite do tamanho de caso para acomodar um volume total de dados e um número total de itens mais altos. Para obter mais detalhes, consulte [vantagens de casos grandes](/microsoft-365/compliance/advanced-ediscovery-large-cases?view=o365-worldwide&preserve-view=true#benefits-of-large-cases).

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
- [Reprovisionar um computador na nuvem](/graph/api/manageddevice-reprovisioncloudpc?view=graph-rest-beta&preserve-view=true) como uma área de trabalho virtual gerenciada na nuvem registrada no Intune.
- [Redimensionar um computador na nuvem](/graph/api/manageddevice-resizecloudpc?view=graph-rest-beta&preserve-view=true) atualizando-o ou rebaixando-o para outra configuração com uma CPU virtual (vCPU) e um tamanho de armazenamento novos.
- [Configurar](/graph/api/virtualendpoint-post-onpremisesconnections?view=graph-rest-beta&preserve-view=true), [listar](/graph/api/virtualendpoint-list-onpremisesconnections?view=graph-rest-beta&preserve-view=true) e [executar verificações de integridade](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) em [conexões de rede locais](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true) para provisionar PCs na nuvem.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações mensais do Intune para a versão beta. No [changelog](https://developer.microsoft.com/graph/changelog), defina o filtro **Data** para setembro de 2021 e procure uma seção com esse mesmo título.

### <a name="education"></a>Educação
- Permitir que os professores [reatribuam](/graph/api/educationsubmission-reassign?view=graph-rest-beta&preserve-view=true) o [envio](/graph/api/resources/educationsubmission?view=graph-rest-beta&preserve-view=true) de uma tarefa ao aluno com comentários para revisão.
- Suporte para adicionar tarefas apenas aos calendários dos alunos se você usar o cabeçalho de solicitação `Prefer: include-unknown-enum-members` para operações nos recursos [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) ou [educationAssignmentDefaults](/graph/api/resources/educationassignmentdefaults?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
[Excluir](/graph/api/accesspackageassignmentrequest-delete?view=graph-rest-beta&preserve-view=true) um [accessPackageAssignmentRequest](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true) para remover uma solicitação negada ou concluída.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
- Permitir que os usuários executem a autenticação multifatorial usando um [token de software OATH](/graph/api/resources/softwareOathAuthenticationMethod?view=graph-rest-beta&preserve-view=true). Um token de software OATH é um gerador de números baseado em software que usa a Senha de Uso Único Baseada em Tempo (TOTP) padrão OATH.
- Identifique se a correspondência de números está habilitada ou desabilitada para autenticação multifator pela política no Azure AD, usando a propriedade **numberMatchingRequiredState** do [microsoftAuthenticatorAuthenticationMethodTarget](/graph/api/resources/microsoftAuthenticatorAuthenticationMethodTarget?view=graph-rest-beta&preserve-view=true).
- Identifique se um contexto adicional do usuário deve ser mostrado na notificação do aplicativo autenticador, usando a propriedade **displayAppInformationRequiredState** do [microsoftAuthenticatorAuthenticationMethodTarget](/graph/api/resources/microsoftAuthenticatorAuthenticationMethodTarget?view=graph-rest-beta&preserve-view=true).
- Use o [fluxo de usuário B2C](/graph/api/resources/b2cidentityuserflow?view=graph-rest-beta&preserve-view=true) e o [fluxo de usuário de inscrição de autoatendimento](/graph/api/resources/b2xidentityuserflow?view=graph-rest-beta&preserve-view=true) em favor da API de [fluxo de usuário](/graph/api/resources/identityuserflow?view=graph-rest-beta&preserve-view=true) anterior, que foi preterida.

### <a name="security--attack-simulation-and-training"></a>Segurança | Treinamento e simulação de ataque
O lançamento da API para [treinamento e simulação de ataque](/microsoft-365/security/office-365-security/attack-simulation-training?view=o365-worldwide&preserve-view=true), que é um serviço disponível como parte do [Microsoft Defender para Office 365](/microsoft-365/security/office-365-security/defender-for-office-365?view=o365-worldwide&preserve-view=true). A API permite que os administradores de locatários [listem os exercícios e treinamentos de simulação lançados](/graph/api/attacksimulationroot-list-simulations?view=graph-rest-beta&preserve-view=true) e obtenham [relatórios](/graph/api/resources/report-m365defender-reports-overview?view=graph-rest-beta&preserve-view=true) sobre os insights derivados dos comportamentos online dos usuários nas simulações de phishing.

## <a name="august-2021-new-and-generally-available"></a>Agosto de 2021: novo e disponível para o público em geral

### <a name="cloud-communications--calls"></a>Comunicações na nuvem | Chamadas
Um [participante](/graph/api/resources/participant) pode incluir metadados como um blob de dados na lista de participantes de uma [chamada](/graph/api/resources/call).

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões on-line
- Crie uma [reunião on-line](/graph/api/resources/onlinemeeting) como evento ao vivo, definindo as [configurações de transmissão](/graph/api/resources/broadcastMeetingSettings) e as [informações dos participantes da reunião](/graph/api/resources/meetingparticipantinfo) com a função de produtor. Confira um [exemplo](/graph/api/application-post-onlinemeetings#example-2-create-a-live-event-with-user-token).
- Habilitar, desabilitar ou limitar a duração do chat de uma reunião online usando a propriedade **allowMeetingChat**.
- Habilitar ou desabilitar reações a uma reunião online usando a propriedade **allowTeamworkReactions**.
- Permitir que um participante ligue sua câmera ou seus microfones usando, respectivamente, as propriedades **allowAttendeeToEnableCamera** ou **allowAttendeeToEnableMic**.

### <a name="cloud-communications--presence"></a>Comunicações na nuvem | Presença
- [Definir o estado de presença de um usuário](/graph/api/presence-setpresence), que é um estado agregado em cada cliente do Teams (desktop, celular ou web).
- [Limpar a sessão de presença](/graph/api/presence-clearpresence) para um usuário.


### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações mensais do Intune para a versão v1.0. Configure o filtro **Data** para agosto de 2021 e procure uma seção com esse mesmo cabeçalho.

### <a name="devices-and-apps--service-health-and-communications"></a>Dispositivos e aplicativos | Integridade do serviço e comunicações
GA da [API de comunicações de serviço](service-communications-concept-overview.md) no Microsoft Graph para acessar o status de integridade e as postagens do centro de mensagens sobre os serviços em nuvem da Microsoft.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Obtenha uma coleção de escopos de revisão de acesso usados para definir revisores e revisores substitutos para uma [instância de revisores de acesso](/graph/api/resources/accessReviewInstance).

### <a name="sites-and-lists--taxonomy"></a>Sites e listas | Taxonomia
Acessar a taxonomia do [repositório de termos](/graph/api/resources/termstore-store) do SharePoint, a hierarquia que consiste de recursos de [grupo](/graph/api/resources/termstore-group), [conjunto](/graph/api/resources/termstore-set), e [termo](/graph/api/resources/termstore-term), e [relacionar](/graph/api/resources/termstore-relation) os recursos entre os termos.

### <a name="teamwork"></a>Trabalho em equipe
[Listar os chats](/graph/api/chat-list) dos quais um usuário faz parte, em um contexto delegado.

## <a name="august-2021-new-in-preview-only"></a>Agosto de 2021: novos somente em versão prévia

### <a name="cloud-communications--calls"></a>Comunicações na nuvem | Chamadas
- Colocar um [participante](/graph/api/resources/participant?view=graph-rest-beta&preserve-view=true) em espera e tocar música em segundo plano usando a ação [startHoldMusic](/graph/api/participant-startHoldMusic?view=graph-rest-beta&preserve-view=true).
- Reincorporar um participante colocado em espera em uma chamada anteriormente usando a ação [stopHoldMusic](/graph/api/participant-stopHoldMusic?view=graph-rest-beta&preserve-view=true).

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões on-line
Configurar uma [reunião on-line](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) para gravar automaticamente.

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
[Encerrar o período de tolerância](/graph/api/cloudPC-endGracePeriod?view=graph-rest-beta&preserve-view=true) para um computador na nuvem. O período de tolerância permite que os usuários acessem os computadores na nuvem até sete dias antes da ocorrência do desprovisionamento. Encerrar o período de tolerância imediatamente desprovisiona o computador na nuvem sem aguardar os sete dias.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações mensais do Intune para a versão beta. Configure o filtro **Data** para agosto de 2021 e procure uma seção com esse mesmo cabeçalho.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- [Reprocesse](/graph/api/accesspackageassignmentrequest-reprocess?view=graph-rest-beta&preserve-view=true) uma [solicitação de atribuição de pacote de acesso](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true) para repetir automaticamente a solicitação de acesso de um usuário ao pacote.
- [Reprocesse](/graph/api/accesspackageassignment-reprocess?view=graph-rest-beta&preserve-view=true)[ uma atribuição de pacote de acesso](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true) para reavaliar e impor automaticamente as atribuições de um usuário.
- [Obtenha um conjunto de requisitos de política](/graph/api/accesspackage-getapplicablepolicyrequirements?view=graph-rest-beta&preserve-view=true) para criar uma [solicitação de atribuição para um pacote de acesso](/graph/api/resources/accesspackageassignmentrequestrequirements?view=graph-rest-beta&preserve-view=true).
- Obtenha uma coleção de recursos de [revisão de acesso](/graph/api/resources/accessreviewreviewer?view=graph-rest-beta&preserve-view=true) que é usada para definir revisores contatados para uma [instância de revisores de acesso](/graph/api/resources/accessReviewInstance?view=graph-rest-beta&preserve-view=true).
- Obtenha ou defina a duração de inatividade a partir da qual as recomendações são definidas nas [configurações de agendamento de uma revisão de acesso](/graph/api/resources/accessReviewScheduleSettings?view=graph-rest-beta&preserve-view=true) usando a propriedade **RecommendationLookBackDuration**.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- As organizações podem usar [políticas para aplicar as melhores práticas para aplicativos usando métodos de autenticação de aplicativos](/graph/api/resources/applicationauthmethodpolicy?view=graph-rest-beta&preserve-view=true). Essas políticas podem ser aplicadas a [aplicativos e entidades de serviço específicos](/graph/api/resources/appmanagementpolicy?view=graph-rest-beta&preserve-view=true) ou a [todos os aplicativos e entidades de serviço em um locatário](/resources/tenantappmanagementpolicy?view=graph-rest-beta&preserve-view=true).
- Suporte para paginação na propriedade de navegação **appRoleAssignments** para [usuários](/api/user-list-approleassignments?view=graph-rest-beta&preserve-view=true), [grupos](/api/group-list-approleassignments?view=graph-rest-beta&preserve-view=true) e [entidades de serviço](/api/serviceprincipal-list-approleassignments?view=graph-rest-beta&preserve-view=true).
- Permitir que um locatário do Azure Active Directory (Azure AD) defina uma [federação com outra organização cujo provedor de identidade (IdP) ofereça suporte ao protocolo SAML ou WS-Fed](/graph/api/resources/samlOrWsFedExternalDomainFederation?view=graph-rest-beta&preserve-view=true). Isso permite que o locatário do Azure AD dê acesso aos seus recursos para usuários convidados.

### <a name="teamwork"></a>Trabalho em equipe
- Obter [informações sobre uma reunião on-line](/graph/api/resources/teamworkOnlineMeetingInfo?view=graph-rest-beta&preserve-view=true) que esteja associada a um [chat](/api/resources/chat?view=graph-rest-beta&preserve-view=true).
- Obter o identificador do locatário no qual um **chat** é criado.

### <a name="users"></a>Usuários
Use os últimos valores de data/hora de login interativo e não interativo do [signInActivity](/graph/api/resources/signInActivity?view=graph-rest-beta&preserve-view=true) dos usuários para [gerenciar contas inativas](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts).


## <a name="july-2021-new-and-generally-available"></a>Julho de 2021: Novo e disponível para o público em geral

### <a name="cloud-communications--calls"></a>Comunicações na nuvem | Chamadas
Suporte para um limite de capacidade para o número de participantes que um aplicativo pode controlar ao [atender](/graph/api/call-answer) uma [chamada](/graph/api/resources/call), em organizações que adotam [gravação baseada em políticas do Teams](/microsoftteams/teams-recording-policy).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- GA de provedores de identidade que compartilham um tipo de base comum [identityProviderBase](/graph/api/resources/identityproviderbase):
  - Provedores de identidade internos para cenários do Azure AD B2B em um locatário do Azure AD. Esses provedores podem oferecer suporte ao Azure AD, conta Microsoft (MSA) ou senhas únicas de email.
  - Provedores de identidade social em um locatário do Azure AD B2C para permitir que os usuários se inscrevam e entrem no serviço usando uma conta de mídia social, como Microsoft, Google, Facebook, Amazon, LinkedIn ou Twitter.
- Descontinuação da API do [provedor de identidade](/graph/api/resources/identityprovider) anterior.

### <a name="users"></a>Usuários
Permitir que um usuário [altere sua própria senha](/graph/api/user-changepassword) sem exigir uma função de administrador.


## <a name="july-2021-new-in-preview-only"></a>Julho de 2021: Novo somente para visualização

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | PC na nuvem
Uma [verificação de integridade](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) de conexão local pode identificar mais alguns tipos de erros de verificação de integridade:
- A conta do computador do PC na Nuvem não foi encontrada na unidade organizacional (`adJoinCheckComputerObjectAlreadyExists`).
- O objeto do PC na Nuvem não foi encontrado no Microsoft Azure Active Directory (`azureAdDeviceSyncCheckDeviceNotFound`).
- Tempo limite para verificar se um objeto do PC na nuvem foi sincronizado com o Microsoft Azure Active Directory (`azureAdDeviceSyncCheckLongSyncCircle`). 

Consulte a [referência](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true#cloudpconpremisesconnectionhealthcheckerrortype-values) para obter detalhes e as ações corretivas recomendadas.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações mensais do Intune para a versão beta. Defina o filtro **Data** para julho de 2021 e procure uma seção com esse mesmo título.

### <a name="devices-and-apps--multi-tenant-management"></a>Dispositivos e aplicativos | Gerenciamento de vários locatários
Lançamento da [API do Microsoft 365 Lighthouse](managedtenants-concept-overview.md) que permite que os Provedores de Serviços Gerenciados (MSPs) gerenciem remotamente vários locatários de clientes em escala para conformidade e detecção de ameaças, e ajudam a manter os dispositivos dos locatários em um estado íntegro e seguro.

### <a name="education"></a>Educação
- Obtenha uma contagem de erros e uma mensagem de status como parte do [status de uma sincronização de dados escolares](/graph/api/resources/educationsynchronizationprofilestatus?view=graph-rest-beta&preserve-view=true).
- Obtenha `extracting` ou `validating` como possíveis estados de tal sincronização.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Obtenha uma coleção de erros no ciclo de vida de uma [instância de revisão de acesso](/graph/api/resources/accessreviewinstance?view=graph-rest-beta&preserve-view=true).

### <a name="search"></a>Pesquisa
- Use a [API de Pesquisa da Microsoft para recuperar informações sobre as pessoas](search-concept-person.md) que são mais relevantes para um usuário. A relevância é determinada pelos padrões de comunicação, colaboração e pelas relações comerciais do usuário. 
- Acesse a [API de indexação de conectores](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true) no sub-namespace microsoft.graph.externalConnectors.

### <a name="teamwork"></a>Trabalho em equipe
- [Inscreva-se para alterar notificações no recurso de chat](teams-changenotifications-chat.md).
- [Inscreva-se para alterar notificações de usuários em um chat](teams-changenotifications-chatmembership.md), em um [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) ou em uma [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) (ou seja, recursos de [conversationMember](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true)).
- Obtenha detalhes de um evento que aconteceu em um chat, canal ou equipe, acessando [eventMessageDetail](/graph/api/resources/EventMessageDetail?view=graph-rest-beta&preserve-view=true) de um [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) ou [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true). Por exemplo, membros adicionados a um canal ou chat, e a descrição da equipe atualizada.


## <a name="june-2021-new-and-generally-available"></a>Junho de 2021: novos e disponíveis para o público em geral

### <a name="applications"></a>Aplicativos
Obter ou definir o status de uma [aplicação](/graph/api/resources/application) ou [serviçoPrincipal](/graph/api/resources/serviceprincipal) para identificar se a Microsoft desativou a aplicação através da propriedade **disabledByMicrosoftStatus**. Os motivos de desabilitação incluem atividades suspeitas, abusivas ou mal-intencionadas ou uma violação do Contrato de Serviços Microsoft.

### <a name="change-notifications"></a>Alterar notificações
Estendeu o comprimento máximo de uma assinatura antes de expirar para os seguintes recursos:
- OneDrive [driveItem](/graph/api/resources/driveitem) e Microsoft Office SharePoint Online[lista](/graph/api/resources/list) de 3 a 30 dias.
- [grupo](/graph/api/resources/group), [usuário](/graph/api/resources/user), ou outros recursos de diretório de 3 a 29 dias.

### <a name="change-tracking"></a>Controle de alterações
Removida a limitação para rastrear mudanças em pastas não-root em OneDrive for Business e Microsoft Office SharePoint Online.

### <a name="education"></a>Educação
As APIs para a educação [serviços de atribuições](/graph/api/resources/educationassignment) agora estão disponíveis. 

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
GA da [revisão de acesso](/graph/api/resources/accessreviewsv2-overview) API. Confira a [visão geral](accessreviews-overview.md) e tutoriais para [rever o acesso a grupos de segurança](tutorial-accessreviews-securitygroup.md) e [acesso a grupos Microsoft 365](tutorial-accessreviews-m365group.md). Observe que o [API de revisão de acesso ao legado](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true) está sendo depreciado e deixará de retornar dados em maio de 2023.


## <a name="june-2021-new-in-preview-only"></a>Junho de 2021: Novo somente para visualização

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões online
Personalizar o controle de áudio e vídeo em [uma Reunião on-line](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true), habilitando ou desabilitando os participantes de ligar suas câmeras e microfones, através da **Permitindo aCâmera de Atendimento** e **Permitindo o Atendimento à Câmera de Habilitação**, respectivamente.

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
- [Atribuir](/graph/api/cloudpcusersetting-assign?view=graph-rest-beta&preserve-view=true) e gerenciar [cloudPcUserSetting](/graph/api/resources/cloudpcusersetting?view=graph-rest-beta&preserve-view=true) para permitir a administração local ou opção de auto-serviço para um usuário em um PC na nuvem. Atualmente, as atribuições podem ser feitas em nível de grupo (usuários pertencentes a um grupo Microsoft 365 ou grupo de segurança).
- [Obter](/graph/api/cloudpc-get?view=graph-rest-beta&preserve-view=true) algumas novas propriedades de um [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true): os nomes da política de provisionamento e da conexão local usada durante o provisionamento e a data/hora de término do período de cortesia pelo qual ocorre o reprovisionamento ou desprovisionamento.
- Suporte para mais status e tipos de erros em um [exame de saúde](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) em uma [conexão no local](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true).

### <a name="education"></a>Educação
- Os professores já podem selecionar o comportamento padrão de um calendário ao publicarem tarefas. Os professores podem controlar o comportamento do calendário da atribuição usando a propriedade **addToCalendarAction** do recurso [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true).
- Os professores já também podem definir um comportamento padrão para um calendário ao publicarem tarefas. Os professores podem controlar o comportamento do calendário padrão da atribuição usando a propriedade **addToCalendarAction** do recurso [educationAssignment](/graph/api/resources/educationAssignmentDefaults?view=graph-rest-beta&preserve-view=true).

### <a name="groups"></a>Grupos
Permitir que um [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) seja atribuído a uma função do Azure Active Directory na criação definindo a propriedade **isAssignableToRole**. Se definida, essa propriedade torna conveniente gerenciar funções para indivíduos – em vez de ter que atribuir uma função a cada pessoa individual, as pessoas qualificadas podem ingressar em um grupo e, atribuindo a função ao grupo, por padrão, atribuiria a função a cada nova pessoa que ingressasse no grupo. 

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Definir usuários ou membros do grupo a serem notificados sobre o progresso de uma [análise de acesso](/graph/api/resources/accessreviewsv2-overview?view=graph-rest-beta&preserve-view=true), usando a propriedade **additionalNotificationRecipients** da [definição de agendamento](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
Definir um filtro para incluir ou excluir dinamicamente dispositivos, usando o **deviceFilter** propriedade de [conditionalAccessDevices](/graph/api/resources/conditionalAccessDevices?view=graph-rest-beta&preserve-view=true).

### <a name="sites-and-lists"></a>Sites e listas
Criar ou obter um [sharingLink](/graph/api/resources/sharinglink?view=graph-rest-beta&preserve-view=true) existente para uma [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) chamando [createLink](/graph/api/listitem-createlink?view=graph-rest-beta&preserve-view=true).

### <a name="teamwork"></a>Trabalho em equipe
- [Obter](/graph/api/chat-get?view=graph-rest-beta&preserve-view=true) uma URL opaca para um [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true) através da **webUrl** propriedade.
- [Assinar notificações de mudança](/graph/webhooks?view=graph-rest-beta&preserve-view=true) de um [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true), [membro de conversação](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true), ou [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) recurso.
- Usar [consentimento específico de recursos](/microsoftteams/platform/graph-api/rsc/resource-specific-consent) permissões com as APIs para [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true), [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true), [chatMessage](/graph/api/resources/chatMessage?view=graph-rest-beta&preserve-view=true), [chatMessageHostedContent](/graph/api/resources/chatMessageHostedContent?view=graph-rest-beta&preserve-view=true), ou [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true).
- Obter uma lista de [permissões específicas de recursos concedidos](/graph/api/resources/resourcespecificpermissiongrant?view=graph-rest-beta&preserve-view=true) para uma [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true), que especifica as aplicações da equipe e as permissões específicas de recursos correspondentes que lhes foram concedidas.
- [Obter](/graph/api/teamsasyncoperation-get?view=graph-rest-beta&preserve-view=true) uma [operação assíncrona específica](/graph/api/resources/teamsasyncoperation?view=graph-rest-beta&preserve-view=true), ou [lista](/graph/api/chat-list-operations?view=graph-rest-beta&preserve-view=true) todas as operações assíncronas que funcionam em um [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).
- Pode especificar um aplicativo[Teams](/graph/api/resources/teamsapp?view=graph-rest-beta&preserve-view=true) ao [criar um chat](/graph/api/chat-post?view=graph-rest-beta&preserve-view=true).
- Usar uma única ação [provisionEmail](/graph/api/channel-provisionemail?view=graph-rest-beta&preserve-view=true) para obter o endereço de email de um [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true), se houver, ou criar um, se não houver. Usar a ação [removeEmail](/graph/api/channel-removeemail?view=graph-rest-beta&preserve-view=true) para remover o endereço de email.

### <a name="teamwork--shifts"></a>Trabalho em equipe | Turnos
- Suporte para as entidades [offerShiftRequest](/graph/api/resources/offershiftrequest?view=graph-rest-beta&preserve-view=true), [timeOff](/graph/api/resources/timeoff?view=graph-rest-beta&preserve-view=true), [timeOffReason](/graph/api/resources/timeoffreason?view=graph-rest-beta&preserve-view=true), e [timeOffRequest](/graph/api/resources/timeoffrequest?view=graph-rest-beta&preserve-view=true) para notificações de alteração síncronas.
- Suporte para gerenciar [recursos do cartão de ponto](/graph/api/resources/timecard?view=graph-rest-beta&preserve-view=true) e funcionalidades comuns, tais como [entrada do relógio](/graph/api/timecard-clockin?view=graph-rest-beta&preserve-view=true), [saída do relógio](/graph/api/timecard-clockout?view=graph-rest-beta&preserve-view=true), [partida inicial](/graph/api/timecard-startbreak?view=graph-rest-beta&preserve-view=true), [partida final](/graph/api/timecard-endbreak?view=graph-rest-beta&preserve-view=true), [confirmar](/graph/api/timecard-confirm?view=graph-rest-beta&preserve-view=true), e [substituir](/graph/api/timecard-replace?view=graph-rest-beta&preserve-view=true).


## <a name="may-2021-new-and-generally-available"></a>Maio de 2021: Novo e disponível para o público geral

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
Descubra quando uma impressora interagiu pela última vez com a Impressão Universal, usando a propriedade **lastSeenDateTime** da [impressora](/graph/api/resources/printer).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
Obtenha ou atualize a função de um usuário convidado usando a propriedade **guestUserRoleId** de [AuthorPolicy](/graph/api/resources/authorizationpolicy).

### <a name="mail"></a>Email
- [Crie rascunhos e envie mensagens do Outlook no formato MIME](outlook-send-mime-message.md), anexe assinaturas digitais S/MIME e criptografe o conteúdo da mensagem em S/MIME.
- Criar um [mailFolder](/graph/api/resources/mailfolder) como uma [pasta oculta](/graph/api/resources/mailfolder#hidden-mail-folders) ao [configurar a propriedade isHidden](/graph/api/user-post-mailfolders#example).

### <a name="microsoft-graph-toolkit"></a>Kit de ferramentas do Microsoft Graph
Experimente os seguintes novos recursos do Kit de Ferramentas do Microsoft Graph 2.2:
- Componentes de[arquivos](/graph/toolkit/components/file) e [lista de arquivos](/graph/toolkit/components/file-list)
- [Provedor de autenticação MSAL 2.0](/graph/toolkit/providers/msal2)
- [Biblioteca da Estrutura do SharePoint](/graph/toolkit/get-started/mgt-spfx)

### <a name="reports--azure-ad-activity-reports"></a>Relatórios | Relatórios de atividade do Microsoft Azure AD
GA da API de relatório para [listar](/graph/api/provisioningobjectsummary-list) as ações realizadas pelo serviço de provisionamento do Microsoft Azure AD e suas propriedades associadas. Alinhou a versão beta anterior à versão v1.0 da API.

## <a name="may-2021-new-in-preview-only"></a>Maio de 2021: Novo somente para visualização

### <a name="connecting-external-content"></a>Conectando conteúdo externo
- Esteja ciente dos [limites operacionais e à implementação](connecting-external-content-api-limits.md) durante a criação de conectores.
- Experimente a [API de conectores com o Postman](connecting-external-content-connectors-api-postman.md).

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
Solicite as permissões de aplicativos com menos privilégios, `CloudPC.Read.All` ou `CloudPC.ReadWrite.All`, para acessar os métodos dos seguintes recursos:
  - Operações de leitura e gravação, e do método de [reprovision](/graph/api/cloudpc-reprovision?view=graph-rest-beta&preserve-view=true) de [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true).
  - Operações de leitura e gravação, e do método [getSourceImages](/graph/api/cloudpcdeviceimage-getsourceimages?view=graph-rest-beta&preserve-view=true) de [cloudPcDeviceImage](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true).
  - Operações de leitura e gravação, e do método [updateAdDomainPassword](/graph/api/cloudpconpremisesconnection-updateaddomainpassword?view=graph-rest-beta&preserve-view=true) de [cloudPcOnPremisesConnection](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true).
  - Operações de leitura e gravação, e do método [assign](/graph/api/cloudpcprovisioningpolicy-assign?view=graph-rest-beta&preserve-view=true) de [cloudPcProvisioningPolicy](/graph/api/resources/cloudpcprovisioningpolicy?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações mensais do Intune para a versão beta. Defina o filtro **Data** para junho de 2021 e procure uma seção com esse mesmo título.

### <a name="education"></a>Educação
- [Configurar uma pasta de recursos do SharePoint](/graph/api/educationAssignment-setupresourcesfolder?view=graph-rest-beta&preserve-view=true) carregar e armazenar todos os recursos baseados em arquivo no mesmo local para um [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true).
- [Configurar uma pasta de recursos do SharePoint](/graph/api/educationsubmission-setupresourcesfolder?view=graph-rest-beta&preserve-view=true) para carregar e armazenar todos os recursos baseados em arquivo como um arquivo Word e Excel no mesmo local para um [educationAssignment](/graph/api/resources/educationsubmission?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- Obtenha uma coleção de recursos de [accessPackageAssignment](/graph/api/resources/accessPackageAssignment?view=graph-rest-beta&preserve-view=true) ao [filtrar no usuário conectado](/graph/api/accesspackageassignment-filterbycurrentuser?view=graph-rest-beta&preserve-view=true).
- Obtenha uma coleção de recursos de [accessPackageAssignmentRequest](/graph/api/resources/accessPackageAssignmentRequest?view=graph-rest-beta&preserve-view=true) ao [filtrar no usuário conectado](/graph/api/accesspackageassignmentrequest-filterbycurrentuser?view=graph-rest-beta&preserve-view=true).

### <a name="use-sdks"></a>Usar SDKs
Experimente a versão de visualização do [Microsoft Graph .NET SDK v4](https://www.nuget.org/packages/Microsoft.Graph/4.0.0-preview.4) e aproveite as seguintes melhorias:
- Use uma única API para autenticação em clientes do Microsoft Graph e Azure .NET.
- Novo suporte para serialização e desserialização JSON.
- Fácil acesso às informações de resposta.
- Melhor experiência de atualização de dependências.

## <a name="april-2021-new-and-generally-available"></a>Abril de 2021: novo e disponível para o público geral

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
- Gerenciar uma [política de autenticação](/graph/api/resources/authenticationflowspolicy) no nível de locatário para ativar ou desativar um [serviço autoatendimento de cadastramento](/graph/api/resources/selfservicesignupauthenticationflowconfiguration) para usuários externos.
- Os administradores podem associar fluxos de usuários a aplicativos que são compartilhados com usuários externos e permitir a [inscrição de autoatendimento](/azure/active-directory/external-identities/self-service-sign-up-overview) nesses aplicativos. Eles podem personalizar um fluxo de usuário de inscrição de autoatendimento e criar uma experiência de inscrição personalizada. Depois que um aplicativo é associado ao fluxo do usuário, os usuários que acessam esse aplicativo poderão iniciar um fluxo de inscrição que provisiona uma conta de convidado.
- Configurar os [atributos de fluxo de usuário](/graph/api/resources/identityuserflowattribute) no seu locatário do Azure AD permite que você colete informações sobre um usuário durante a inscrição. Você também pode coletar um conjunto embutido de atributos ou configurar atributos de fluxo de usuário personalizado para coletar informações de um usuário que não está integrado ao diretório. 
- Em um [fluxo de usuário do Azure Active Directory](/graph/api/resources/b2xidentityuserflow), você pode gerenciar os padrões de idioma e [personalizar o idioma e as cadeias de caracteres exibidas para os usuários no fluxo do usuário](/graph/api/resources/userflowlanguageconfiguration).
- Use um [conector de API](/graph/api/resources/identityapiconnector) em fluxos de usuário para inscrição de autoatendimento do Azure Active Directory e inscrição do Azure Active Directory B2C, para chamar uma API em uma etapa específica para afetar a execução do fluxo de usuário.

### <a name="teamwork"></a>Trabalho em equipe
- Identifique o canal pela propriedade **channelIdentity**, se uma [chatMessage](/graph/api/resources/chatmessage) estiver em um [canal](/graph/api/resources/channel).
- Identifique o chat pela propriedade **chatId**, se o **[chatMessage](/graph/api/resources/chatmessage)** estiver em um [chat](/graph/api/resources/chat).
- Use o relacionamento de **mensagens** para obter todos os recursos [chatMessage](/graph/api/resources/chatmessage) em um [chat](/graph/api/resources/chat).
- Use as permissões do aplicativo [obter](/graph/api/chat-get) propriedades de um [chat](/graph/api/resources/chat) específico.
- Use as permissões do aplicativo para [receber um membro específico do chat](/graph/api/chat-get-members) ou [todos os membros do chat](/graph/api/chat-list-members) incluídos em um chat. Como os dados dos usuários como membros do chat são confidenciais, além de obter permissões do aplicativo, [solicite acesso adicional](teams-protected-apis.md) para essas operações.

### <a name="use-the-toolkit"></a>Usar o kit de ferramentas
Novo no [Kit de ferramentas do Microsoft Graph](/graph/toolkit/overview)? Experimente o novo [caminho de aprendizagem do Kit de ferramentas ](/learn/paths/m365-msgraph-toolkit/?WT.mc_id=m365-19989-cxa), utilize o conjunto de componentes da web e provedores de autenticação do Kit de ferramentas para conectar um aplicativo da web ao Microsoft Graph e carregar dados do Microsoft 365.

## <a name="april-2021-new-in-preview-only"></a>Abril de 2021: Novo somente para visualização

### <a name="cloud-communications--online-meetings"></a>Comunicações na nuvem | Reuniões online
- Receba um [relatório](/graph/api/resources/meetingattendancereport?view=graph-rest-beta&preserve-view=true) da [participação de cada participante](/graph/api/resources/attendancerecord?view=graph-rest-beta&preserve-view=true) em uma reunião online agendada, por meio da propriedade **meetingAttendanceReport** de [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true).
- Habilitar, desabilitar ou limitar a duração do chat de uma reunião online usando a propriedade **allowMeetingChat**.
- Habilitar ou desabilitar reações a uma reunião online usando a propriedade **allowTeamworkReactions**.

### <a name="compliance"></a>Conformidade
[Obter](/graph/api/ediscovery-settings-get?view=graph-rest-beta&preserve-view=true), [atualizar](/graph/api/ediscovery-settings-update?view=graph-rest-beta&preserve-view=true)ou [redefinir para padrão](/graph/api/ediscovery-settings-resettodefault?view=graph-rest-beta&preserve-view=true) as seguintes [configurações ](/graph/api/resources/ediscovery-settings?view=graph-rest-beta&preserve-view=true) para um [caso](/graph/api/resources/ediscovery-case?view=graph-rest-beta&preserve-view=true) de Descoberta Eletrônica:
- [Detecção de duplicatas, quase duplicatas](/microsoft-365/compliance/near-duplicate-detection-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true), e [thread de email](/microsoft-365/compliance/email-threading-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true), por meio da propriedade **redundancyDetection**.
- [Identificar os temas](/microsoft-365/compliance/themes-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true) que são ideias predominantes em documentos de um conjunto de revisão, por meio da propriedade **topicModeling** área de trabalho.
- [Extração de texto de arquivos de imagens por reconhecimento óptico de caracteres (OCR)](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true#optical-character-recognition-ocr), por meio da propriedade **ocr**.

Essas configurações fornecem funcionalidade de análise que [seleciona dados de forma inteligente](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide&preserve-view=true#cull-data-intelligently) no fluxo de trabalho de ponta a ponta da [Descoberta Eletrônica Avançada](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide&preserve-view=true).

### <a name="devices-and-apps--device-updates"></a>Dispositivos e aplicativos | Atualizações do dispositivo
Serviço de inicialização de APIs para a implantação do Windows Update para Empresas. O serviço dá suporte à implantação de atualizações de recursos do Windows 10 e à acelerar as atualizações de segurança do Windows 10 em dispositivos. Para saber mais, comece com a visão geral [da API de atualizações do Windows](windowsupdates-concept-overview.md).

### <a name="education"></a>Educação
- Associe uma pasta a um [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) para armazenar todos os recursos de arquivo relacionados, por meio da propriedade **resourcesFolderUrl**.
- Vínculo profundo em um [EducationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) por meio da propriedade **WebUrl**.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Os administradores podem [obter](/graph/api/accessreviewpolicy-get?view=graph-rest-beta&preserve-view=true) ou [atualizar](/graph/api/accessreviewpolicy-update?view=graph-rest-beta&preserve-view=true) políticas no nível de diretório para revisar o acesso, usando o recurso [accessReviewPolicy](/graph/api/resources/accessreviewpolicy?view=graph-rest-beta&preserve-view=true). Por exemplo, os administradores podem usar uma política de revisão do acesso para habilitar ou desabilitar os proprietários do grupo que estão avaliando o acesso em grupos que eles possuem.

### <a name="search"></a>Pesquisar
[Habilitar sugestões de ortografia ou correções](search-concept-speller.md) para uma consulta de usuário. Isso é útil quando uma consulta de usuário contém erros de digitação ou quando os erros não renderam nenhum resultado de pesquisa.

### <a name="teamwork"></a>Trabalho em equipe
- Use a [concessão de permissão específica do recurso](/graph/api/resources/resourcespecificpermissiongrant?view=graph-rest-beta&preserve-view=true) para listar os aplicativos com acesso a um determinado [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) ou [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).
- [Obter](/graph/api/teamsappicon-get?view=graph-rest-beta&preserve-view=true) as propriedades de um [ícone](/graph/api/resources/teamsAppIcon?view=graph-rest-beta&preserve-view=true) associado a um aplicativo do Teams. Para obter a imagem real do ícone, use [obter conteúdo hospedado](/graph/api/teamworkhostedcontent-get?view=graph-rest-beta&preserve-view=true).

### <a name="use-sdks"></a>Usar SDKs
- Experimente a [prévia da versão da biblioteca do cliente JavaScript do Microsoft Graph, versão 3.0.0](https://www.npmjs.com/package/@microsoft/microsoft-graph-client/v/3.0.0-Preview.1). Esta versão permite vários fluxos de autenticação, autenticação do lado do servidor, Stream Node.js de carregamento de arquivos grandes e acompanhamento de progresso e muito mais. Consulte o [guia de atualização](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/changelogs/v3-upgrade-guide.md) para obter detalhes.
- Experimente um novo caminho de aprendizagem para [explorar os cenários do Microsoft Graph para desenvolvimento do JavaScript](/learn/paths/m365-msgraph-scenarios/?WT.mc_id=m365-16105-cxa).


## <a name="march-2021-new-and-generally-available"></a>Março de 2021: novo e disponível para o público geral

### <a name="applications"></a>Aplicativos
- GA do recurso [applicationTemplate](/graph/api/resources/applicationtemplate) que suporta a [listagem](/graph/api/applicationtemplate-list) de aplicativos na galeria de aplicativos do Azure AD e a [adição](/graph/api/applicationtemplate-instantiate) de uma instância desse aplicativo a um diretório.
- Use a permissão somente para aplicativo `Application.ReadWrite.OwnedBy`ao[adicionar](/graph/api/applicationtemplate-instantiate) tal instância.
- Use a propriedade **signInAudience** do [servicePrincipal](/graph/api/resources/serviceprincipal) para obter as contas de usuário compatíveis com o aplicativo atual.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- GA da [API de impressão em nuvem](universal-print-concept-overview.md) para Impressão Universal! Veja o [comunicado](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/universal-print-is-ready-for-business/ba-p/2176778) e confira como [começar com a Impressão Universal](/universal-print/fundamentals/universal-print-license).
- [Inscreva-se para alterar as notificações](universal-print-webhook-notifications.md) em uma [definição de tarefa de impressão](/graph/api/resources/printtaskdefinition) ou recurso [impressora](/graph/api/resources/printer).

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- Use as [solicitações de consentimento](/graph/api/resources/consentrequests-root) do Azure Active Directory (Azure AD) para gerenciar o fluxo de trabalho de solicitação para usuários que tentam acessar aplicativos que exigem aprovação do administrador. A API usa os seguintes recursos:
  - O recurso [adminConsentRequestPolicy](/graph/api/resources/adminconsentrequestpolicy) para criar e gerenciar solicitações de acesso ao aplicativo para a organização.
  - O recurso [appConsentRequest](/graph/api/resources/appconsentrequest) para agregar e gerenciar solicitações de usuário para acessar um aplicativo específico.
  - O recurso [userConsentRequest](/graph/api/resources/userConsentRequest) para usuários que solicitam acesso a um aplicativo que requer autorização de administrador. 
  - O recurso [accessReviewReviewerScope](/graph/api/resources/accessReviewReviewerScope)define quem é indicado em **adminConsentRequestPolicy** para revisar os objetos **appConsentRequest** e **userConsentRequest**.
  - O recurso de [aprovação](/graph/api/resources/approval) representa uma decisão de aprovação para uma solicitação.
- GA da API de Termos de Uso que oferece suporte a um [contrato de Termos de Uso](/graph/api/resources/agreement) personalizável de um locatário no Azure AD.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
- GA dos [métodos de autenticação](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true), incluindo as [chaves de segurança FIDO2](/graph/api/resources/fido2authenticationmethod),o [aplicativo Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethod) e o [Windows Hello para Empresas](/graph/api/resources/windowshelloforbusinessauthenticationmethod).
- GA das [políticas de método de autenticação](/graph/api/resources/authenticationmethodspolicies-overview) que definem os métodos de autenticação e os usuários que têm permissão para usá-los para se conectar e executar a autenticação multifator (MFA) no Azure AD. As políticas de métodos de autenticação que podem ser gerenciadas no Microsoft Graph incluem as [chaves de segurança FIDO2](/graph/api/resources/fido2authenticationmethodconfiguration), a Entrada por Telefone sem Senha com o [aplicativo Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethodconfiguration) e a [política de métodos de autenticação OTP de email](/graph/api/resources/emailauthenticationmethodconfiguration) do locatário.
- GA da [política de distribuição de recursos](/graph/api/resources/featureRolloutPolicy) que ajuda os administradores de locatários a ter recursos piloto para grupos específicos antes de habilitá-los para toda a organização.
- GA das [propriedades de identidade visual da organização](/graph/api/resources/organizationalbrandingproperties) que permite uma aparência personalizada das telas de entrada do Azure Active Directory. As organizações podem personalizar com base na localidade para usuários específicos.

### <a name="tasks-and-plans"></a>Tarefas e planos
- Use a permissão delegada de `Tasks.Read` para ler as operações de todos os recursos do Planner.
- Use a permissão delegada de `Tasks.ReadWrite` para ler e gravar as operações de todos os recursos do Planner.

### <a name="teamwork"></a>Trabalho em equipe
- GA de operações de [chat](/graph/api/resources/chat), chat [conversationMember](/graph/api/resources/conversationmember), [aplicativo](/graph/api/resources/teamsappinstallation) de chat, [guia](/graph/api/resources/teamstab) de chat e os seus métodos.
- GA de mais algumas propriedades de [teamsAppDefinition](/graph/api/resources/teamsAppDefinition), que representam detalhes de uma versão de um aplicativo no catálogo de aplicativos do Microsoft Teams, incluindo o seguinte:
  - **createdBy**, **description**, **shortDescription**, **lastModifiedDateTime**
  - **publishingState**, que pode ser `submitted` e em revisão, `published` ou `rejected` pelo administrador
  - Relação de **bot** do tipo [teamworkBot](/graph/api/resources/teamworkbot), representando os detalhes do bot especificado no manifesto do aplicativo Teams.
- Use a API de notificações de feed de atividades para envolver melhor os usuários em três contextos:
  - [Enviar notificação ao usuário em um chat](/graph/api/chat-sendactivitynotification)
  - [Enviar notificação ao usuário em uma equipe](/graph/api/team-sendactivitynotification)
  - [Enviar notificação ao usuário](/graph/api/userteamwork-sendactivitynotification)
- Migre o histórico de mensagens e dados dos usuários de um sistema externo para um canal do Teams, permitindo que os usuários continuem as suas comunicações facilmente. Use os seguintes métodos que suportam o cenário de migração:
  - [Criar equipe](/graph/api/team-post)
  - [Criar canal](/graph/api/channel-post)
  - [Criar chatMessage em um canal](/graph/api/channel-post-messages)
  - [Responder a uma mensagem em um canal](/graph/api/channel-post-messagereply)
  - [Concluir a migração de mensagens em uma equipe](/graph/api/team-completemigration)
  - [Concluir a migração de mensagens em um canal](/graph/api/channel-completemigration)
- [Liste](/graph/api/chatmessage-list-chatmessagehostedcontents) ou [obtenha](/graph/api/chatmessagehostedcontent-get) conteúdo avançado hospedado em uma [chatMessage](/graph/api/resources/chatmessage), como imagens ou trechos de código.
- Suporte de permissões delegadas de `ChannelMessage.Read.All` para subscrever notificações de mudança em recursos [chatMessage](/graph/api/resources/chatmessage).

## <a name="march-2021-new-in-preview-only"></a>Março de 2021: Novo somente para visualização

### <a name="applications"></a>Aplicativos
[Criar e adicionar certificados autoassinados](/graph/api/servicePrincipal-addTokenSigningCertificate?view=graph-rest-beta&preserve-view=true) aos seus aplicativos SAML. Use isso para ajudar a habilitar o logon único para aplicativos da galeria do Azure Active Directory em seu locatário, permitindo que o Azure Active Directory assine respostas SAML.

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
Adicionados ao recurso [cloudPcDeviceImage](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) mais dois motivos para falha no upload de uma imagem de origem do dispositivo: sistema operacional não compatível (`osVersionNotSupported`) ou uma imagem de origem inválida para provisionar uma VM do Windows (`sourceImageInvalid`).

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
Obtenha a data/hora mais recente (propriedade **lastSeenDateTime**) em que uma impressora interagiu com a Impressão Universal.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
As atualizações de [março](https://developer.microsoft.com/graph/changelog/?from=2021-03-01&to=2021-03-31&filterBy=Corporate%20management) do Intune para a versão beta.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Aplique o novo modelo de [revisões de acesso](/graph/api/resources/accessreviewsv2-overview?view=graph-rest-beta&preserve-view=true) a associações de grupo e todos os outros tipos de recursos suportados. Preterir o [modelo herdado de revisões de acesso](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true).

### <a name="sites-and-lists"></a>Sites e listas
- Suporta a um tipo ou modelo de conteúdo específico para documentos ou conjuntos de documentos em conjuntos de sites específicos, por meio de um conjunto de novas propriedades e métodos na entidade [contentType](/graph/api/resources/contentType?view=graph-rest-beta&preserve-view=true). Os métodos incluem o seguinte:
  - [addCopy](/graph/api/contenttype-addcopy?view=graph-rest-beta&preserve-view=true)
  - [associateWithHubSites](/graph/api/contenttype-associatewithhubsites?view=graph-rest-beta&preserve-view=true)
  - [copyToDefaultContentLocation](/graph/api/contenttype-copytodefaultcontentlocation?view=graph-rest-beta&preserve-view=true)
  - [isPublished](/graph/api/contenttype-ispublished?view=graph-rest-beta&preserve-view=true)
  - [publish](/graph/api/contenttype-publish?view=graph-rest-beta&preserve-view=true)
  - [unpublish](/graph/api/contenttype-unpublish?view=graph-rest-beta&preserve-view=true)
- Personalize os tipos de conteúdo por suas colunas. As colunas são representadas pela entidade [columnDefinition](/graph/api/resources/columndefinition?view=graph-rest-beta&preserve-view=true) e dão suporte ao conjunto completo de operações CRUD.
- [Obtenha os tipos de conteúdo de um site que podem ser aplicados a uma lista](/graph/api/site-getApplicableContentTypesForList?view=graph-rest-beta&preserve-view=true).
- Diferencie os tipos de coluna pelas seguintes propriedades na entidade **columnDefinition**: booliana, calculada, escolha, moeda, dateTime, pesquisa, número, personOrGroup, texto. Essas propriedades são mutuamente exclusivas.

### <a name="sites-and-lists--taxonomy"></a>Sites e listas | Taxonomia
- Navegue de um [site](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) para um [repositório de termos de taxonomia](/graph/api/resources/termstore-store?view=graph-rest-beta&preserve-view=true) usando a relação **termStore**.
- Na direção inversa, obtenha a ID do site pai de um repositório de termos usando a propriedade **parentSiteId**.

### <a name="users"></a>Usuários
- [Obter](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta&preserve-view=true) ou [atualizar](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta&preserve-view=true) preferências de [um usuário para traduzir idiomas](/graph/api/resources/translationpreferences?view=graph-rest-beta&preserve-view=true). Por exemplo, se deve ou não traduzir, traduzir automaticamente ou avisar antes de traduzir idiomas específicos em mensagens, chats e páginas da Web, e qualquer [substituição de tradução](/graph/api/resources/translationlanguageoverride?view=graph-rest-beta&preserve-view=true).
- [Ative um plano de serviço](/graph/api/user-activateServicePlan?view=graph-rest-beta&preserve-view=true) para um usuário.


## <a name="february-2021-new-and-generally-available"></a>Fevereiro de 2021: novo e disponível para o público geral

### <a name="cloud-communications--online-meeting"></a>Comunicações em nuvem | Reunião online
Use permissões de aplicativo baseada em políticas `OnlineMeetings.Read.All` ou `OnlineMeetings.ReadWrite.All` sobre as operações e métodos do recurso [onlineMeeting](/graph/api/resources/onlinemeeting). Isso significa que os administradores podem [configurar a política de acesso a aplicativos](cloud-communication-online-meeting-application-access-policy.md) para permitir que os aplicativos acessem as reuniões online em nome de um usuário.

### <a name="sites-and-lists"></a>Sites e listas
Use o recurso de [permissão](/graph/api/resources/permission) e suas operações CRUD para gerenciar a permissão de compartilhamento concedida para um [driveItem](/graph/api/resources/driveitem). Permissões com uma faceta link representam links de compartilhamento criados no item. Permissões com uma faceta invitation representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.

## <a name="february-2021-new-in-preview-only"></a>Fevereiro de 2021: novo apenas em pré-visualização

### <a name="applications"></a>Aplicativos
Use permissões de aplicativo para as [APIs de sincronização](/graph/api/resources/synchronization-overview?view=graph-rest-beta&preserve-view=true) que automatizam o provisionamento (criação, manutenção) e o desprovisionamento (remoção) de identidades no Azure AD.

### <a name="cloud-communications--calls"></a>Comunicações na nuvem | Chamadas
Suporte para [gravação baseada em políticas para chamadas](/microsoftteams/teams-recording-policy) onde, usando a política administrativa, as chamadas são gravadas automaticamente para processamento e retenção subsequentes, conforme exigido pela política corporativa ou regulamentar relevante. Antes de um participante baseado em política ingressar em uma chamada, a política solicita o envio de um [participantJoiningNotification](/graph/api/resources/participantJoiningNotification?view=graph-rest-beta&preserve-view=true) ao bot associado à política que tem capacidade para lidar com o novo participante. O bot responde com [acceptJoinResponse](/graph/api/resources/acceptjoinresponse?view=graph-rest-beta&preserve-view=true), [rejectJoinResponse](/graph/api/resources/rejectjoinresponse?view=graph-rest-beta&preserve-view=true) ou [inviteNewBotResponse](/graph/api/resources/invitenewbotresponse?view=graph-rest-beta&preserve-view=true) em seu conteúdo de resposta.

### <a name="compliance--ediscovery"></a>Conformidade | Descoberta Eletrônica
- Use o recurso [legalHold](/graph/api/resources/ediscovery-legalhold?view=graph-rest-beta&preserve-view=true) e suas APIs para proteger o conteúdo indefinidamente contra exclusão, para fins de litígio, investigação interna ou outras ações legais.
- Use o recurso [sourceColection](/graph/api/resources/ediscovery-sourcecollection?view=graph-rest-beta&preserve-view=true) e suas APIs para pesquisar e identificar documentos relevantes de locais com ou sem custódia no Microsoft 365.
- Use o recurso [tag](/graph/api/resources/ediscovery-tag?view=graph-rest-beta&preserve-view=true) e as APIs para marcar documentos durante a revisão para separar o conteúdo responsivo e não responsivo.
- [Exporte](/graph/api/ediscovery-reviewset-export?view=graph-rest-beta&preserve-view=true) documentos de um [conjunto de revisão](/graph/api/resources/ediscovery-reviewset?view=graph-rest-beta&preserve-view=true).
- Use a ação [addToReviewSet](/graph/api/ediscovery-reviewset-addtoreviewset?view=graph-rest-beta&preserve-view=true) para adicionar documentos em uma **sourceColection** a um **reviewSet**.
- [Aplique tags](/graph/api/ediscovery-reviewsetquery-applytags?view=graph-rest-beta&preserve-view=true) a documentos baseados em uma [consulta de conjunto de revisão](/graph/api/resources/ediscovery-reviewsetquery?view=graph-rest-beta&preserve-view=true).
- API de Descoberta eletrônica definida no namespace `microsoft.graph.ediscovery`.
- Modelo de permissões delegadas alterado de `User.Read` para `eDiscovery.Read.All` e `eDiscovery.ReadWrite.All`.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
- Atualizações do Intune de [fevereiro](https://developer.microsoft.com/graph/changelog/?from=2021-02-01&to=2021-02-28&filterBy=Corporate%20management) para a versão beta.
- Novas propriedades definidas pelo Intune no recurso do [dispositivo](/graph/api/resources/device?view=graph-rest-beta&preserve-view=true): **deviceCategory**, **deviceOwnership**, **domainName**, **enrollmentProfileName**, **enrollmentType**, **isRooted**, **managementType**, and **registrationDateTime**.

### <a name="education"></a>Educação
Use [educationAssignmentDefaults](/graph/api/resources/educationAssignmentDefaults?view=graph-rest-beta&preserve-view=true) para especificar práticas padrão em uma atribuição para uma classe, por exemplo, hora de conclusão da atribuição, URL do canal para notificações em uma atribuição. Você ainda pode personalizar valores ao criar uma atribuição.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
- Use o recurso [smsAuthenticationMethodConfiguration](/graph/api/resources/smsAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true) para [obter](/graph/api/smsauthenticationmethodconfiguration-get?view=graph-rest-beta&preserve-view=true), [atualizar](/graph/api/smsauthenticationmethodconfiguration-update?view=graph-rest-beta&preserve-view=true) ou [excluir](/graph/api/smsauthenticationmethodconfiguration-delete?view=graph-rest-beta&preserve-view=true) as definições de configuração de uma política de autenticação de mensagem de texto em uma organização.
- Use o recurso [temporaryAccessPassAuthenticationMethodConfiguration](/graph/api/resources/temporaryaccesspassauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true) para [obter](/graph/api/temporaryaccesspassauthenticationmethodconfiguration-get?view=graph-rest-beta&preserve-view=true), [atualizar](/graph/api/temporaryaccesspassauthenticationmethodconfiguration-update?view=graph-rest-beta&preserve-view=true) ou [excluir](/graph/api/temporaryaccesspassauthenticationmethodconfiguration-delete?view=graph-rest-beta&preserve-view=true) as definições de configuração de uma política de autenticação de passe de acesso temporário em uma organização.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- Atribua informações de geolocalização a um recurso de [pacote de acesso](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true) na [solicitação de atribuição de pacote de acesso](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true).
- Obtenha uma lista de todos os [ambientes de recursos de pacote de acesso](/graph/api/resources/accesspackageresourceenvironment?view=graph-rest-beta&preserve-view=true) que representam as geolocalizações que armazenam os recursos do Microsoft Office SharePoint Online.
- Use permissões de aplicativos (`EntitlementManagement.Read.All` ou `EntitlementManagement.ReadWrite.All`) para operações dos seguintes recursos:
  - [accessPackage](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignment](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignmentPolicy](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignmentRequest](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignmentResourceRole](/graph/api/resources/accesspackageassignmentresourcerole?view=graph-rest-beta&preserve-view=true)
  - [accessPackageCatalog](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true)
  - [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta&preserve-view=true)
  - [connectedOrganization](/graph/api/resources/connectedorganization?view=graph-rest-beta&preserve-view=true)
  - [entitlementManagementSettings](/graph/api/resources/entitlementmanagementsettings?view=graph-rest-beta&preserve-view=true)

### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
Obtenha mais propriedades incluídas em [relatórios detalhados para uso do site SharePoint](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta&preserve-view=true): anonymousLinkCount, companyLinkCount, externalSharing, geolocation, secureLinkForGuestCount, secureLinkForMemberCount, siteSensitivityLabelId, e unmanagedDevicePolicy.

### <a name="tasks-and-plans"></a>Tarefas e planos
- Defina até 25 categorias em um objeto de [detalhes do plano](/graph/api/resources/plannerplandetails?view=graph-rest-beta&preserve-view=true) para um plano. Para cada categoria, especifique um rótulo descritivo e associe tarefas em um plano com uma ou mais destas categorias. 
- Use uma [lista de participantes](/graph/api/resources/plannerRoster?view=graph-rest-beta&preserve-view=true) para representar um conjunto de usuários colaborando em um [plano](/graph/api/resources/plannerplan?view=graph-rest-beta&preserve-view=true). Use a relação **rosterPlans** para obter as listas de participantes das quais o usuário é um [membro](/graph/api/resources/plannerrostermember?view=graph-rest-beta&preserve-view=true). 
- Para planos que são apresentados em experiências fora do Planner, como o Microsoft Teams, especifique nos [detalhes de contexto do plano](/graph/api/resources/plannerplancontextdetails?view=graph-rest-beta&preserve-view=true) como exibir o link para o [contexto do plano](/graph/api/resources/plannerPlanContext?view=graph-rest-beta&preserve-view=true). 

### <a name="use-sdks"></a>Usar SDKs
Experimente a versão prévia do [Microsoft Graph Java SDK v3](https://github.com/microsoftgraph/msgraph-sdk-java/tree/feature/v3)! Para mais informações, confira a [postagem no blog](https://developer.microsoft.com/graph/blogs/announcing-the-public-preview-of-microsoft-graph-java-sdk-v3/) relacionada.

## <a name="january-2021-new-in-preview-only"></a>Janeiro de 2021: novo apenas em pré-visualização

### <a name="cloud-communications"></a>Comunicações na nuvem
- Organize um evento ao vivo como uma [reuniãoOnline ](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) - veja um [exemplo](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true#example-3-create-a-live-event-with-a-user-token). 
- Obtenha o fluxo de conteúdo de um [relatório de participante](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-4-retrieve-the-attendee-report-of-a-live-event), [gravação](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-5-retrieve-the-recording-of-a-live-event) ou gravação alternativa do evento ao vivo.
- Obtenha o status de [presença](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true) de um usuário que está [fora do escritório](/graph/api/resources/outofofficesettings?view=graph-rest-beta&preserve-view=true) e qualquer mensagem definida para esse status.

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Cloud PC
- [Atualize uma senha de domínio do Active Directory ](/graph/api/cloudpconpremisesconnection-updateaddomainpassword?view=graph-rest-beta&preserve-view=true) para uma [conexão de rede local bem-sucedida](/graph/api/resources/cloudPcOnPremisesConnection?view=graph-rest-beta&preserve-view=true).
- [Executar verificações de integridade em uma conexão de rede local](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) agora pode expor 5 tipos de erros adicionais no recurso de [verificação de integridade da conexão local](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true). Para obter mais informações sobre os tipos de erro, confira o [log de mudanças](https://developer.microsoft.com/graph/changelog) de janeiro de 2021.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- [Assine para alterar notificações de impressão em nuvens](universal-print-webhook-notifications.md) - quando um trabalho de impressão é iniciado, e quando o trabalho de impressão está pronto para ser baixado por uma impressora.
- Obtenha uma gama completa de [valores possíveis](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true#printerprocessingstatedetail-values) para o status de uma [impressora](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true).
- Use permissões delegadas em aplicativos em nome do usuário conectado:
  - `PrinterShare.ReadBasic.All` para ler informações básicas sobre compartilhamentos de impressoras, excluindo informações de controle de acesso.
  - `PrintConnector.Read.All` para ler conectores de impressão.
  - `PrintConnector.ReadWrite.All` para ler ou gravar conectores de impressão.
  - `PrintJob.Create` para criar trabalhos de impressão e fazer upload de conteúdo para trabalhos de impressão.
  - `PrintSettings.Read.All` para ler as configurações de impressão de todo o locatário.
  - `PrintSettings.ReadWrite.All` para ler ou gravar configurações de impressão para todo o locatário.
  - `Reports.Read.All` para ler o resumo do uso de impressão por usuário especificado ou por impressora.

### <a name="education"></a>Educação
Use [configurações de tarefas](/graph/api/resources/educationAssignmentSettings?view=graph-rest-beta&preserve-view=true) a nível de classe para habilitar ou desabilitar a animação para comemorar a entrega de uma tarefa.

### <a name="groups"></a>Grupos
Obtenha o status de processamento de um grupo dinâmico baseado em regra usando a propriedade **membershipRuleProcessingStatus**. Isso é útil quando um atributo de um usuário é alterado, a associação do usuário em um [grupo Microsoft 365](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) baseado em regras é reavaliada com base nas regras de associação de grupo definidas para a organização. 

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
Obtenha o [direito de uso](/graph/api/resources/UsageRight?view=graph-rest-beta&preserve-view=true) que um usuário ou dispositivo tem sobre software de terceiros criado no Power Apps ou o direito de uso de um dispositivo em uma assinatura. O direito de uso inclui identificadores para o serviço ou produto correspondente, e o estado atual do direito de uso, como ativo, inativo, em alerta, ou em suspensão.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
- Os aplicativos podem usar as permissões do aplicativo para permitir que os administradores gerenciem os [métodos de autenticação](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true) dos usuários.
- Suporte ao [Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethod?view=graph-rest-beta&preserve-view=true) como um método de autenticação de um usuário para entrar ou executar autenticação multifator no Azure Active Directory.
- Use a [política do Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true) para definir as configurações e usuários ou grupos que podem usar o Microsoft Authenticator como método de autenticação. Use a política do Microsoft Authenticator no lugar da [política de login por telefone sem senha do Microsoft Authenticator](/graph/api/resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true), que está obsoleta. 
- Ofereça suporte ao [Windows Hello para Empresas](/graph/api/resources/windowshelloforbusinessauthenticationmethod?view=graph-rest-beta&preserve-view=true) como um método de autenticação para um usuário entrar em dispositivos Windows sem usar uma senha.

### <a name="reports--identity-and-access-reports"></a>Relatórios | Relatórios de identidade e acesso
- [Obtenha um relatório do número de usuários que estão registrados, ou que possuem vários recursos de registro](/graph/api/authenticationmethodsroot-usersregisteredbyfeature?view=graph-rest-beta&preserve-view=true), incluindo autenticação multifator, redefinição de senha de autoatendimento, ou autenticação sem senha.
- [Obtenha um relatório do número de usuários registrados para cada método de autenticação](/graph/api/authenticationmethodsroot-usersregisteredbymethod?view=graph-rest-beta&preserve-view=true), incluindo senha, Windows Hello para Empresas, ou logon de telefone sem senha.

## <a name="december-2020-new-and-generally-available"></a>Dezembro de 2020: Novo e disponível para o público geral

### <a name="calendar"></a>Calendário
- Os organizadores da reunião podem usar a propriedade **hideAttendees** de um [evento](/graph/api/resources/event) para controlar se os participantes podem ver uns aos outros na lista de **acompanhamento** da reunião.
- GA da propriedade **isDraft** e método de [cancelamento](/graph/api/event-cancel) que estão disponíveis para os organizadores e o método de [encaminhamento](/graph/api/event-forward) disponível para organizadores e participantes para gerenciar melhor os recursos do [evento](/graph/api/resources/event) em um calendário.
- GA das propriedades **hexColor** e **isDefault** de um [calendário](/graph/api/resources/calendar) para gerenciar melhor os calendários.

### <a name="cloud-communications"></a>Comunicações na nuvem
GA do recurso de [presença](/graph/api/resources/presence), permitindo obter a presença de um ou mais usuários, como disponibilidade e atividade do usuário.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
Experimente um novo [tutorial](tutorial-riskdetection-api.md) para aprender como usar a [API de proteção de identidade](/graph/api/resources/identityprotectionroot) para identificar o risco e configurar um fluxo de trabalho para confirmar o comprometimento ou habilitar a correção.

### <a name="teamwork"></a>Trabalho em equipe
- GA da [API para gerenciar a instalação do aplicativo Teams](/graph/api/resources/teamsappinstallation), incluindo a instalação de aplicativos ou a adição, a remoção ou a atualização do aplicativo em uma equipe ou no escopo pessoal de um usuário.
- [Obtenha um chat entre um usuário e um aplicativo do Teams](/graph/api/userscopeteamsappinstallation-get-chat).

### <a name="use-the-toolkit"></a>Usar o kit de ferramentas
GA do Kit de ferramentas do Microsoft Graph 2.0 – esta versão inclui um novo [componente para tarefas pendentes do Microsoft Graph](./toolkit/components/todo.md), diferente do [componente de tarefas do Planner](./toolkit/components/tasks.md)e um [componente de cartão pessoal](./toolkit/components/person-card.md) aprimorado. Consulte a [postagem de blog relacionada](https://developer.microsoft.com/graph/blogs/announcing-the-general-availability-of-microsoft-graph-toolkit-2-0/) para obter mais informações.


## <a name="december-2020-new-in-preview-only"></a>Dezembro de 2020: novo apenas em pré-visualização

### <a name="compliance--ediscovery"></a>Conformidade | Descoberta Eletrônica
Continuar a cumprir o pipeline das [APIs do Centro de conformidade do Microsoft 365](/graph/api/resources/ediscoveryapioverview?view=graph-rest-beta&preserve-view=true)é o recurso de [guardião](/graph/api/resources/custodian?view=graph-rest-beta&preserve-view=true) e suas operações e métodos relacionados para [liberar](/graph/api/custodian-release?view=graph-rest-beta&preserve-view=true) ou [ativar](/graph/api/custodian-activate?view=graph-rest-beta&preserve-view=true) um guardião. Use o recurso do **guardião** para acessar os dados do guardião ([userSource](/graph/api/resources/userSource?view=graph-rest-beta&preserve-view=true)) em uma caixa de correio do Exchange Online e OneDrive for Business, sites do Microsoft Office SharePoint Online ([siteSource](/graph/api/resources/siteSource?view=graph-rest-beta&preserve-view=true)) e grupos do Microsoft 365 ([unifiedGroupSource](/graph/api/resources/unifiedGroupSource?view=graph-rest-beta&preserve-view=true)).

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
Identifique o status de falha de um desktop virtual gerenciado em nuvem coletivamente como `failed`, na propriedade de **status** do recurso [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- [Atualize](/graph/api/printjob-update-configuration?view=graph-rest-beta&preserve-view=true) a [configuração](/graph/api/resources/printjobconfiguration?view=graph-rest-beta&preserve-view=true) de um [trabalho de impressão](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true).
- Para obter detalhes sobre a renomeação de algumas propriedades e redigitação de relacionamentos, confira a seção de dezembro de 2020 do [changelog da API](https://developer.microsoft.com/graph/changelog/) para obter detalhes.

### <a name="education"></a>Educação
- Se os alunos forem adicionados após a publicação da tarefa, os professores podem controlar o comportamento da tarefa usando a propriedade **addedStudentAction** do recurso [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true).
- Os professores podem postar notificação de publicação de tarefa por meio da propriedade **notificationChannelUrl** do recurso **educationAssignment**.

### <a name="identity-and-access"></a>Identidade e acesso
Obtenha ou defina a versão e os metadados de criação para um [contrato](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true) de [termos de uso](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true) do Azure Active Directory, [arquivo de contrato](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true) e [localização de contrato](/graph/api/resources/agreementfilelocalization?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
Como parte do [gerenciamento de direitos](/graph/api/resources/entitlementmanagement-overview?view=graph-rest-beta&preserve-view=true) do Azure Active Directory, quando os usuários que acessam grupos, aplicativos ou sites do SharePoint Online solicitam um período de acesso a um [pacote de acesso](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true), eles podem responder às [perguntas](/graph/api/resources/accesspackagequestion?view=graph-rest-beta&preserve-view=true) representadas no [conteúdo localizado](/graph/api/resources/accesspackagelocalizedcontent?view=graph-rest-beta&preserve-view=true) na [solicitação de permanência do pacote de acesso](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- Os administradores podem associar fluxos de usuários a aplicativos que são compartilhados com usuários externos e permitir a [inscrição de autoatendimento](/azure/active-directory/external-identities/self-service-sign-up-overview) nesses aplicativos. Eles podem personalizar um fluxo de usuário de inscrição de autoatendimento e criar uma experiência de inscrição personalizada. Especificamente, eles criam um [ouvinte para um evento de início de inscrição para chamar um fluxo de usuário customizado](/graph/api/resources/invokeuserflowlistener?view=graph-rest-beta&preserve-view=true). Depois que um aplicativo é associado ao fluxo do usuário, os usuários que acessam esse aplicativo poderão iniciar um fluxo de inscrição que provisiona uma conta de convidado.
- Em um [fluxo de usuário do Azure Active Directory](/graph/api/resources/b2xidentityuserflow?view=graph-rest-beta&preserve-view=true) ou no [fluxo de usuário do locatário do Azure Active Directory B2C](/graph/api/resources/b2cidentityuserflow?view=graph-rest-beta&preserve-view=true), você pode gerenciar os padrões de idioma e [personalizar o idioma e as cadeias de caracteres exibidas para os usuários no fluxo do usuário](/graph/api/resources/userflowlanguageconfiguration?view=graph-rest-beta&preserve-view=true).
- Use um [conector de API](/graph/api/resources/identityapiconnector?view=graph-rest-beta&preserve-view=true) em fluxos de usuário para inscrição de autoatendimento do Azure Active Directory e inscrição do Azure Active Directory B2C, para chamar uma API em uma etapa específica para afetar a execução do fluxo de usuário.
- Defina uma [política de métodos de autenticação OTP de email](/graph/api/resources/emailauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true) para um locatário.

### <a name="teamwork"></a>Trabalho em equipe
- Para um recurso de [membro](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true) em uma [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true), [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) ou contexto de [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true), agora você pode:
  - Diferencie um membro que é um [usuário do Azure Active Directory](/graph/api/resources/aaduserconversationmember?view=graph-rest-beta&preserve-view=true), observando a ID do usuário, o endereço de email e a ID do locatário do Azure Active Directory. 
  - [Adicione vários usuários como membros de uma equipe](/graph/api/conversationmembers-add?view=graph-rest-beta&preserve-view=true).
- Para um recurso de [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true):
  - [Obtenha todas as mensagens em chats dos quais o usuário especificado participou](/graph/api/chats-getallmessages?view=graph-rest-beta&preserve-view=true), incluindo chats individuais, chats em grupo e chats de reunião.
  - Use toda a gama de funcionalidades para listar, obter, adicionar, remover e atualizar um [aplicativo](/graph/api/resources/teamsappinstallation?view=graph-rest-beta&preserve-view=true) ou uma [guia](/graph/api/resources/teamstab?view=graph-rest-beta&preserve-view=true) em um chat.
  - Use a propriedade **chatType** para distinguir um chat individual de um chat em grupo ou de um chat associado a uma reunião online.
  - [Crie](/graph/api/chat-post?view=graph-rest-beta&preserve-view=true) ou [atualize](/graph/api/chat-patch?view=graph-rest-beta&preserve-view=true) um chat.
  - Para um membro em um contexto de chat, use a propriedade **visibleHistoryStartDateTime** para definir ou obter um carimbo de data/hora que representa quanto tempo atrás o histórico de uma conversa é compartilhado com esse membro.
  - [Crie](/graph/api/chat-post-members?view=graph-rest-beta&preserve-view=true) ou [exclua](/graph/api/chat-delete-members?view=graph-rest-beta&preserve-view=true) membro de um chat especificado. 
- Para o recurso de [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true):
  - [Obtenha todas as mensagens em todos os canais em uma equipe](/graph/api/channels-getallmessages?view=graph-rest-beta&preserve-view=true).
  - Os proprietários da equipe podem ativar a [moderação de um canal](/graph/api/resources/channelmoderationsettings?view=graph-rest-beta&preserve-view=true) para controlar quem pode iniciar novas postagens ou responder às postagens nesse canal, usando a propriedade **moderationSettings** do canal.
- Como parte da [definição de um aplicativo Teams](/graph/api/resources/teamsappdefinition?view=graph-rest-beta&preserve-view=true), use o relacionamento de **bot** para se conectar a um bot de [trabalho em equipe](/graph/api/resources/teamworkbot?view=graph-rest-beta&preserve-view=true).

### <a name="to-do-tasks"></a>Tarefas pendentes
Assine para [receber notificações de alterações](webhooks.md) de [Tarefas Pendentes](/graph/api/resources/todoTask?view=graph-rest-beta&preserve-view=true).


## <a name="november-2020-new-and-generally-available"></a>Novembro de 2020: Novo e geralmente disponível

### <a name="cloud-communications"></a>Comunicações na nuvem
- O GA da propriedade **função** do tipo [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo), que distingue a função de um participante em uma [reunião online](/graph/api/resources/onlinemeeting) como um participante ou apresentador.
- O GA da propriedade **lobbyBypassSettings** e seus [valores](/graph/api/resources/lobbybypasssettings#lobbybypassscope-values) para admitir usuários para uma reunião online.
- O GA da propriedade **isEntryExitAnnounced** para personalizar as configurações de apresentação de autores de chamada ou de sair de uma reunião online.
- O GA da propriedade **allowedPresenters** para permitir apresentadores específicos na reunião.

### <a name="search"></a>Pesquisar
- O GA da [consulta da API](/graph/api/resources/search-api-overview) Pesquisa da Microsoft, oferecendo suporte à pesquisa em escopo dos seguintes tipos de dados:
  - [Mensagens do Outlook](./search-concept-messages.md)
  - [Eventos do calendário do Outlook](./search-concept-events.md)
  - [Recursos do Microsoft OneDrive e do Microsoft Office SharePoint Online](./search-concept-files.md).

### <a name="teamwork"></a>Trabalho em equipe

- GA de permissões RSC (consentimento específico de recurso). As permissões RSC permitem que os proprietários da equipe deem consentimento granular a um aplicativo de produção para acessar e/ou modificar dados específicos de uma equipe; como por exemplo, ler as configurações da equipe ou modificar nomes de canal, descrições e outras configurações.
- GA de APIs que se aplicam a um [canal](/graph/api/resources/channel) ou mensagens dentro de um canal. As APIs incluem:
  - [Criar](/graph/api/conversationmember-add) ou [excluir](/graph/api/conversationmember-delete) um membro de conversa de um canal.
  - [Atualizar a função de um membro](/graph/api/conversationmember-update) em um canal.
  - Receber uma mensagem específica ou todas as mensagens em um canal.
  - Receber uma resposta específica ou todas as respostas em um canal.
  - [Acompanhar mensagens novas ou atualizadas em um canal](/graph/api/chatmessage-delta).


## <a name="november-2020-new-in-preview-only"></a>Novembro de 2020: Novidades somente na pré-visualização

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
Estreia da [API de computador na nuvem](/graph/api/resources/virtualendpoint?view=graph-rest-beta&preserve-view=true) que permite que as organizações provisionem e gerenciem as máquinas virtuais para os funcionários. Use-o em conjunto com a API do Intune para gerenciar os pontos de extremidade físicos e virtuais.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
[Inscreva-se para alterar as notificações](webhooks.md) em uma [definição de tarefa de impressão](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gestão corporativa
As atualizações de [Novembro](changelog.md#november-2020) do Intune para a versão beta.

### <a name="identity-and-access"></a>Identidade e acesso
- Especificar URLs para envio de tokens de entrada de usuário e URIs de códigos de autorização e tokens de acesso, na propriedade **spa** de [aplicativo](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true).
- Personalize a aparência das telas de entrada do Azure Active Directory usando as [propriedades de identidade visual organização](/graph/api/resources/organizationalbrandingproperties?view=graph-rest-beta&preserve-view=true). As organizações podem personalizar com base na localidade para usuários específicos.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
A estreia da [API de revisão de acesso para a associação de grupo](/graph/api/resources/accessreviewsv2-overview?view=graph-rest-beta&preserve-view=true) para revisar regularmente o acesso de usuários, certifique-se de que apenas as pessoas certas tenham acesso contínuo e gerenciem os membros do grupo de forma eficiente.

### <a name="search"></a>Pesquisar
Você pode agregar resultados de pesquisa de tipo numérico ou cadeia de caracteres que são importados por [conectores do Microsoft Graph](/microsoftsearch/connectors-overview) e que são configurados para serem refináveis no [esquema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true). Veja mais informações sobre[refinar resultados de pesquisa usando agregações](search-concept-aggregation.md).

## <a name="october-2020-new-and-generally-available"></a>Outubro de 2020: novo e geralmente disponível

### <a name="application"></a>Aplicativo
- Permitir [email como uma ID de login alternativa para o Azure Active Directory](/azure/active-directory/authentication/howto-authentication-use-email-signin), usando uma política de [Descoberta de Realm Inicial](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#home-realm-discovery). Uma política de Descoberta de Realm Inicial determina, depois que um usuário fornece uma ID de entrada, se deve solicitar a autenticação do usuário. Nesse caso, definir a propriedade **AlternateIdLogin** de um recurso [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy) pode habilitar que um usuário conecte-se com um endereço de email.
- Obtenha as informações verificadas do fornecedor para um [aplicativo](/graph/api/resources/application) ou [servicePrincipal](/graph/api/resources/serviceprincipal) e [defina](/graph/api/application-setverifiedpublisher) ou [remova](/graph/api/application-unsetverifiedpublisher) as informações verificadas do fornecedor para um **aplicativo**.

### <a name="change-notifications"></a>Mudar notificações
Os aplicativos de produção agora podem assinar notificações de ciclo de vida do Outlook [mensagem](/graph/api/resources/message), [evento](/graph/api/resources/event) e [contato](/graph/api/resources/contact) e do Microsoft Teams [chatMessage](/graph/api/resources/chatmessage) em ordem a [reduzir a falta de assinaturas e alterar as notificações](webhooks-lifecycle.md).

### <a name="identity-and-access"></a>Identidade e acesso
- GA de opções avançadas de consulta do sistema OData (`$count`,`$search` e `$filter`) em objetos de diretório.
- Confira exemplos que mostram o elenco do OData em objetos de diretório.
- Confira a seção Identidade e acesso das atualizações de [outubro](changelog.md#october-2020) no log de mudanças para obter as listas de APIs aprimoradas.

### <a name="teamwork"></a>Trabalho em equipe
- O GA do conjunto completo de operações CRUD para [chatMember](/graph/api/resources/conversationmember) e [aadUserConversationMember](/graph/api/resources/aaduserconversationmember). Esses recursos representam um membro em um chat ou conversa de canal, que pode ou não ser um usuário no Microsoft Azure Active Directory.
- O GA de notificações de ciclo de vida para recursos do Teams de [chatMessage](/graph/api/resources/chatmessage), para [reduzir assinaturas ausentes e notificações de alteração](webhooks-lifecycle.md).

### <a name="to-do-tasks"></a>Tarefas pendentes
O GA da [API Microsoft To-Do](/graph/api/resources/todo-overview?view=graph-rest-1.0&preserve-view=true) - use a API de tarefas em um aplicativo de produção para criar e gerenciar tarefas que fazem parte do fluxo de trabalho de um usuário, como criar uma tarefa de um email.  

### <a name="users"></a>Comercial
Obtenha novas propriedades aplicáveis ​​a um [usuário](/graph/api/resources/user) que é funcionário corporativo: data de contratação, associação organizacional, como divisão e centro de custo, e tipo de funcionário, como consultor, contratado ou fornecedor. Essas propriedades exigem a especificação do `$select`parâmetro de consulta OData na operação GET.

## <a name="october-2020-new-in-preview-only"></a>Outubro de 2020: novo apenas na pré-visualização

### <a name="cloud-communications--online-meeting"></a>Comunicações em nuvem | Reunião online
- Diferencie a função de um participante em uma [reunião online](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) como um participante ou apresentador, usando a propriedade **função** do tipo [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo?view=graph-rest-beta&preserve-view=true).
- Obtenha uma [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) ao [filtrar na propriedade joinWebUrl da reunião](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-3-retrieve-an-online-meeting-by-joinweburl).

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem

- Descontinue a ação **uploadData** em favor de [criar uma sessão de upload](/graph/api/printdocument-createuploadsession?view=graph-rest-beta&preserve-view=true) para [fazer upload de um documento](upload-data-to-upload-session.md) para uma impressora ou compartilhamento de impressora.
- Cancele a propriedade **configuração** em [printDocument](/graph/api/resources/printdocument?view=graph-rest-beta&preserve-view=true) em favor de uma propriedade de **configuração** semelhante em [printJob](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true).
- Obtenha o URL do trabalho de origem ou de destino para um **printJob** que está sendo redirecionado, usando a propriedade **redirectedFrom** ou **redirectedTo**.
- Obtenha o status atual de um **printJob** usando a propriedade **estado** e a nova propriedade **detalhes**.
- Obtenha a coleção de compartilhamentos de impressora associados a uma [impressora](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true) usando a relação **compartilhamentos**. 
- Substitua a propriedade **processingStateReasons** da **impressora** em favor da propriedade **status**. A propriedade **status** é do tipo [status da impressora](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true) e expõe uma propriedade **detalhes**. Use a propriedade **detalhes** para identificar o motivo de uma impressora estar no estado atual.
- Cancele a propriedade **feedDirections** em [printerCapabilities](/graph/api/resources/printercapabilities?view=graph-rest-beta&preserve-view=true) em favor da propriedade **feedOrientations**, para obter orientações de alimentação suportadas por uma impressora.
- Confira a seção de impressão na nuvem das atualizações de [outubro](changelog.md#october-2020) no log de mudanças para algumas renomeações de API, propriedades e algumas outras descontinuações.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gestão corporativa
Atualizações do Intune de [outubro](changelog.md#october-2020) para a versão beta.

### <a name="files"></a>Arquivos
[Revogar](/graph/api/permission-revokegrants?view=graph-rest-beta&preserve-view=true) o acesso à para um [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) ou [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true) concedido por meio de um link de compartilhamento.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- Gerenciar [políticas de método de autenticação](/graph/api/resources/authenticationmethodspolicies-overview?view=graph-rest-beta&preserve-view=true) para identificar usuários que podem usar métodos de autenticação multifator específicos para entrar no Azure Active Directory. Configure políticas para definir o seguinte:
  - Os tipos de chaves de segurança FIDO2 que podem ser usadas no locatário do Azure AD.
  - Os usuários ou grupos de usuários que têm permissão para usar chaves de segurança FIDO2 ou a Entrada por Telefone sem Senha para entrar no Azure AD.
- Configure um [método de autenticação de email](/graph/api/resources/emailauthenticationmethod?view=graph-rest-beta&preserve-view=true) para que os usuários possam redefinir a senha sozinhos.
- Use o [Azure AD B2C](/azure/active-directory-b2c/overview) e [escolha um mecanismo para configurar e permitir que os usuários finais se autentiquem por contas locais](/graph/api/resources/b2cauthenticationmethodspolicy?view=graph-rest-beta&preserve-view=true).
- Use o `Policy.ReadWrite.AuthenticationMethod` para ler ou gravar as políticas do método de autenticação de uma organização, como uma permissão delegada em nome de um usuário conectado ou como uma permissão de aplicativo sem ter um usuário conectado.
- Especifique em uma [política de autorização](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true) se e quem pode convidar usuários externos para uma organização.

### <a name="people-and-workplace-intelligence--insights"></a>Inteligência de pessoas e local de trabalho | Intuições 
Os administradores podem ver os [exemplos de uso de cmdlets do Windows PowerShell](insights-customize-item-insights-privacy.md#configure-item-insights-settings-via-powershell) para personalizar as configurações de percepção do item para uma organização.

### <a name="teamwork"></a>Trabalho em equipe
- Use o atributo de instância **channelCreationMode** para indicar que um [canal](/graph/api/resources/channel?preserve-view=true&view=graph-rest-beta#instance-attributes) está sendo criado para servir à migração de dados. Use o [completeMigration](/graph/api/channel-completemigration?view=graph-rest-beta&preserve-view=true) para indicar que a migração terminou, de forma que os membros possam postar e ler mensagens.
- Use o atributo de instância **teamCreationMode** para indicar que uma [equipe](/graph/api/resources/team?preserve-view=true&view=graph-rest-beta#instance-attributes) está sendo criada para atender à migração. Use o [completeMigration](/graph/api/team-completemigration?view=graph-rest-beta&preserve-view=true) para indicar que a migração terminou, de forma que as operações dos membros podem acontecer e os membros podem postar mensagens.

## <a name="september-2020-new-and-generally-available"></a>Setembro de 2020: novo e disponível para o público geral

### <a name="calendar"></a>Calendário
O GA da propriedade **transactionId** do recurso de [evento](/graph/api/resources/event), que é definido opcionalmente por um aplicativo cliente para evitar operações de POSTAGEM redundantes em caso de o cliente tentar criar o mesmo evento. Isso é útil quando a conectividade de rede baixa faz com que o cliente expire antes de receber uma resposta do servidor para a solicitação anterior de criação de evento do cliente.

### <a name="cloud-communications"></a>Comunicações na nuvem
[Excluir um participante](/graph/api/participant-delete) de uma [chamada](/graph/api/resources/call). Você pode usar essa operação mesmo em situações em que é necessário excluir um participante de uma chamada ativa.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
As atualizações de [setembro](changelog.md#september-2020) do Intune para a versão v1.0.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
Os [APIs das unidades administrativas](/graph/api/resources/administrativeunit) permitem às organizações subdividir seu Azure Active Directory e delegar tarefas administrativas a essas subdivisões. As subdivisões podem representar regiões, departamentos, centros de custo e assim por diante.

### <a name="reports"></a>Relatórios
[Obtenha um relatório que inclua o número de usuários exclusivos](/graph/api/reportroot-getemailappusageversionsusercounts) do Outlook 2019 e do Outlook no Microsoft 365.

### <a name="teamwork"></a>Trabalho em equipe
- Obtenha a propriedade **lastEditedDateTime** para descobrir quando um remetente editar pela última vez uma [mensagem de chat](/graph/api/resources/chatmessage).
- Obtenha a propriedade **lastModifiedDateTime** para descobrir quando um remetente cria uma mensagem de bate-papo ou quando alguém a altera de outras maneiras, incluindo a adição ou a remoção de uma reação. 
- [Receba notificações sobre alterações](webhooks.md) em [mensagens de chat](/graph/api/resources/chatmessage).
- [Atualizar](/graph/api/chatmessage-update?view=graph-rest-beta&preserve-view=true) propriedade **policyViolation** de uma [chatMessage](/graph/api/resources/chatmessagepreserve-view=true) em um [canal](/graph/api/resources/channel&preserve-view=true) ou [chat](/graph/api/resources/chat&preserve-view=true), permitindo que os aplicativos de prevenção contra perda de dados (DLP) monitorem [violação de política da mensagem de chat](/graph/api/resources/chatmessagepolicyviolation?preserve-view=true) para evitar que as mensagens contenham dados que os usuários não devem enviar.

### <a name="use-the-sdks"></a>Use os SDKs
Com o lançamento do [SDK do Microsoft Graph PowerShell](https://github.com/microsoftgraph/msgraph-sdk-powershell) o acesso a toda a superfície do Microsoft Graph agora é simples e consistente.

### <a name="use-the-toolkit"></a>Usar o kit de ferramentas
Experimente o novo tutorial de introdução passo a passo para o Microsoft Graph Toolkit e experimente a comodidade que o Toolkit oferece:
- [Criar um aplicativo Web (JavaScript)](./toolkit/get-started/build-a-web-app.md)
- [Criar uma web part do Microsoft Office SharePoint Online](./toolkit/get-started/build-a-sharepoint-web-part.md)
- [Criar uma guia do Microsoft Teams](./toolkit/get-started/build-a-microsoft-teams-tab.md)
- [Usar o kit de ferramentas com reagir](./toolkit/get-started/use-toolkit-with-react.md)
- [Usar o kit de ferramentas com o Angular](./toolkit/get-started/use-toolkit-with-angular.md)

### <a name="users"></a>Usuários
Além de obter o endereço SMTP de um [usuário](/graph/api/resources/user) por meio da propriedade de **email**, você pode definir essa propriedade e atualizar o endereço de email do usuário. 

## <a name="september-2020-new-in-preview-only"></a>Setembro de 2020: novidades somente na pré-visualização

### <a name="application"></a>Aplicativo
Crie, liste ou exclua [classificações de permissões delegadas](/graph/api/resources/delegatedpermissionclassification?view=graph-rest-beta&preserve-view=true) que uma [entidade de serviço](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) expõe. Use as classificações de permissão delegada em combinação com as [configurações de consentimento do usuário](/azure/active-directory/manage-apps/configure-user-consent) para definir limites sobre quando os usuários finais têm permissão para dar consentimento aos aplicativos.

### <a name="cloud-communications"></a>Comunicações na nuvem
- A substituição da propriedade **autoAdmittedUsers** do [ onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true). Em vez disso, use a propriedade **lobbyBypassSettings** e seus [valores](/graph/api/resources/lobbybypasssettings?view=graph-rest-beta&preserve-view=true#lobbybypassscope-values).
- Use configurações adicionais sobre como anunciar os chamadores que ingressam em uma reunião online (propriedade **isEntryExitAnnounced**) e permitir apresentadores específicos na reunião (propriedade **allowedPresenters**).

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- [Obtenha os documentos para cada um dos trabalhos de impressão associados a uma impressora](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true), aplicando uma `$expand` [opção de consulta do sistema OData](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters). 
- Filtre trabalhos de impressão pelo usuário que os criou, aplicando uma opção de`$filter` [consulta do sistema OData](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters).

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
As atualizações de [setembro](changelog.md#september-2020) do Intune para a versão beta.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- [Obtenha uma chave de recuperação do BitLocker](/graph/api/bitlockerrecoverykey-get?view=graph-rest-beta&preserve-view=true) em nome do usuário conectado que é o proprietário do dispositivo ou em uma função adequada. Obter uma chave de recuperação gera um [log de auditoria](/azure/active-directory/reports-monitoring/concept-audit-logs), em paridade com a experiência do usuário final.
- Obtenha a quantidade total e usada da [cota do diretório](/graph/api/resources/directorysizequota?view=graph-rest-beta&preserve-view=true) de uma [organização](/graph/api/resources/organization?view=graph-rest-beta&preserve-view=true), por meio da propriedade **directorySizeQuota**.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
É possível incluir uma [agenda](/graph/api/resources/requestschedule?view=graph-rest-beta&preserve-view=true) ao solicitar ou remover uma [atribuição de um usuário para um pacote do Access](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true), que especifica o acesso aos grupos, aplicativos ou sites do SharePoint.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
As organizações podem [obter](/graph/api/continuousaccessevaluationpolicy-get?view=graph-rest-beta&preserve-view=true) ou [atualizar](/graph/api/continuousaccessevaluationpolicy-update?view=graph-rest-beta&preserve-view=true) a [política de avaliação de acesso contínuo](/graph/api/resources/continuousAccessEvaluationPolicy?view=graph-rest-beta&preserve-view=true) para gerenciar sessões de autenticação em tempo real.

### <a name="search"></a>Pesquisar

- Use recursos adicionais no [API de Pesquisa da Microsoft](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true) para OneDrive, SharePoint, conectores do Microsoft Graph: 

  - Obtenha [tipos adicionais](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#scope-search-based-on-entity-types) de conteúdo do OneDrive e do Microsoft Office SharePoint Online: **unidade**, **lista**, **listItem** e **site**. 
  - Propriedades de escopo nos resultados da pesquisa para [propriedades selecionadas](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#get-selected-properties). 
  - Obtenha propriedades personalizadas no recurso [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true).
  - [Classifique](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#sort-search-results) os resultados da pesquisa do OneDrive e do Microsoft Office SharePoint Online em qualquer propriedade classificável.
  - [Refine os resultados usando agregações](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#refine-results-using-aggregations) para o OneDrive e o Microsoft Office SharePoint Online.
- Consultar dados externos ingeridos pelos conectores do Microsoft Graph em [mais de um de conexão](./search-concept-custom-types.md).
- Aproveite o conteúdo aprimorado para os conectores do Microsoft Graph para saber mais sobre:
  - [Gerenciando Conectores](connecting-external-content-manage-connections.md)
  - [Gerenciar esquema](connecting-external-content-manage-schema.md)
  - [Gerenciar itens](connecting-external-content-manage-items.md)
- Acompanhe o estado de uma[conexão](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true)do Microsoft Graph.
- Defina um [grupo externo](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) a fim de definir permissões em objetos de [item externo](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) adicionados a uma [conexão](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true) do Microsoft Graph. Os grupos externos podem representar os grupos do Active Directory que não sejam do Azure ou construções similares, como unidades de negócios, que determinam permissões sobre o conteúdo na fonte de dados externa.

### <a name="teamwork"></a>Trabalho em equipe
- Obtenha a data e a hora em que um [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true)do Teams ou [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) é criada.


## <a name="august-2020-new-and-generally-available"></a>Agosto de 2020: novo e disponível para o público geral

### <a name="change-notifications"></a>Notificações de alteração
[Acompanhar alterações](delta-query-overview.md) de recursos com suporte no Microsoft Graph para a nuvem nacional do governo dos EUA.

### <a name="cloud-communications"></a>Comunicações na nuvem
- [Cancele](/graph/api/call-cancelmediaprocessing) as ações de IVR (Resposta de Voz Interativas) que estão sendo processadas ou na fila, estejam elas [reproduzindo um prompt de áudio](/graph/api/call-playprompt) ou [gravando uma resposta](/graph/api/call-record).
- Obtenha [informações sobre as transcrições da chamada](/graph/api/resources/calltranscriptioninfo) por meio da propriedade **transcrição**.

### <a name="teamwork"></a>Trabalho em equipe
- Use uma maneira alternativa de [criar uma equipe](/graph/api/team-post) diretamente sem criar um grupo primeiro.
- Use a propriedade de navegação **members** para adicionar membros a uma equipe com maior confiabilidade e latência menor.
- Obtenha o status de publicação de um [aplicativo](/graph/api/resources/teamsapp) do Microsoft Teams através da propriedade **publishingState** da [definição do aplicativo](/graph/api/resources/teamsappdefinition). Os valores de status possíveis são `submitted`, `published` e `rejected`. Veja um [exemplo](/graph/api/teamsapp-list?view=graph-rest-beta&preserve-view=true#example-3-list-applications-with-a-given-id-and-return-the-submission-review-state).
- Use a permissão delegada `AppCatalog.Submit` para permitir que um usuário [envie um aplicativo](/graph/api/teamsapp-publish) e solicite a revisão do administrador. Use a mesma permissão para um usuário [cancelar](/graph/api/teamsapp-delete) um aplicativo enviado anteriormente que não foi publicado. 


## <a name="august-2020-new-in-preview-only"></a>Agosto de 2020: novidade apenas na versão prévia

### <a name="applications"></a>Aplicativos
Ofereça suporte a logon único baseado em senha para recursos de aplicativos de [entidade de serviço](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) e especifique essas [configurações](/graph/api/resources/passwordsinglesignonsettings?view=graph-rest-beta&preserve-view=true) na propriedade **passwordSingleSignOnSettings**. Para obter informações sobre logon único baseado em senha no Azure AD, confira [configurar logon único baseado em senha](/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).

### <a name="calendar"></a>Calendário
Melhore o suporte programático para cenários que envolvem um [evento](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) recorrente:
- Identifique com confiança qualquer ocorrência em uma série recorrente, incluindo uma ocorrência modificada ou cancelada, usando a propriedade **occurrenceId**.
- Obtenha qualquer exceção em uma série recorrente usando a propriedade **exceptionOccurrences**.
- Obtenha qualquer cancelamento em uma série usando a propriedade **cancelledOccurrences**.

### <a name="change-notifications"></a>Alterar notificações
- Use a propriedade **includeResourceData** de uma [assinatura](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true) para [configurar notificações de alteração que incluem dados de recursos](webhooks-with-resource-data.md). Não use a propriedade **includeProperties**.
- Receba [notificações de alteração via Hub de Eventos](change-notifications-delivery.md).

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- Conceda acesso para todos os usuários e grupos a um [compartilhamento de impressora](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) usando a propriedade **allowAllUser**.
- Use novas permissões delegadas e de aplicativo para acessar ou gerenciar um [documento de impressão](/graph/api/resources/printDocument?view=graph-rest-beta&preserve-view=true), [trabalho de impressão](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true), [impressora](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true), [compartilhamento de impressora](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true)ou [definição de tarefa de impressão](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true). Para obter detalhes, consulte as atualizações de [agosto](changelog.md#august-2020) sobre impressão na nuvem.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações de [agosto](changelog.md#august-2020) do Intune na versão beta.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- Personalize um [contrato de termos de uso](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true) para oferecer suporte a uma data de vencimento e cadência de contrato, exigir que o usuário aceite o contrato por dispositivo ou aceite novamente o contrato em uma frequência definida. 
- Use a propriedade do **file** para navegar até um [contrato personalizado](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true) para termos de uso. Não use a propriedade **files**.
- Adicione, remova e liste patrocinadores internos ou externos que podem aprovar solicitações de uma [organização conectada](/graph/api/resources/connectedorganization?view=graph-rest-beta&preserve-view=true) para acessar um grupo, aplicativo ou site do Microsoft Office SharePoint Online. Consulte [gerenciamento de direitos](/graph/api/resources/entitlementmanagement-overview?view=graph-rest-beta&preserve-view=true) para obter mais informações.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- Habilite a personalização de uma [política de autorização](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true) para um locatário, como autorizar que a [função de usuário padrão](/graph/api/resources/defaultuserrolepermissions?view=graph-rest-beta&preserve-view=true) crie aplicativos, grupos de segurança ou leia outros usuários, e autorizar que os usuários se inscrevam em assinaturas baseadas em email, associem o locatário por validação de email ou permita que os usuários redefinam senhas de maneira autônoma.
- Gerenciar [políticas configuráveis e predefinidas como fluxos de usuário em um locatário do Azure Active Directory B2C](/graph/api/resources/b2cuserflows?view=graph-rest-beta&preserve-view=true). Confira mais informações sobre o [fluxo do usuário B2C](/azure/active-directory-b2c/user-flow-overview).
- Habilite a [experiência de inscrição de maneira autônoma como o fluxo de usuário B2X em um locatário do Azure Active Directory](/graph/api/resources/b2xuserflows?view=graph-rest-beta&preserve-view=true). Saiba mais sobre [inscrição de maneira autônoma](/azure/active-directory/external-identities/self-service-sign-up-overview).

### <a name="people-and-workplace-intelligence--profile"></a>Inteligência de pessoas e do local de trabalho | Perfil
Adicione e gerencie as seguintes propriedades adicionais no [perfil](/graph/api/resources/profile?view=graph-rest-beta&preserve-view=true) de um usuário, e que podem ser exibidas em experiências pessoais compartilhadas no Microsoft 365 e em aplicativos de terceiros:
- [addresses](/graph/api/resources/itemAddress?view=graph-rest-beta&preserve-view=true)
- [anniversaries](/graph/api/resources/personAnniversary?view=graph-rest-beta&preserve-view=true)
- [awards](/graph/api/resources/personAward?view=graph-rest-beta&preserve-view=true)
- [certifications](/graph/api/resources/personCertification?view=graph-rest-beta&preserve-view=true)
- [notes](/graph/api/resources/personAnnotation?view=graph-rest-beta&preserve-view=true)
- [patents](/graph/api/resources/itemPatent?view=graph-rest-beta&preserve-view=true)
- [publications](/graph/api/resources/itemPublication?view=graph-rest-beta&preserve-view=true)


### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
Obtenha [relatórios sobre o uso de aplicativos do Microsoft 365](/graph/api/resources/microsoft-365-apps-usage-report?view=graph-rest-beta&preserve-view=true), especificamente sobre detalhes de usuários, contagens de usuários e contagens de usuários da plataforma.

### <a name="teamwork"></a>Trabalho em equipe
Obtenha [conteúdo hospedado em uma mensagem de chat](/graph/api/resources/chatMessageHostedContent?view=graph-rest-beta&preserve-view=true), como imagens ou trechos de códigos. Veja um [exemplo](/graph/api/chatmessagehostedcontent-get?view=graph-rest-beta&preserve-view=true&branch=master#example-2-get-hosted-content-bytes-for-an-image) para obter os bytes de conteúdo de uma imagem.

### <a name="to-do-tasks"></a>Tarefas To do
- Lançamento de um novo conjunto de API para o [Microsoft To Do](todo-concept-overview.md), permitindo aos usuários de aplicativos a organização e o acompanhamento de tarefas pessoais através de aplicativos do cliente Microsoft 365. Consulte [Use a API do Microsoft To Do](/graph/api/resources/todo-overview?view=graph-rest-beta&preserve-view=true) para mais informações.
- Preterido a [API de tarefas do Outlook](/graph/api/resources/outlooktask?view=graph-rest-beta&preserve-view=true).


## <a name="july-2020-new-and-generally-available"></a>Julho de 2020: novos e disponíveis para o público em geral

### <a name="calendar"></a>Calendário
GA do recurso que permite aos organizadores permitir propostas de horário alternativo para reuniões ou convites para [propor novos horários para uma reunião](outlook-calendar-meeting-proposals.md) quando eles [aceitarem provisoriamente](/graph/api/event-tentativelyaccept?view=graph-rest-1.0&preserve-view=true&preserve-view=true) ou [recusarem](/graph/api/event-decline?view=graph-rest-1.0&preserve-view=true&preserve-view=true) um evento.

### <a name="change-notifications"></a>Notificações de alteração
Removida do recurso [changeNotification](/graph/api/resources/changenotification) a propriedade **sequenceNumber** introduzida erroneamente.

### <a name="groups"></a>Grupos
DG das seguintes propriedades para a entidade [group](/graph/api/resources/group): **assignedLabels**, **expirationDateTime**, **membershipRule**, **membershipRuleProcessingState**, **preferredLanguage** e **theme**.

### <a name="identity-and-access"></a>Identidade e acesso
- Remover um usuário como proprietário registrado ou usuário de um [dispositivo](/graph/api/resources/device).
- Acompanhe as alterações de representações locais de aplicativos recém-criadas, atualizadas ou deletadas (representada por recursos[servicePrincipals](/graph/api/resources/serviceprincipal)) e permissões delegadas concedidas (representadas por recursos[oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant)) sem executar uma leitura completa de toda a coleção de recursos.
- GA da [política para reforçar o padrão de segurança](/graph/api/resources/identitysecuritydefaultsenforcementpolicy) que protege as organizações contra ataques comuns.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- GA de [políticas de acesso condicional](/graph/api/resources/conditionalAccessPolicy) que são regras personalizadas que definem um cenário de acesso.
- GA de [posições nomeadas](/graph/api/resources/namedLocation) representando regras personalizadas que definem os locais de rede usados em uma política de acesso condicional.

### <a name="schema-extensions"></a>Extensões de esquema
O recurso [extensões de esquema](/graph/api/resources/schemaextension) já está disponível para o público em geral no[Microsoft Cloud for US Government](./deployments.md).

### <a name="teamwork"></a>Trabalho em equipe
Use as permissões delegadas de `TeamsAppInstallation.ReadForTeam` ou `TeamsAppInstallation.ReadWriteForTeam` ou permissões de aplicativo de `TeamsAppInstallation.ReadForTeam.All` ou `TeamsAppInstallation.ReadWriteForTeam.All` para [listar aplicativos instalados em uma equipe](/graph/api/teamsappinstallation-list).

## <a name="july-2020-new-in-preview-only"></a>Julho de 2020: novos apenas na visualização

### <a name="cloud-communications"></a>Comunicações na nuvem
- Use a operação [atualizar](/graph/api/onlinemeeting-update?view=graph-rest-beta&preserve-view=true&preserve-view=true) para atualizar **startDateTime**, **endDateTime**, **participantes**, ou propriedade de **assunto** de uma [reunião online](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true&preserve-view=true).
- Inscreva-se para receber notificações sobre alterações na disponibilidade de um usuário do Microsoft Teams, conforme representado pelo recurso [presence](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true).

### <a name="cloud-communications--call-records"></a>Comunicação em nuvem | Gravação
- [Obtenha](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta&preserve-view=true) os registros de chamadas da rede pública de telefonia comutada (PSTN).
- [Obtenha](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta&preserve-view=true) os registros de chamadas de roteamento direto.

### <a name="compliance--ediscovery"></a>Conformidade | Descoberta eletrônica
Estréia dos [Casos de descoberta eletrônica](/graph/api/resources/ediscoverycase?view=graph-rest-beta&preserve-view=true) que podem conter responsáveis, bloqueios, coleções, conjuntos de revisão, e exportações que podem ser usados como evidência em casos jurídicos.
Os aplicativos agora podem [consultar](/graph/api/resources/reviewsetquery?view=graph-rest-beta&preserve-view=true) e [revisar o conjunto de dados](/graph/api/resources/reviewset?view=graph-rest-beta&preserve-view=true) coletado para uso em litígio, investigação ou solicitação regulatória. Esse estreia faz parte da [Descoberta Eletrônica Avançada](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide&preserve-view=true)do Microsoft 365.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- Use as permissões do aplicativo `Printer.ReadWrite.All` e a [codificação do IPP (Protocolo de Impressão via Internet)](https://tools.ietf.org/html/rfc8010) para [atualizar uma impressora ](/graph/api/printer-update?view=graph-rest-beta&preserve-view=true).
- Use uma das permissões de aplicativo, `PrintJob.ReadBasic.All`, `PrintJob.Read.All`, `PrintJob.ReadWriteBasic.All`ou `PrintJob.ReadWrite.All`, para [obter um trabalho de impressão](/graph/api/printjob-get?view=graph-rest-beta&preserve-view=true) ou [listar trabalhos de impressão para uma impressora](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true).
- Quando [obtiver um trabalho de impressão](/graph/api/printjob-get?view=graph-rest-beta&preserve-view=true), use `$expand` para obter [tarefas de impressão](/graph/api/resources/printtask?view=graph-rest-beta&preserve-view=true) que estão executando ou que foram executadas no trabalho. Imprimir tarefas, [definições de tarefas](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true)e [disparadores de tarefas](/graph/api/resources/printtasktrigger?view=graph-rest-beta&preserve-view=true) são usados em [impressão segura](universal-print-concept-overview.md#enable-pull-printing).
- [Redirecione um trabalho de impressão](/graph/api/printjob-redirect?view=graph-rest-beta&preserve-view=true) para uma impressora diferente, como parte da impressão segura.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações do Intune em [julho](changelog.md#july-2020) em beta.

### <a name="groups"></a>Grupos
Use a propriedade **isAssignableToRole** de um [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) do Microsoft 365 e a defina durante a criação de um grupo para indicar se ele pode ser atribuído a uma função do Azure AD. Isso [ajuda a gerenciar as atribuições de função no Azure AD](/azure/active-directory/users-groups-roles/roles-groups-concept), de modo que, em vez de atribuir um usuário individual a uma função do Azure AD, um administrador global ou um administrador de funções privilegiadas pode criar um grupo do Microsoft 365 e atribuir o grupo a essa função, para que quando os usuários se unam ao _grupo_, eles recebam a função pretendida indiretamente.

### <a name="identity-and-access"></a>Identidade e acesso
- [Adquira um token de acesso](/graph/api/synchronization-synchronization-acquireAccessToken?view=graph-rest-beta&preserve-view=true) para autorizar o serviço de provisionamento do Azure AD para provisionar usuários em um aplicativo.
- [Obtenha](/graph/api/entitlementmanagementsettings-get?view=graph-rest-beta&preserve-view=true) ou [atualize](/graph/api/entitlementmanagementsettings-update?view=graph-rest-beta&preserve-view=true) as configurações de gerenciamento de qualificação que controlam o acesso a grupos, aplicativos e sites do SharePoint Online para usuários internos e externos à sua organização. 

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- Inclua os níveis de risco do usuário (`low`, `medium`, `high`, `none`) como consideração para aplicar uma [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- [Use a alteração de senha como um controle Grant](/graph/api/resources/conditionalaccessgrantcontrols?view=graph-rest-beta&preserve-view=true#special-considerations-when-using-passwordchange-as-a-control) para passar uma política de acesso condicional.
- Use um [provedor de conexão de ID aberta](/graph/api/resources/openidconnectprovider?view=graph-rest-beta&preserve-view=true) (ODIC) como um provedor de identidade em um locatário do Azure AD e um locatário do Azure AD B2C. Sua propriedade **claimsMapping** permite que o Azure AD [mapeie as declarações](/graph/api/resources/claimsmapping?view=graph-rest-beta&preserve-view=true) de um provedor OIDC para as declarações que o Azure AD reconhece e usa.

### <a name="people-and-workplace-intelligence--insights"></a>Inteligência social e do ambiente de trabalho | Ideias
Use mais o [controle de privacidade granular](insights-customize-item-insights-privacy.md) sobre a disponibilidade e a exibição das [informações do item](/graph/api/resources/iteminsights?view=graph-rest-beta&preserve-view=true) no Microsoft 365. Essas informações representam as relações entre um usuário e documentos no OneDrive for Business, calculadas usando uma análise avançada e técnicas de aprendizado de máquina. 

### <a name="people-and-workplace-intelligence--profile-card-customization"></a>Inteligência de pessoas e local de trabalho | Personalização de cartão de perfil
Os administradores podem [personalizar as propriedades expostas no cartão de perfil de suas organizações](add-properties-profilecard.md) usando a API para [propriedade de cartão de perfil](/graph/api/resources/profilecardproperty?view=graph-rest-beta&preserve-view=true).

### <a name="sites-and-lists"></a>Sites e listas
Acesse a taxonomia do [repositório de termos](/graph/api/resources/termstore-store?view=graph-rest-beta&preserve-view=true) a hierarquia que consite em recursos de [grupo](/graph/api/resources/termstore-group?view=graph-rest-beta&preserve-view=true), [definição](/graph/api/resources/termstore-set?view=graph-rest-beta&preserve-view=true), e [termo](/graph/api/resources/termstore-term?view=graph-rest-beta&preserve-view=true), e [relacione](/graph/api/resources/termstore-relation?view=graph-rest-beta&preserve-view=true) recursos entre os termos.

### <a name="workbooks-and-charts"></a>Pastas de trabalho e gráficos
[Obtenha o status e todos os resultados](/graph/api/workbookoperation-get?view=graph-rest-beta&preserve-view=true) de uma operação [de longa execução](/graph/api/resources/workbookoperation?view=graph-rest-beta&preserve-view=true) em uma [pasta de trabalho](/graph/api/resources/workbook?view=graph-rest-beta&preserve-view=true).



## <a name="june-2020-new-and-generally-available"></a>Junho de 2020: novos e disponíveis para o público em geral

### <a name="cloud-communications--online-meeting"></a>Comunicações na nuvem | Reunião online
- Use o cabeçalho HTTP `Accept-Language`ao [criar uma reunião online](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0&preserve-view=true&preserve-view=true) para fornecer informações de participação baseadas no local.
- Use [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-1.0&preserve-view=true&preserve-view=true) para retornar uma reunião online que tenha um valor **externalId** específico ou, caso nenhum valor desse tipo exista, para simplificar a incorporação da reunião resultante a um calendário de terceiros.

### <a name="files"></a>Arquivos
- Suporte aprimorado à sincronização:
  - Use a propriedade **pendingOperations** para identificar quaisquer [operações](/graph/api/resources/pendingoperations) que possam atualizar o conteúdo binário de um arquivo [driveItem](/graph/api/resources/driveitem) e que estejam pendentes.
  - [Restaure](/graph/api/driveitem-restore) um **driveItem** que tenha sido excluído e esteja na lixeira do OneDrive pessoal.
- Obtenha ou defina a orientação de uma [foto](/graph/api/resources/photo). A configuração é compatível com o OneDrive Personal.
- Use o Algoritmo de Hash Seguro (SHA-256) para aprimorar a segurança e a integridade dos dados do [arquivo](/graph/api/resources/file).
- Use o parâmetro `deferCommit` para adiar a criação final ao [carregar geralmente um arquivo grande](/graph/api/driveitem-createuploadsession) no OneDrive for Business, até que um aplicativo faça uma solicitação para concluir o carregamento.
- Use a propriedade **fileSize** para fornecer uma estimativa como parte do parâmetro do **item**, de modo a fazer uma verificação de cota antes de [carregar um arquivo](/graph/api/driveitem-createuploadsession) no OneDrive pessoal.
- Localize [storagePlanInformation](/graph/api/resources/storageplaninformation) por meio da propriedade **cota** de um recurso de [unidade](/graph/api/resources/drive) para ver se existem planos de uma cota de armazenamento mais alta disponíveis.

### <a name="groups"></a>Grupos
Use as permissões de aplicativo `Group.Read.All` e `Group.ReadWrite.All` para obter recursos de uma [conversa](/graph/api/resources/conversation) do grupo e de uma [sequência de conversa](/graph/api/resources/conversationthread).

### <a name="identity-and-access"></a>Identidade e acesso 
- Disponibilidade generalizada de dois conjuntos de APIs de [proteção de identidade](/graph/api/resources/identityprotectionroot): APIs de [detecção de riscos](/graph/api/resources/riskdetection) e de [usuário arriscado](/graph/api/resources/riskyuser).

### <a name="security"></a>Segurança
- Rastreie o seguinte como propriedades de um [alerta](/graph/api/resources/alert?view=graph-rest-1.0&preserve-view=true&preserve-view=true):
  - IDs de incidentes relacionados ao alerta.
  - Identificar um [recurso](/graph/api/resources/securityResource?view=graph-rest-1.0&preserve-view=true#securityresourcetype-values) como atacado ou como um recurso relacionado no alerta.
  - Especificar os locais de origem e destino de uma [conexão de rede](/graph/api/resources/networkconnection?view=graph-rest-1.0&preserve-view=true) relacionada ao alerta.

### <a name="sites-and-lists"></a>Sites e listas
Especifique dados de localização geográfica em uma [definição de coluna](/graph/api/resources/columndefinition) para um recurso de uma [lista](/graph/api/resources/list) do SharePoint.

### <a name="teamwork"></a>Trabalho em equipe
- Use a permissão delegada [AppCatalog.Read.All](./permissions-reference.md#appcatalog-resource-permissions) para listar [aplicativos](/graph/api/resources/teamsapp?view=graph-rest-1.0&preserve-view=true) do catálogo de aplicativos do Microsoft Teams.
- [Obtenha informações sobre a pasta](/graph/api/channel-get-filesfolder) que mapeia para a guia **Arquivos** de um [canal](/graph/api/resources/channel) do Teams.
- [Obtenha o do canal padrão](/graph/api/team-get-primarychannel) — rotulado como **Geral** — de uma [equipe](/graph/api/resources/team).


## <a name="june-2020-new-in-preview-only"></a>Junho de 2020: novos apenas na visualização

### <a name="calendar"></a>Calendário
Além de monitorar as alterações incrementais de eventos em um **calendarView** (um conjunto ou eventos delimitados por datas de início _e_ fim), use a função [delta](/graph/api/event-delta?view=graph-rest-beta&preserve-view=true) nos eventos de uma caixa de correio do usuário ou eventos em um calendário específico do usuário.

### <a name="cloud-communications--presence"></a>Comunicações na nuvem | Presença
[Obtenha o status de presença](/graph/api/presence-get?view=graph-rest-beta&preserve-view=true) de todos os usuários em uma organização ou de um usuário específico na organização.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- Especificar as [margens de impressão](/graph/api/resources/printmargin?view=graph-rest-beta&preserve-view=true) ao configurar um [documento para impressão](/graph/api/resources/printdocument?view=graph-rest-beta&preserve-view=true).
- Compatível com os seguintes [recursos da impressora](/graph/api/resources/printercapabilities?view=graph-rest-beta&preserve-view=true):
  - instruções de alimentação
  - impressão de intervalos de páginas
  - resolução da impressão em DPIs
  - tamanho máximo da fila de tarefas de impressão em bytes
  - compartimentos de entrada
  - margens
  - ordenação
  - escala do documento
- Compatível com a resolução da impressão (DPI) e com a escala do documento como parte das [configurações padrão da impressora](/graph/api/resources/printerdefaults?view=graph-rest-beta&preserve-view=true).
- Compatível com as seguintes [configurações do documento](/graph/api/resources/printerdocumentconfiguration?view=graph-rest-beta&preserve-view=true):
  - compartimentos de entrada
  - compartimentos de saída
  - tamanhos de papel
  - margens
  - tipos de papel
  - acabamentos como grampeamento ou encadernação
  - páginas por folha
  - layout multipáginas especificando a direção do layout das páginas na folha
  - ordenação
  - escala
- Expandir os documentos ao [listar as tarefas de impressão](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true).
- [Registre uma impressora ]() e use o recurso [printerCreateOperation](/graph/api/resources/printercreateoperation?view=graph-rest-beta&preserve-view=true) para monitorar e verificar o registro da impressora.
- [Obtenha a operação de registro](/graph/api/printoperation-get?view=graph-rest-beta&preserve-view=true) da impressora de longa duração no usuário atual ou no locatário do aplicativo.
- Algumas propriedades e tipos de enumeração renomeados; confira os detalhes nas atualizações do log de alterações da impressão em nuvem do mês de [junho](changelog.md#june-2020).

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações do Intune em [junho](changelog.md#june-2020) — em beta.

### <a name="education"></a>Educação
- Possibilidade de usar permissões delegadas `EduRoster.ReadBasic` para [obter](/graph/api/educationuser-get?view=graph-rest-beta&preserve-view=true) a ID de um(a) [professor(a)](/graph/api/resources/educationteacher?view=graph-rest-beta&preserve-view=true) ou [aluno(a)](/graph/api/resources/educationstudent?view=graph-rest-beta&preserve-view=true) em um programa de uma fonte externa, na forma de uma propriedade **externalId**.
- Use a propriedade **externalSource** para monitorar o valor `lms` se uma [organização](/graph/api/resources/educationorganization?view=graph-rest-beta&preserve-view=true) de ensino ou [aula](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true) forem criados a partir de um sistema de gerenciamento de aprendizagem (LMS).

### <a name="identity-and-access"></a>Identidade e acesso
- Os profissionais de TI podem usar os recursos do [conector](/graph/api/resources/connector?view=graph-rest-beta&preserve-view=true) que sejam agentes leves para se conectar ao [Proxy de Aplicativos do Azure AD](/azure/active-directory/manage-apps/what-is-application-proxy) e [publicar aplicativos web locais externamente](/graph/api/resources/onpremisespublishing?view=graph-rest-beta&preserve-view=true)para que os usuários remotos de suas organizações possam acessá-los de forma segura.
- Gerenciar uma [política de autenticação](/graph/api/resources/authenticationflowspolicy?view=graph-rest-beta&preserve-view=true) no nível de locatário para ativar ou desativar um [serviço autoatendimento de cadastramento](/graph/api/resources/selfservicesignupauthenticationflowconfiguration?view=graph-rest-beta&preserve-view=true) para usuários externos.
- [Provisionar uma conta de usuário sob demanda](/graph/api/synchronization-synchronizationjob-provision-on-demand?view=graph-rest-beta&preserve-view=true) e ser capaz de especificar quais objetos provisionar e quais regras de sincronização executar.

### <a name="search"></a>Busca
- Utilizar os aperfeiçoamentos de uma [propriedade](/graph/api/resources/property?view=graph-rest-beta&preserve-view=true) em um [esquema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true): **isRefinable** para habilitar a filtragem dos resultados de busca e obter um controle mais refinado da experiência de busca, além de **aliases** e **rótulos** para maior relevância.
- Capacidade de especificar até 128 recursos de **propriedades** em um **esquema**.
- Use [get externalItem](/graph/api/externalitem-get?view=graph-rest-beta&preserve-view=true) para fins de diagnóstico.

### <a name="users"></a>Usuários
- Use a propriedade **userPurpose** em [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true) para identificar e diferenciar uma caixa de correio para um único usuário de uma caixa de correio compartilhada e do equipamento de caixa de correio no Exchange Online. 
- Use as [configurações de usuário](/graph/api/resources/usersettings?view=graph-rest-beta&preserve-view=true) para [obter](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta&preserve-view=true) ou [atualizar](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta&preserve-view=true) [idiomas preferenciais e configurações regionais](/graph/api/resources/regionalandlanguagesettings?view=graph-rest-beta&preserve-view=true).
- As configurações do usuário são uma relação acessível por meio do [usuário](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true) que permite uma experiência de usuário consistente entre aplicativos, tocando no perfil de usuário do Azure Active Directory para refletir as mesmas preferências do usuário. Consulte [como as configurações do usuário diferem das configurações de caixa de correio](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true#user-preferences-for-languages-and-regional-formats).


## <a name="may-2020-new-and-generally-available"></a>Maio de 2020: novos e disponíveis para o público em geral

### <a name="calendar--place"></a>Calendário | Local
GA da [API de locais](/graph/api/resources/place) na v1.0: use essa API em aplicativos de produção para obter, atualizar ou excluir uma [sala](/graph/api/resources/room) ou [lista de salas](/graph/api/resources/roomlist) em um locatário. [Saiba mais](outlook-calendar-concept-overview.md#build-apps-with-location-awareness-and-provide-intelligent-context) sobre a API de locais.

### <a name="change-notifications"></a>Notificações de alteração
- Inscreva-se para alterar as notificações no Microsoft Cloud for US Government.

### <a name="cloud-communications--call-records"></a>Comunicações na nuvem | Registros de chamadas
- GA da [API de registros de chamadas](/graph/api/resources/callrecords-api-overview?view=graph-rest-1.0&preserve-view=true): use o recurso [callRecord](/graph/api/resources/callrecord?view=graph-rest-1.0&preserve-view=true) para obter os metadados de chamadas e reuniões online no Microsoft Teams e no Skype.
- Inscreva-se para [alterar notificações](./webhooks.md) de alterações para todos os recursos de **callRecord** em uma organização.
- [Liste as sessões](/graph/api/callrecords-session-list?view=graph-rest-1.0&preserve-view=true) em um **callRecord** e, opcionalmente, [expanda cada sessão para listar os segmentos](/graph/api/callrecords-session-list?view=graph-rest-1.0&preserve-view=true#example-2-get-session-list-with-segments) no registro de chamadas.
- Suporte para 60 GHz (`frequency60GHz`) e valores de banda de WiFi de `unknownFutureValue` para um ponto de extremidade de mídia em um segmento.
- Suporte à caixa postal como um possível tipo de ponto de extremidade do lado do serviço em um [segmento](/graph/api/resources/callrecords-segment) de comunicação.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações de [maio](changelog.md#may-2020) do Intune v1.0.

### <a name="graph-explorer"></a>Explorador do Graph
Use os vários novos recursos do [Explorador do Graph](https://developer.microsoft.com/en-us/graph/graph-explorer) que aprimoram o aprendizado e a prototipagem na área restrita. Por exemplo:
- Exiba trechos de código que correspondam à consulta da API REST inserida em C#, Java, JavaScript e Objective C.
- Conecte-se com um locatário, exiba e copie um token de acesso para seu aplicativo cliente REST favorito.

Para mais detalhes, confira [O novo Explorador do Graph já está disponível](https://developer.microsoft.com/graph/blogs/new-graph-explorer-is-now-ga/).

### <a name="groups"></a>Grupos
- Agora, a sincronização do diretório local com o Azure Active Directory via Azure AD Connect retorna as propriedades **onPremisesDomainName**, **onPremisesNetBiosName** e **onPremisesSamAccountName** como parte do recurso de [grupo](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true).
- Inscreva-se para alterar as notificações de recursos de [grupo](/graph/api/resources/group) no Microsoft Cloud China operado pela 21Vianet.

### <a name="identity-and-access"></a>Identidade e acesso
- GA da API de entidades de serviço na v1.0: use o recurso [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0&preserve-view=true) em aplicativos de produção para gerenciar programaticamente instâncias de aplicativos e controlar o que um aplicativo pode fazer em seu locatário. Você pode controlar quem pode usar um aplicativo, quais recursos o aplicativo tem acesso, como a adição de credenciais de senha, a expiração de certificados, e o gerenciamento de permissões delegadas e atribuições de funções de aplicativos.
- GA da API [appRoleAssignment](/graph/api/resources/appRoleAssignment?view=graph-rest-1.0&preserve-view=true) que registra a atribuição de um [appRole](/graph/api/resources/approle?view=graph-rest-1.0&preserve-view=true) (representando a declaração de `roles` em tokens de ID e tokens de acesso) a um [usuário](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true), [grupo](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true) ou [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0&preserve-view=true).
- Use o Facebook como provedor de identidade no Azure Active Directory.
- Use a permissão delegada ou de aplicativo do`AppRoleAssignment.ReadWrite.All` para permitir que um aplicativo gerencie concessões de permissões de aplicativo para qualquer API (incluindo o Microsoft Graph) e atribuições de aplicativo para qualquer aplicativo, respectivamente com ou sem o usuário conectado.


### <a name="microsoft-graph-sdks"></a>SDKs do Microsoft Graph
Confira as novas diretrizes de SDK em:
- [Paginação](./sdks/paging.md)
- [Envio em lote](./sdks/batch-requests.md)
- [Carregando arquivos grandes no OneDrive](./sdks/large-file-upload.md)
- [Personalizando o cliente do serviço SDK por meio dos componentes middleware HTTP](./sdks/customize-client.md).

### <a name="teamwork"></a>Trabalho em equipe
- Se o seu cenário envolver reuniões online no Teams, confira as novas diretrizes sobre [como escolher](choose-online-meeting-api.md) entre a [API de calendário](outlook-calendar-online-meetings.md) e a [API de comunicações na nuvem](cloud-communications-online-meetings.md) para criar e ingressar em reuniões online.
- [Enviar](/graph/api/channel-post-messages?view=graph-rest-1.0&preserve-view=true) e [responder](/graph/api/channel-post-messagereply?view=graph-rest-1.0&preserve-view=true) mensagens em um [canal](/graph/api/resources/channel?view=graph-rest-1.0&preserve-view=true).
- Obtenha a localização dos arquivos do OneDrive for Business de um [canal](/graph/api/resources/channel?view=graph-rest-1.0&preserve-view=true), usando a propriedade de navegação **fileFolder**.

### <a name="teamwork--shifts"></a>Trabalho em equipe | Turnos
GA da [API de turnos](/graph/api/resources/shift?view=graph-rest-1.0&preserve-view=true) na v1.0: use esta API em aplicativos de produção para criar, atualizar e gerenciar cronogramas de funcionários da linha de frente, permitindo que eles estejam em contato e colaborem efetivamente.

### <a name="users"></a>Usuários
- Inscreva-se para alterar notificações de recursos de [usuário](/graph/api/resources/user) no Microsoft Cloud China operado pela 21Vianet.
- Acompanhe o status e a data/hora da última alteração de status de um usuário externo, que foi [convidado](/graph/api/invitation-post?view=graph-rest-1.0&preserve-view=true) a ingressar na organização, usando as propriedades **externalUserState** e **externalUserStateChangeDateTime** do recurso de **usuário**.

## <a name="may-2020-new-in-preview-only"></a>Maio de 2020: novo somente para visualização

### <a name="change-notifications"></a>Notificações de alteração
- Use os tipos esquematizados formalmente [changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta&preserve-view=true) e [changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta&preserve-view=true) para processar notificações de alteração de recursos. 
- Acompanhe se as notificações estão em sequência ou se uma notificação está ausente, usando a propriedade **sequenceNumber** no recurso **changeNotification**.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- Os recursos da [impressora](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true) e do [printerShare](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) agora estão em paridade e têm as mesmas propriedades.
- Algumas limpezas de nomes de tipos e de propriedades sobre compartilhamentos da impressora:
  - Use a propriedade de navegação **compartilhada** de [impressão](/graph/api/resources/print?view=graph-rest-beta&preserve-view=true) para obter a lista de compartilhamentos de impressora registrados no locatário. 
  - Veja os detalhes no changelog de [maio](changelog.md#may-2020).

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações de [maio](changelog.md#may-2020) do Intune beta.

### <a name="groups"></a>Grupos
- [Avaliar](/graph/api/group-evaluatedynamicmembership?view=graph-rest-beta&preserve-view=true) se um usuário ou dispositivo é ou seria membro de um grupo dinâmico, usando a regra existente para o [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) ou uma regra especificada. [A associação dinâmica baseada em regra](/azure/active-directory/users-groups-roles/groups-dynamic-membership) reduz a sobrecarga administrativa de adicionar e remover membros.
- Ao criar um [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) do Microsoft 365, configure os comportamentos do grupo especificando-os na propriedade **resourceBehaviorOptions**. Por exemplo, permita que os membros postem, inscrevam novos membros na conversa, desabilitem o email de boas-vindas e ocultem o grupo nas experiências do Outlook.
- Especifique os recursos a serem fornecidos na propriedade **resourceProvisioningOptions** que normalmente não fazem parte da criação do [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) padrão. Atualmente há suporte para provisionamento de um grupo como uma [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) com os recursos do Microsoft Teams.

### <a name="identity-and-access"></a>Identidade e acesso
- Aplica opções de consulta do sistema OData (`$count`, `$filter`, `$search`) ao obter coleções de entidades derivadas do [directoryObject](/graph/api/resources/directoryObject). Você pode [pesquisar tokens específicos](/graph/search-query-parameter#using-search-on-directory-object-collections) nas propriedades **displayName** e **description** dessas entidades, e usar a conversão OData para aparar os resultados do **directoryObject** para determinados tipos derivados. Veja mais detalhes em [Criar consultas avançadas no Microsoft Graph com $count, $filter, $search e $orderby](https://developer.microsoft.com/en-us/graph/blogs/build-advanced-queries-with-count-filter-search-and-orderby/).
- Como parte da [API de proteção de identidade](/graph/api/resources/identityprotection-root?view=graph-rest-beta&preserve-view=true), use a propriedade **riskEventType** para [obter o tipo de risco detectado](/graph/api/riskdetection-get?view=graph-rest-beta&preserve-view=true) ou [obter o tipo de risco no histórico de um usuário](/graph/api/riskyuser-list-history?view=graph-rest-beta&preserve-view=true). Não use a propriedade **riskType** porque ela já foi preterida.
- Especifique os tipos de aplicativo cliente na propriedade **clientAppTypes** do [conjunto de condições](/graph/api/resources/conditionalaccessconditionset?view=graph-rest-beta&preserve-view=true) de uma [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- Use a permissão delegada de `EntitlementManagement.Read.All` para permitir ao aplicativo solicitar acesso para ler pacotes de acesso e recursos de gerenciamento de direitos relacionados em nome do usuário conectado.
- Use as permissões delegadas ou de aplicativo do `Application.Read.All` e do `Application.ReadWrite.All` para [listar aplicativos](/graph/api/application-list?view=graph-rest-beta&preserve-view=true) em uma organização.
- Controle as configurações de autorização no Azure AD usando o tipo de recurso [authorizationPolicy](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true).

### <a name="teamwork"></a>Trabalho em equipe
- Os aplicativos do Teams que oferecem [suporte a SSO (logon único)](/microsoftteams/platform/tabs/how-to/authentication/auth-aad-sso) podem especificar o `WebApplicationInfo.id` a partir do manifesto do aplicativo Teams, na propriedade **azureADAppId** do [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta&preserve-view=true).
- Use as [permissões mais refinadas](./permissions-reference.md#team-resource-specific-consent-permissions) para acessar os recursos da [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) e do [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true).


## <a name="april-2020-new-and-generally-available"></a>Abril de 2020: novo e geralmente disponível.

### <a name="calendar"></a>Calendário
- [Compartilhar ou delegar calendários](outlook-share-or-delegate-calendar.md) de forma programática, com uma maior paridade com a experiência do usuário do Outlook. Além de controlar as permissões do usuário atual e o status de compartilhamento de um calendário:
  - Para cada [calendário](/graph/api/resources/calendar?view=graph-rest-1.0&preserve-view=true), você pode gerenciar as [permissões](/graph/api/resources/calendarpermission?view=graph-rest-1.0&preserve-view=true) de cada usuário com o qual o calendário é compartilhado. 
  - Para cada [caixa de correio](/graph/api/resources/mailboxsettings?view=graph-rest-1.0&preserve-view=true), você pode especificar se um representante, proprietário de caixa de correio ou ambos receberão mensagens da reunião e respostas da reunião. 
- [Criar ou atualizar um evento como uma reunião online](outlook-calendar-online-meetings.md):
  - Para cada **calendário**, especifique os provedores de reuniões online permitidos e padrão.
  - Crie ou atualize um [evento](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true) que esteja disponível online e forneça detalhes para que os participantes possam ingressar na reunião online. 
  - Em particular, use as novas propriedades **onlineMeetingProvider** e **onlineMeeting** do **evento** para definir ou identificar o Microsoft Teams como um provedor de reuniões online, uma solução alternativa para um [problema conhecido](known-issues.md#onlinemeetingurl-property-is-not-supported-for-microsoft-teams) com a propriedade **onlineMeetingUrl**.
- Adicione [anexos de arquivo de até 150 MB](outlook-large-attachments.md) a um [evento](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true).

### <a name="files"></a>Arquivos
- [Check-out](/graph/api/driveitem-checkout?view=graph-rest-1.0&preserve-view=true) ou [check-in](/graph/api/driveitem-checkin?view=graph-rest-1.0&preserve-view=true) de um arquivo para o OneDrive para gerenciar a atualização do arquivo e disponibilizar atualizações para outras pessoas quando as atualizações estiverem prontas.
- Aplique senha opcional e data/hora de vencimento como parâmetros do [convite](/graph/api/driveitem-invite?view=graph-rest-1.0&preserve-view=true) e das ações de [criar link de compartilhamento](/graph/api/driveitem-createlink?view=graph-rest-1.0&preserve-view=true) para compartilhar um [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true).
- Obtenha ou defina a senha e a data/hora de vencimento de uma [permissão](/graph/api/resources/permission?view=graph-rest-1.0&preserve-view=true) e rastreie o [identitySet](/graph/api/resources/identityset?view=graph-rest-1.0&preserve-view=true) de usuários que receberam permissão para compartilhar um **driveItem**.
- Obtenha a [permissão](/graph/api/resources/permission?view=graph-rest-1.0&preserve-view=true) de um [item de drive compartilhado](/graph/api/resources/shareddriveitem?view=graph-rest-1.0&preserve-view=true) usando a propriedade de navegação de **permissão**.
- Limite os usuários com um [link de compartilhamento](/graph/api/resources/sharinglink?view=graph-rest-1.0&preserve-view=true) para somente visualização e não poder baixar o conteúdo de um **driveItem** compartilhado no OneDrive for Business ou no SharePoint.

### <a name="identity-and-access"></a>Identidade e acesso
- Para gerenciar funções e atribuir acesso a recursos nos provedores de controle de acesso baseado em função (RBAC), como o Microsoft Intune, use [unifiedRoleAssignmentMultiple](/graph/api/resources/unifiedroleassignmentmultiple?view=graph-rest-1.0&preserve-view=true). O recurso **unifiedRoleAssignmentMultiple** permite definir uma única função em uma matriz de escopos e atribuir a função a várias entidades (como usuários).
- Acessar tipos específicos de [políticas de uma organização](/graph/api/resources/policy-overview?view=graph-rest-1.0&preserve-view=true) usando o `/policies`segmento URL e especificando o tipo de política. Por exemplo, uma organização pode forçar uma política a entrar automaticamente no usuário de uma sessão da Web após um período de inatividade, confira as operações CRUD para instâncias de [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-1.0&preserve-view=true). Essa é um [alteração significativa](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-1.0/) para que seja mais fácil descobrir todas as políticas, agrupando todas as políticas digitadas sob o `/policies`segmento. Acesse outras políticas digitadas de uma abordagem semelhante: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-1.0&preserve-view=true), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-1.0&preserve-view=true), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-1.0&preserve-view=true)e [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-1.0&preserve-view=true). 

### <a name="mail"></a>Correio
Adicione [anexos de arquivo de até 150 MB](outlook-large-attachments.md) a uma [mensagem](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true).

### <a name="sites-and-lists"></a>Sites e listas
- [Faça uma lista de sites](/graph/api/sites-list-followed?view=graph-rest-1.0&preserve-view=true) que o usuário conectado seguiu.
- Identifique a região geográfica de um [conjunto de sites](/graph/api/resources/sitecollection?view=graph-rest-1.0&preserve-view=true) usando a propriedade **dataLocationCode**.
- Identifique o locatário de um arquivo, pasta ou outro item no SharePoint, acessando a propriedade **tenantId** que faça parte do **sharepointIds** de um [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true).

## <a name="april-2020-new-in-preview-only"></a>Abril de 2020: novo somente para visualização

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem

Designar usuários e grupos permitidos para usar compartilhamentos de impressoras [específicos](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) em impressão universal, a infraestrutura de impressão baseada na nuvem do Microsoft 365. Para experimentar recursos de gerenciamento de impressão eficientes e centralizados, assim como oferecer uma experiência de impressão simples, porém rica e segura para os usuários de impressão, consulte o [Anúncio de impressão universal](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/announcing-universal-print-a-cloud-based-print-solution/ba-p/1204775) e participe do programa de visualização.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações de [abril](changelog.md#april-2020) do Intune.

### <a name="groups"></a>Grupos
Identifique o aplicativo que criou um [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) pela sua ID do aplicativo.

### <a name="identity-and-access"></a>Identidade e acesso
- [Controlar alterações](/graph/api/administrativeunit-delta?view=graph-rest-beta&preserve-view=true) para [unidades administrativas](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true).
- [Controlar alterações](/graph/api/oauth2permissiongrant-delta?view=graph-rest-beta&preserve-view=true) para [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant?view=graph-rest-beta&preserve-view=true).
- [Gerenciar](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true) [métodos de autenticação](/graph/api/resources/authenticationmethod?view=graph-rest-beta&preserve-view=true) de um usuário que incluem [senha](/graph/api/resources/passwordauthenticationmethod?view=graph-rest-beta&preserve-view=true) ou [telefone](/graph/api/resources/phoneauthenticationmethod?view=graph-rest-beta&preserve-view=true). Por exemplo, [redefinir uma senha de usuário](/graph/api/passwordauthenticationmethod-resetpassword?view=graph-rest-beta&preserve-view=true) e [obter o status de redefinição](/graph/api/authenticationoperation-get?view=graph-rest-beta&preserve-view=true)ou [adicionar um número de telefone](/graph/api/authentication-post-phonemethods?view=graph-rest-beta&preserve-view=true) para um usuário para autenticação de SMS ou chamada de voz, se a política estiver habilitada para o usuário.

### <a name="reports--identity-and-access-reports"></a>Relatórios | Relatórios de identidade e acesso
[Listar](/graph/api/relyingpartydetailedsummary-list?view=graph-rest-beta&preserve-view=true) [participantes confiáveis](/windows-server/identity/ad-fs/technical-reference/understanding-key-ad-fs-concepts) configurados nos Serviços de Federação do Active Directory.

### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
Exibir dados de **Reunião Criada** e de **Reunião Interagida** nos relatórios CSV para [contagens de atividades de email](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta&preserve-view=true), [contagens de atividades de email do usuário](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta&preserve-view=true) e [detalhes de atividades de email do usuário](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta&preserve-view=true).


## <a name="march-2020-new-and-generally-available"></a>Março de 2020: Novo e disponível para o público geral

### <a name="cloud-communications"></a>Comunicações na nuvem
- Obtenha o roteamento de chamadas e o contexto de entrada de um [chamada](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true).
- Um aplicativo pode [Atualizar o status da gravação](/graph/api/call-updaterecordingstatus?view=graph-rest-1.0&preserve-view=true) de uma chamada.
- Gravar as informações especificamente para um [participante](/graph/api/resources/participant?view=graph-rest-1.0&preserve-view=true), incluindo o iniciador e o status da gravação.
- Identifique de forma exclusiva os participantes de uma conferência ou [chamada](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true) de participante a participante usando a propriedade **callChainId**.
- Identifique como parte do [participantInfo](/graph/api/resources/participantinfo?view=graph-rest-1.0&preserve-view=true) o código do país e o tipo de ponto de extremidade (como o Skype for Business ou o Skype for Business VOIP) do participante.
- Parceiros de dispositivos VTC (videoconferência de terceiros) podem registrar e fornecer dados de qualidade de mídia para seus dispositivos de teleconferência de vídeo por meio de um bot CVI (Interoperabilidade de Vídeo na Nuvem) e usando a função [logTeleconferenceDeviceQuality](/graph/api/call-logteleconferencedevicequality?view=graph-rest-1.0&preserve-view=true). A qualidade da mídia inclui dados de tipo aberto para [áudio](/graph/api/resources/teleconferencedeviceaudioquality?view=graph-rest-1.0&preserve-view=true), [vídeo](/graph/api/resources/teleconferencedevicevideoquality?view=graph-rest-1.0&preserve-view=true)e [compartilhamento de tela](/graph/api/resources/teleconferencedevicescreensharingquality?view=graph-rest-1.0&preserve-view=true).

### <a name="files"></a>Arquivos
- [Os itens remotos](/graph/api/resources/remoteitem?view=graph-rest-1.0&preserve-view=true) compartilhados com um usuário, adicionados ao OneDrive do usuário, ou retornados como resultado de pesquisa podem conter metadados para uma imagem ou um vídeo.
- [Siga](/graph/api/driveitem-follow?view=graph-rest-1.0&preserve-view=true) um [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true) para obter um acesso conveniente ou para facilitar ações como mover, copiar e salvar como. Use [deixar de serguir](/graph/api/driveitem-unfollow?view=graph-rest-1.0&preserve-view=true) para deixar de seguir o item da unidade.
- [Conceda](/graph/api/permission-grant?view=graph-rest-1.0&preserve-view=true) permissões aos usuários para acessarem um link de compartilhamento para compartilhar o item da unidade correspondente.

### <a name="identity-and-access"></a>Identidade e acesso
- [Controle de alterações](/graph/api/orgcontact-delta?view=graph-rest-1.0&preserve-view=true) para [contatos organizacionais](/graph/api/resources/orgcontact?view=graph-rest-1.0&preserve-view=true).
- Use a propriedade **riskEventTypes_v2** para obter os tipos de eventos de risco associados a [entrada](/graph/api/resources/signin?view=graph-rest-1.0&preserve-view=true).
- Use a permissão delegada `User.ManageIdentities.All` para permitir que um aplicativo leia, atualize ou exclua identidades associadas à conta de um usuário, às quais o usuário conectado tem acesso. Use essa permissão no nível do aplicativo sem um usuário conectado. Isso permite ao aplicativo [gerenciar](/graph/api/user-update?view=graph-rest-1.0&preserve-view=true) com quais identidades um usuário pode se inscrever.

### <a name="reports"></a>Relatórios
O administrador de serviços do Teams e o administrador de comunicações do Teams devem ser usados como funções de usuário aceitas para permitir que os aplicativos leiam os relatórios de uso do serviço do Microsoft 365 em nome de um usuário, como [formas de autorização delegada pelo usuário](reportroot-authorization.md). 

### <a name="sites"></a>Sites
- Permitir que os usuários [sigam](/graph/api/site-follow?view=graph-rest-1.0&preserve-view=true) ou [parem de seguir](/graph/api/site-unfollow?view=graph-rest-1.0&preserve-view=true) os sites do SharePoint.
- [Inscreva-se para alterar as notificações](/graph/api/resources/subscription?view=graph-rest-1.0&preserve-view=true) para uma lista  [do SharePoint](/graph/api/resources/list?view=graph-rest-1.0&preserve-view=true).

## <a name="march-2020-new-in-preview-only"></a>Março de 2020: novo somente para visualização

### <a name="calendar"></a>Calendário
- Use a propriedade **calendarGroupId** para obter o [grupo de calendário](/graph/api/resources/calendargroup?view=graph-rest-beta&preserve-view=true) em que um [calendário](/graph/api/resources/calendar?view=graph-rest-beta&preserve-view=true) foi criado.
- Use a propriedade **isDraft** para identificar um [evento](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) como uma reunião que o usuário atualizou no Outlook, mas não enviou para atualizar os participantes.

### <a name="cloud-communications"></a>Comunicações na nuvem
- Use [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-beta&preserve-view=true) para obter uma instância de [reunião online](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) por um ID externo personalizado e criar uma quando não houver nenhuma.
- Você tem a opção de usar a propriedade **externalId** para identificar uma reunião online com a ID externa personalizada.
- Use o `Accept-Language` cabeçalho opcional da solicitação HTTP para [criar](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true) ou [obter](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) uma instância da reunião online, para que a operação bem-sucedida exiba o conteúdo da propriedade **joinInformation** no idioma especificado e variante de localidade.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [março](changelog.md#march-2020) do Intune

### <a name="identity-and-access"></a>Identidade e acesso
- Use a permissão `AuditLog.Read.All` para listar a [atividade de entrada](/graph/api/resources/signinactivity?view=graph-rest-beta&preserve-view=true) de um [usuário](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true).
- Use a `PrivilegedAccess.Read.AzureResources` permissão no nível do aplicativo para [PIM (gerenciamento de identidades privilegiadas) dos recursos do Azure](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta&preserve-view=true), para configurar o fluxo de trabalho de acesso just-in-time para funções de infraestrutura do Azure em um grupo de gerenciamento, assinatura, grupo de recursos ou nível de recurso.
- Use a entidade [identitySecurityDefaultsEnforcementPolicy](/graph/api/resources/identitysecuritydefaultsenforcementpolicy?view=graph-rest-beta&preserve-view=true) para [obter](/graph/api/identitysecuritydefaultsenforcementpolicy-get?view=graph-rest-beta&preserve-view=true) ou [atualizar](/graph/api/identitysecuritydefaultsenforcementpolicy-update?view=graph-rest-beta&preserve-view=true) as configurações de segurança padrão pré-definidas que protegem as organizações contra ataques comuns.
- Use um segmento `identity` ao chamar APIs de acesso condicional. Por exemplo, para [obter](/graph/api/conditionalaccesspolicy-get?view=graph-rest-beta&preserve-view=true) ou uma [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true): `GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}`.
- Use a propriedade **authenticationRequirement** para obter o nível mais alto de autenticação necessária por meio de todas as etapas de entrada para que a [entrada](/graph/api/resources/signin?view=graph-rest-beta&preserve-view=true) seja bem-sucedida.
- Use a paginação quando [listar eventos de provisionamento](/graph/api/provisioningobjectsummary-list?view=graph-rest-beta&preserve-view=true) ocorridos no locatário.

### <a name="search"></a>Pesquisa
- Para adicionar dados em um arquivo para pesquisar resultados, indexe os dados como um [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true). O tipo **externalFile** foi preterido.
- Agora é possível [atualizar](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true) um [item no índice](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true), atualizando especificamente a representação de texto simples do item (representado pela propriedade **conteúdo**), ou o conjunto de propriedades do item (representado pela propriedade **propriedades**). A atualização de qualquer propriedade no conjunto de propriedades substitui todo conjunto de propriedades, por isso certifique-se de incluir explicitamente todas as propriedades do item na atualização.
- Verifique o `HTTP 429` e o cabeçalho de resposta `Retry-After` depois de chamar a operação para [criar](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true), [atualizar](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true) ou [excluir](/graph/api/externalitem-delete?view=graph-rest-beta&preserve-view=true) de **externalItem**. Desativar solicitações usando o atraso `Retry-After` é a forma mais rápida de se recuperar da [limitação](throttling.md#best-practices-to-handle-throttling).

### <a name="teamwork"></a>Trabalho em equipe
Use a `ChannelMessage.Read.All` permissão no nível do aplicativo para ler [instâncias de](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true)chatMessage em canais sem um usuário conectado.

### <a name="universal-print"></a>Impressão universal
Estréia da [API de impressão universal](universal-print-concept-overview.md), que permite que os usuários imprimam na Web ou de um aplicativo. A API permite que os administradores de TI gerenciem o acesso de usuários e grupos a impressoras na nuvem do Microsoft 365, compartilhamento remoto da impressora para manter a disponibilidade, monitorar o status da impressora e emitir relatórios sobre trabalho de impressão arquivado e uso. 

Observe que a partir de março de 2020, o serviço de _impressão universal_ está na visualização particular. Confira [anunciando a impressão universal: uma solução de impressão baseada na nuvem](https://aka.ms/announcinguniversalprint) para obter informações sobre a participação.


## <a name="february-2020-new-and-generally-available"></a>Fevereiro de 2020: novo e disponível para o público geral

### <a name="calendar"></a>Calendário
Vamos examinar um exemplo de [criação de um evento em um calendário compartilhado ou delegado](outlook-create-event-in-shared-delegated-calendar.md), além das ações e propriedades disponíveis para o representante, os convidados e o proprietário do calendário durante esse processo.

### <a name="identity-and-access"></a>Identidade e acesso
- Para aumentar a segurança ao assinar as [notificações de alteração dos dados do usuário](webhooks.md), [impor o Protocolo TLS 1.2](/configmgr/core/plan-design/security/enable-tls-1-2) ou mais recente em clientes e servidores de sites usados no processo de notificação. O novo requisito será lançado em estágios a partir de 15 de fevereiro de 2020. A partir de 15 de maio de 2020, todos os pontos de extremidade de notificação devem atendem ao novo requisito de TLS. [Descubra os estágios do lançamento](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) e, se necessário, use a nova propriedade **latestSupportedTlsVersion** como uma solução alternativa temporária para evitar falhas de assinatura antes de concluir a atualização de TLS.
- Use os respectivos tipos de [solicitação de avaliação de ameaças](/graph/api/resources/threatAssessmentRequest?view=graph-rest-1.0&preserve-view=true) para controlar as ameaças de [email](/graph/api/resources/mailassessmentrequest?view=graph-rest-1.0&preserve-view=true), um [arquivo de mensagem de email](/graph/api/resources/emailfileassessmentrequest?view=graph-rest-1.0&preserve-view=true) (arquivo .EML), [arquivo de anexo de email](/graph/api/resources/fileassessmentrequest?view=graph-rest-1.0&preserve-view=true) (texto, Word ou arquivo binário) ou [URL](/graph/api/resources/urlassessmentrequest?view=graph-rest-1.0&preserve-view=true).

### <a name="users"></a>Usuários
[Reprocessar](/graph/api/user-reprocesslicenseassignment?view=graph-rest-1.0&preserve-view=true) todas as atribuições de licença baseadas em grupo para um [usuário](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true).


## <a name="february-2020-new-in-preview-only"></a>Fevereiro de 2020: nova somente para visualização

### <a name="calendar"></a>Calendário
Confira [tarefas com suporte por APIs de visualização que gerenciam o compartilhamento de calendários e a delegação](outlook-share-or-delegate-calendar.md).

### <a name="cloud-communications"></a>Comunicações na nuvem

- Use o novo recurso [registros de chamadas](/graph/api/resources/callrecord?view=graph-rest-beta&preserve-view=true) para obter metadados de chamadas e reuniões online do Microsoft Teams e do Skype for Business para uma organização.
- Para um participante de uma reunião, use a propriedade **Iniciador** para obter as informações de identidade do iniciador de uma [gravação](/graph/api/resources/recordinginfo?view=graph-rest-beta&preserve-view=true), se houver uma.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [fevereiro](changelog.md#february-2020) do Intune.

### <a name="groups"></a>Grupos
Use o método [assignLicense](/graph/api/group-assignlicense?view=graph-rest-beta&preserve-view=true) para atribuir licenças de produtos, como o Microsoft 365 ou o Enterprise Mobility + Security, a um grupo. Como o Azure AD garante que as licenças sejam designadas para os membros do grupo, os membros que ingressarem ou saírem de um grupo não precisarão mais de gerenciamento de licenças no nível individual.

### <a name="identity-and-access"></a>Identidade e acesso
- Defina as configurações de solicitação, aprovação e revisar ao criar uma [política de atribuição de pacote](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true).
- Acessar tipos específicos de [políticas de uma organização](/graph/api/resources/policy-overview?view=graph-rest-beta&preserve-view=true) usando o `/policies`segmento URL e especificando o tipo de política. Por exemplo, uma organização pode forçar uma política a entrar automaticamente no usuário de uma sessão da Web após um período de inatividade, confira as operações CRUD para instâncias de [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-beta&preserve-view=true). Essa é um [alteração significativa](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/) para que seja mais fácil descobrir todas as políticas, agrupando todas as políticas digitadas sob o `/policies`segmento. Acesse outras políticas digitadas de uma abordagem semelhante: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta&preserve-view=true), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-beta&preserve-view=true), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta&preserve-view=true)e [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-beta&preserve-view=true). 
- Use a permissão de nível de aplicativo e `Policy.ReadWrite.ApplicationConfiguration` delegada para operações de leitura e gravação na configuração do aplicativo [políticas](/graph/api/resources/policy-overview?view=graph-rest-beta&preserve-view=true) mencionadas no item anterior.

### <a name="teamwork"></a>Trabalho em equipe
- Use [alterar as notificações](/graph/api/resources/webhooks?view=graph-rest-beta&preserve-view=true) em todas as mensagens do canal ou em todas as mensagens de chat em uma organização.
- [Recuse](/graph/api/swapshiftschangerequest-decline?view=graph-rest-beta&preserve-view=true) uma [solicitação de troca de turnos](/graph/api/resources/swapshiftschangerequest?view=graph-rest-beta&preserve-view=true) com outro usuário em uma [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true).

## <a name="january-2020-new-and-generally-available"></a>Janeiro de 2020: Novo e disponível para o público geral

### <a name="security"></a>Segurança
Como parte do gerenciamento de alerta de cliente, use o método de [alerta de atualização](/graph/api/alert-update?view=graph-rest-1.0&preserve-view=true) e atualize o campo **comentários** como `Closed in IPC` ou `Closed in MCAS`.

### <a name="teamwork"></a>Trabalho em equipe
Use a propriedade de navegação **primaryChannel** de uma [equipe](/graph/api/resources/team?view=graph-rest-1.0&preserve-view=true) para acessar o canal padrão, **Geral**.

### <a name="users"></a>Usuários
Use a propriedade **identities** para acessar uma ou mais identidades que um [usuário](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true) pode usar para entrar em uma conta de usuário do Azure AD. As identidades podem ser fornecidas pela Microsoft, por organizações ou por provedores de identidade social, como Facebook, Google ou Microsoft. Essa propriedade permite que o usuário entre na conta de usuário com uma dessas identidades.

## <a name="january-2020-new-in-preview"></a>Janeiro de 2020: novidades na versão prévia

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [janeiro](changelog.md#january-2020) do Intune.


## <a name="december-2019-new-and-generally-available"></a>Dezembro de 2019: Novo e disponível para o público geral

### <a name="cloud-communications"></a>Comunicações na nuvem
A API de comunicações na nuvem tem o GA'd e as APIs para [chamada](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true) e [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-1.0&preserve-view=true) estão [disponíveis na v1.0](/graph/api/resources/communications-api-overview?view=graph-rest-1.0&preserve-view=true).

### <a name="education"></a>Educação
Use a propriedade **classSettings** para gerenciar configurações específicas de classe, como habilitar o envio de resumos de atribuições semanais. Esta propriedade está disponível no recurso [equipe](/graph/api/resources/team?view=graph-rest-1.0&preserve-view=true) quando a equipe representa uma [classe educacional](/graph/api/resources/educationclass?view=graph-rest-1.0&preserve-view=true).

### <a name="identity-and-access"></a>Identidade e acesso 
[Tentar obter objetos de contêiner com permissões limitadas retorna dados parciais](permissions-reference.md#limited-information-returned-for-inaccessible-member-objects). Um exemplo é uma instância de [grupo](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true) associada a um [usuário](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true), outro **grupo** e um [dispositivo](/graph/api/resources/device?view=graph-rest-1.0&preserve-view=true). Um aplicativo que tem somente as permissões User.Read.All e Group.Read.All e tentar acessar essa instância de **grupo** obteria os objetos de **usuário** e **grupo**, mas dados limitados para o objeto de **dispositivo** (apenas o tipo de dados e a ID do objeto e não os valores da propriedade).

### <a name="people-and-workplace-intelligence"></a>Inteligência de pessoas e local de trabalho
A API de insights foi GA. Use a API em aplicativos de produção para identificar os documentos mais relevantes que são:

- [Tendências de](/graph/api/insights-list-trending?view=graph-rest-1.0&preserve-view=true) um usuário
- [Usado por](/graph/api/insights-list-used?view=graph-rest-1.0&preserve-view=true) um usuário
- [Compartilhados com ou por](/graph/api/insights-list-shared?view=graph-rest-1.0&preserve-view=true) um usuário

### <a name="reports"></a>Relatórios
Para obter relatórios de uso do Microsoft 365 usando permissões delegadas por um usuário, os administradores devem ter atribuído ao usuário uma função de administrador limitado do Azure AD. Podendo ser uma das seguintes funções: administrador da empresa, administrador do Exchange, administrador do SharePoint, administrador do Lync, leitor global ou leitor de relatórios. Para mais detalhes, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](reportroot-authorization.md).

### <a name="toolkit"></a>Kit de ferramentas
O Kit de ferramentas do Microsoft Graph v1.1 foi lançado. Para obter uma lista de aprimoramentos e correções de bugs, consulte a [seção de dezembro de 2019](changelog.md#december-2019) do log de mudanças.

## <a name="december-2019-new-in-preview"></a>Dezembro de 2019: novidades na versão prévia

### <a name="cloud-communications"></a>Comunicações na nuvem
- Use o novo recurso [presença](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true) para obter informações sobre a disponibilidade e a atividade atual de um ou mais usuários.
- [Exclua](/graph/api/onlinemeeting-delete?view=graph-rest-beta&preserve-view=true) uma instância de um [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true).
- Confira a [seção de dezembro de 2019](changelog.md#december-2019) do log de alterações para a renomeação e a remoção de alguns membros dos recursos da [chamada](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true) e do [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true), para estar na paridade com a versão v1 desses recursos.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [Dezembro](changelog.md#december-2019) do Intune

### <a name="identity-and-access"></a>Identidade e acesso 
- Correção de comportamento nos relacionamentos **appRoleAssignments** e **appRoleAssignedTo** em [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true).
- Use [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta&preserve-view=true) em [gerenciamento de direitos do Azure AD](/graph/api/resources/entitlementmanagement-overview?view=graph-rest-beta&preserve-view=true) para solicitar a adição de um recurso a um [catálogo](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true), para que as funções desse recurso possam ser usadas em um [pacote de acesso](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true).
- Use a [API de avaliação de ameaças](/graph/api/resources/threatassessment-api-overview?view=graph-rest-beta&preserve-view=true) para capacitar os administradores a relatar emails suspeitos, URLs de phishing, anexos de email ou outros arquivos. O veredicto de varredura de thread pode então informá-los a ajustar a política organizacional adequadamente.

### <a name="teamwork"></a>Trabalho em equipe
- [Configure as notificações que incluem dados de recursos](webhooks-with-resource-data.md) para recursos do [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) nos canais e bate-papos do Microsoft Teams.
- [Assine as notificações](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true) de [mensagens de canal ou de bate-papo](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) novas ou modificadas.
- Use o recurso [shiftPreferences](/graph/api/resources/shiftpreferences?view=graph-rest-beta&preserve-view=true) para permitir que a especificação da disponibilidade de um usuário seja atribuída a turnos em um [cronograma](/graph/api/resources/schedule?view=graph-rest-beta&preserve-view=true). Obtenha ou defina isso como parte das [configurações](/graph/api/resources/usersettings?view=graph-rest-beta&preserve-view=true) do usuário.


## <a name="november-2019-new-and-generally-available"></a>Novembro de 2019: novo e disponível para o público geral

### <a name="groups"></a>Grupos
- Use permissões delegadas ou de aplicativo, GroupMember.Read.All e GroupMember.ReadWrite.All, para listar grupos, leia as propriedades básicas do grupo, leia (e atualize a permissão de leitura/gravação) a associação dos grupos aos quais o aplicativo tem acesso.
- Use a permissão do aplicativo, Group.Create, para criar grupos sem um usuário conectado.
- Para um [grupo](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true) especificado, [verifique a associação](/graph/api/group-checkmemberobjects?view=graph-rest-1.0&preserve-view=true) em outros grupos ou funções de diretório.

### <a name="identity-and-access"></a>Identidade e acesso
- Registre [aplicativos](/graph/api/resources/application?view=graph-rest-1.0&preserve-view=true) que se autenticam com o Azure Active Directory (Azure AD). Use as [permissões](./permissions-reference.md#application-resource-permissions) delegadas, Application.Read.All e Application.ReadWrite.All ou as permissões de aplicativos, Application.Read.All, conforme apropriado.
- Para um [dispositivo](/graph/api/resources/device?view=graph-rest-1.0&preserve-view=true) especificado, [verifique a associação](/graph/api/device-checkmemberobjects?view=graph-rest-1.0&preserve-view=true) em outros grupos ou funções de diretório.

### <a name="mail"></a>Email
- Use a propriedade **conversationIndex** para obter a posição de uma mensagem em uma conversa de email do Outlook.
- Use a permissão delegada, Mail.ReadBasic e a permissão de aplicativo, Mail.ReadBasic.All, para obter os recursos de [mensagem](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) ou de [pasta de email](/graph/api/resources/mailfolder?view=graph-rest-1.0&preserve-view=true), acompanhar suas alterações e gerenciar [assinaturas](/graph/api/resources/subscription?view=graph-rest-1.0&preserve-view=true) para notificações de alteração nas mensagens.

### <a name="users"></a>Usuários
- [Verifique se há associações de grupo](/graph/api/user-checkmemberobjects?view=graph-rest-1.0&preserve-view=true) de um [usuário](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true) específico.
- Use a propriedade **creationType** para descobrir como uma conta de usuário foi criada, por exemplo, se a conta foi criada como uma conta corporativa ou de estudante ou como uma conta externa, etc.

## <a name="november-2019-new-in-preview"></a>Novembro de 2019: Novidades na versão prévia

### <a name="calendar"></a>Calendário
- [Use o Outlook para organizar e participar de reuniões online](outlook-calendar-online-meetings.md).
- [Defina as propriedades](/graph/api/place-update?view=graph-rest-beta&preserve-view=true) para os tipos de local avançado de [sala](/graph/api/resources/room?view=graph-rest-beta&preserve-view=true) e [lista de sala](/graph/api/resources/roomlist?view=graph-rest-beta&preserve-view=true).

### <a name="cloud-communication"></a>Comunicação na nuvem
O tipo de recurso de [chamada](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true) dá suporte aos seguintes recursos adicionais:

- O [contexto de uma chamada de entrada](/graph/api/resources/incomingcontext?view=graph-rest-beta&preserve-view=true)
- O tipo de ponto de extremidade de um participante, como correio de voz ou Skype for Business
- A capacidade de [atualizar](/graph/api/call-updaterecordingstatus?view=graph-rest-beta&preserve-view=true) as [informações de registro](/graph/api/resources/recordinginfo?view=graph-rest-beta&preserve-view=true) de um [participante](/graph/api/resources/participant?view=graph-rest-beta&preserve-view=true)

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [novembro](changelog.md#november-2019) do Intune

### <a name="education"></a>Educação
Os administradores podem habilitar as configurações de toda a classe por meio da propriedade **classSettings** da [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) associada à [classe](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true). Atualmente, há uma configuração para notificar os guardiões sobre tarefas semanais.

### <a name="identity-and-access"></a>Identidade e acesso
- Use a permissão do aplicativo, Policy.Read.All, para ler todas as políticas de acesso condicional da sua localização e locais nomeados, sem um usuário conectado.
- Permita que a [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true) esteja em um estado somente de relatório, `enabledForReportingButNotEnforced`.
- Use a permissão delegada, ThreatAssessment.ReadWrite.All, ou a permissão de aplicativo, ThreatAssessment.Read.All, leia (ou crie uma permissão de leitura/gravação) solicitações para avaliar ameaças em uma organização.

### <a name="mail"></a>Email
Use a permissão delegada, Mail.ReadBasic e a permissão de aplicativo, Mail.ReadBasic.All, para gerenciar as [assinaturas](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true) para notificações de alteração no recurso de [mensagem](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true).

### <a name="notifications"></a>Notificações
Use as novas notificações simples [SDK Web](https://aka.ms/GNSDK) em vez do [SDK do Project Rome](https://github.com/Microsoft/project-rome), para aproveitar um modelo de autenticação aperfeiçoado e suporte a aplicativos da Web usando o push da Web. 

### <a name="people-and-workplace-intelligence"></a>Inteligência de pessoas e local de trabalho
Estreia do recurso do [perfil](/graph/api/resources/profile?view=graph-rest-beta&preserve-view=true) que é uma representação avançada da próxima geração de entidades de pessoas nos serviços da Microsoft. Esse recurso se relaciona aos atributos comuns e práticos de pessoas, incluindo informações sobre datas significativas, como [aniversários](/graph/api/resources/personanniversary?view=graph-rest-beta&preserve-view=true), [escolaridade](/graph/api/resources/educationalactivity?view=graph-rest-beta&preserve-view=true), [cargos](/graph/api/resources/workposition?view=graph-rest-beta&preserve-view=true), [interesses](/graph/api/resources/personinterest?view=graph-rest-beta&preserve-view=true), [idioma](/graph/api/resources/languageproficiency?view=graph-rest-beta&preserve-view=true) e [habilidades](/graph/api/resources/skillproficiency?view=graph-rest-beta&preserve-view=true) e competências, [participação em projetos](/graph/api/resources/projectparticipation?view=graph-rest-beta&preserve-view=true), [associação em sites](/graph/api/resources/personwebsite?view=graph-rest-beta&preserve-view=true) e outras informações de contato e [conta](/graph/api/resources/useraccountinformation?view=graph-rest-beta&preserve-view=true).

### <a name="search"></a>Pesquisar
Estreia da [API de Pesquisa da Microsoft](search-concept-overview.md) que permite aos usuários do aplicativo obter os resultados de pesquisa mais atualizados, personalizados e relevantes com a plataforma Microsoft Graph. Use o recurso de [consulta](/graph/api/search-query?view=graph-rest-beta&preserve-view=true)por padrão, pesquisas mensagens e eventos do Outlook e arquivos do OneDrive e do SharePoint na nuvem da Microsoft. Use os conectores [disponíveis](/microsoftsearch/connectors-overview) na [galeria de conectores do Microsoft Graph](/microsoftsearch/connectors-gallery), para incluir dados de pesquisa fora do Microsoft Cloud. Como alternativa, [construa seus próprios conectores](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases), indexe arquivos e itens personalizados externos e consulte fontes de dados externas específicas.

### <a name="teamwork"></a>Trabalho em equipe
Obtenha os recursos de [arquivo](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true) associados a uma [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) e [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) usando a seguinte sintaxe de solicitação de HTTP:

```http
GET /teams/{teamId}/channels/{channelId}/filesFolder
```

### <a name="users"></a>Usuários
Use a propriedade **creationType** para descobrir como uma conta de usuário foi criada, por exemplo, se a conta foi criada como uma conta corporativa ou de estudante ou como uma conta externa, etc.


## <a name="october-2019-new-and-generally-available"></a>Outubro de 2019: Novo e geralmente disponível

### <a name="identity-and-access"></a>Identidade e acesso
- Use [contatos da organização](/graph/api/resources/orgcontact?view=graph-rest-1.0&preserve-view=true) em aplicativos de produção. Os contatos da organização são gerenciados por administradores da organização, sincronizados de um Active Directory local ou do Exchange Online.
- Configure a [autenticação baseada em certificado](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started) em uma [organização](/graph/api/resources/organization?view=graph-rest-1.0&preserve-view=true).
- Adicionar e remover [credenciais de senha](/graph/api/resources/passwordcredential?view=graph-rest-1.0&preserve-view=true) para [aplicativos](/graph/api/resources/application?view=graph-rest-1.0&preserve-view=true).

### <a name="mail"></a>Email
Use o novo parâmetro de **mensagem** para atualizar quaisquer propriedades de [mensagem](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) graváveis ao [responder](/graph/api/message-reply?view=graph-rest-1.0&preserve-view=true) a uma mensagem, por exemplo, [adicionar um destinatário à resposta](/graph/api/message-reply#example?view=graph-rest-1.0&preserve-view=true).

### <a name="microsoft-graph-data-connect"></a>Conexão de dados do Microsoft Graph
Os desenvolvedores e os cientistas de dados agora podem usar [ferramentas para traduzir dados do Office 365 para o formato Modelo de Dados Comum](https://github.com/OfficeDev/MS-Graph-Data-Connect/blob/master/Common-Data-Model/README.md), tornando-o esquematicamente consistente com outros conjuntos de dados prontos da Open Data Initiative (ODI). 


### <a name="microsoft-graph-sdks"></a>SDKs do Microsoft Graph
- Use os manipuladores de caos no SDK do JavaScript para verificar se um aplicativo é resistente a falhas de servidor que são difíceis de iniciar.
- Ler sobre [fazer chamadas API usando os SDKs](./sdks/create-requests.md).

### <a name="users"></a>Usuários
- [Obtenha](/graph/api/user-get-mailboxsettings?view=graph-rest-1.0&preserve-view=true) ou [defina](/graph/api/user-update-mailboxsettings?view=graph-rest-1.0&preserve-view=true) as configurações preferenciais de formato de data e hora do usuário [para a caixa de correio do usuário](/graph/api/resources/mailboxsettings?view=graph-rest-1.0&preserve-view=true). 
- Rastreie a data/hora da última alteração de senha de um [usuário](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true).

## <a name="october-2019-new-in-preview"></a>Outubro de 2019: Novo em visualização

### <a name="calendar"></a>Calendário
- Os organizadores da reunião podem [permitir que os convidados proponham horários de reunião alternativos](outlook-calendar-meeting-proposals.md). Ao receber uma resposta de reunião que inclui uma proposta de horário alternativo, o organizador pode decidir aceitar a proposta e [atualizar](/graph/api/event-update?view=graph-rest-beta&preserve-view=true) o horário da reunião.
- O compartilhamento de calendário programático está mais parecido com a experiência do usuário do Outlook. Além de controlar as permissões do usuário atual e o status de compartilhamento de um calendário:
  - Para cada [calendário](/graph/api/resources/calendar?view=graph-rest-beta&preserve-view=true), você pode gerenciar as [permissões](/graph/api/resources/calendarpermission?view=graph-rest-beta&preserve-view=true) de cada usuário com o qual o calendário é compartilhado. 
  - Para cada [caixa de correio](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true), você pode especificar se um representante, proprietário de caixa de correio ou ambos receberão mensagens da reunião e respostas da reunião. 
- Suporte adicional para reuniões online:
  - Para cada **calendário**, especifique os provedores de reuniões online permitidos e padrão.
  - Crie ou atualize um [evento](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) que esteja disponível online e forneça detalhes para que os participantes possam ingressar na reunião online. 
  - Em particular, use as novas propriedades **onlineMeetingProvider** e **onlineMeeting** do **evento** para definir ou identificar o Microsoft Teams como um provedor de reuniões online, uma solução alternativa para um [problema conhecido](known-issues.md#onlinemeetingurl-property-is-not-supported-for-microsoft-teams) com a propriedade **onlineMeetingUrl**.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [outubro](changelog.md#october-2019) do Intune

### <a name="graph-explorer"></a>Graph Explorer
Experimente a [próxima versão do Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/preview) e confira informações contextuais úteis, como permissões, tokens de acesso e trechos de código do SDK nas novas guias **Permissões**, **Autenticação** e **Trechos de código**. Use o controle deslizante **Visualizar** para alternar entre a [produção](https://developer.microsoft.com/graph/graph-explorer) e a nova versão de visualização do Graph Explorer.

### <a name="groups"></a>Grupos
- Use as propriedades **hideFromAddressLists** e **hideFromOutlookClients** para controlar a visibilidade de um [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) em determinadas partes da interface do usuário do Outlook ou em um cliente do Outlook.
- [Atribuir](/graph/api/group-assignlicense?view=graph-rest-beta&preserve-view=true) ou remover licenças de usuários em um [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access"></a>Identidade e acesso
- Use [políticas de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true) para personalizar regras de acesso para uma organização. Essas regras consideram sinais sobre um usuário ou uma identidade de dispositivo, como associação de usuário ou grupo, local de IP e comportamentos, como tentativas de acessar aplicativos específicos e comportamentos de entrada arriscados.
- Use o [gerenciamento de direitos](/graph/api/resources/entitlementmanagement-overview?view=graph-rest-beta&preserve-view=true) para gerenciar o acesso a grupos, aplicativos e sites do SharePoint Online para usuários dentro e fora de uma organização.
- Adicione e remova [credenciais de senha](/graph/api/resources/passwordcredential?view=graph-rest-beta&preserve-view=true) para [aplicativos](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) e [entidades de serviço](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true).
- Gerenciar a [política de estrutura confiável](/graph/api/resources/trustframeworkkeyset?view=graph-rest-beta&preserve-view=true) do Azure AD B2C.
- Defina as políticas de [fluxo de usuário](/graph/api/resources/identityuserflow?view=graph-rest-beta&preserve-view=true) do Azure AD B2C para entrar, inscrever-se, entrar e Inscrever-se combinados, redefinir senha e atualizar perfil.
- Configure [rótulos de proteção de informações](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta&preserve-view=true) para classificar a confidencialidade de um usuário ou locatário.
- Aplicativos existentes usando as APIs para [eventos de risco de identidade](/graph/api/resources/identityriskevent?view=graph-rest-beta&preserve-view=true) devem fazer ar transição para [ detecção de risco](/graph/api/resources/riskdetection?view=graph-rest-beta&preserve-view=true) no Azure AD Identity Protection. Confira a postagem de blog [ postagem de blog](https://developer.microsoft.com/graph/blogs/deprecatation-of-the-identityriskevents-api/) relacionada para obter mais detalhes e cronograma de descontinuação.


### <a name="mail"></a>Email
[Anexe arquivos grandes de até 150MB](outlook-large-attachments.md) a uma instância de [mensagem](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true), criando uma [sessão de upload](/graph/api/resources/uploadsession?view=graph-rest-beta&preserve-view=true) e carregando iterativamente os intervalos do arquivo até que todos os bytes do arquivo tenham sido carregados. 

### <a name="microsoft-graph-security-api"></a>API de Segurança do Microsoft Graph
- Visualize a integração com a RSA NetWitness, ServiceNow e Splunk, para correlacionar e sincronizar [alertas](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true#alerts)e melhorar a proteção contra ameaças e respostas.
- Novos disparadores adicionados ao [Conector de Segurança do Microsoft Graph](/connectors/microsoftgraphsecurity/) e [guias estratégicos](/azure/security-center/security-center-playbooks) para Aplicativos de Lógica e Fluxo. Confira [exemplos de guias estratégicos](https://github.com/microsoftgraph/security-api-solutions/tree/master/Playbooks).
- Suporte para enviar [indicadores de ameaça](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true#threat-indicators-preview) para o Microsoft Defender para Ponto de Extremidade para bloquear ou alertar sobre ameaças usando suas próprias fontes de inteligência. Integrações com parceiros como o ThreatConnect permitem que os clientes enviem indicadores diretamente das soluções de inteligência e automação contra ameaças. 

### <a name="notifications"></a>Notificações
- [Crie e envie notificações](/graph/api/user-post-notifications?view=graph-rest-beta&preserve-view=true) a todos os clientes de aplicativos em todos os pontos de extremidade do dispositivo que um usuário está conectado, sem ter que gerenciar as permissões de usuário delegadas.
- Use [os pontos de extremidade da política de destino](/graph/api/resources/targetpolicyendpoints?view=graph-rest-beta&preserve-view=true) em [notificações](/graph/api/resources/notification?view=graph-rest-beta&preserve-view=true) do usuário para direcionar especificamente notificações para as plataformas Windows, iOS, Android ou WebPush.
- Especificar uma [política de retirada](/graph/api/resources/fallbackpolicy?view=graph-rest-beta&preserve-view=true) nas notificações para pontos de extremidade iOS, enviar notificações brutas de alta prioridade que podem não ser entregues aos dispositivos, caso contrário, devido a restrições específicas da plataforma, como o modo de economia de bateria.

 
### <a name="powershell-sdk"></a>SDK do PowerShell 
Os desenvolvedores e profissionais de TI podem observar o lançamento da [SDK do Microsoft Graph PowerShell](https://github.com/microsoftgraph/msgraph-sdk-powershell), que criará módulos que contêm cmdlets para criar solicitações da API REST do Microsoft Graph.

## <a name="september-2019-new-and-generally-available"></a>Setembro de 2019: novo e disponível para o público geral

### <a name="calendar-mail-and-group"></a>Calendário, email e grupo
[Obter o conteúdo bruto de um arquivo, ou o conteúdo MIME de um item](/graph/api/attachment-get?view=graph-rest-1.0&preserve-view=true#get-the-raw-contents-of-a-file-or-item-attachment) que foi adicionado como um [anexo](/graph/api/resources/attachment?view=graph-rest-1.0&preserve-view=true) a um[evento](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true), [ mensagem](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true)ou[ postagem](/graph/api/resources/post?view=graph-rest-1.0&preserve-view=true) de grupo.

### <a name="calendar-mail-outlook-task-personal-contact"></a>Calendário, email, tarefa do Outlook, contato pessoal
Use a função [translateExchange](/graph/api/user-translateexchangeids?view=graph-rest-1.0&preserve-view=true) para converter uma ID de item do Outlook [entre](/graph/api/user-translateexchangeids?view=graph-rest-1.0&preserve-view=true#exchangeidformat-values)formatos suportados, incluindo o formato de ID padrão do Microsoft Graph e o formato de ID imutável. 

Os recursos a seguir são compatíveis com a conversão de formato de ID:

- [attachment](/graph/api/resources/attachment?view=graph-rest-1.0&preserve-view=true)
- [contato](/graph/api/resources/contact?view=graph-rest-1.0&preserve-view=true)
- [event](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true)
- [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-1.0&preserve-view=true)
- [message](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true)
- [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-1.0&preserve-view=true)

### <a name="mail"></a>Email
[Obter conteúdo MIME de uma mensagem](outlook-get-mime-message.md).

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph Toolkit
Use o [Microsoft Graph Toolkit](toolkit/overview.md) para desenvolver aplicativos de produção que ofereçam uma aparência consistente do Microsoft 365 e economize tempo na autenticação e acesso a dados do Microsoft Graph.

## <a name="september-2019-new-in-preview"></a>Setembro de 2019: novidades na versão prévia

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status GA. Não os use em aplicativos de produção.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [Setembro](changelog.md#september-2019) do Intune

### <a name="files"></a>Arquivos
- Suporte aprimorado à sincronização:

  - Use a nova propriedade **pendingOperations** para identificar operações que podem afetar o conteúdo binário de um [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true).
  - [Restaure](/graph/api/driveitem-restore?view=graph-rest-beta&preserve-view=true) um **driveItem** excluído. 
- Use o Algoritmo de Hash Seguro (SHA-256) para aprimorar a segurança e a integridade dos [dados](/graph/api/resources/file?view=graph-rest-beta&preserve-view=true) do arquivo.
- Obtenha ou defina a orientação de uma [foto](/graph/api/resources/photo?view=graph-rest-beta&preserve-view=true). A configuração é compatível com o OneDrive Personal.

### <a name="identity-and-access"></a>Identidade e acesso
- Use a propriedade new **identities** e obtenha as identidades que um [usuário](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true) pode usar para entrar em uma conta. As identidades podem ser fornecidas por organizações ou provedores de identidade social, como Facebook, Google e Microsoft.
- Aperfeiçoamentos incrementais para [sincronizar identidades](/graph/api/resources/synchronization-overview?view=graph-rest-beta&preserve-view=true) em um aplicativo de nuvem para um locatário:

  - Armazenar configurações para um [trabalho de sincronização](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta&preserve-view=true)
  - Especifique um motivo para impor a [quarentena](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta&preserve-view=true) a um trabalho de sincronização

### <a name="teamwork"></a>Trabalho em equipe
Use o canal **Geral** de uma [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) ou personalize as [configurações de membros](/graph/api/resources/teammembersettings?view=graph-rest-beta&preserve-view=true) para permitir que eles criem canais privados na **equipe**.

### <a name="users"></a>Usuários
- Obtenha ou atualize as identidades com as quais um [usuário](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true) pode entrar em uma conta. Essas identidades podem ser fornecidas por organizações de negócios ou por provedores de identidade social, como o Facebook, o Google e a Microsoft.
- Obtenha ou atualize as [configurações da caixa de correio](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true) do formato de data e hora escolhidas pelo usuário.


## <a name="august-2019-new-and-generally-available"></a>Agosto de 2019: novo e disponível para o público geral 

### <a name="reports"></a>Relatórios
- Obtenha dados [adicionais de uso da caixa de correio](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0&preserve-view=true) sobre o tamanho e a contagem de itens excluídos.
- Acompanhe as IDs do grupo do Microsoft 365 ao [obter detalhes da atividade do grupo](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0&preserve-view=true).
- Rastreie o nome principal do proprietário ao obter [detalhes da conta de uso do OneDrive](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0&preserve-view=true) e [ detalhes de uso do site do SharePoint](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0&preserve-view=true).
- Obtenha o número de usuários ativos e inativos no Microsoft 365, ao [receber um relatório sobre contagens de usuários por serviço do Microsoft 365](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0&preserve-view=true).

### <a name="security"></a>Segurança
- Use o novo [complemento da API de Segurança do Microsoft Graph para Splunk](https://aka.ms/graphsecuritysplunkaddon) para transmitir alertas de segurança e insights de muitos produtos de parceiros para o Splunk, permitindo uma correlação mais simples de seus dados de segurança em tempo real. Consulte o [anúncio](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Introducing-the-new-Microsoft-Graph-Security-API-add-on-for/ba-p/815972) para mais informações. 
- [Confira uma lista de outras soluções e conectores](security-integration.md) criados pela Microsoft ou por parceiros da Microsoft que se conectam à API de segurança e permitem que você trabalhe com dados em um formato unificado.


## <a name="august-2019-new-in-preview"></a>Agosto de 2019: novidades na versão prévia

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status GA. Não os use em aplicativos de produção.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [agosto](changelog.md#august-2019) do Intune

### <a name="education"></a>Educação
- Associe um [professor](/graph/api/resources/educationuser?view=graph-rest-beta&preserve-view=true) ou uma [atribuição](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) com uma [lista de critérios de avaliação classificada](/graph/api/resources/educationrubric?view=graph-rest-beta&preserve-view=true) para considerar qualidades e níveis específicos em atribuições. Um exemplo de qualidade é a ortografia e a gramática, e exemplos de níveis são "bons" e "ruins". Você pode ainda associar pontos e pesos a lista de critérios de avaliação. Para saber mais, confira [visão geral da lista de critérios de avaliação educacional](education-rubric-overview.md).
- Avaliar uma atribuição e apresentar os resultados em termos de [feedback](/graph/api/resources/educationfeedbackoutcome?view=graph-rest-beta&preserve-view=true), de um [grau numérico](/graph/api/resources/educationpointsoutcome?view=graph-rest-beta&preserve-view=true), ou de [lista de critérios de avaliação](/graph/api/resources/educationrubricoutcome?view=graph-rest-beta&preserve-view=true).

### <a name="files"></a>Arquivos
Até esse ponto, você pode [seguir](/graph/api/driveitem-follow?view=graph-rest-beta&preserve-view=true) um [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true) para obter um acesso conveniente ou para facilitar ações como, mover, copiar e salvar como. Agora você pode usar a ação [deixar de seguir](/graph/api/driveitem-unfollow?view=graph-rest-beta&preserve-view=true) para parar de seguir esses itens da unidade.

### <a name="identity-and-access"></a>Identidade e acesso
- Os provedores de controle de acesso baseado em função (RBAC) podem [gerenciar funções](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true) do Azure Active Directory, [definindo ações de funções](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true)que podem ser realizadas em recursos específicos e [atribuindo funções](/graph/api/resources/unifiedroleassignment?view=graph-rest-beta&preserve-view=true) aos usuários com base em tais definições de função, fornecendo o acesso correspondente a esses recursos.
- Os administradores podem [listar as revisões de acesso](/graph/api/accessreview-list?view=graph-rest-beta&preserve-view=true) para facilitar de maneira eficiente a análise de associações de grupos, o acesso a aplicativos corporativos e as atribuições de funções. As revisões de acesso regular garantem que apenas as pessoas adequadas tenham acesso contínuo aos recursos de maneiras específicas.

### <a name="social-and-workplace-intelligence"></a>Inteligência social e do local de trabalho
Os usuários finais podem usar o aplicativo [MyAnalytics](social-intel-concept-overview.md#why-integrate-with-document-based-insights) do Microsoft 365 para obter insights sobre gerenciamento de tempo, colaboração no trabalho e equilíbrio profissional. Agora você pode usar a [API de análise](/graph/api/resources/social-overview?view=graph-rest-beta&preserve-view=true#help-users-gain-insights-into-their-work-patterns) para integrar dados sobre tempo gasto em atividades de trabalho, como chamadas, chats e email, para ajudar a melhorar a produtividade e o bem-estar do usuário. 


## <a name="july-2019-new-and-generally-available"></a>Julho de 2019: novo e disponível para o público geral 

### <a name="example-code-snippets"></a>Exemplo de trechos de código
Agora há trechos do código Objective-C em todos os tópicos da API nas referências v 1.0 e beta. Veja o exemplo do Objective-C de como [obter um evento](/graph/api/event-get?view=graph-rest-1.0&preserve-view=true&tabs=objective-c#example).

### <a name="group"></a>Grupo
- Use a função[validateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0&preserve-view=true) para verificar se o nome de exibição ou apelido de email de um grupo existente do Microsoft 365 está em conformidade com as políticas de nomenclatura.
- Como alternativa, antes de criar o grupo, você pode usar a função[ ValidateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0&preserve-view=true)para um[directoryobject](/graph/api/resources/directoryobject?view=graph-rest-1.0&preserve-view=true) para validar primeiro os nomes.

### <a name="identity-and-access"></a>Identidade e acesso
- Use as [novas permissões delegadas e de aplicativo](permissions-reference.md#organization-permissions), _Organization.Read.All_ e _Organization.ReadWrite.All_ para acessar uma [organização](/graph/api/resources/organization?view=graph-rest-1.0&preserve-view=true) e recursos relacionados, como [SKUs inscritos](/graph/api/resources/subscribedsku?view=graph-rest-1.0&preserve-view=true).
- Use [novas permissões delegadas e de aplicativo](permissions-reference.md#role-management-permissions), _RoleManagement. Read.Directory_ e _RoleManagement. ReadWrite.Directory_, para controle de acesso baseado em função ( RBAC) para o diretório da empresa:

  - Use a permissão de leitura/gravação para [ativar](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0&preserve-view=true) primeiro uma função de diretório. 
  - Com a função ativada, você pode usar a permissão de leitura para[ler funções de diretório](/graph/api/directoryrole-list?view=graph-rest-1.0&preserve-view=true), [listar os membros da função](/graph/api/directoryrole-list-members?view=graph-rest-1.0&preserve-view=true) e [listar modelos de função de diretório](/graph/api/directoryroletemplate-list?view=graph-rest-1.0&preserve-view=true). 
  - Você também pode usar a permissão de leitura/gravação para[adicionar](/graph/api/directoryrole-post-members?view=graph-rest-1.0&preserve-view=true)e [remover](/graph/api/directoryrole-delete-member?view=graph-rest-1.0&preserve-view=true) membros da função.


## <a name="july-2019-new-in-preview"></a>Julho de 2019: Novo na visualização

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status GA. Não os use em aplicativos de produção.

### <a name="calendar"></a>Calendário 
Use a nova [API de locais](/graph/api/resources/place?view=graph-rest-beta&preserve-view=true) para usar vários tipos de locais, como [salas](/graph/api/resources/room?view=graph-rest-beta&preserve-view=true) e [lista de salas](/graph/api/resources/roomlist?view=graph-rest-beta&preserve-view=true), conforme configurado pelos administradores do Exchange Online.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [julho](changelog.md#july-2019) do Intune

### <a name="files"></a>Arquivos 
Aplique a data/hora de vencimento ou a senha ao [criar um link de compartilhamento](/graph/api/driveitem-createlink?view=graph-rest-beta&preserve-view=true) para um arquivo, pasta, ou outros [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access"></a>Identidade e acesso
- Use [nova permissão de aplicativo](./permissions-reference.md#access-reviews-permissions) _AccessReview.ReadWrite.Membership_ para operações CRUD nas [análises de acesso](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true). 
- Use [novas permissões delegadas e de aplicativo](permissions-reference.md#administrative-units-permissions),_AdministrativeUnit.Read.All_ e _AdministrativeUnit. ReadWrite.All_, para ler ou gravar respectivamente (incluindo criar, atualizar, excluir ou gerenciar a associação) recursos da [unidade de administração](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true).
- Use as [novas permissões delegadas e de aplicativo](permissions-reference.md#organization-permissions), _Organization.Read.All_ e _Organization.ReadWrite.All_ para acessar uma [organização](/graph/api/resources/organization?view=graph-rest-beta&preserve-view=true) e recursos relacionados, como [SKU inscritos](/graph/api/resources/subscribedsku?view=graph-rest-beta&preserve-view=true).
- Use a nova função[descobrir](/graph/api/directorydefinition-discover?view=graph-rest-beta&preserve-view=true) para encontrar o [esquema de sincronização](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta&preserve-view=true)de diretório mais recente, para sincronizar objetos de diretório, atributos e seus tipos de aplicativo.
- Use a [política de distribuição de recursos](/graph/api/resources/featureRolloutPolicy?view=graph-rest-beta&preserve-view=true) para ajudar os administradores de locatários a testar recursos em grupos específicos antes de habilitá-los para toda a organização.

### <a name="mail"></a>Email
Use permissões de aplicativo mais granulares _Mail.ReadBasic.All_ para ler a caixa de correio de um usuário, com exceção de qualquer corpo de mensagem, corpo de visualização, anexos e propriedades estendidas e com exceção da pesquisa na caixa de correio. Agora aplicável ao [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta&preserve-view=true) e ao [acompanhamento de alterações](delta-query-overview.md) para [mensagem](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) e **mailFolder**.

### <a name="reports"></a>Relatórios
- Obtenha dados [adicionais de uso da caixa de correio](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta&preserve-view=true) sobre o tamanho e a contagem de itens excluídos.

### <a name="teamwork"></a>Trabalho em equipe
- [Instalar](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta&preserve-view=true), [desinstalar](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta&preserve-view=true), [atualizar ](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta&preserve-view=true) e [listar aplicativos do Microsoft Teams instalados ](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta&preserve-view=true) para um usuário. 
- Use o acesso somente para aplicativos para ler mensagens de canal, respostas a mensagens de canal e mensagens em um chat. [Solicite e obtenha aprovação](teams-protected-apis.md) para esse acesso.

## <a name="may---june-2019-new-and-generally-available"></a>Maio e julho de 2019: novo e disponível para o público geral

### <a name="calendar-mail-and-personal-contacts"></a>Calendário, email e contatos pessoais
Os administradores do Exchange podem conceder permissões de aplicativo a um aplicativo e [restringir o seu acesso apenas a um subconjunto de caixas de correio em um ](auth-limit-mailbox-access.md), ao invés do padrão, que é o acesso a todas as caixas de correio na organização. Este acesso restrito se aplicaria a quaisquer permissões de aplicativos concedidas ao aplicativo para [calendários](permissions-reference.md#calendars-permissions), [contatos](permissions-reference.md#contacts-permissions) e [configurações de email e de caixa de correio](permissions-reference.md#mail-permissions). Confira o [anúncio do blog](https://developer.microsoft.com/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/) relacionado.

### <a name="mail"></a>Email
Use a API de [pastas de pesquisa de email](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0&preserve-view=true) para pesquisar mensagens e acessar os resultados de pesquisa de email do Outlook. Consulte o [anúncio do blog](https://developer.microsoft.com/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/) relacionado.

### <a name="postman"></a>Postman
Como uma alternativa ao Explorador do Graph, experimente a API do Microsoft Graph na [coleção do Microsoft Graph Postman](use-postman.md) para aprender o comportamento da API e acelerar o desenvolvimento de aplicativos.

### <a name="tutorials"></a>Tutoriais
Experimente o novo [tutorial para criar um aplicativo de console do Java](/graph/tutorials/java) para obter informações sobre um calendário de usuário.

### <a name="user"></a>Usuário
Administradores ou usuários podem [revogar](/graph/api/user-revokesigninsessions?view=graph-rest-1.0&preserve-view=true) todos os tokens de atualização emitidos para um usuário. Isso geralmente é usado para impedir que aplicativos em um dispositivo perdido ou roubado acessem os dados de uma organização.


## <a name="may---june-2019-new-in-preview"></a>Maio e junho de 2019: novidades na versão prévia

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status GA. Não os use em aplicativos de produção.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
- Atualizações de [maio](changelog.md#may-2019) do Intune 
- Atualizações de [junho](changelog.md#june-2019) do Intune

### <a name="education"></a>Educação
- Consulta Delta para um objeto [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta&preserve-view=true).
- Consulta Delta e adições de propriedade para objetos [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true) e [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta&preserve-view=true).

### <a name="group"></a>Grupo
Obtenha [rótulos de confidencialidade](/graph/api/resources/assignedlabel?view=graph-rest-beta&preserve-view=true) para ajudar a proteger dados confidenciais de grupos do Microsoft 365 e atender às políticas de conformidade. Esses rótulos são objetos [assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta&preserve-view=true), publicados por administradores no Centro de Conformidade e Segurança do Microsoft 365, como parte dos recursos de Proteção de Informações do Microsoft Purview. 

### <a name="identity-and-access"></a>Identidade e acesso
- Obtenha uma instância de um [aplicativo](/graph/api/resources/applicationtemplate?view=graph-rest-beta&preserve-view=true) ou adicione uma instância da galeria de aplicativos do Azure AD ao seu diretório como modelo.
- Obtenha um log de todos os diretórios de[eventos de provisionamento](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta&preserve-view=true) em um locatário.
- Obtenha informações sobre [usuário detectado ou riscos de login](/graph/api/resources/riskdetection?view=graph-rest-beta&preserve-view=true) em um ambiente do Azure AD. Esta funcionalidade de detecção de riscos faz parte do Azure AD Identity Protection.

### <a name="mail"></a>Email
Use uma permissão delegada mais granular, _Mail.ReadBasic_, para ler a caixa de correio de um usuário, exceto para qualquer corpo da mensagem, corpo da visualização, anexos e propriedades estendidas, exceto para pesquisar a caixa de correio. Disponível para ler métodos de [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta&preserve-view=true)e [acompanhamento de alterações](delta-query-overview.md)para [mensagem](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) e **mailFolder**.

### <a name="microsoft-graph-toolkit"></a>Kit de ferramentas do Microsoft Graph
O [kit de ferramentas do Microsoft Graph](./toolkit/overview.md) é um conjunto de colaboradores e de componentes da Web de estrutura independente que oferece conveniência para autenticar e acessar dados no Microsoft Graph. Como o kit de ferramentas do Microsoft Graph está no status de visualização, use provedores e componentes do kit de ferramentas somente em aplicativos que não são de produção.

### <a name="reports"></a>Relatórios
- Obtenha [relatórios sobre os métodos de autenticação](/graph/api/resources/authenticationmethods-usage-insights-overview?view=graph-rest-beta&preserve-view=true) adotados pelos usuários em uma organização, como rest de senha de autoatendimento e autenticação multifator (MFA).

### <a name="sites"></a>Sites
Permitir que os usuários [sigam](/graph/api/site-follow?view=graph-rest-beta&preserve-view=true) ou [parem de seguir](/graph/api/site-unfollow?view=graph-rest-beta&preserve-view=true) os sites do SharePoint.

### <a name="teamwork"></a>Trabalho em equipe
- Hospede [imagens](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta&preserve-view=true) em [mensagens de bate-papo](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) do Microsoft Teams.
- Suporte para [configurar](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta&preserve-view=true) como uma equipe privada pode ser descoberta.


## <a name="january---april-2019-new-and-generally-available"></a>Janeiro a abril de 2019: novo e disponível para o público geral

[Microsoft Graph data connect](data-connect-concept-overview.md)

### <a name="calendar"></a>Calendário
[Obter agenda de disponibilidade](outlook-get-free-busy-schedule.md)

### <a name="identity-and-access"></a>Identidade e acesso
[Fornecedores de identidade](/graph/api/resources/identityprovider?view=graph-rest-1.0&preserve-view=true)
[melhores guias de autenticação](./auth/index.yml)
[migrando aplicativos do Azure AD Graph para o Microsoft Graph](migrate-azure-ad-graph-planning-checklist.md)

### <a name="sdks"></a>SDKs
[Guias SDK](/sdks/sdks-overview.md)Trechos de API ([exemplo](/graph/api/user-get?view=graph-rest-1.0&preserve-view=true&tabs=cs#sdk-sample-code))

### <a name="security"></a>Segurança
[Classificação de segurança do locatário](/graph/api/resources/securescore?view=graph-rest-1.0&preserve-view=true)

## <a name="january---april-2019-new-in-preview"></a>Janeiro a abril de 2019: novo na versão prévia

### <a name="calendar-group-mail-to-do-tasks"></a>Calendário, grupo, email, tarefas pendentes
[Obter o conteúdo bruto/MIME de anexos de arquivo ou item](/graph/api/attachment-get?view=graph-rest-beta&preserve-view=true#get-the-raw-contents-of-a-file-or-item-attachment) para um evento, mensagem, tarefa do Outlook ou postagem do grupo

### <a name="change-notifications"></a>Notificações de alteração
[Reduzir notificações ausentes de alteração](webhooks-lifecycle.md)

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
- Atualizações [de](changelog.md#january-2019) janeiro do Intune 
- Atualizações [de](changelog.md#february-2019) fevereiro do Intune
- Atualizações [de](changelog.md#march-2019) março do Intune
- Atualizações [de](changelog.md#april-2019) abril do Intune

### <a name="files"></a>Arquivos
[Compartilhamento de convite](/graph/api/driveitem-invite?view=graph-rest-beta&preserve-view=true) inclui data de vencimento e senha

### <a name="financials"></a>Finanças
[Dynamics 365 Business Central](dynamics-business-central-concept-overview.md)

### <a name="identity-and-access"></a>Identidade e acesso
[O Access revisa](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true) as permissões de aplicativo suporte [auditoria e registros](/graph/api/resources/azure-ad-auditlog-overview?view=graph-rest-beta&preserve-view=true)
[de entrada personalizado, entre e inscreva-se no Azure AD B2C](/graph/api/resources/trustframeworkpolicy?view=graph-rest-beta&preserve-view=true)
[usuário arriscado](/graph/api/resources/riskyuser?view=graph-rest-beta&preserve-view=true) e [histórico](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta&preserve-view=true)

### <a name="mail"></a>Correio
[Obter conteúdo MIME de mensagens](outlook-get-mime-message.md)

### <a name="reports"></a>Relatórios
[Relatórios de entrada do aplicativo](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta&preserve-view=true)

### <a name="security"></a>Segurança
[Indicadores de ameaça ](/graph/api/resources/securityaction?view=graph-rest-beta&preserve-view=true)
[de Ações de segurança](/graph/api/resources/tiindicator?view=graph-rest-beta&preserve-view=true)

### <a name="teamwork"></a>Trabalho em equipe
[O gerenciamento](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)
[de conversas em 1:1](/graph/api/resources/shift?view=graph-rest-beta&preserve-view=true)

## <a name="see-also"></a>Confira também
- Confira [O que há de novo](whats-new-overview.md) no Microsoft Graph.
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).
