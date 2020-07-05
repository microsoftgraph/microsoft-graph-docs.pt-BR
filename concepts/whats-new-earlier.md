---
title: Destaques de versões anteriores no Microsoft Graph
description: O que havia de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: f9d62486ba64e0ee597872276f1f62f869d8a632
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038636"
---
# <a name="highlights-of-earlier-releases"></a>Destaques de versões anteriores

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

### <a name="teamwork"></a>Trabalho em equipe
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
- Ao criar um [grupo](/graph/api/resources/group?view=graph-rest-beta)do Microsoft 365, configure os comportamentos do grupo especificando-os na propriedade **resourceBehaviorOptions** . Por exemplo, permitir que os Membros publiquem, assinar novos membros para conversa, desabilitar o email de boas-vindas e ocultar o grupo nas experiências do Outlook.
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


## <a name="april-2020-new-and-generally-available"></a>Abril de 2020: novo e geralmente disponível.

### <a name="calendar"></a>Calendário
- [Compartilhar ou delegar calendários](outlook-share-or-delegate-calendar.md) de forma programática, com uma maior paridade com a experiência do usuário do Outlook. Além de controlar as permissões do usuário atual e o status de compartilhamento de um calendário:
  - Para cada [calendário](/graph/api/resources/calendar?view=graph-rest-1.0), você pode gerenciar as [permissões](/graph/api/resources/calendarpermission?view=graph-rest-1.0) de cada usuário com o qual o calendário é compartilhado. 
  - Para cada [caixa de correio](/graph/api/resources/mailboxsettings?view=graph-rest-1.0), você pode especificar se um representante, proprietário de caixa de correio ou ambos receberão mensagens da reunião e respostas da reunião. 
- [Criar ou atualizar um evento como uma reunião online](outlook-calendar-online-meetings.md):
  - Para cada **calendário**, especifique os provedores de reuniões online permitidos e padrão.
  - Crie ou atualize um [evento](/graph/api/resources/event?view=graph-rest-1.0) que esteja disponível online e forneça detalhes para que os participantes possam ingressar na reunião online. 
  - Em particular, use as novas propriedades **onlineMeetingProvider** e **onlineMeeting** do **evento** para definir ou identificar o Microsoft Teams como um provedor de reuniões online, uma solução alternativa para um [problema conhecido](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams) com a propriedade **onlineMeetingUrl**.
- Adicione [anexos de arquivo de até 150 MB](outlook-large-attachments.md) a um [evento](/graph/api/resources/event?view=graph-rest-1.0).

### <a name="files"></a>Arquivos
- [Check-out](/graph/api/driveitem-checkout?view=graph-rest-1.0) ou [check-in](/graph/api/driveitem-checkin?view=graph-rest-1.0) de um arquivo para o OneDrive para gerenciar a atualização do arquivo e disponibilizar atualizações para outras pessoas quando as atualizações estiverem prontas.
- Aplicar a senha opcional e a data/hora de vencimento como parâmetros das ações de link de [convite](/graph/api/driveitem-invite?view=graph-rest-1.0) e [criação de compartilhamento](/graph/api/driveitem-createlink?view=graph-rest-1.0) para compartilhar um [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0).
- Obter ou definir a senha e a data/hora de validade de uma [permissão](/graph/api/resources/permission?view=graph-rest-1.0)e controlar o [identityset](/graph/api/resources/identityset?view=graph-rest-1.0) de usuários concedidos à permissão para compartilhar um **driveItem**.
- Obter a [permissão](/graph/api/resources/permission?view=graph-rest-1.0) de um [item de unidade compartilhada](/graph/api/resources/shareddriveitem?view=graph-rest-1.0) usando a propriedade de navegação **Permission** .
- Limitar os usuários com um [link de compartilhamento](/graph/api/resources/sharinglink?view=graph-rest-1.0) somente para o modo de exibição e não podem baixar o conteúdo de um**DriveItem** compartilhado no onedrive for Business ou no SharePoint.

### <a name="identity-and-access"></a>Identidade e acesso
- Para gerenciar funções e atribuir acesso a recursos nos provedores de controle de acesso baseado em função (RBAC), como o Microsoft Intune, use [unifiedRoleAssignmentMultiple](/graph/api/resources/unifiedroleassignmentmultiple?view=graph-rest-1.0). O recurso **unifiedRoleAssignmentMultiple** permite definir uma única função em uma matriz de escopos e atribuir a função a várias entidades (como usuários).
- Acessar tipos específicos de [políticas de uma organização](/graph/api/resources/policy-overview?view=graph-rest-1.0) usando o `/policies`segmento URL e especificando o tipo de política. Por exemplo, uma organização pode forçar uma política a entrar automaticamente no usuário de uma sessão da Web após um período de inatividade, confira as operações CRUD para instâncias de [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-1.0). Essa é um [alteração significativa](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-1.0/) para que seja mais fácil descobrir todas as políticas, agrupando todas as políticas digitadas sob o `/policies`segmento. Acesse outras políticas digitadas de uma abordagem semelhante: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-1.0), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-1.0), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-1.0)e [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-1.0). 

### <a name="mail"></a>Correio
Adicione [anexos de arquivo de até 150 MB](outlook-large-attachments.md) a uma [mensagem](/graph/api/resources/message?view=graph-rest-1.0).

### <a name="sites-and-lists"></a>Sites e listas
- [Faça uma lista de sites](/graph/api/sites-list-followed?view=graph-rest-1.0) que o usuário conectado seguiu.
- Identificar a região geográfica de um [conjunto de sites](/graph/api/resources/sitecollection?view=graph-rest-1.0) usando a propriedade **dataLocationCode** .
- Identifique o locatário de um arquivo, pasta ou outro item no SharePoint acessando a propriedade **tenantid** que é parte do **SharepointIds** de um [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0).

## <a name="april-2020-new-in-preview-only"></a>Abril de 2020: novo somente para visualização

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem

