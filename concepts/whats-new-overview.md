---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 4f75b6df6cfae4026de6e1a917002d4531a2ff73
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524463"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Confira os destaques das novidades do Microsoft Graph e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista completa das atualizações de API, consulte as seções [maio](changelog.md#may-2020) e [abril](changelog.md#april-2020) do changelog da API. 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.

## <a name="may-2020-new-and-generally-available"></a>Maio de 2020: novo e geralmente disponível

### <a name="calendar--place"></a>Calendário | Local
GA da [API de locais](/graph/api/resources/place) em v 1.0 – Use esta API em aplicativos de produção para obter, atualizar ou excluir uma lista de [salas](/graph/api/resources/room) ou [salas](/graph/api/resources/roomlist) em um locatário. [Saiba mais](outlook-calendar-concept-overview.md#build-apps-with-location-awareness-and-provide-intelligent-context) sobre a API de locais.

### <a name="cloud-communications--call-records"></a>Comunicação em nuvem | Gravação
- GA da [API de registros de chamadas](/graph/api/resources/callrecords-api-overview?view=graph-rest-1.0) – use o recurso [callRecord](/graph/api/resources/callrecord?view=graph-rest-1.0) para obter os metadados de chamadas e reuniões online no Microsoft Teams e no Skype.
- Inscreva-se para [alterar as notificações](/graph/webhooks) de alterações em todos os recursos do **callRecord** em uma organização.
- [Listar sessões](/graph/api/callrecords-session-list?view=graph-rest-1.0) em um **callRecord**e, opcionalmente, [expanda cada sessão para listar segmentos](/graph/api/callrecords-session-list?view=graph-rest-1.0#example-2-get-session-list-with-segments) no registro de chamada.
- Suporte para os valores de banda de 60-GHz ( `frequency60GHz` ) e `unknownFutureValue` WiFi de um ponto de extremidade de mídia em um segmento.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
O Intune [pode](changelog.md#may-2020) atualizar em v 1.0.

### <a name="graph-explorer"></a>Explorador do Graph
Use os vários novos recursos do [Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer) que aprimoram o aprendizado e o protótipo na área restrita. Por exemplo:
- Exibir trechos de código que correspondem à consulta da API REST inserida, em C#, Java, JavaScript e objetivo C.
- Conectado com um locatário, exiba e copie um token de acesso para seu aplicativo de cliente REST favorito.

Consulte o [novo explorador do Graph agora está disponível](https://developer.microsoft.com/graph/blogs/new-graph-explorer-is-now-ga/) para obter mais detalhes.

### <a name="identity-and-access"></a>Identidade e acesso
- GA da API de entidades de serviço no v 1.0 – Use o [recurso servicePrincipalName](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) nos aplicativos de produção para gerenciar programaticamente as instâncias de aplicativos e controlar o que um aplicativo pode fazer dentro do seu locatário. Você pode controlar quem pode usar um aplicativo, a quais recursos o aplicativo tem acesso, como a adição de credenciais de senha, o cancelamento de certificados de expiração e o gerenciamento de permissões delegadas e atribuições de função de aplicativo.
- GA da API [appRoleAssignment](/graph/api/resources/appRoleAssignment?view=graph-rest-1.0) , que registra a atribuição de um [appRole](/graph/api/resources/approle?view=graph-rest-1.0) (representando a `roles` declaração em tokens de ID e tokens de acesso) a um [usuário](/graph/api/resources/user?view=graph-rest-1.0), [grupo](/graph/api/resources/group?view=graph-rest-1.0)ou [servicePrincipalName](/graph/api/resources/serviceprincipal?view=graph-rest-1.0).
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


## <a name="may-2020-new-in-preview-only"></a>Maio de 2020: novo na visualização

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

### <a name="reports--office-365-usage-reports"></a>Relatórios | Relatórios de uso do Office 365
Exibir dados de **Reunião Criada** e de **Reunião Interagida** nos relatórios CSV para [contagens de atividades de email](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta), [contagens de atividades de email do usuário](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta) e [detalhes de atividades de email do usuário](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta).


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

