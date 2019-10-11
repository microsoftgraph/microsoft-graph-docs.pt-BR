---
title: Destaques de versões anteriores no Microsoft Graph
description: O que havia de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 3eb7b2d73fa1e277c1db6762c9ac5c96326889aa
ms.sourcegitcommit: f23cc661a0e30d01a6b59cfdae90768c55b80ae2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/08/2019
ms.locfileid: "37418276"
---
# <a name="highlights-of-earlier-releases"></a>Destaques de versões anteriores

## <a name="august-2019-new-and-generally-available"></a>Agosto de 2019: novo e disponível para o público geral 

### <a name="reports"></a>Relatórios
- Obtenha dados [adicionais de uso da caixa de correio](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0) sobre o tamanho e a contagem de itens excluídos.
- Acompanhar as IDs do grupo do Office 365 ao [obter detalhes da atividade do grupo](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0).
- Rastreie o nome principal do proprietário ao obter [detalhes da conta de uso do OneDrive](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0) e [ detalhes de uso do site do SharePoint](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0).
- Obtenha o número de usuários ativos e inativos no Office 365, ao [receber um relatório sobre contagens de usuários por serviço do Office 365](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0).

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
Os usuários finais vêm podendo usar o aplicativo [MyAnalytics](social-intel-concept-overview.md#why-integrate-with-document-based-insights-preview) do Office 365para obter insights sobre gerenciamento de tempo, colaboração no trabalho e equilíbrio profissional. Agora você pode usar a [API de análise](/graph/api/resources/social-overview?view=graph-rest-beta#help-users-gain-insights-into-their-work-patterns) para integrar dados sobre tempo gasto em atividades de trabalho, como chamadas, chats e email, para ajudar a melhorar a produtividade e o bem-estar do usuário. 


## <a name="july-2019-new-and-generally-available"></a>Julho de 2019: novo e disponível para o público geral 

### <a name="example-code-snippets"></a>Exemplo de trechos de código
Agora há trechos do código Objective-C em todos os tópicos da API nas referências v 1.0 e beta. Veja o exemplo do Objective-C de como [obter um evento](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example).

### <a name="group"></a>Grupo
- Use a função[ValidateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0) para verificar se o nome de exibição ou apelido de email de um grupo existente do Office 365 está em conformidade com as políticas de nomenclatura.
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

### <a name="mail"></a>Email
Use permissões de aplicativo mais granulares _Mail.ReadBasic.All_ para ler a caixa de correio de um usuário, com exceção de qualquer corpo de mensagem, corpo de visualização, anexos e propriedades estendidas e com exceção da pesquisa na caixa de correio. Agora aplicável a [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) e [controle de alterações](delta-query-overview.md) para [mensagem](/graph/api/resources/message?view=graph-rest-beta) e**mailFolder.**

### <a name="reports"></a>Relatórios
- Obtenha dados [adicionais de uso da caixa de correio](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta) sobre o tamanho e a contagem de itens excluídos.

### <a name="teamwork"></a>Trabalho em equipe
- [Instalar](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta), [desinstalar](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta), [atualizar ](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta) e [listar aplicativos do Microsoft Teams instalados ](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta) para um usuário. 
- Use o acesso somente para aplicativos para ler mensagens de canal, respostas a mensagens de canal e mensagens em um chat. [Solicite a aprovação](teams-protected-apis.md) para tal acesso.

## <a name="may---june-2019-new-and-generally-available"></a>Maio e julho de 2019: novo e disponível para o público geral

### <a name="calendar-mail-and-personal-contacts"></a>Calendário, email e contatos pessoais
Os administradores do Exchange podem conceder permissões de aplicativo a um aplicativo e [restringir o seu acesso apenas a um subconjunto de caixas de correio em um ](auth-limit-mailbox-access.md), ao invés do padrão, que é o acesso a todas as caixas de correio na organização. Este acesso restrito se aplicaria a quaisquer permissões de aplicativos concedidas ao aplicativo para [calendários](permissions-reference.md#calendars-permissions), [contatos](permissions-reference.md#contacts-permissions) e [configurações de email e de caixa de correio](permissions-reference.md#mail-permissions). Confira o [anúncio do blog](https://developer.microsoft.com/pt-BR/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/) relacionado.

### <a name="mail"></a>Email
Use a API de [pastas de pesquisa de email](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0) para pesquisar mensagens e acessar os resultados de pesquisa de email do Outlook. Confira o [anúncio do blog](https://developer.microsoft.com/pt-BR/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/) relacionado.

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
Obtenha [rótulos de confidencialidade](/graph/api/resources/assignedlabel?view=graph-rest-beta) para ajudar a proteger dados confidenciais de grupos do Office 365 e atender às políticas de conformidade. Esses rótulos são objetos [assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta), publicados por administradores no Centro de Conformidade e Segurança do Microsoft 365, como parte dos recursos de Proteção de Informações da Microsoft. 

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

### <a name="teamwork"></a>Trabalho em equipe
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
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/pt-BR/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).