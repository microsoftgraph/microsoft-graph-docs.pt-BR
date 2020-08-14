---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 2dfeaa8ba656adac608de31028772f8b5665f4f0
ms.sourcegitcommit: 2e6fb1c0fef8cb3af1a72c115aa54902c71c99f5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2020
ms.locfileid: "46658225"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](changelog.md). 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.

## <a name="august-2020-new-and-generally-available"></a>Agosto de 2020: novo e disponível para o público geral

### <a name="change-notifications"></a>Notificações de alteração
[Controle de alterações](delta-query-overview.md) de recursos com suporte para a nuvem nacional do Microsoft Graph para o Governo dos EUA.


## <a name="august-2020-new-in-preview-only"></a>Agosto de 2020: novidade apenas na versão prévia

### <a name="applications"></a>Aplicativos
Ofereça suporte a logon único baseado em senha para recursos de aplicativos de [entidade de serviço](/graph/api/resources/serviceprincipal?view=graph-rest-beta) e especifique essas [configurações](/graph/api/resources/passwordsinglesignonsettings?view=graph-rest-beta) na propriedade **passwordSingleSignOnSettings**. Para obter informações sobre logon único baseado em senha no Azure AD, confira [configurar logon único baseado em senha](/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).

### <a name="change-notifications"></a>Notificações de alteração
- Use a propriedade **includeResourceData** de uma [assinatura](/graph/api/resources/subscription?view=graph-rest-beta) para [configurar notificações de alteração que incluam dados de recursos](webhooks-with-resource-data.md). Não use a propriedade **includeProperties**.
- Receba [notificações de alteração via Hub de Eventos](change-notifications-delivery.md).

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- Personalize um [contrato de termos de uso](/graph/api/resources/agreement?view=graph-rest-beta) para oferecer suporte a uma data de vencimento e cadência de contrato, exigir que o usuário aceite o contrato por dispositivo ou aceite novamente o contrato em uma frequência definida. 
- Use a propriedade do**arquivo** para navegar até um [contrato personalizado](/graph/api/resources/agreementfile?view=graph-rest-beta) para termos de uso. Não use a propriedade de **arquivos**.

### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
Obtenha [relatórios sobre o uso de aplicativos do Microsoft 365](/graph/api/resources/microsoft-365-apps-usage-report?view=graph-rest-beta), especificamente sobre detalhes de usuários, contagens de usuários e contagens de usuários da plataforma.

