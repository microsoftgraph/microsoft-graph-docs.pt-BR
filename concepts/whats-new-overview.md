---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 448c9b0063a04cf0ddaa375092a1dd9ceff6694a
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557847"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Confira os destaques das novidades do Microsoft Graph e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista completa das atualizações da API, confira as seções de [março](changelog.md#april-2020) e [fevereiro](changelog.md#march-2020) do log de alterações da API. 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.

## <a name="april-2020-new-and-generally-available"></a>Abril de 2020: novo e geralmente disponível.

### <a name="calendar"></a>Calendário
- [Compartilhar ou delegar calendários](outlook-share-or-delegate-calendar.md) de forma programática, com uma maior paridade com a experiência do usuário do Outlook. Além de controlar as permissões do usuário atual e o status de compartilhamento de um calendário:
  - Para cada [calendário](/graph/api/resources/calendar?view=graph-rest-1.0), você pode gerenciar as [permissões](/graph/api/resources/calendarpermission?view=graph-rest-1.0) de cada usuário com o qual o calendário é compartilhado. 
  - Para cada [caixa de correio](/graph/api/resources/mailboxsettings?view=graph-rest-1.0), você pode especificar se um representante, proprietário de caixa de correio ou ambos receberão mensagens da reunião e respostas da reunião. 
- [Criar ou atualizar um evento como uma reunião online](outlook-calendar-online-meetings.md):
  - Para cada **calendário**, especifique os provedores de reuniões online permitidos e padrão.
  - Crie ou atualize um [evento](/graph/api/resources/event?view=graph-rest-1.0) que esteja disponível online e forneça detalhes para que os participantes possam ingressar na reunião online. 
  - Em particular, use as novas propriedades **onlineMeetingProvider** e **onlineMeeting** do **evento** para definir ou identificar o Microsoft Teams como um provedor de reuniões online, uma solução alternativa para um [problema conhecido](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams) com a propriedade **onlineMeetingUrl**.

### <a name="files"></a>Arquivos
- [Check-out](/graph/api/driveitem-checkout?view=graph-rest-1.0) ou [check-in](/graph/api/driveitem-checkin?view=graph-rest-1.0) de um arquivo para o OneDrive para gerenciar a atualização do arquivo e disponibilizar atualizações para outras pessoas quando as atualizações estiverem prontas.

### <a name="identity-and-access"></a>Identidade e acesso
- Para gerenciar funções e atribuir acesso a recursos nos provedores de controle de acesso baseado em função (RBAC), como o Microsoft Intune, use [unifiedRoleAssignmentMultiple](/graph/api/resources/unifiedroleassignmentmultiple?view=graph-rest-1.0). O recurso **unifiedRoleAssignmentMultiple** permite definir uma única função em uma matriz de escopos e atribuir a função a várias entidades (como usuários).
- Acessar tipos específicos de [políticas de uma organização](/graph/api/resources/policy-overview?view=graph-rest-1.0) usando o `/policies`segmento URL e especificando o tipo de política. Por exemplo, uma organização pode forçar uma política a entrar automaticamente no usuário de uma sessão da Web após um período de inatividade, confira as operações CRUD para instâncias de [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-1.0). Essa é um [alteração significativa](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-1.0/) para que seja mais fácil descobrir todas as políticas, agrupando todas as políticas digitadas sob o `/policies`segmento. Acesse outras políticas digitadas de uma abordagem semelhante: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-1.0), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-1.0), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-1.0)e [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-1.0). 

## <a name="april-2020-new-in-preview-only"></a>Abril de 2020: novo somente para visualização

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [abril](changelog.md#april-2020) do Intune.

### <a name="identity-and-access"></a>Identidade e acesso
- [Controlar alterações](/graph/api/administrativeunit-delta?view=graph-rest-beta) para [unidades administrativas](/graph/api/resources/administrativeunit?view=graph-rest-beta).
- [Controlar alterações](/graph/api/oauth2permissiongrant-delta?view=graph-rest-beta) para [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant?view=graph-rest-beta).
- [Gerenciar](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta) os [métodos de autenticação](/graph/api/resources/authenticationmethod?view=graph-rest-beta) de um usuário que incluem a [senha](/graph/api/resources/passwordauthenticationmethod?view=graph-rest-beta) ou [telefone](/graph/api/resources/phoneauthenticationmethod?view=graph-rest-beta). Por exemplo, [redefinir uma senha de usuário](/graph/api/passwordauthenticationmethod-resetpassword?view=graph-rest-beta), [obter o status da redefinição](/graph/api/authenticationoperation-get?view=graph-rest-beta) ou [adicionar um número de telefone](/graph/api/authentication-post-phonemethods?view=graph-rest-beta) para um usuário para autenticação de SMS ou chamada de voz, se a política estiver habilitada para o usuário.

### <a name="reports--identity-and-access-reports"></a>Relatórios | Relatórios de identidade e acesso
[Listar](/graph/api/relyingpartydetailedsummary-list?view=graph-rest-beta) [participantes confiáveis](https://docs.microsoft.com/windows-server/identity/ad-fs/technical-reference/understanding-key-ad-fs-concepts) configurados nos Serviços de Federação do Active Directory.

### <a name="reports--office-365-usage-reports"></a>Relatórios | Relatórios de uso do Office 365
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
O administrador de serviços do Teams e o administrador de comunicações do Teams devem ser usados como funções de usuário aceitas para permitir que os aplicativos leiam os relatórios de uso do serviço do Office 365 em nome de um usuário, como [formas de autorização delegada pelo usuário](reportroot-authorization.md). 

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

