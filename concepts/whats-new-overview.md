---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 5a69232c58469f09e953af9e9d06667509a76568
ms.sourcegitcommit: a700f1c283a5d847cd1697e26bcd47bc8625384e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2019
ms.locfileid: "36049614"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Você sabia que alguns dos novos recursos do Microsoft Graph se originam de solicitações populares da comunidade de desenvolvedores? 

A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

1. Estreia no status de visualização **_prévia_**. As atualizações da API REST relacionadas estão no ponto de extremidade (`https://graph.microsoft.com/beta`). Os recursos no modo de visualização podem ser alterados sem aviso. Não use-os em aplicativos de produção. 

2. Promovido para status de**_disponibilidade geral_ (DG)**, se um feedback suficiente indicar a viabilidade.. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). Use somente os recursos do status do GA em aplicativos de produção.

Vamos percorrer o que há de novo no Microsoft Graph e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para detalhes sobre as atualizações da API, consulte as seções de [maio](changelog.md#may-2019), [junho](changelog.md#june-2019) e [julho](changelog.md#july-2019) do changelog. 

## <a name="new-and-generally-available-released-may---july-2019"></a>Novo e disponível para o público em geral (lançado em maio - julho de 2019)

### <a name="calendar-mail-and-personal-contacts"></a>Calendário, email e contatos pessoais
Os administradores do Exchange podem conceder permissões de aplicativo a um aplicativo e [restringir o seu acesso apenas a um subconjunto de caixas de correio em um ](auth-limit-mailbox-access.md), ao invés do padrão, que é o acesso a todas as caixas de correio na organização. Este acesso restrito se aplicaria a quaisquer permissões de aplicativos concedidas ao aplicativo para [calendários](permissions-reference.md#calendars-permissions), [contatos](permissions-reference.md#contacts-permissions) e [configurações de email e de caixa de correio](permissions-reference.md#mail-permissions). Confira o [anúncio do blog](https://developer.microsoft.com/en-us/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/) relacionado.

### <a name="example-code-snippets"></a>Exemplo de trechos de código
Além do C# e do JavaScript, agora há trechos de código do Objective-C em todos os tópicos da API nas referências v1.0 e beta. Veja o exemplo do Objective-C de como [obter um evento](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example).

### <a name="group"></a>Grupo
- Use a função[ValidateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0) para verificar se o nome de exibição ou apelido de email de um grupo existente do Office 365 está em conformidade com as políticas de nomenclatura.
- Como alternativa, antes de criar o grupo, você pode usar a função[ ValidateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0)para um[directoryobject](/graph/api/resources/directoryobject?view=graph-rest-1.0) para validar primeiro os nomes.

### <a name="identity-and-access"></a>Identidade e acesso
- Use as [novas permissões delegadas e de aplicativo](permissions-reference.md#organization-permissions), _Organization.Read.All_ e _Organization.ReadWrite.All_ para acessar uma [organização](/graph/api/resources/organization?view=graph-rest-1.0) e recursos relacionados, como [SKUs inscritos](/graph/api/resources/subscribedsku?view=graph-rest-1.0).
- Use [novas permissões delegadas e de aplicativo ](permissions-reference.md#role-management-permissions), _RoleManagement. Read.Directory _ e_RoleManagement. ReadWrite.Directory_, para controle de acesso baseado em função ( RBAC) para o diretório da empresa:

  - Use a permissão de leitura/gravação para [ativar](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0) primeiro uma função de diretório. 
  - Com a função ativada, você pode usar a permissão de leitura para[ler funções de diretório](/graph/api/directoryrole-list?view=graph-rest-1.0), [listar os membros da função](/graph/api/directoryrole-list-members?view=graph-rest-1.0) e [listar modelos de função de diretório](/graph/api/directoryroletemplate-list?view=graph-rest-1.0). 
  - Você também pode usar a permissão de leitura/gravação para[adicionar](/graph/api/directoryrole-post-members?view=graph-rest-1.0)e [remover](/graph/api/directoryrole-delete-member?view=graph-rest-1.0) membros da função. 

### <a name="mail"></a>Email
Use a API de [pastas de pesquisa de email](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0) para pesquisar mensagens e acessar os resultados de pesquisa de email do Outlook. Confira o [anúncio do blog](https://developer.microsoft.com/en-us/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/) relacionado.

### <a name="postman"></a>Postman
Como uma alternativa ao Explorador do Graph, experimente a API do Microsoft Graph na [coleção do Microsoft Graph Postman](use-postman.md) para aprender o comportamento da API e acelerar o desenvolvimento de aplicativos.

### <a name="tutorials"></a>Tutoriais
Experimente o novo [tutorial para criar um aplicativo de console do Java](/graph/tutorials/java) para obter informações sobre um calendário de usuário.

### <a name="user"></a>Usuário
Administradores ou usuários podem [revogar](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) todos os tokens de atualização emitidos para um usuário. Isso geralmente é usado para impedir que aplicativos em um dispositivo perdido ou roubado acessem os dados de uma organização.


## <a name="new-in-preview-released-may---july-2019"></a>Novidades na visualização (lançado em maio - junho de 2019)

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use-os em aplicativos de produção.

### <a name="calendar"></a>Calendário 
Use a nova [API de locais](/graph/api/resources/place?view=graph-rest-beta) para usar vários tipos de locais, como [salas](/graph/api/resources/room?view=graph-rest-beta) e [lista de salas](/graph/api/resources/roomlist?view=graph-rest-beta), conforme configurado pelos administradores do Exchange Online.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
- Atualizações de [maio](changelog.md#may-2019) do Intune 
- Atualizações de [junho](changelog.md#june-2019) do Intune
- Atualizações de [julho](changelog.md#july-2019) do Intune

### <a name="education"></a>Educação
- Consulta Delta para um objeto [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta).
- Consulta Delta e adições de propriedade para objetos [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta) e [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta).

### <a name="files"></a>Arquivos 
Aplique a data/hora de vencimento ou a senha ao [criar um link de compartilhamento](/graph/api/driveitem-createlink?view=graph-rest-beta) para um arquivo, pasta, ou outros [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta).

### <a name="group"></a>Grupo
Obtenha [rótulos de confidencialidade](/graph/api/resources/assignedlabel?view=graph-rest-beta) para ajudar a proteger dados confidenciais de grupos do Office 365 e atender às políticas de conformidade. Esses rótulos são objetos [assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta), publicados por administradores no Centro de Conformidade e Segurança do Microsoft 365, como parte dos recursos de Proteção de Informações da Microsoft. 

### <a name="identity-and-access"></a>Identidade e acesso
- Obtenha uma instância de um [aplicativo](/graph/api/resources/applicationtemplate?view=graph-rest-beta) ou adicione uma instância da galeria de aplicativos do Azure AD ao seu diretório como modelo.
- Obtenha um log de todos os diretórios de[eventos de provisionamento](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta) em um locatário.
- Use a nova função[descobrir](/graph/api/directorydefinition-discover?view=graph-rest-beta) para encontrar o [esquema de sincronização](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta)de diretório mais recente, para sincronizar objetos de diretório, atributos e seus tipos de um aplicativo.
- Obtenha informações sobre [usuário detectado ou riscos de login](/graph/api/resources/riskdetection?view=graph-rest-beta) em um ambiente do Azure AD. Esta funcionalidade de detecção de riscos faz parte do Azure AD Identity Protection.
- Use [novas permissões delegadas e de aplicativo ](permissions-reference.md#administrative-units-permissions),_AdministrativeUnit.Read.All _ e _AdministrativeUnit. ReadWrite.All_, para ler ou gravar respectivamente (incluindo criar, atualizar, excluir ou gerenciar a associação) recursos[unidade de administração](/graph/api/resources/administrativeunit?view=graph-rest-beta). 
- Use as [novas permissões delegadas e de aplicativo](permissions-reference.md#organization-permissions), _Organization.Read.All_ e _Organization.ReadWrite.All_ para acessar uma [organização](/graph/api/resources/organization?view=graph-rest-beta) e recursos relacionados, como [SKUs inscritos](/graph/api/resources/subscribedsku?view=graph-rest-beta).

### <a name="mail"></a>Email
Use permissões delegadas mais granulares _Mail.ReadBasic_ e permissão de aplicativo _Mail.ReadBasic.All_, para ler a caixa de correio de um usuário, com exceção de qualquer corpo de mensagem, corpo de visualização, anexos e Propriedades estendidas e com exceção da pesquisa na caixa de correio. Disponibilizado anteriormente para [lista](/graph/api/user-list-messages?view=graph-rest-beta) e [recebo](/graph/api/message-get?view=graph-rest-beta) uma mensagem, agora também aplicável a [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) e [alterar as notificações ](webhooks.md) para [mensagem](/graph/api/resources/message?view=graph-rest-beta) e **mailFolder**. 

### <a name="microsoft-graph-toolkit"></a>Kit de ferramentas do Microsoft Graph
O [kit de ferramentas do Microsoft Graph](/graph/toolkit/overview) é um conjunto de colaboradores e de componentes da Web de estrutura independente que oferece conveniência para autenticar e acessar dados no Microsoft Graph. Como o kit de ferramentas do Microsoft Graph está no status de visualização, use provedores e componentes do kit de ferramentas somente em aplicativos que não são de produção.

### <a name="reports"></a>Relatórios
- Obtenha [relatórios sobre os métodos de autenticação](/graph/api/resources/authenticationmethods-usage-insights-overview?view=graph-rest-beta) adotados pelos usuários em uma organização, como rest de senha de autoatendimento e autenticação multifator (MFA).
- Obtenha dados [adicionais de uso da caixa de correio](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta) sobre o tamanho e a contagem de itens excluídos.

### <a name="sites"></a>Sites
Permitir que os usuários [sigam](/graph/api/site-follow?view=graph-rest-beta) ou [parem de seguir](/graph/api/site-unfollow?view=graph-rest-beta) os sites do SharePoint.

### <a name="teamwork"></a>Trabalho em equipe
- Hospede [imagens](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta) em [mensagens de bate-papo](/graph/api/resources/chatmessage?view=graph-rest-beta) do Microsoft Teams.
- Suporte para [configurar](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta) como uma equipe privada pode ser descoberta.
- [Instalar](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta), [desinstalar](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta), [atualizar ](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta) e [lista instalar aplicativos do Microsoft Teams ](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta) para um usuário. 
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