### <a name="teamwork"></a>Trabalho em equipe
Obtenha [conteúdo hospedado em uma mensagem de chat](/graph/api/resources/chatMessageHostedContent?view=graph-rest-beta), como imagens ou trechos de códigos. Veja um [exemplo](/graph/api/chatmessagehostedcontent-get?view=graph-rest-beta&branch=master#example-2-get-hosted-content-bytes-for-an-image) para obter os bytes de conteúdo de uma imagem.

## <a name="july-2020-new-and-generally-available"></a>Julho de 2020: novos e disponíveis para o público em geral

### <a name="calendar"></a>Calendário
GA do recurso que permite aos organizadores permitir propostas de horário alternativo para reuniões ou convites para [propor novos horários para uma reunião](outlook-calendar-meeting-proposals.md) quando eles [aceitarem provisoriamente](/graph/api/event-tentativelyaccept?view=graph-rest-1.0) ou [recusarem](/graph/api/event-decline?view=graph-rest-1.0) um evento.

### <a name="change-notifications"></a>Notificações de alteração
Removida do recurso [changeNotification](/graph/api/resources/changenotification) a propriedade **sequenceNumber** introduzida erroneamente.

### <a name="groups"></a>Grupos
DG das seguintes propriedades para a entidade [group](/graph/api/resources/group?view=graph-rest-v1.0): **assignedLabels**, **expirationDateTime**, **membershipRule**, **membershipRuleProcessingState**, **preferredLanguage**e **theme**.

### <a name="identity-and-access"></a>Identidade e acesso
- Remover um usuário como proprietário registrado ou usuário de um [dispositivo](/graph/api/resources/device).
- Acompanhe as alterações de representações locais de aplicativos recém-criadas, atualizadas ou deletadas (representada por recursos[servicePrincipals](/graph/api/resources/serviceprincipal)) e permissões delegadas concedidas (representadas por recursos[oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant)) sem executar uma leitura completa de toda a coleção de recursos.
- GA da [política para reforçar o padrão de segurança](/graph/api/resources/identitysecuritydefaultsenforcementpolicy) que protege as organizações contra ataques comuns.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- GA de [políticas de acesso condicional](/graph/api/resources/conditionalAccessPolicy) que são regras personalizadas que definem um cenário de acesso.
- GA de [posições nomeadas](/graph/api/resources/namedLocation) representando regras personalizadas que definem os locais de rede usados em uma política de acesso condicional.

### <a name="schema-extensions"></a>Extensões de esquema
O recurso [extensões de esquema](/graph/api/resources/schemaextension) já está disponível para o público em geral no[Microsoft Cloud for US Government](/graph/deployments).

### <a name="teamwork"></a>Trabalho em equipe
Use as permissões delegadas de `TeamsAppInstallation.ReadForTeam` ou `TeamsAppInstallation.ReadWriteForTeam` ou permissões de aplicativo de `TeamsAppInstallation.ReadForTeam.All` ou `TeamsAppInstallation.ReadWriteForTeam.All` para [listar aplicativos instalados em uma equipe](/graph/api/teamsappinstallation-list).

## <a name="july-2020-new-in-preview-only"></a>Julho de 2020: novos apenas na visualização

### <a name="cloud-communications"></a>Comunicações na nuvem
- Use a operação [atualizar](/graph/api/onlinemeeting-update?view=graph-rest-beta) para atualizar **startDateTime**, **endDateTime**, **participantes**, ou propriedade de **assunto**de uma [reunião online](/graph/api/resources/onlinemeeting?view=graph-rest-beta).
- Inscreva-se para receber notificações sobre alterações na disponibilidade de um usuário do Microsoft Teams, conforme representado pelo recurso [presence](/graph/api/resources/presence?view=graph-rest-beta).

### <a name="cloud-communications--call-records"></a>Comunicação em nuvem | Gravação
- [Obtenha](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta) os registros de chamadas da rede pública de telefonia comutada (PSTN).
- [Obtenha](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta) os registros de chamadas de roteamento direto.

### <a name="compliance--ediscovery"></a>Conformidade | Descoberta eletrônica
Estréia dos [Casos de descoberta eletrônica](/graph/api/resources/ediscoverycase?view=graph-rest-beta) que podem conter responsáveis, bloqueios, coleções, conjuntos de revisão, e exportações que podem ser usados como evidência em casos jurídicos.
Os aplicativos agora podem [consultar](/graph/api/resources/reviewsetquery?view=graph-rest-beta) e [revisar o conjunto de dados](/graph/api/resources/reviewset?view=graph-rest-beta) coletado para uso em litígio, investigação ou solicitação regulatória. Esse estreia faz parte da [Descoberta Eletrônica Avançada](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide)do Microsoft 365.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- Use as permissões do aplicativo `Printer.ReadWrite.All` e a [codificação do IPP (Protocolo de Impressão via Internet)](https://tools.ietf.org/html/rfc8010) para [atualizar uma impressora ](/graph/api/printer-update?view=graph-rest-beta).
- Use uma das permissões de aplicativo, `PrintJob.ReadBasic.All`, `PrintJob.Read.All`, `PrintJob.ReadWriteBasic.All`ou `PrintJob.ReadWrite.All`, para [obter um trabalho de impressão](/graph/api/printjob-get?view=graph-rest-beta) ou [listar trabalhos de impressão para uma impressora](/graph/api/printer-list-jobs?view=graph-rest-beta).
- Quando [obtiver um trabalho de impressão](/graph/api/printjob-get?view=graph-rest-beta), use `$expand` para obter [tarefas de impressão](/graph/api/resources/printtask?view=graph-rest-beta) que estão executando ou que foram executadas no trabalho. Imprimir tarefas, [definições de tarefas](/graph/api/resources/printtaskdefinition?view=graph-rest-beta)e [disparadores de tarefas](/graph/api/resources/printtasktrigger?view=graph-rest-beta) são usados em [impressão segura](universal-print-concept-overview.md#extending-universal-print-to-support-pull-printing).
- [Redirecione um trabalho de impressão](/graph/api/printjob-redirect?view=graph-rest-beta) para uma impressora diferente, como parte da impressão segura.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações do Intune em [julho](changelog.md#july-2020) em beta.

### <a name="groups"></a>Grupos
Use a propriedade **isAssignableToRole** de um [grupo](/graph/api/resources/group?view=graph-rest-beta) do Microsoft 365 e a defina durante a criação de um grupo para indicar se ele pode ser atribuído a uma função do Azure AD. Isso [ajuda a gerenciar as atribuições de função no Azure AD](/azure/active-directory/users-groups-roles/roles-groups-concept), de modo que, em vez de atribuir um usuário individual a uma função do Azure AD, um administrador global ou um administrador de funções privilegiadas pode criar um grupo do Microsoft 365 e atribuir o grupo a essa função, para que quando os usuários se unam ao _grupo_, eles recebam a função pretendida indiretamente.

### <a name="identity-and-access"></a>Identidade e acesso
- [Adquira um token de acesso](/graph/api/synchronization-synchronization-acquireAccessToken?view=graph-rest-beta) para autorizar o serviço de provisionamento do Azure AD para provisionar usuários em um aplicativo.
- [Obtenha](/graph/api/entitlementmanagementsettings-get?view=graph-rest-beta) ou [atualize](/graph/api/entitlementmanagementsettings-update?view=graph-rest-beta) as configurações de gerenciamento de qualificação que controlam o acesso a grupos, aplicativos e sites do SharePoint Online para usuários internos e externos à sua organização. 

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- Inclua os níveis de risco do usuário (`low`, `medium`, `high`, `none`) como consideração para aplicar uma [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta).
- [Use a alteração de senha como um controle Grant](/graph/api/resources/conditionalaccessgrantcontrols?view=graph-rest-beta#special-considerations-when-using-passwordchange-as-a-control) para passar uma política de acesso condicional.
- Use um [provedor de conexão de ID aberta](/graph/api/resources/openidconnectprovider?view=graph-rest-beta) (ODIC) como um provedor de identidade em um locatário do Azure AD e um locatário do Azure AD B2C. Sua propriedade **claimsMapping** permite que o Azure AD [mapeie as declarações](/graph/api/resources/claimsmapping?view=graph-rest-beta) de um provedor OIDC para as declarações que o Azure AD reconhece e usa.

### <a name="people-and-workplace-intelligence--insights"></a>Inteligência social e do ambiente de trabalho | Ideias
Use mais o [controle de privacidade granular](insights-customize-item-insights-privacy.md) sobre a disponibilidade e a exibição das [informações do item](/graph/api/resources/iteminsights?view=graph-rest-beta) no Microsoft 365. Essas informações representam as relações entre um usuário e documentos no OneDrive for Business, calculadas usando uma análise avançada e técnicas de aprendizado de máquina. 

### <a name="people-and-workplace-intelligence--profile-card-customization"></a>Inteligência de pessoas e local de trabalho | Personalização de cartão de perfil
Os administradores podem [personalizar as propriedades expostas no cartão de perfil de suas organizações](add-properties-profilecard.md) usando a API para [propriedade de cartão de perfil](/graph/api/resources/profilecardproperty?view=graph-rest-beta).

### <a name="sites-and-lists"></a>Sites e listas
Acesse a taxonomia do [repositório de termos](/graph/api/resources/termstore-store?view=graph-rest-beta) a hierarquia que consite em recursos de [grupo](/graph/api/resources/termstore-group?view=graph-rest-beta), [definição](/graph/api/resources/termstore-set?view=graph-rest-beta), e [termo](/graph/api/resources/termstore-term?view=graph-rest-beta), e [relacione](/graph/api/resources/termstore-relation?view=graph-rest-beta) recursos entre os termos.

### <a name="workbooks-and-charts"></a>Pastas de trabalho e gráficos
[Obtenha o status e todos os resultados](/graph/api/workbookoperation-get?view=graph-rest-beta) de uma operação [de longa execução](/graph/api/resources/workbookoperation?view=graph-rest-beta) em uma [pasta de trabalho](/graph/api/resources/workbook?view=graph-rest-beta).


## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de visualização **_prévia_**. As atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de**_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/office/dev-program), ganhe uma assinatura gratuita do Microsoft 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).

