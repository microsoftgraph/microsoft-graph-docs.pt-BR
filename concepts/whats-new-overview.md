---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: ae6cd9109faf46aa9ab2b55c0015f846f494a619
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/14/2020
ms.locfileid: "41119781"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Confira os destaques das novidades do Microsoft Graph e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista completa de atualizações da API, confira as seções de [dezembro](changelog.md#december-2019) e [novembro](changelog.md#november-2019) do log de alterações da API. 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.

## <a name="january-2020-new-and-generally-available"></a>Janeiro de 2020: Novo e disponível para o público geral

### <a name="security"></a>Segurança
Como parte do gerenciamento de alerta de cliente, use o método de [alerta de atualização](/graph/api/alert-update?view=graph-rest-1.0) e atualize o campo **comentários** como `Closed in IPC` ou `Closed in MCAS`.

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
Para obter relatórios de uso do Office 365 usando permissões delegadas por um usuário, os administradores devem ter atribuído ao usuário uma função de administrador limitado do Azure AD. Podendo ser uma das seguintes funções: administrador da empresa, administrador do Exchange, administrador do SharePoint, administrador do Lync, leitor global ou leitor de relatórios. Para mais detalhes, confira [Autorização para APIs lerem os relatórios de uso do Office 365](reportroot-authorization.md).

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

### <a name="teamwork"></a>Trabalho em equipe
- [Configure as notificações que incluem dados de recursos](webhooks-with-resource-data.md) para recursos do [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) nos canais e bate-papos do Microsoft Teams.
- [Assine as notificações](/graph/api/resources/subscription?view=graph-rest-beta) de [mensagens de canal ou de bate-papo](/graph/api/resources/chatmessage?view=graph-rest-beta) novas ou modificadas.
- Use o recurso [shiftPreferences](/graph/api/resources/shiftpreferences?view=graph-rest-beta) para permitir que a especificação da disponibilidade de um usuário seja atribuída a turnos em um [cronograma](/graph/api/resources/schedule?view=graph-rest-beta). Obtenha ou defina isso como parte das [configurações](/graph/api/resources/usersettings?view=graph-rest-beta) do usuário.


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

