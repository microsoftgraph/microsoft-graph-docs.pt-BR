---
title: Novidades do Microsoft Graph
description: Exiba os destaques das novidades Microsoft Graph nos últimos dois meses, o que foi adicionado em versões anteriores e como você pode compartilhar suas ideias.
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 7fd388275a31b3b7e426e3f27dc6f5861b9a297f
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160276"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Recursos, incluindo APIs e ferramentas, no status de _visualização_ podem mudar sem aviso prévio e alguns podem nunca ser promovidos ao status de disponibilidade geral (GA). Não utilize recursos de visualização em aplicativos de produção.


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
