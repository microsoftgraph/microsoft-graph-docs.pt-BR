---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 4840dbb711f2088f011c5c66d6c59d47d58145af
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622625"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Você sabia que alguns dos novos recursos do Microsoft Graph se originam de solicitações populares da comunidade de desenvolvedores? 

A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

1. Estreia no status de visualização **_prévia_**. As atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

2. Promovido para o status de**_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 

Abaixo, veja o que há de novo no Microsoft Graph e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para detalhes sobre as atualizações da API, consulte as seções de [Agosto](changelog.md#august-2019) e [Julho](changelog.md#july-2019) do log de alterações da API. 


## <a name="august-2019-new-and-generally-available"></a>Agosto de 2019: Novo e disponível para o público geral 

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

## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?
- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Office 365](https://developer.microsoft.com/pt-BR/office/dev-program), obtenha uma assinatura gratuita do Office 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/en-us/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).