Designar usuários e grupos permitidos para usar compartilhamentos de impressoras [específicos](/graph/api/resources/printershare?view=graph-rest-beta) em impressão universal, a infraestrutura de impressão baseada na nuvem do Microsoft 365. Para experimentar recursos de gerenciamento de impressão eficientes e centralizados, assim como oferecer uma experiência de impressão simples, porém rica e segura para os usuários de impressão, consulte o [Anúncio de impressão universal](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/announcing-universal-print-a-cloud-based-print-solution/ba-p/1204775) e participe do programa de visualização.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações de [abril](changelog.md#april-2020) do Intune.

### <a name="groups"></a>Grupos
Identifique o aplicativo que criou um [grupo](/graph/api/resources/group?view=graph-rest-beta) pela sua ID do aplicativo.

### <a name="identity-and-access"></a>Identidade e acesso
- [Controlar alterações](/graph/api/administrativeunit-delta?view=graph-rest-beta) para [unidades administrativas](/graph/api/resources/administrativeunit?view=graph-rest-beta).
- [Controlar alterações](/graph/api/oauth2permissiongrant-delta?view=graph-rest-beta) para [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant?view=graph-rest-beta).
- [Gerenciar](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta) os [métodos de autenticação](/graph/api/resources/authenticationmethod?view=graph-rest-beta) de um usuário que incluem a [senha](/graph/api/resources/passwordauthenticationmethod?view=graph-rest-beta) ou [telefone](/graph/api/resources/phoneauthenticationmethod?view=graph-rest-beta). Por exemplo, [redefinir uma senha de usuário](/graph/api/passwordauthenticationmethod-resetpassword?view=graph-rest-beta), [obter o status da redefinição](/graph/api/authenticationoperation-get?view=graph-rest-beta) ou [adicionar um número de telefone](/graph/api/authentication-post-phonemethods?view=graph-rest-beta) para um usuário para autenticação de SMS ou chamada de voz, se a política estiver habilitada para o usuário.

### <a name="reports--identity-and-access-reports"></a>Relatórios | Relatórios de identidade e acesso
[Listar](/graph/api/relyingpartydetailedsummary-list?view=graph-rest-beta) [participantes confiáveis](https://docs.microsoft.com/windows-server/identity/ad-fs/technical-reference/understanding-key-ad-fs-concepts) configurados nos Serviços de Federação do Active Directory.

### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
Exibir dados de **Reunião Criada** e de **Reunião Interagida** nos relatórios CSV para [contagens de atividades de email](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta), [contagens de atividades de email do usuário](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta) e [detalhes de atividades de email do usuário](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta).


## <a name="march-2020-new-and-generally-available"></a>Março de 2020: Novo e disponível para o público geral

### <a name="cloud-communications"></a>Comunicações na nuvem
- Obtenha o roteamento de chamadas e o contexto de entrada de um [chamada](/graph/api/resources/call?view=graph-rest-1.0).
- Um aplicativo pode [Atualizar o status da gravação](/graph/api/call-updaterecordingstatus?view=graph-rest-1.0) de uma chamada.
- Gravar as informações especificamente para um [participante](/graph/api/resources/participant?view=graph-rest-1.0), incluindo o iniciador e o status da gravação.
- Identifique de forma exclusiva os participantes de uma conferência ou [chamada](/graph/api/resources/call?view=graph-rest-1.0) de participante a participante usando a propriedade **callChainId**.
- Identifique como parte do [participantInfo](/graph/api/resources/participantinfo?view=graph-rest-1.0) o código do país e o tipo de ponto de extremidade (como o Skype for Business ou o Skype for Business VOIP) do participante.
- Os parceiros de dispositivos de VTC (teleconferência por vídeo de terceiros) podem registrar e fornecer dados de qualidade de mídia para dispositivos de teleconferência por vídeo através de um bot de CVI (Interoperabilidade de vídeo em nuvem) e usando a função [logTeleconferenceDeviceQuality](/graph/api/call-logteleconferencedevicequality?view=graph-rest-1.0). A qualidade da mídia inclui dados do tipo aberto para [áudio](/graph/api/resources/teleconferencedeviceaudioquality?view=graph-rest-1.0), [vídeo](/graph/api/resources/teleconferencedevicevideoquality?view=graph-rest-1.0) e [compartilhamento de tela](/graph/api/resources/teleconferencedevicescreensharingquality?view=graph-rest-1.0).

### <a name="files"></a>Arquivos
- [Os itens remotos](/graph/api/resources/remoteitem?view=graph-rest-1.0) compartilhados com um usuário, adicionados ao OneDrive do usuário, ou retornados como resultado de pesquisa podem conter metadados para uma imagem ou um vídeo.
- [Siga](/graph/api/driveitem-follow?view=graph-rest-1.0) um [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) para obter um acesso conveniente ou para facilitar ações como mover, copiar e salvar como. Use [deixar de serguir](/graph/api/driveitem-unfollow?view=graph-rest-1.0) para deixar de seguir o item da unidade.
- [Conceda](/graph/api/permission-grant?view=graph-rest-1.0) permissões aos usuários para acessarem um link de compartilhamento para compartilhar o item da unidade correspondente.

### <a name="identity-and-access"></a>Identidade e acesso
- [Controle de alterações](/graph/api/orgcontact-delta?view=graph-rest-1.0) para [contatos organizacionais](/graph/api/resources/orgcontact?view=graph-rest-1.0).
- Use a propriedade **riskEventTypes_v2** para obter os tipos de eventos de risco associados a [entrada](/graph/api/resources/signin?view=graph-rest-1.0).
- Use a permissão delegada `User.ManageIdentities.All` para permitir que um aplicativo leia, atualize ou exclua identidades associadas à conta de um usuário, às quais o usuário conectado tem acesso. Use essa permissão no nível do aplicativo sem um usuário conectado. Isso permite ao aplicativo [gerenciar](/graph/api/user-update?view=graph-rest-1.0) com quais identidades um usuário pode se inscrever.

### <a name="reports"></a>Relatórios
Use o administrador de serviços do Teams e o administrador de comunicações do teams como funções de usuário aceitas para permitir que os aplicativos leiam os relatórios de uso do serviço Microsoft 365 em nome de um usuário, como [formas de autorização delegada pelo usuário](reportroot-authorization.md). 

### <a name="sites"></a>Sites
- Permitir que os usuários [sigam](/graph/api/site-follow?view=graph-rest-1.0) ou [parem de seguir](/graph/api/site-unfollow?view=graph-rest-1.0) os sites do SharePoint.
- [Inscreva-se para alterar as notificações](/graph/api/resources/subscription?view=graph-rest-1.0) para uma lista  [do SharePoint](/graph/api/resources/list?view=graph-rest-1.0).

## <a name="march-2020-new-in-preview-only"></a>Março de 2020: novo somente para visualização

### <a name="calendar"></a>Calendário
- Use a propriedade **calendarGroupId** para obter o [grupo de calendário](/graph/api/resources/calendargroup?view=graph-rest-beta) em que um [calendário](/graph/api/resources/calendar?view=graph-rest-beta) foi criado.
- Use a propriedade **isDraft** para identificar um [evento](/graph/api/resources/event?view=graph-rest-beta) como uma reunião que o usuário atualizou no Outlook, mas não enviou para atualizar os participantes.

### <a name="cloud-communications"></a>Comunicações na nuvem
- Use [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-beta) para obter uma instância de [reunião online](/graph/api/resources/onlinemeeting?view=graph-rest-beta) por um ID externo personalizado e criar uma quando não houver nenhuma.
- Você tem a opção de usar a propriedade **externalId** para identificar uma reunião online com a ID externa personalizada.
- Use o `Accept-Language` cabeçalho opcional da solicitação HTTP para [criar](/graph/api/application-post-onlinemeetings?view=graph-rest-beta) ou [obter](/graph/api/onlinemeeting-get?view=graph-rest-beta) uma instância da reunião online, para que a operação bem-sucedida exiba o conteúdo da propriedade **joinInformation** no idioma especificado e variante de localidade.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [março](changelog.md#march-2020) do Intune

### <a name="identity-and-access"></a>Identidade e acesso
- Use a permissão `Auditlogs.Read.All` para listar a [atividade de entrada](/graph/api/resources/signinactivity?view=graph-rest-beta) de um [usuário](/graph/api/resources/user?view=graph-rest-beta).
- Use a `PrivilegedAccess.Read.AzureResources` permissão no nível do aplicativo para [PIM (gerenciamento de identidades privilegiadas) dos recursos do Azure](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta), para configurar o fluxo de trabalho de acesso just-in-time para funções de infraestrutura do Azure em um grupo de gerenciamento, assinatura, grupo de recursos ou nível de recurso.
- Use a entidade [identitySecurityDefaultsEnforcementPolicy](/graph/api/resources/identitysecuritydefaultsenforcementpolicy?view=graph-rest-beta) para [obter](/graph/api/identitysecuritydefaultsenforcementpolicy-get?view=graph-rest-beta) ou [atualizar](/graph/api/identitysecuritydefaultsenforcementpolicy-update?view=graph-rest-beta) as configurações de segurança padrão pré-definidas que protegem as organizações contra ataques comuns.
- Use um segmento `identity` ao chamar APIs de acesso condicional. Por exemplo, para [obter](/graph/api/conditionalaccesspolicy-get?view=graph-rest-beta) ou uma [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta): `GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}`.
- Use a propriedade **authenticationRequirement** para obter o nível mais alto de autenticação necessária por meio de todas as etapas de entrada para que a [entrada](/graph/api/resources/signin?view=graph-rest-beta) seja bem-sucedida.
- Use a paginação quando [listar eventos de provisionamento](/graph/api/provisioningobjectsummary-list?view=graph-rest-beta) ocorridos no locatário.

### <a name="search"></a>Pesquisa
- Para adicionar dados em um arquivo para pesquisar resultados, indexe os dados como um [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta). O tipo **externalFile** foi substituído.
- Agora é possível [atualizar](/graph/api/externalitem-update?view=graph-rest-beta) um [item no índice](/graph/api/resources/externalitem?view=graph-rest-beta), atualizando especificamente a representação de texto simples do item (representado pela propriedade **conteúdo**), ou o conjunto de propriedades do item (representado pela propriedade **propriedades**). A atualização de qualquer propriedade no conjunto de propriedades substitui todo conjunto de propriedades, por isso certifique-se de incluir explicitamente todas as propriedades do item na atualização.
- Verifique o `HTTP 429` e o cabeçalho de resposta `Retry-After` depois de chamar a operação para [criar](/graph/api/externalconnection-put-items?view=graph-rest-beta), [atualizar](/graph/api/externalitem-update?view=graph-rest-beta) ou [excluir](/graph/api/externalitem-delete?view=graph-rest-beta) de **externalItem**. Desativar solicitações usando o atraso `Retry-After` é a forma mais rápida de se recuperar da [limitação](throttling.md#best-practices-to-handle-throttling).

### <a name="teamwork"></a>Trabalho em equipe
Use a `ChannelMessage.Read.All` permissão no nível do aplicativo para ler [instâncias de](/graph/api/resources/chatmessage?view=graph-rest-beta)chatMessage em canais sem um usuário conectado.

### <a name="universal-print"></a>Impressão universal
Estréia da [API de impressão universal](universal-print-concept-overview.md), que permite que os usuários imprimam na Web ou de um aplicativo. A API permite que os administradores de TI gerenciem o acesso de usuários e grupos a impressoras na nuvem do Microsoft 365, compartilhamento remoto da impressora para manter a disponibilidade, monitorar o status da impressora e emitir relatórios sobre trabalho de impressão arquivado e uso. 

Observe que a partir de março de 2020, o serviço de _impressão universal_ está na visualização particular. Confira [anunciando a impressão universal: uma solução de impressão baseada na nuvem](https://aka.ms/announcinguniversalprint) para obter informações sobre a participação.


## <a name="february-2020-new-and-generally-available"></a>Fevereiro de 2020: novo e disponível para o público geral

### <a name="calendar"></a>Calendário
Vamos examinar um exemplo de [criação de um evento em um calendário compartilhado ou delegado](outlook-create-event-in-shared-delegated-calendar.md), além das ações e propriedades disponíveis para o representante, os convidados e o proprietário do calendário durante esse processo.

### <a name="identity-and-access"></a>Identidade e acesso
- Para aumentar a segurança ao assinar as [notificações de alteração dos dados do usuário](webhooks.md), [impor o Protocolo TLS 1.2](https://docs.microsoft.com/configmgr/core/plan-design/security/enable-tls-1-2) ou mais recente em clientes e servidores de sites usados no processo de notificação. O novo requisito será lançado em estágios a partir de 15 de fevereiro de 2020. A partir de 15 de maio de 2020, todos os pontos de extremidade de notificação devem atendem ao novo requisito de TLS. [Descubra os estágios do lançamento](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) e, se necessário, use a nova propriedade **latestSupportedTlsVersion** como uma solução alternativa temporária para evitar falhas de assinatura antes de concluir a atualização de TLS.
- Use os respectivos tipos de [solicitação de avaliação de ameaças](/graph/api/resources/threatAssessmentRequest?view=graph-rest-1.0) para controlar as ameaças de [email](/graph/api/resources/mailassessmentrequest?view=graph-rest-1.0), um [arquivo de mensagem de email](/graph/api/resources/emailfileassessmentrequest?view=graph-rest-1.0) (arquivo .EML), [arquivo de anexo de email](/graph/api/resources/fileassessmentrequest?view=graph-rest-1.0) (texto, Word ou arquivo binário) ou [URL](/graph/api/resources/urlassessmentrequest?view=graph-rest-1.0).

### <a name="users"></a>Usuários
[Reprocessar](/graph/api/user-reprocesslicenseassignment?view=graph-rest-1.0) todas as atribuições de licença baseadas em grupo para um [usuário](/graph/api/resources/user?view=graph-rest-1.0).


## <a name="february-2020-new-in-preview-only"></a>Fevereiro de 2020: nova somente para visualização

### <a name="calendar"></a>Calendário
Confira [tarefas com suporte por APIs de visualização que gerenciam o compartilhamento de calendários e a delegação](outlook-share-or-delegate-calendar.md).

### <a name="cloud-communications"></a>Comunicações na nuvem

- Use o novo recurso [registros de chamadas](/graph/api/resources/callrecord?view=graph-rest-beta) para obter metadados de chamadas e reuniões online do Microsoft Teams e do Skype for Business para uma organização.
- Para um participante de uma reunião, use a propriedade **Iniciador** para obter as informações de identidade do iniciador de uma [gravação](/graph/api/resources/recordinginfo?view=graph-rest-beta), se houver uma.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [fevereiro](changelog.md#february-2020) do Intune.

### <a name="groups"></a>Grupos
Use o método [assignLicense](/graph/api/group-assignlicense?view=graph-rest-beta) para atribuir licenças para produtos, como o Microsoft 365 ou o Enterprise Mobility + Security, a um grupo. Como o Azure AD garante que as licenças sejam designadas para os membros do grupo, os membros que ingressarem ou saírem de um grupo não precisarão mais de gerenciamento de licenças no nível individual.

### <a name="identity-and-access"></a>Identidade e acesso
- Defina as configurações de solicitação, aprovação e revisar ao criar uma [política de atribuição de pacote](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta).
- Acessar tipos específicos de [políticas de uma organização](/graph/api/resources/policy-overview?view=graph-rest-beta) usando o `/policies`segmento URL e especificando o tipo de política. Por exemplo, uma organização pode forçar uma política a entrar automaticamente no usuário de uma sessão da Web após um período de inatividade, confira as operações CRUD para instâncias de [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-beta). Essa é um [alteração significativa](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/) para que seja mais fácil descobrir todas as políticas, agrupando todas as políticas digitadas sob o `/policies`segmento. Acesse outras políticas digitadas de uma abordagem semelhante: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-beta), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta)e [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-beta). 
- Use a permissão de nível de aplicativo e `Policy.ReadWrite.ApplicationConfiguration` delegada para operações de leitura e gravação na configuração do aplicativo [políticas](/graph/api/resources/policy-overview?view=graph-rest-beta) mencionadas no item anterior.

### <a name="teamwork"></a>Trabalho em equipe
- Use [alterar as notificações](/graph/api/resources/webhooks?view=graph-rest-beta) em todas as mensagens do canal ou em todas as mensagens de chat em uma organização.
- [Recuse](/graph/api/swapshiftschangerequest-decline?view=graph-rest-beta) uma [solicitação de troca de turnos](/graph/api/resources/swapshiftschangerequest?view=graph-rest-beta) com outro usuário em uma [equipe](/graph/api/resources/team?view=graph-rest-beta).

## <a name="january-2020-new-and-generally-available"></a>Janeiro de 2020: Novo e disponível para o público geral

### <a name="security"></a>Segurança
Como parte do gerenciamento de alerta de cliente, use o método de [alerta de atualização](/graph/api/alert-update?view=graph-rest-1.0) e atualize o campo **comentários** como `Closed in IPC` ou `Closed in MCAS`.

### <a name="teamwork"></a>Teamwork
Use a propriedade de navegação **primaryChannel** de uma [equipe](/graph/api/resources/team?view=graph-rest-1.0) para acessar o canal padrão, **Geral**.

### <a name="users"></a>Usuários
Use a propriedade **identities** para acessar uma ou mais identidades que um [usuário](/graph/api/resources/user?view=graph-rest-1.0) pode usar para entrar em uma conta de usuário do Azure AD. As identidades podem ser fornecidas pela Microsoft, por organizações ou por provedores de identidade social, como Facebook, Google ou Microsoft. Essa propriedade permite que o usuário entre na conta de usuário com uma dessas identidades.

## <a name="january-2020-new-in-preview"></a>Janeiro de 2020: novidades na versão prévia

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [janeiro](changelog.md#january-2020) do Intune.


## <a name="december-2019-new-and-generally-available"></a>Dezembro de 2019: Novo e disponível para o público geral

### <a name="cloud-communications"></a>Comunicações na nuvem
A API de comunicações na nuvem tem o GA'd e as APIs para [chamada](/graph/api/resources/call?view=graph-rest-1.0) e [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-1.0) estão [disponíveis na v1.0](/graph/api/resources/communications-api-overview?view=graph-rest-1.0).

### <a name="education"></a>Educação
Use a propriedade **classSettings** para gerenciar configurações específicas de classe, como habilitar o envio de resumos de atribuições semanais. Esta propriedade está disponível no recurso [equipe](/graph/api/resources/team?view=graph-rest-1.0) quando a equipe representa uma [classe educacional](/graph/api/resources/educationclass?view=graph-rest-1.0).

### <a name="identity-and-access"></a>Identidade e acesso 
[Tentar obter objetos de contêiner com permissões limitadas retorna dados parciais](permissions-reference.md#limited-information-returned-for-inaccessible-member-objects). Um exemplo é uma instância de [grupo](/graph/api/resources/group?view=graph-rest-1.0) associada a um [usuário](/graph/api/resources/user?view=graph-rest-1.0), outro **grupo** e um [dispositivo](/graph/api/resources/device?view=graph-rest-1.0). Um aplicativo que tem somente as permissões User.Read.All e Group.Read.All e tentar acessar essa instância de **grupo** obteria os objetos de **usuário** e **grupo**, mas dados limitados para o objeto de **dispositivo** (apenas o tipo de dados e a ID do objeto e não os valores da propriedade).

### <a name="people-and-workplace-intelligence"></a>Inteligência de pessoas e local de trabalho
A API do insights tem GA'd. Use a API em aplicativos de produção para identificar os documentos mais relevantes, que são:

- [Tendências de](/graph/api/insights-list-trending?view=graph-rest-1.0) um usuário
- [Usado por](/graph/api/insights-list-used?view=graph-rest-1.0) um usuário
- [Compartilhados com ou por](/graph/api/insights-list-shared?view=graph-rest-1.0) um usuário

### <a name="reports"></a>Relatórios
Para obter os relatórios de uso do Microsoft 365 usando permissões delegadas por um usuário, os administradores devem ter atribuído ao usuário uma função de administrador limitada do Azure AD. Podendo ser uma das seguintes funções: administrador da empresa, administrador do Exchange, administrador do SharePoint, administrador do Lync, leitor global ou leitor de relatórios. Consulte [Authorization for APIs para ler os relatórios de uso do Microsoft 365](reportroot-authorization.md) para obter detalhes.

### <a name="toolkit"></a>Kit de ferramentas
O Microsoft Graph Toolkit v1.1 foi lançado. Para obter uma lista de aperfeiçoamentos e correções de bugs, confira a [seção de dezembro de 2019](changelog.md#december-2019) do log de alterações.

## <a name="december-2019-new-in-preview"></a>Dezembro de 2019: novidades na versão prévia

### <a name="cloud-communications"></a>Comunicações na nuvem
- Use o novo recurso [presença](/graph/api/resources/presence?view=graph-rest-beta) para obter informações sobre a disponibilidade e a atividade atual de um ou mais usuários.
- [Exclua](/graph/api/onlinemeeting-delete?view=graph-rest-beta) uma instância de um [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta).
- Confira a [seção de dezembro de 2019](changelog.md#december-2019) do log de alterações para a renomeação e a remoção de alguns membros dos recursos da [chamada](/graph/api/resources/call?view=graph-rest-beta) e do [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta), para estar na paridade com a versão v1 desses recursos.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [Dezembro](changelog.md#december-2019) do Intune

### <a name="identity-and-access"></a>Identidade e acesso 
- Correção de comportamento nos relacionamentos **appRoleAssignments** e **appRoleAssignedTo** em [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta).
- Use [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta) em [gerenciamento de direitos do Azure AD](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta) para solicitar a adição de um recurso a um [catálogo](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta), para que as funções desse recurso possam ser usadas em um [pacote de acesso](/graph/api/resources/accesspackage?view=graph-rest-beta).
- Use a [API de avaliação de ameaças](/graph/api/resources/threatassessment-api-overview?view=graph-rest-beta) para capacitar os administradores a relatar emails suspeitos, URLs de phishing, anexos de email ou outros arquivos. O veredicto de varredura de thread pode então informá-los a ajustar a política organizacional adequadamente.

### <a name="teamwork"></a>Teamwork
- [Configure as notificações que incluem dados de recursos](webhooks-with-resource-data.md) para recursos do [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) nos canais e bate-papos do Microsoft Teams.
- [Assine as notificações](/graph/api/resources/subscription?view=graph-rest-beta) de [mensagens de canal ou de bate-papo](/graph/api/resources/chatmessage?view=graph-rest-beta) novas ou modificadas.
- Use o recurso [shiftPreferences](/graph/api/resources/shiftpreferences?view=graph-rest-beta) para permitir que a especificação da disponibilidade de um usuário seja atribuída a turnos em um [cronograma](/graph/api/resources/schedule?view=graph-rest-beta). Obtenha ou defina isso como parte das [configurações](/graph/api/resources/usersettings?view=graph-rest-beta) do usuário.


## <a name="november-2019-new-and-generally-available"></a>Novembro de 2019: novo e disponível para o público geral

### <a name="groups"></a>Grupos
- Use permissões delegadas ou de aplicativo, GroupMember.Read.All e GroupMember.ReadWrite.All, para listar grupos, leia as propriedades básicas do grupo, leia (e atualize a permissão de leitura/gravação) a associação dos grupos aos quais o aplicativo tem acesso.
- Use a permissão do aplicativo, Group.Create, para criar grupos sem um usuário conectado.
- Para um [grupo](/graph/api/resources/group?view=graph-rest-1.0) especificado, [verifique a associação](/graph/api/group-checkmemberobjects?view=graph-rest-1.0) em outros grupos ou funções de diretório.

### <a name="identity-and-access"></a>Identidade e acesso
- Registre [aplicativos](/graph/api/resources/application?view=graph-rest-1.0) que se autenticam com o Azure Active Directory (Azure AD). Use as [permissões](/graph/permissions-reference#application-resource-permissions) delegadas, Application.Read.All e Application.ReadWrite.All ou as permissões de aplicativos, Application.Read.All, conforme apropriado.
- Para um [dispositivo](/graph/api/resources/device?view=graph-rest-1.0) especificado, [verifique a associação](/graph/api/device-checkmemberobjects?view=graph-rest-1.0) em outros grupos ou funções de diretório.

### <a name="mail"></a>Correio
- Use a propriedade **conversationIndex** para obter a posição de uma mensagem em uma conversa de email do Outlook.
- Use a permissão delegada, Mail.ReadBasic e a permissão de aplicativo, Mail.ReadBasic.All, para obter os recursos de [mensagem](/graph/api/resources/message?view=graph-rest-1.0) ou de [pasta de email](/graph/api/resources/mailfolder?view=graph-rest-1.0), acompanhar suas alterações e gerenciar [assinaturas](/graph/api/resources/subscription?view=graph-rest-1.0) para notificações de alteração nas mensagens.

### <a name="users"></a>Usuários
- [Verifique se há associações de grupo](/graph/api/user-checkmemberobjects?view=graph-rest-1.0) de um [usuário](/graph/api/resources/user?view=graph-rest-1.0) específico.
- Use a propriedade **creationType** para descobrir como uma conta de usuário foi criada, por exemplo, se a conta foi criada como uma conta corporativa ou de estudante ou como uma conta externa, etc.

## <a name="november-2019-new-in-preview"></a>Novembro de 2019: Novidades na versão prévia

### <a name="calendar"></a>Calendário
- [Use o Outlook para organizar e participar de reuniões online](outlook-calendar-online-meetings.md).
- [Defina as propriedades](/graph/api/place-update?view=graph-rest-beta) para os tipos de local avançado de [sala](/graph/api/resources/room?view=graph-rest-beta) e [lista de sala](/graph/api/resources/roomlist?view=graph-rest-beta).

### <a name="cloud-communication"></a>Comunicação na nuvem
O tipo de recurso de [chamada](/graph/api/resources/call?view=graph-rest-beta) dá suporte aos seguintes recursos adicionais:

- O [contexto de uma chamada de entrada](/graph/api/resources/incomingcontext?view=graph-rest-beta)
- O tipo de ponto de extremidade de um participante, como correio de voz ou Skype for Business
- A capacidade de [atualizar](/graph/api/call-updaterecordingstatus?view=graph-rest-beta) as [informações de registro](/graph/api/resources/recordinginfo?view=graph-rest-beta) de um [participante](/graph/api/resources/participant?view=graph-rest-beta)

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [novembro](changelog.md#november-2019) do Intune

### <a name="education"></a>Educação
Os administradores podem habilitar as configurações de toda a classe por meio da propriedade **classSettings** da [equipe](/graph/api/resources/team?view=graph-rest-beta) associada à [classe](/graph/api/resources/educationclass?view=graph-rest-beta). Atualmente, há uma configuração para notificar os guardiões sobre tarefas semanais.

### <a name="identity-and-access"></a>Identidade e acesso
- Use a permissão do aplicativo, Policy.Read.All, para ler todas as políticas de acesso condicional da sua localização e locais nomeados, sem um usuário conectado.
- Permita que a [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta) esteja em um estado somente de relatório, `enabledForReportingButNotEnforced`.
- Use a permissão delegada, ThreatAssessment.ReadWrite.All, ou a permissão de aplicativo, ThreatAssessment.Read.All, leia (ou crie uma permissão de leitura/gravação) solicitações para avaliar ameaças em uma organização.

### <a name="mail"></a>Email
Use a permissão delegada, Mail.ReadBasic e a permissão de aplicativo, Mail.ReadBasic.All, para gerenciar as [assinaturas](/graph/api/resources/subscription?view=graph-rest-beta) para notificações de alteração no recurso de [mensagem](/graph/api/resources/message?view=graph-rest-beta).

### <a name="notifications"></a>Notificações
Use as novas notificações simples [SDK Web](https://aka.ms/GNSDK) em vez do [SDK do Project Rome](https://github.com/Microsoft/project-rome), para aproveitar um modelo de autenticação aperfeiçoado e suporte a aplicativos da Web usando o push da Web. 

### <a name="people-and-workplace-intelligence"></a>Inteligência de pessoas e no local de trabalho
Estreia do recurso do [perfil](/graph/api/resources/profile?view=graph-rest-beta) que é uma representação avançada da próxima geração de entidades de pessoas nos serviços da Microsoft. Esse recurso se relaciona aos atributos comuns e práticos de pessoas, incluindo informações sobre datas significativas, como [aniversários](/graph/api/resources/personanniversary?view=graph-rest-beta), [escolaridade](/graph/api/resources/educationalactivity?view=graph-rest-beta), [cargos](/graph/api/resources/workposition?view=graph-rest-beta), [interesses](/graph/api/resources/personinterest?view=graph-rest-beta), [idioma](/graph/api/resources/languageproficiency?view=graph-rest-beta) e [habilidades](/graph/api/resources/skillproficiency?view=graph-rest-beta) e competências, [participação em projetos](/graph/api/resources/projectparticipation?view=graph-rest-beta), [associação em sites](/graph/api/resources/personwebsite?view=graph-rest-beta) e outras informações de contato e [conta](/graph/api/resources/useraccountinformation?view=graph-rest-beta).

### <a name="search"></a>Pesquisar
Estreia da [API de Pesquisa da Microsoft](search-concept-overview.md) que permite aos usuários do aplicativo obter os resultados de pesquisa mais atualizados, personalizados e relevantes com a plataforma Microsoft Graph. Use o recurso de [consulta](/graph/api/search-query?view=graph-rest-beta)por padrão, pesquisas mensagens e eventos do Outlook e arquivos do OneDrive e do SharePoint na nuvem da Microsoft. Use os conectores [disponíveis](/microsoftsearch/connectors-overview) na [galeria de conectores do Microsoft Graph](/microsoftsearch/connectors-gallery), para incluir dados de pesquisa fora do Microsoft Cloud. Como alternativa, [construa seus próprios conectores](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), indexe arquivos e itens personalizados externos e consulte fontes de dados externas específicas.

### <a name="teamwork"></a>Trabalho em equipe
Obtenha os recursos de [arquivo](/graph/api/resources/driveitem?view=graph-rest-beta) associados a uma [equipe](/graph/api/resources/team?view=graph-rest-beta) e [canal](/graph/api/resources/channel?view=graph-rest-beta) usando a seguinte sintaxe de solicitação de HTTP:

```http
GET /teams/{teamId}/channels/{channelId}/filesFolder
```

### <a name="users"></a>Usuários
Use a propriedade **creationType** para descobrir como uma conta de usuário foi criada, por exemplo, se a conta foi criada como uma conta corporativa ou de estudante ou como uma conta externa, etc.


## <a name="october-2019-new-and-generally-available"></a>Outubro de 2019: Novo e geralmente disponível

### <a name="identity-and-access"></a>Identidade e acesso
- Use [contatos da organização](/graph/api/resources/orgcontact?view=graph-rest-1.0) em aplicativos de produção. Os contatos da organização são gerenciados por administradores da organização, sincronizados de um Active Directory local ou do Exchange Online.
- Configure a [autenticação baseada em certificado](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started) em uma [organização](/graph/api/resources/organization?view=graph-rest-1.0).
- Adicionar e remover [credenciais de senha](/graph/api/resources/passwordcredential?view=graph-rest-1.0) para [aplicativos](/graph/api/resources/application?view=graph-rest-1.0).

### <a name="mail"></a>Correio
Use o novo parâmetro de **mensagem** para atualizar quaisquer propriedades de [mensagem](/graph/api/resources/message?view=graph-rest-1.0) graváveis ao [responder](/graph/api/message-reply?view=graph-rest-1.0) a uma mensagem, por exemplo, [adicionar um destinatário à resposta](/graph/api/message-reply#example?view=graph-rest-1.0).

### <a name="microsoft-graph-data-connect"></a>Conexão de dados do Microsoft Graph
Os desenvolvedores e os cientistas de dados agora podem usar [ferramentas para traduzir dados do Office 365 para o formato Modelo de Dados Comum](https://github.com/OfficeDev/MS-Graph-Data-Connect/blob/master/Common-Data-Model/README.md), tornando-o esquematicamente consistente com outros conjuntos de dados prontos da Open Data Initiative (ODI). 


### <a name="microsoft-graph-sdks"></a>SDKs do Microsoft Graph
- Use os manipuladores de caos no SDK do JavaScript para verificar se um aplicativo é resistente a falhas de servidor que são difíceis de iniciar.
- Ler sobre [fazer chamadas API usando os SDKs](/graph/sdks/create-requests).

### <a name="users"></a>Usuários
- [Obtenha](/graph/api/user-get-mailboxsettings?view=graph-rest-1.0) ou [defina](/graph/api/user-update-mailboxsettings?view=graph-rest-1.0) as configurações preferenciais de formato de data e hora do usuário [para a caixa de correio do usuário](/graph/api/resources/mailboxsettings?view=graph-rest-1.0). 
- Rastreie a data/hora da última alteração de senha de um [usuário](/graph/api/resources/user?view=graph-rest-1.0).

## <a name="october-2019-new-in-preview"></a>Outubro de 2019: Novo em visualização

### <a name="calendar"></a>Calendário
- Os organizadores de reuniões podem [permitir que os convidados proponham horários de reunião alternativos ](outlook-calendar-meeting-proposals.md). Ao receber uma resposta de reunião que inclua um horário alternativo proposto, o organizador pode decidir aceitar a proposta e [atualizar](/graph/api/event-update?view=graph-rest-beta) o horário da reunião.
- O compartilhamento de calendário programático está mais parecido com a experiência do usuário do Outlook. Além de controlar as permissões do usuário atual e o status de compartilhamento de um calendário:
  - Para cada [calendário](/graph/api/resources/calendar?view=graph-rest-beta), você pode gerenciar as [permissões](/graph/api/resources/calendarpermission?view=graph-rest-beta) de cada usuário com o qual o calendário é compartilhado. 
  - Para cada [caixa de correio](/graph/api/resources/mailboxsettings?view=graph-rest-beta), você pode especificar se um representante, proprietário de caixa de correio ou ambos receberão mensagens da reunião e respostas da reunião. 
- Suporte adicional para reuniões online:
  - Para cada **calendário**, especifique os provedores de reuniões online permitidos e padrão.
  - Crie ou atualize um [evento](/graph/api/resources/event?view=graph-rest-beta) que esteja disponível online e forneça detalhes para que os participantes possam ingressar na reunião online. 
  - Em particular, use as novas propriedades **onlineMeetingProvider** e **onlineMeeting** do **evento** para definir ou identificar o Microsoft Teams como um provedor de reuniões online, uma solução alternativa para um [problema conhecido](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams) com a propriedade **onlineMeetingUrl**.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [outubro](changelog.md#october-2019) do Intune

### <a name="graph-explorer"></a>Graph Explorer
Experimente a [próxima versão do Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/preview) e confira informações contextuais úteis, como permissões, tokens de acesso e trechos de código do SDK nas novas guias **Permissões**, **Autenticação** e **Trechos de código**. Use o controle deslizante **Visualizar** para alternar entre a [produção](https://developer.microsoft.com/graph/graph-explorer) e a nova versão de visualização do Graph Explorer.

### <a name="groups"></a>Grupos
- Use as propriedades **hideFromAddressLists** e **hideFromOutlookClients** para controlar a visibilidade de um [grupo](/graph/api/resources/group?view=graph-rest-beta) em determinadas partes da interface do usuário do Outlook ou em um cliente do Outlook.
- [Atribuir](/graph/api/group-assignlicense?view=graph-rest-beta) ou remover licenças de usuários em um [grupo](/graph/api/resources/group?view=graph-rest-beta).

### <a name="identity-and-access"></a>Identidade e acesso
- Use as [políticas de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta) para personalizar regras de acesso para uma organização. Essas regras consideram sinais sobre uma identidade de um usuário ou dispositivo, como associação a um usuário ou grupo, localização do IP e comportamentos, como tentativas de acesso a aplicativos específicos e comportamentos arriscados de logon.
- Use o [gerenciamento de direitos](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta) para gerenciar o acesso a grupos, aplicativos e sites do SharePoint Online para usuários dentro e fora de uma organização.
- Adicione e remova [credenciais de senha](/graph/api/resources/passwordcredential?view=graph-rest-beta) para [aplicativos](/graph/api/resources/application?view=graph-rest-beta) e [entidades de serviço](/graph/api/resources/serviceprincipal?view=graph-rest-beta).
- Gerenciar a [política de estrutura confiável](/graph/api/resources/trustframeworkkeyset?view=graph-rest-beta) do Azure AD B2C.
- Defina as políticas de [fluxo de usuário](/graph/api/resources/identityuserflow?view=graph-rest-beta) do Azure AD B2C para entrar, inscrever-se, entrar e Inscrever-se combinados, redefinir senha e atualizar perfil.
- Configure [rótulos de proteção de informações](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta) para classificar a confidencialidade de um usuário ou locatário.
- Aplicativos existentes usando as APIs para [eventos de risco de identidade](/graph/api/resources/identityriskevent?view=graph-rest-beta) devem fazer ar transição para [ detecção de risco](/graph/api/resources/riskdetection?view=graph-rest-beta) no Azure AD Identity Protection. Confira a postagem de blog [ postagem de blog](https://developer.microsoft.com/graph/blogs/deprecatation-of-the-identityriskevents-api/) relacionada para obter mais detalhes e cronograma de descontinuação.


### <a name="mail"></a>Email
[Anexe arquivos grandes de até 150MB](outlook-large-attachments.md) a uma instância de [mensagem](/graph/api/resources/message?view=graph-rest-beta), criando uma [sessão de upload](/graph/api/resources/uploadsession?view=graph-rest-beta) e carregando iterativamente os intervalos do arquivo até que todos os bytes do arquivo tenham sido carregados. 

### <a name="microsoft-graph-security-api"></a>API de Segurança do Microsoft Graph
- Visualize a integração com a RSA NetWitness, ServiceNow e Splunk, para correlacionar e sincronizar [alertas](/graph/api/resources/security-api-overview?view=graph-rest-beta#alerts)e melhorar a proteção contra ameaças e respostas.
- Novos disparadores adicionados ao [Conector de Segurança do Microsoft Graph](https://docs.microsoft.com/connectors/microsoftgraphsecurity/) e [guias estratégicos](https://docs.microsoft.com/azure/security-center/security-center-playbooks) para Aplicativos de Lógica e Fluxo. Confira [exemplos de guias estratégicos](https://github.com/microsoftgraph/security-api-solutions/tree/master/Playbooks).
- Suporte no envio de [indicadores ameaças](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview) para o Microsoft Defender ATP para bloquear ou alertar ameaças usando suas próprias fontes de inteligência. Integrações com parceiros como o ThreatConnect permitem que os clientes enviem indicadores diretamente das soluções de inteligência e automação contra ameaças. 

### <a name="notifications"></a>Notificações
- [Crie e envie notificações](/graph/api/user-post-notifications?view=graph-rest-beta) a todos os clientes de aplicativos em todos os pontos de extremidade do dispositivo que um usuário está conectado, sem ter que gerenciar as permissões de usuário delegadas.
- Use [os pontos de extremidade da política de destino](/graph/api/resources/targetpolicyendpoints?view=graph-rest-beta) em [notificações](/graph/api/resources/notification?view=graph-rest-beta) do usuário para direcionar especificamente notificações para as plataformas Windows, iOS, Android ou WebPush.
- Especificar uma [política de retirada](/graph/api/resources/fallbackpolicy?view=graph-rest-beta) nas notificações para pontos de extremidade iOS, enviar notificações brutas de alta prioridade que podem não ser entregues aos dispositivos, caso contrário, devido a restrições específicas da plataforma, como o modo de economia de bateria.

 
### <a name="powershell-sdk"></a>SDK do PowerShell 
Os desenvolvedores e profissionais de TI podem observar o lançamento da [SDK do Microsoft Graph PowerShell](https://github.com/microsoftgraph/msgraph-sdk-powershell), que criará módulos que contêm cmdlets para criar solicitações da API REST do Microsoft Graph.

## <a name="september-2019-new-and-generally-available"></a>Setembro de 2019: novo e disponível para o público geral

### <a name="calendar-mail-and-group"></a>Calendário, email e grupo
[Obter o conteúdo bruto de um arquivo, ou o conteúdo MIME de um item](/graph/api/attachment-get?view=graph-rest-1.0#get-the-raw-contents-of-a-file-or-item-attachment) que foi adicionado como um [anexo](/graph/api/resources/attachment?view=graph-rest-1.0) a um[evento](/graph/api/resources/event?view=graph-rest-1.0), [ mensagem](/graph/api/resources/message?view=graph-rest-1.0)ou[ postagem](/graph/api/resources/post?view=graph-rest-1.0) de grupo.

### <a name="calendar-mail-outlook-task-personal-contact"></a>Calendário, email, tarefa do Outlook, contato pessoal
Use a função [translateExchange](/graph/api/user-translateexchangeids?view=graph-rest-1.0) para converter uma ID de item do Outlook [entre](/graph/api/user-translateexchangeids?view=graph-rest-1.0#exchangeidformat-values)formatos suportados, incluindo o formato de ID padrão do Microsoft Graph e o formato de ID imutável. 

Os recursos a seguir são compatíveis com a conversão de formato de ID:

- [attachment](/graph/api/resources/attachment?view=graph-rest-1.0)
- [contato](/graph/api/resources/contact?view=graph-rest-1.0)
- [event](/graph/api/resources/event?view=graph-rest-1.0)
- [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-1.0)
- [message](/graph/api/resources/message?view=graph-rest-1.0)
- [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-1.0)

### <a name="mail"></a>Correio
[Obter conteúdo MIME de uma mensagem](outlook-get-mime-message.md).

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph Toolkit
Use o [Microsoft Graph Toolkit](toolkit/overview.md) para desenvolver aplicativos de produção que ofereçam uma aparência consistente do Microsoft 365 e economize tempo na autenticação e acesso a dados do Microsoft Graph.

## <a name="september-2019-new-in-preview"></a>Setembro de 2019: novidades na versão prévia

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status GA. Não use-os em aplicativos de produção.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [Setembro](changelog.md#september-2019) do Intune

### <a name="files"></a>Arquivos
- Suporte aprimorado à sincronização:

  - Use a nova propriedade **pendingOperations** para identificar operações que podem afetar o conteúdo binário de um [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta).
  - [Restaure](/graph/api/driveitem-restore?view=graph-rest-beta) um **driveItem** excluído. 
- Use o Algoritmo de Hash Seguro (SHA-256) para aprimorar a segurança e a integridade dos [dados](/graph/api/resources/file?view=graph-rest-beta) do arquivo.
- Obtenha ou defina a orientação de uma [foto](/graph/api/resources/photo?view=graph-rest-beta). A configuração é compatível com o OneDrive Personal.

### <a name="identity-and-access"></a>Identidade e acesso
- Use a propriedade new **identities** e obtenha as identidades que um [usuário](/graph/api/resources/user?view=graph-rest-beta) pode usar para entrar em uma conta. As identidades podem ser fornecidas por organizações ou provedores de identidade social, como Facebook, Google e Microsoft.
- Aperfeiçoamentos incrementais para [sincronizar identidades](/graph/api/resources/synchronization-overview?view=graph-rest-beta) em um aplicativo de nuvem para um locatário:

  - Armazenar configurações para um [trabalho de sincronização](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta)
  - Especifique um motivo para impor a [quarentena](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta) a um trabalho de sincronização

### <a name="teamwork"></a>Teamwork
Use o canal **Geral** de uma [equipe](/graph/api/resources/team?view=graph-rest-beta) ou personalize as [configurações de membros](/graph/api/resources/teammembersettings?view=graph-rest-beta) para permitir que eles criem canais privados na **equipe**.

### <a name="users"></a>Usuários
- Obtenha ou atualize as identidades com as quais um [usuário](/graph/api/resources/user?view=graph-rest-beta) pode entrar em uma conta. Essas identidades podem ser fornecidas por organizações de negócios ou por provedores de identidade social, como o Facebook, o Google e a Microsoft.
- Obtenha ou atualize as [configurações da caixa de correio](/graph/api/resources/mailboxsettings?view=graph-rest-beta) do formato de data e hora escolhidas pelo usuário.


## <a name="august-2019-new-and-generally-available"></a>Agosto de 2019: novo e disponível para o público geral 

### <a name="reports"></a>Relatórios
- Obtenha dados [adicionais de uso da caixa de correio](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0) sobre o tamanho e a contagem de itens excluídos.
- Acompanhe as IDs de grupo do Microsoft 365 ao [obter detalhes da atividade do grupo](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0).
- Rastreie o nome principal do proprietário ao obter [detalhes da conta de uso do OneDrive](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0) e [ detalhes de uso do site do SharePoint](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0).
- Obtenha o número de usuários ativos e inativos no Microsoft 365, ao [obter um relatório sobre contagens de usuários por serviço microsoft 365](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0).

### <a name="security"></a>Segurança
- Use o novo [complemento Microsoft Graph Security API para Splunk](https://aka.ms/graphsecuritysplunkaddon) para transmitir alertas de segurança e insights de muitos produtos de parceiros para o Splunk, permitindo uma correlação mais simples de seus dados de segurança. Para saber mais, confira o [comunicado](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Introducing-the-new-Microsoft-Graph-Security-API-add-on-for/ba-p/815972). 
- [Confira uma lista de outras soluções e conectores](security-integration.md) criados pela Microsoft ou por parceiros da Microsoft que se conectam à API de segurança e permitem que você trabalhe com dados em um formato unificado.


## <a name="august-2019-new-in-preview"></a>Agosto de 2019: novidades na versão prévia

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status GA. Não use-os em aplicativos de produção.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [agosto](changelog.md#august-2019) do Intune

### <a name="education"></a>Educação
- Associe um [professor](/graph/api/resources/educationuser?view=graph-rest-beta) ou uma [atribuição](/graph/api/resources/educationassignment?view=graph-rest-beta) com uma [lista de critérios de avaliação classificada](/graph/api/resources/educationrubric?view=graph-rest-beta) para considerar qualidades e níveis específicos em atribuições. Um exemplo de qualidade é a ortografia e a gramática, e exemplos de níveis são "bons" e "ruins". Você pode ainda associar pontos e pesos a lista de critérios de avaliação. Para saber mais, confira [visão geral da lista de critérios de avaliação educacional](education-rubric-overview.md).
- Avaliar uma atribuição e apresentar os resultados em termos de [feedback](/graph/api/resources/educationfeedbackoutcome?view=graph-rest-beta), de um [grau numérico](/graph/api/resources/educationpointsoutcome?view=graph-rest-beta), ou de [lista de critérios de avaliação](/graph/api/resources/educationrubricoutcome?view=graph-rest-beta).

### <a name="files"></a>Arquivos
Até esse ponto, você pode [seguir](/graph/api/driveitem-follow?view=graph-rest-beta) um [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) para obter um acesso conveniente ou para facilitar ações como, mover, copiar e salvar como. Agora você pode usar a ação [deixar de seguir](/graph/api/driveitem-unfollow?view=graph-rest-beta) para parar de seguir esses itens da unidade.

### <a name="identity-and-access"></a>Identidade e acesso
- Os provedores de controle de acesso baseado em função (RBAC) podem [gerenciar funções](/graph/api/resources/rolemanagement?view=graph-rest-beta) do Azure Active Directory, [definindo ações de funções](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta)que podem ser realizadas em recursos específicos e [atribuindo funções](/graph/api/resources/unifiedroleassignment?view=graph-rest-beta) aos usuários com base em tais definições de função, fornecendo o acesso correspondente a esses recursos.
- Os administradores podem [listar as revisões de acesso](/graph/api/accessreview-list?view=graph-rest-beta) para facilitar de maneira eficiente a análise de associações de grupos, o acesso a aplicativos corporativos e as atribuições de funções. As revisões de acesso regular garantem que apenas as pessoas adequadas tenham acesso contínuo aos recursos de maneiras específicas.

### <a name="social-and-workplace-intelligence"></a>Inteligência social e do local de trabalho
Os usuários finais podem usar o aplicativo Microsoft 365 [myAnalytics](social-intel-concept-overview.md#why-integrate-with-document-based-insights) para obter informações sobre o gerenciamento de tempo, colaboração no trabalho e saldo de vida útil. Agora você pode usar a [API de análise](/graph/api/resources/social-overview?view=graph-rest-beta#help-users-gain-insights-into-their-work-patterns) para integrar dados sobre tempo gasto em atividades de trabalho, como chamadas, chats e email, para ajudar a melhorar a produtividade e o bem-estar do usuário. 


## <a name="july-2019-new-and-generally-available"></a>Julho de 2019: novo e disponível para o público geral 

### <a name="example-code-snippets"></a>Exemplo de trechos de código
Agora há trechos do código Objective-C em todos os tópicos da API nas referências v 1.0 e beta. Veja o exemplo do Objective-C de como [obter um evento](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example).

### <a name="group"></a>Grupo
- Use a função [ValidateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0) para certificar-se de que o nome de exibição ou o apelido de email de um grupo existente do Microsoft 365 esteja em conformidade com as políticas de nomeação.
- Como alternativa, antes de criar o grupo, você pode usar a função[ ValidateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0)para um[directoryobject](/graph/api/resources/directoryobject?view=graph-rest-1.0) para validar primeiro os nomes.

### <a name="identity-and-access"></a>Identidade e acesso
- Use as [novas permissões delegadas e de aplicativo](permissions-reference.md#organization-permissions), _Organization.Read.All_ e _Organization.ReadWrite.All_ para acessar uma [organização](/graph/api/resources/organization?view=graph-rest-1.0) e recursos relacionados, como [SKUs inscritos](/graph/api/resources/subscribedsku?view=graph-rest-1.0).
- Use [novas permissões delegadas e de aplicativo ](permissions-reference.md#role-management-permissions), _RoleManagement. Read.Directory _ e_RoleManagement. ReadWrite.Directory_, para controle de acesso baseado em função ( RBAC) para o diretório da empresa:

  - Use a permissão de leitura/gravação para [ativar](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0) primeiro uma função de diretório. 
  - Com a função ativada, você pode usar a permissão de leitura para[ler funções de diretório](/graph/api/directoryrole-list?view=graph-rest-1.0), [listar os membros da função](/graph/api/directoryrole-list-members?view=graph-rest-1.0) e [listar modelos de função de diretório](/graph/api/directoryroletemplate-list?view=graph-rest-1.0). 
  - Você também pode usar a permissão de leitura/gravação para[adicionar](/graph/api/directoryrole-post-members?view=graph-rest-1.0)e [remover](/graph/api/directoryrole-delete-member?view=graph-rest-1.0) membros da função.


## <a name="july-2019-new-in-preview"></a>Julho de 2019: Novo na visualização

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status GA. Não use-os em aplicativos de produção.

### <a name="calendar"></a>Calendário 
Use a nova [API de locais](/graph/api/resources/place?view=graph-rest-beta) para usar vários tipos de locais, como [salas](/graph/api/resources/room?view=graph-rest-beta) e [lista de salas](/graph/api/resources/roomlist?view=graph-rest-beta), conforme configurado pelos administradores do Exchange Online.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [julho](changelog.md#july-2019) do Intune

### <a name="files"></a>Arquivos 
Aplique a data/hora de vencimento ou a senha ao [criar um link de compartilhamento](/graph/api/driveitem-createlink?view=graph-rest-beta) para um arquivo, pasta, ou outros [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta).

### <a name="identity-and-access"></a>Identidade e acesso
- Use [nova permissão de aplicativo](/graph/permissions-reference?#accessreviews-permissions) _AccessReview.ReadWrite.Membership_ para operações CRUD nas [análises de acesso](/graph/api/resources/accessreviews-root?view=graph-rest-beta). 
- Use [novas permissões delegadas e de aplicativo ](permissions-reference.md#administrative-units-permissions),_AdministrativeUnit.Read.All _ e _AdministrativeUnit. ReadWrite.All_, para ler ou gravar respectivamente (incluindo criar, atualizar, excluir ou gerenciar a associação) recursos da [unidade de administração](/graph/api/resources/administrativeunit?view=graph-rest-beta).
- Use as [novas permissões delegadas e de aplicativo](permissions-reference.md#organization-permissions), _Organization.Read.All_ e _Organization.ReadWrite.All_ para acessar uma [organização](/graph/api/resources/organization?view=graph-rest-beta) e recursos relacionados, como [SKU inscritos](/graph/api/resources/subscribedsku?view=graph-rest-beta).
- Use a nova função[descobrir](/graph/api/directorydefinition-discover?view=graph-rest-beta) para encontrar o [esquema de sincronização](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta)de diretório mais recente, para sincronizar objetos de diretório, atributos e seus tipos de aplicativo.
- Use a [política de distribuição de recursos](/graph/api/resources/featureRolloutPolicy?view=graph-rest-beta) para ajudar os administradores de locatários a testar recursos em grupos específicos antes de habilitá-los para toda a organização.

### <a name="mail"></a>Correio
Use permissões de aplicativo mais granulares _Mail.ReadBasic.All_ para ler a caixa de correio de um usuário, com exceção de qualquer corpo de mensagem, corpo de visualização, anexos e propriedades estendidas e com exceção da pesquisa na caixa de correio. Agora aplicável a [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) e [controle de alterações](delta-query-overview.md) para [mensagem](/graph/api/resources/message?view=graph-rest-beta) e**mailFolder.**

### <a name="reports"></a>Relatórios
- Obtenha dados [adicionais de uso da caixa de correio](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta) sobre o tamanho e a contagem de itens excluídos.

### <a name="teamwork"></a>Trabalho em equipe
- [Instalar](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta), [desinstalar](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta), [atualizar ](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta) e [listar aplicativos do Microsoft Teams instalados ](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta) para um usuário. 
- Use o acesso somente para aplicativos para ler mensagens de canal, respostas a mensagens de canal e mensagens em um chat. [Solicite a aprovação](teams-protected-apis.md) para tal acesso.

## <a name="may---june-2019-new-and-generally-available"></a>Maio e julho de 2019: novo e disponível para o público geral

### <a name="calendar-mail-and-personal-contacts"></a>Calendário, email e contatos pessoais
Os administradores do Exchange podem conceder permissões de aplicativo a um aplicativo e [restringir o seu acesso apenas a um subconjunto de caixas de correio em um ](auth-limit-mailbox-access.md), ao invés do padrão, que é o acesso a todas as caixas de correio na organização. Este acesso restrito se aplicaria a quaisquer permissões de aplicativos concedidas ao aplicativo para [calendários](permissions-reference.md#calendars-permissions), [contatos](permissions-reference.md#contacts-permissions) e [configurações de email e de caixa de correio](permissions-reference.md#mail-permissions). Confira o [anúncio do blog](https://developer.microsoft.com/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/) relacionado.

### <a name="mail"></a>Email
Use a API de [pastas de pesquisa de email](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0) para pesquisar mensagens e acessar os resultados de pesquisa de email do Outlook. Confira o [anúncio do blog](https://developer.microsoft.com/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/) relacionado.

### <a name="postman"></a>Postman
Como uma alternativa ao Explorador do Graph, experimente a API do Microsoft Graph na [coleção do Microsoft Graph Postman](use-postman.md) para aprender o comportamento da API e acelerar o desenvolvimento de aplicativos.

### <a name="tutorials"></a>Tutoriais
Experimente o novo [tutorial para criar um aplicativo de console do Java](/graph/tutorials/java) para obter informações sobre um calendário de usuário.

### <a name="user"></a>Usuário
Administradores ou usuários podem [revogar](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) todos os tokens de atualização emitidos para um usuário. Isso geralmente é usado para impedir que aplicativos em um dispositivo perdido ou roubado acessem os dados de uma organização.


## <a name="may---june-2019-new-in-preview"></a>Maio e junho de 2019: novidades na versão prévia

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status GA. Não use-os em aplicativos de produção.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
- Atualizações de [maio](changelog.md#may-2019) do Intune 
- Atualizações de [junho](changelog.md#june-2019) do Intune

### <a name="education"></a>Educação
- Consulta Delta para um objeto [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta).
- Consulta Delta e adições de propriedade para objetos [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta) e [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta).

### <a name="group"></a>Grupo
Obtenha [Rótulos de confidencialidade](/graph/api/resources/assignedlabel?view=graph-rest-beta) para ajudar a proteger dados confidenciais de um grupo do Microsoft 365 e atender a políticas de conformidade. Esses rótulos são objetos [assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta), publicados por administradores no Centro de Conformidade e Segurança do Microsoft 365, como parte dos recursos de Proteção de Informações da Microsoft. 

### <a name="identity-and-access"></a>Identidade e acesso
- Obtenha uma instância de um [aplicativo](/graph/api/resources/applicationtemplate?view=graph-rest-beta) ou adicione uma instância da galeria de aplicativos do Azure AD ao seu diretório como modelo.
- Obtenha um log de todos os diretórios de[eventos de provisionamento](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta) em um locatário.
- Obtenha informações sobre [usuário detectado ou riscos de login](/graph/api/resources/riskdetection?view=graph-rest-beta) em um ambiente do Azure AD. Esta funcionalidade de detecção de riscos faz parte do Azure AD Identity Protection.

### <a name="mail"></a>Email
Use permissões de aplicativo mais detalhadas _Mail.ReadBasic.All_ para ler a caixa de correio de um usuário, com exceção de qualquer corpo de mensagem, corpo de visualização, anexos e propriedades estendidas e com exceção da pesquisa na caixa de correio. Disponível para métodos de leitura [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) e [controle de alterações](delta-query-overview.md) para [mensagem](/graph/api/resources/message?view=graph-rest-beta) e **mailFolder.**

### <a name="microsoft-graph-toolkit"></a>Kit de ferramentas do Microsoft Graph
O [kit de ferramentas do Microsoft Graph](/graph/toolkit/overview) é um conjunto de colaboradores e de componentes da Web de estrutura independente que oferece conveniência para autenticar e acessar dados no Microsoft Graph. Como o kit de ferramentas do Microsoft Graph está no status de visualização, use provedores e componentes do kit de ferramentas somente em aplicativos que não são de produção.

### <a name="reports"></a>Relatórios
- Obtenha [relatórios sobre os métodos de autenticação](/graph/api/resources/authenticationmethods-usage-insights-overview?view=graph-rest-beta) adotados pelos usuários em uma organização, como rest de senha de autoatendimento e autenticação multifator (MFA).

### <a name="sites"></a>Sites
Permitir que os usuários [sigam](/graph/api/site-follow?view=graph-rest-beta) ou [parem de seguir](/graph/api/site-unfollow?view=graph-rest-beta) os sites do SharePoint.

### <a name="teamwork"></a>Teamwork
- Hospede [imagens](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta) em [mensagens de bate-papo](/graph/api/resources/chatmessage?view=graph-rest-beta) do Microsoft Teams.
- Suporte para [configurar](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta) como uma equipe privada pode ser descoberta.


## <a name="january---april-2019-new-and-generally-available"></a>Janeiro a abril de 2019: novo e disponível para o público geral

[Microsoft Graph data connect](data-connect-concept-overview.md)

### <a name="calendar"></a>Calendário
[Obter agenda de disponibilidade](outlook-get-free-busy-schedule.md)

### <a name="identity-and-access"></a>Identidade e acesso
[Fornecedores de identidade](/graph/api/resources/identityprovider?view=graph-rest-1.0)
[melhores guias de autenticação](/graph/auth)
[migrando aplicativos do Azure AD Graph para o Microsoft Graph](migrate-azure-ad-graph-overview.md)

### <a name="sdks"></a>SDKs
[Guias SDK](/sdks/sdks-overview.md)Trechos de API ([exemplo](/graph/api/user-get?view=graph-rest-1.0&tabs=cs#sdk-sample-code))

### <a name="security"></a>Segurança
[Classificação de segurança do locatário](/graph/api/resources/securescore?view=graph-rest-1.0)

## <a name="january---april-2019-new-in-preview"></a>Janeiro a abril de 2019: novo na versão prévia

### <a name="calendar-group-mail-to-do-tasks"></a>Calendário, grupo, email, tarefas pendentes
[Obter o conteúdo bruto/MIME de anexos de arquivo ou item](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment) para um evento, mensagem, tarefa do Outlook ou postagem do grupo

### <a name="change-notifications"></a>Notificações de alteração
[Reduzir as notificações de alteração ausentes para recursos do Outlook](webhooks-outlook-authz.md)

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
- Atualizações [de](changelog.md#january-2019) janeiro do Intune 
- Atualizações [de](changelog.md#february-2019) fevereiro do Intune
- Atualizações [de](changelog.md#march-2019) março do Intune
- Atualizações [de](changelog.md#april-2019) abril do Intune

### <a name="files"></a>Arquivos
[Compartilhamento de convite](/graph/api/driveitem-invite?view=graph-rest-beta) inclui data de vencimento e senha

### <a name="financials"></a>Finanças
[Dynamics 365 Business Central](dynamics-business-central-concept-overview.md)

### <a name="identity-and-access"></a>Identidade e acesso
[O Access revisa](/graph/api/resources/accessreviews-root?view=graph-rest-beta) as permissões de aplicativo suporte [auditoria e registros](/graph/api/resources/azure-ad-auditlog-overview?view=graph-rest-beta)
[de entrada personalizado, entre e inscreva-se no Azure AD B2C](/graph/api/resources/trustframeworkpolicy?view=graph-rest-beta)
[usuário arriscado](/graph/api/resources/riskyuser?view=graph-rest-beta) e [histórico](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta)

### <a name="mail"></a>Correio
[Obter conteúdo MIME de mensagens](outlook-get-mime-message.md)

### <a name="reports"></a>Relatórios
[Relatórios de entrada do aplicativo](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta)

### <a name="security"></a>Segurança
[Indicadores de ameaça ](/graph/api/resources/securityaction?view=graph-rest-beta)
[de Ações de segurança](/graph/api/resources/tiindicator?view=graph-rest-beta)

### <a name="teamwork"></a>Trabalho em equipe
[O gerenciamento](/graph/api/resources/chat?view=graph-rest-beta)
[de conversas em 1:1](/graph/api/resources/shift?view=graph-rest-beta)

## <a name="see-also"></a>Confira também
- Confira [O que há de novo](whats-new-overview.md) no Microsoft Graph.
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).