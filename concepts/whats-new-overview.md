---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 69cc7d0ba5232770bb3b014690991ffefff6df02
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597169"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](changelog.md). 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.

## <a name="december-2020-new-and-generally-available"></a>Dezembro de 2020: Novo e disponível para o público geral

### <a name="cloud-communications"></a>Comunicações na nuvem
GA do recurso [presença](/graph/api/resources/presence), permitindo obter as informações de presença de um ou mais usuários.

### <a name="teamwork"></a>Trabalho em equipe
- GA da [API para gerenciar a instalação do aplicativo Teams](/graph/api/resources/teamsappinstallation), incluindo a instalação de aplicativos ou a adição, a remoção ou a atualização do aplicativo em uma equipe ou no escopo pessoal de um usuário.
- [Obtenha um chat entre um usuário e um aplicativo do Teams](/graph/api/userscopeteamsappinstallation-get-chat).

## <a name="december-2020-new-in-preview-only"></a>Dezembro de 2020: Novidades somente na pré-visualização

### <a name="identity-and-access"></a>Identidade e acesso
Obtenha ou defina os metadados de versão e criação de um Azure AD [termos de uso](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true) [contrato](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true), [arquivo de contrato](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true) e [agreementfilelocalization](/graph/api/resources/agreementfilelocalization?view=graph-rest-beta&preserve-view=true)

## <a name="november-2020-new-and-generally-available"></a>Novembro de 2020: Novo e geralmente disponível

### <a name="cloud-communications"></a>Comunicações na nuvem
- O GA da propriedade **função** do tipo [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo), que distingue a função de um participante em uma [reunião online](/graph/api/resources/onlinemeeting) como um participante ou apresentador.
- O GA da propriedade **lobbyBypassSettings** e seus [valores](/graph/api/resources/lobbybypasssettings#lobbybypassscope-values) para admitir usuários para uma reunião online.
- O GA da propriedade **isEntryExitAnnounced** para personalizar as configurações de apresentação de autores de chamada ou de sair de uma reunião online.
- O GA da propriedade **allowedPresenters** para permitir apresentadores específicos na reunião.

### <a name="search"></a>Pesquisar
- O GA da [consulta da API](/graph/api/resources/search-api-overview) Pesquisa da Microsoft, oferecendo suporte à pesquisa em escopo dos seguintes tipos de dados:
  - [Mensagens do Outlook](/graph/search-concept-messages)
  - [Eventos do calendário do Outlook](/graph/search-concept-events)
  - [Recursos do Microsoft OneDrive e do Microsoft Office SharePoint Online](/graph/search-concept-files).

### <a name="teamwork"></a>Trabalho em equipe

- GA de permissões de consentimento específicas de recurso (RSC). As permissões RSC permitem que os proprietários da equipe concedam consentimento granular a um aplicativo de produção para acessar e/ou modificar dados específicos de uma equipe, como por exemplo, ler as configurações da equipe ou modificar nomes de canal, descrições e outras configurações.
- GA de APIs que se aplicam a um [canal](/graph/api/resources/channel) ou mensagens dentro de um canal. As APIs incluem:
  - [Criar](/graph/api/conversationmember-add) ou [excluir](/graph/api/conversationmember-delete) um membro de conversa de um canal.
  - [Atualizar a função de um membro](/graph/api/conversationmember-update) em um canal.
  - Receber uma mensagem específica ou todas as mensagens em um canal.
  - Receber uma resposta específica ou todas as respostas em um canal.
  - [Acompanhar mensagens novas ou atualizadas em um canal](/graph/api/chatmessage-delta).


## <a name="november-2020-new-in-preview-only"></a>Novembro de 2020: Novidades somente na pré-visualização

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
Estreia da [API de computador na nuvem](/graph/api/resources/virtualendpoint?view=graph-rest-beta&preserve-view=true) que permite que as organizações provisionem e gerenciem as máquinas virtuais para os funcionários. Use-o em conjunto com a API do Intune para gerenciar os pontos de extremidade físicos e virtuais.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
[Inscreva-se para alterar as notificações](webhooks.md) em uma [definição de tarefa de impressão](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gestão corporativa
As atualizações de [Novembro](changelog.md#november-2020) do Intune para a versão beta.

### <a name="identity-and-access"></a>Identidade e acesso
- Especificar URLs para envio de tokens de entrada de usuário e URIs de códigos de autorização e tokens de acesso, na propriedade **spa** de [aplicativo](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true).
- Personalize a aparência das telas de entrada do Azure Active Directory usando as [propriedades de identidade visual organização](/graph/api/resources/organizationalbrandingproperties?view=graph-rest-beta&preserve-view=true). As organizações podem personalizar com base na localidade para usuários específicos.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
A estreia da [API de revisão de acesso para a associação de grupo](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) para revisar regularmente o acesso de usuários, certifique-se de que apenas as pessoas certas tenham acesso contínuo e gerenciem os membros do grupo de forma eficiente.

### <a name="search"></a>Pesquisar
Você pode agregar resultados de pesquisa de tipo numérico ou cadeia de caracteres que são importados por [conectores do Microsoft Graph](/microsoftsearch/connectors-overview) e que são configurados para serem refináveis no [esquema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true). Veja mais informações sobre [refinar resultados de pesquisa usando agregações](search-concept-aggregation.md).


## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de visualização **_prévia_**. As atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de **_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/office/dev-program), ganhe uma assinatura gratuita do Microsoft 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).
