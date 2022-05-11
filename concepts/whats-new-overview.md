---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 75b01f4903153249131cc69e336bb2d12e26095d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316158"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Recursos, incluindo APIs e ferramentas, no status de _visualização_ podem mudar sem aviso prévio e alguns podem nunca ser promovidos ao status de disponibilidade geral (GA). Não utilize recursos de visualização em aplicativos de produção.


## <a name="april-2022-new-in-preview-only"></a>Abril de 2022: novo somente para visualização

### <a name="customer-bookings"></a>Reservas do Cliente
- [Obtenha informações de disponibilidade](/graph/api/bookingbusiness-getstaffavailability?view=graph-rest-beta&preserve-view=true) para recursos de um [membro da equipe](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true) em uma [empresa](/graph/api/resources/bookingbusiness?view=graph-rest-beta&preserve-view=true).
- Use a permissão de aplicativo `Bookings.Read.All` em operações de leitura para recursos de[empresas](/graph/api/resources/bookingbusiness?view=graph-rest-beta&preserve-view=true), [membro da equipe](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true), [serviço](/graph/api/resources/bookingservice?view=graph-rest-beta&preserve-view=true), [cliente](/graph/api/resources/bookingcustomer?view=graph-rest-beta&preserve-view=true) e [compromisso](/graph/api/resources/bookingappointment?view=graph-rest-beta&preserve-view=true).
- Use a permissão de aplicativo `BookingsAppointment.ReadWrite.All` para operações de leitura/gravação para recursos de cliente e compromisso.

### <a name="device-and-app-management--cloud-pc"></a>Gerenciamento de dispositivos e aplicativos | PC na nuvem
Especifique [Configurações do Windows](/graph/api/resources/cloudpcwindowssettings?view=graph-rest-beta&preserve-view=true) como parte das [configurações da organização do PC na nuvem](/graph/api/resources/cloudPcOrganizationSettings?view=graph-rest-beta&preserve-view=true) para um locatário.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
Configure [ configurações de federação](/graph/api/resources/internalDomainFederation?view=graph-rest-beta&preserve-view=true) para federar domínios com o Azure Active Directory.

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
- [Remova um canal compartilhado com uma equipe](/graph/api/team-delete-incomingchannel?view=graph-rest-beta&preserve-view=true).
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
