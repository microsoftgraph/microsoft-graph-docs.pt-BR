---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: e03d5035aff0736d94415167c891fac3478bec00
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845642"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Confira os destaques das novidades do Microsoft Graph e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista completa das atualizações da API, consulte as seções [May](changelog.md#may-2020) [e o](changelog.md#june-2020) que são as do changelog da API. 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.


## <a name="june-2020-new-and-generally-available"></a>Junho de 2020: novo e geralmente disponível

### <a name="cloud-communications--online-meeting"></a>Comunicações na nuvem | Reunião online
- Use o `Accept-Language` cabeçalho HTTP ao [criar uma reunião online](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0) para fornecer informações de ingresso com base na localidade.
- Use [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-1.0) para retornar uma reunião online que tenha um valor **externalId** especificado ou crie um se nenhum já existir, para simplificar a incorporação da reunião resultante em um calendário de terceiros.

### <a name="groups"></a>Grupos
Use permissões de aplicativo `Group.Read.All` e `Group.ReadWrite.All` para obter recursos de [conversa](/graph/api/resources/conversation) de grupo e [thread de conversa](/graph/api/resources/conversationthread) .

### <a name="security"></a>Segurança
- Acompanhar o seguinte como propriedades de um [alerta](/graph/api/resources/alert?view=graph-rest-1.0):
  - IDs de incidentes relacionados ao alerta.
  - Identifique um [recurso](/graph/api/resources/securityResource?view=graph-rest-1.0#securityresourcetype-values) como atacado ou como um recurso relacionado no alerta.
  - Especifique os locais de origem e de destino de uma [conexão de rede](/graph/api/resources/networkconnection?view=graph-rest-1.0) relacionada ao alerta.

### <a name="teamwork"></a>Teamwork
- Use a permissão delegada [AppCatalog. Read. All](/graph/permissions-reference#appcatalog-resource-permissions) para listar [aplicativos](/graph/api/resources/teamsapp?view=graph-rest-1.0) do catálogo de aplicativos do Microsoft Teams.
- [Obtenha informações sobre a pasta](/graph/api/channel-get-filesfolder) que mapeia a guia **arquivos** de um [canal](/graph/api/resources/channel)do teams.
- [Obtenha o canal padrão](/graph/api/team-get-primarychannel), rotulado como **geral**, de uma [equipe](/graph/api/resources/team).


## <a name="june-2020-new-in-preview-only"></a>Junho de 2020: novo na visualização apenas
### <a name="cloud-communications--presence"></a>Comunicações em nuvem | Presença
[Obter o status de presença](/graph/api/presence-get?view=graph-rest-beta) de todos os usuários em uma organização ou de um usuário específico na organização.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações do Intune em [junho](changelog.md#june-2020) no beta.

### <a name="identity-and-access"></a>Identidade e acesso
- Os profissionais de ti podem usar os recursos de [conectores](/graph/api/resources/connector?view=graph-rest-beta) que são agentes leves para se conectarem ao [proxy de aplicativo do Azure ad](/azure/active-directory/manage-apps/what-is-application-proxy)e [publicar aplicativos Web no local externamente](/graph/api/resources/onpremisespublishing?view=graph-rest-beta), para que os usuários remotos de suas organizações possam acessar esses aplicativos de uma maneira segura.
- Gerenciar uma [política de autenticação](/graph/api/resources/authenticationflowspolicy?view=graph-rest-beta) em nível de locatário para habilitar ou desabilitar [a inscrição de autoatendimento](/graph/api/resources/selfservicesignupauthenticationflowconfiguration?view=graph-rest-beta) de usuários externos.

### <a name="users"></a>Usuários
Use [as configurações do usuário](/graph/api/resources/usersettings?view=graph-rest-beta) para [obter](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta) ou [Atualizar](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta) [languaes preferenciais e configurações regionais](/graph/api/resources/regionalandlanguagesettings?view=graph-rest-beta).

Configurações de usuário é uma relação acessível por meio do [usuário](/graph/api/resources/user?view=graph-rest-beta) que permite uma experiência de usuário consistente entre aplicativos, tocando no perfil de usuário do Azure ad para refletir as mesmas preferências do usuário. Veja [como as configurações de usuário diferenciam as configurações de caixa de correio](/graph/api/resources/user?view=graph-rest-beta#user-preferences-for-languages-and-regional-formats).

## <a name="may-2020-new-and-generally-available"></a>Maio de 2020: novo e geralmente disponível

### <a name="calendar--place"></a>Calendário | Local
GA da [API de locais](/graph/api/resources/place) em v 1.0 – Use esta API em aplicativos de produção para obter, atualizar ou excluir uma lista de [salas](/graph/api/resources/room) ou [salas](/graph/api/resources/roomlist) em um locatário. [Saiba mais](outlook-calendar-concept-overview.md#build-apps-with-location-awareness-and-provide-intelligent-context) sobre a API de locais.

### <a name="change-notifications"></a>Notificações de alteração
- Assine as notificações de alteração no Microsoft Cloud para o governo dos EUA.

### <a name="cloud-communications--call-records"></a>Comunicação em nuvem | Gravação
- GA da [API de registros de chamadas](/graph/api/resources/callrecords-api-overview?view=graph-rest-1.0) – use o recurso [callRecord](/graph/api/resources/callrecord?view=graph-rest-1.0) para obter os metadados de chamadas e reuniões online no Microsoft Teams e no Skype.
- Inscreva-se para [alterar as notificações](/graph/webhooks) de alterações em todos os recursos do **callRecord** em uma organização.
- [Listar sessões](/graph/api/callrecords-session-list?view=graph-rest-1.0) em um **callRecord**e, opcionalmente, [expanda cada sessão para listar segmentos](/graph/api/callrecords-session-list?view=graph-rest-1.0#example-2-get-session-list-with-segments) no registro de chamada.
- Suporte para os valores de banda de 60-GHz ( `frequency60GHz` ) e `unknownFutureValue` WiFi de um ponto de extremidade de mídia em um segmento.
- Suporte para caixa postal como um possível tipo de ponto de extremidade do serviço em um [segmento](/graph/api/resources/callrecords-segment)de comunicação.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
O Intune [pode](changelog.md#may-2020) atualizar em v 1.0.

### <a name="graph-explorer"></a>Explorador do Graph
Use os vários novos recursos do [Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer) que aprimoram o aprendizado e o protótipo na área restrita. Por exemplo:
- Exibir trechos de código que correspondem à consulta da API REST inserida, em C#, Java, JavaScript e objetivo C.
- Conectado com um locatário, exiba e copie um token de acesso para seu aplicativo de cliente REST favorito.

Consulte o [novo explorador do Graph agora está disponível](https://developer.microsoft.com/graph/blogs/new-graph-explorer-is-now-ga/) para obter mais detalhes.

### <a name="groups"></a>Grupos
- A sincronização do diretório local com o Azure Active Directory por meio do Azure AD Connect agora retorna as propriedades **onPremisesDomainName**, **onPremisesNetBiosName** e **onPremisesSamAccountName** como parte do recurso de [grupo](/graph/api/resources/group?view=graph-rest-1.0) .
- Assine as notificações de alteração para recursos de [grupo](/graph/api/resources/group) no Microsoft Cloud China operado pela 21vianet.

### <a name="identity-and-access"></a>Identidade e acesso
- GA da API de entidades de serviço no v 1.0 – Use o [recurso servicePrincipalName](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) nos aplicativos de produção para gerenciar programaticamente as instâncias de aplicativos e controlar o que um aplicativo pode fazer dentro do seu locatário. Você pode controlar quem pode usar um aplicativo, a quais recursos o aplicativo tem acesso, como a adição de credenciais de senha, o cancelamento de certificados de expiração e o gerenciamento de permissões delegadas e atribuições de função de aplicativo.
- GA da API [appRoleAssignment](/graph/api/resources/appRoleAssignment?view=graph-rest-1.0) , que registra a atribuição de um [appRole](/graph/api/resources/approle?view=graph-rest-1.0) (representando a `roles` declaração em tokens de ID e tokens de acesso) a um [usuário](/graph/api/resources/user?view=graph-rest-1.0), [grupo](/graph/api/resources/group?view=graph-rest-1.0)ou [servicePrincipalName](/graph/api/resources/serviceprincipal?view=graph-rest-1.0).
- Use o Facebook como um provedor de identidade no Azure Active Directory.
- Use a permissão delegada ou de aplicativo `AppRoleAssignment.ReadWrite.All` para permitir que um aplicativo gerencie as autorizações de permissões de aplicativo para qualquer API (incluindo o Microsoft Graph) e atribuições de aplicativo para qualquer aplicativo, respectivamente com ou sem o usuário conectado.


### <a name="microsoft-graph-sdks"></a>SDKs do Microsoft Graph
Veja novas orientações sobre o SDK no seguinte:
- [Paginação](/graph/sdks/paging)
- [Envio em lote](/graph/sdks/batch-requests)
- [Carregar arquivos grandes no OneDrive](/graph/sdks/large-file-upload)
- [Personalizando o cliente do serviço SDK por meio de componentes middleware de http](/graph/sdks/customize-client).

### <a name="teamwork"></a>Teamwork
- Se seu cenário envolve reuniões online no Teams, consulte novas orientações sobre [como escolher](choose-online-meeting-api.md) entre a API de [calendário](outlook-calendar-online-meetings.md) e a API de [comunicações em nuvem](cloud-communications-online-meetings.md) para criar e participar de reuniões online.
- [Enviar](/graph/api/channel-post-messages?view=graph-rest-1.0) e [responder](/graph/api/channel-post-messagereply?view=graph-rest-1.0) a mensagens em um [canal](/graph/api/resources/channel?view=graph-rest-1.0).
- Obter o local do OneDrive for Business dos arquivos de um [canal](/graph/api/resources/channel?view=graph-rest-1.0), usando a propriedade de navegação **fileFolder** .

### <a name="teamwork--shifts"></a>Trabalho em equipe | Turnos
GA da [API de turnos](/graph/api/resources/shift?view=graph-rest-1.0) no v 1.0 – Use esta API em aplicativos de produção para criar, atualizar e gerenciar agendas de funcionários de primeiro lugar, para permitir que eles permaneçam em contato e colabore de forma eficaz.

### <a name="users"></a>Usuários
- Assine as notificações de alteração para recursos do [usuário](/graph/api/resources/user) no Microsoft Cloud China operado pela 21vianet.
- Acompanhar o status e a data/hora da última alteração de status de um usuário externo, que foi [convidado](/graph/api/invitation-post?view=graph-rest-1.0) a participar da organização, usando as propriedades **externalUserState** e **externalUserStateChangeDateTime** do recurso do **usuário** .

## <a name="may-2020-new-in-preview-only"></a>Maio de 2020: novo na visualização

### <a name="change-notifications"></a>Notificações de alteração
- Use os tipos formalmente esquematizado [changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta) e [changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta) para processar notificações de alteração de recurso. 
- Rastrear se as notificações estiverem em sequência ou se uma notificação estiver ausente usando a propriedade **sequenceNumber** no recurso **changeNotification** .

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- Os recursos de [impressora](/graph/api/resources/printer?view=graph-rest-beta) e [printerShare](/graph/api/resources/printershare?view=graph-rest-beta) agora estão em paridade e têm as mesmas propriedades de cada um.
- Algumas propriedades e tipos de nomes limpeza ao redor de compartilhamentos de impressora:
  - Use a propriedade de navegação **compartilhada** de [Print](/graph/api/resources/print?view=graph-rest-beta) para obter a lista de compartilhamentos de impressora registrados no locatário. 
  - Confira os detalhes no Changelog de [maio](changelog.md#may-2020) .

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
O Intune [pode](changelog.md#may-2020) atualizar na versão beta.

### <a name="groups"></a>Grupos
- [Avaliar](/graph/api/group-evaluatedynamicmembership?view=graph-rest-beta) se um usuário ou dispositivo é ou se seria um membro de um grupo dinâmico, usando a regra existente para o [grupo](/graph/api/resources/group?view=graph-rest-beta) ou uma regra especificada. [A associação dinâmica baseada em regra reduz a](/azure/active-directory/users-groups-roles/groups-dynamic-membership) sobrecarga administrativa de adição e remoção de membros.
- Ao criar um [grupo](/graph/api/resources/group?view=graph-rest-beta)do Office 365, configure os comportamentos do grupo especificando-os na propriedade **resourceBehaviorOptions** . Por exemplo, permitir que os Membros publiquem, assinar novos membros para conversa, desabilitar o email de boas-vindas e ocultar o grupo nas experiências do Outlook.
- Especifique os recursos a serem provisionados na propriedade **resourceProvisioningOptions** que normalmente não fazem parte da criação de [grupo](/graph/api/resources/group?view=graph-rest-beta) padrão. Atualmente, há suporte para o provisionamento de um grupo como uma [equipe](/graph/api/resources/team?view=graph-rest-beta) com recursos do Microsoft Teams.

### <a name="identity-and-access"></a>Identidade e acesso
- Aplicar as opções de consulta do sistema OData ( `$count` , `$filter` , `$search` ) ao obter coleções de entidades derivadas de [directoryobject](). Você pode [procurar tokens específicos](/graph/query-parameters?#using-search-on-directory-object-collections) nas propriedades **DisplayName** e **Description** dessas entidades e usar a conversão OData para aparar resultados de **directoryobject** para determinados tipos derivados. Veja mais detalhes em [criar consultas avançadas no Microsoft Graph com $Count, $Filter, $Search e $OrderBy](https://developer.microsoft.com/en-us/graph/blogs/build-advanced-queries-with-count-filter-search-and-orderby/).
- Como parte da [API de proteção de identidade](/graph/api/resources/identityprotection-root?view=graph-rest-beta), use a propriedade **riskEventType** para [obter o tipo de risco detectado](/graph/api/riskdetection-get?view=graph-rest-beta)ou [obter o tipo de risco no histórico de um usuário](/graph/api/riskyuser-list-history?view=graph-rest-beta). Não use a propriedade **risktype** , pois ela foi preterida.
- Especifique os tipos de aplicativo cliente na propriedade **clientAppTypes** do [conjunto de condições](/graph/api/resources/conditionalaccessconditionset?view=graph-rest-beta) para uma [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta).
- Use a permissão delegada de `EntitlementManagement.Read.All` para permitir que um aplicativo Leia pacotes de acesso e recursos de gerenciamento de qualificação relacionados em nome do usuário conectado.
- Usar as permissões delegadas ou de aplicativo `Application.Read.All` do `Application.ReadWrite.All` e [listar aplicativos](/graph/api/application-list?view=graph-rest-beta) em uma organização.
- Controlar as configurações de autorização no Azure AD usando o tipo de recurso [authorizationPolicy](/graph/api/resources/authorizationpolicy?view=graph-rest-beta) .

### <a name="teamwork"></a>Teamwork
- Os aplicativos do teams que [oferecem suporte a logon único (SSO)](/microsoftteams/platform/tabs/how-to/authentication/auth-aad-sso) podem especificar o `WebApplicationInfo.id` do manifesto do aplicativo do Teams, na propriedade **azureADAppId** do [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta).
- Use [permissões refinadas](/graph/permissions-reference#teams-resource-specific-consent-permissions) mais finas para acessar recursos de [canal](/graph/api/resources/channel?view=graph-rest-beta) e [equipe](/graph/api/resources/team?view=graph-rest-beta) .




## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de visualização **_prévia_**. As atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de**_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Office 365](https://developer.microsoft.com/office/dev-program), obtenha uma assinatura gratuita do Office 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).

