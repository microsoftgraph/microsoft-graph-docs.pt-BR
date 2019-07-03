---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 416ba84527957b59ad4f8ff9e6d8c0194d60f245
ms.sourcegitcommit: ee710ff556f4a7907181df5c323e345f52808ce2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35420423"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Você sabia que alguns dos novos recursos do Microsoft Graph se originam de solicitações populares da comunidade de desenvolvedores? 

Neste artigo, percorreremos o ciclo de vida típico de um novo recurso, o que há de novo no Microsoft Graph e como você pode [compartilhar as suas ideias](#want-to-stay-in-the-loop).

## <a name="life-cycle-of-a-feature"></a>Ciclo de vida de um recurso

Os proprietários de serviço do Microsoft Graph avaliam periodicamente as ideias de recursos e as necessidades dos clientes para oferecer novos cenários de suporte. Para criar um novo recurso, eles podem adicionar ou atualizar as APIs REST. Eles podem manter a mesma sintaxe da API e estender o comportamento dos recursos. Ou, eles podem oferecer uma experiência melhor de aprendizado ou desenvolvimento.

Na maioria dos casos, os proprietários de serviço lançam novos recursos na seguinte ordem:

1. Estreia no status de **_visualização_**, o que significa que o comportamento do recurso pode mudar sem aviso prévio. O proprietário expõe quaisquer adições ou atualizações relacionadas à API REST no ponto de extremidade beta (`https://graph.microsoft.com/beta`). Não use recursos de visualização, incluindo as APIs, em aplicativos de produção.

2. Se um proprietário de serviço receber comentários suficientes e considerar o recurso viável, o proprietário poderá promover o recurso para o status **_disponibilidade geral_ (DG)**. O proprietário também inclui quaisquer adições ou atualizações da API relacionadas ao ponto de extremidade v1.0 (`https://graph.microsoft.com/v1.0`). Você pode usar o recurso (incluindo as APIs) no status DG em aplicativos de produção.

As seções a seguir destacam as novidades de maio e junho de 2019. Para detalhes sobre as atualizações da API, consulte as seções de [maio](changelog.md#may-2019) e [junho](changelog.md#june-2019) do changelog. 

## <a name="new-and-generally-available-released-may---june-2019"></a>Novo e disponível para o público em geral (lançado em maio - junho de 2019)

### <a name="calendar-mail-and-personal-contacts"></a>Calendário, email e contatos pessoais
Os administradores do Exchange podem conceder permissões de aplicativo a um aplicativo e [restringir o seu acesso apenas a um subconjunto de caixas de correio em um ](auth-limit-mailbox-access.md), ao invés do padrão, que é o acesso a todas as caixas de correio na organização. Este acesso restrito se aplicaria a quaisquer permissões de aplicativos concedidas ao aplicativo para [calendários](permissions-reference.md#calendars-permissions), [contatos](permissions-reference.md#contacts-permissions) e [configurações de email e de caixa de correio](permissions-reference.md#mail-permissions). Confira o [anúncio do blog](https://developer.microsoft.com/en-us/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/) relacionado.

### <a name="example-code-snippets"></a>Exemplo de trechos de código
Além do C# e do JavaScript, agora há trechos de código do Objective-C em todos os tópicos da API nas referências v1.0 e beta. Veja o exemplo do Objective-C de como [obter um evento](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example).

### <a name="mail"></a>Email
Use a API de [pastas de pesquisa de email](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0) para pesquisar mensagens e acessar os resultados de pesquisa de email do Outlook. Confira o [anúncio do blog](https://developer.microsoft.com/en-us/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/) relacionado.

### <a name="postman"></a>Postman
Como uma alternativa ao Explorador do Graph, experimente a API do Microsoft Graph na [coleção do Microsoft Graph Postman](use-postman.md) para aprender o comportamento da API e acelerar o desenvolvimento de aplicativos.

### <a name="tutorials"></a>Tutoriais
Experimente o novo [tutorial para criar um aplicativo de console do Java](/graph/tutorials/java) para obter informações sobre um calendário de usuário.

### <a name="user"></a>Usuário
Administradores ou usuários podem [revogar](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) todos os tokens de atualização emitidos para um usuário. Isso geralmente é usado para impedir que aplicativos em um dispositivo perdido ou roubado acessem os dados de uma organização.


## <a name="new-in-preview-released-may---june-2019"></a>Novidades em visualização (lançado em maio - junho de 2019)

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use-os em aplicativos de produção.

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
- Obtenha uma lista de todos os [eventos de provisionamento](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta) em um locatário.
- Obtenha informações sobre [usuário detectado ou riscos de login](/graph/api/resources/riskdetection?view=graph-rest-beta) em um ambiente do Azure AD. Esta funcionalidade de detecção de riscos faz parte do Azure AD Identity Protection.

### <a name="mail"></a>Email
Use a [permissão Mail.ReadBasic](permissions-reference.md#mail-permissions) na API [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) e nas [notificações de alteração](webhooks.md) para [mensagem](/graph/api/resources/message?view=graph-rest-beta) e **mailFolder**.

### <a name="microsoft-graph-toolkit"></a>Kit de ferramentas do Microsoft Graph
O [kit de ferramentas do Microsoft Graph](/graph/toolkit/overview) é um conjunto de colaboradores e de componentes da Web de estrutura independente que oferece conveniência para autenticar e acessar dados no Microsoft Graph. Como o kit de ferramentas do Microsoft Graph está no status de visualização, use provedores e componentes do kit de ferramentas somente em aplicativos que não são de produção.

### <a name="sites"></a>Sites
Permitir que os usuários [sigam](/graph/api/site-follow?view=graph-rest-beta) ou [parem de seguir](/graph/api/site-unfollow?view=graph-rest-beta) os sites do SharePoint.

### <a name="teamwork"></a>Trabalho em equipe
Hospede [imagens](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta) em [mensagens de bate-papo](/graph/api/resources/chatmessage?view=graph-rest-beta) do Microsoft Teams.
Suporte para [configurar](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta) como uma equipe privada pode ser descoberta.


## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?
- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Office 365](https://developer.microsoft.com/pt-BR/office/dev-program), obtenha uma assinatura gratuita do Office 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/en-us/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).

