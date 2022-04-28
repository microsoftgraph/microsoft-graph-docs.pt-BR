---
title: Trabalhar com usuários no Microsoft Graph
description: Crie experiências atraentes para aplicativos baseadas nos usuários, suas relações com outros usuários e grupos, seus emails, calendários e arquivos.
ms.localizationpriority: high
author: jpettere
ms.prod: users
doc_type: conceptualPageType
ms.openlocfilehash: 2f36771ccc92bfec6fd4aeb723891a3a712c6269
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65059967"
---
# <a name="working-with-users-in-microsoft-graph"></a>Trabalhar com usuários no Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode usar o Microsoft Graph para criar experiências de aplicativo atraentes com base em usuários, suas relações com outros usuários e grupos e os recursos que eles acessam como, por exemplo, seus emails, calendários, arquivos, funções administrativas e associações de grupo.

Você pode acessar usuários pelo Microsoft Graph de duas maneiras:

- Por sua ID, `/users/{id}`
- Usando o alias `/me` para o usuário conectado, que é igual a `/users/{signed-in user's id}`

Há dois tipos de usuários no Azure AD: membros e usuários convidados. Os usuários convidados ingressam na organização por meio do resgate de seu convite. Os usuários convidados podem ser convertidos em membros para aproveitar todos os privilégios dos membros.

## <a name="authorization"></a>Autorização

Uma das seguintes [permissões](/graph/permissions-reference) é necessária para acessar operações de usuário. As três primeiras permissões podem ser concedidas a um aplicativo por um usuário. O restante só pode ser concedido a um aplicativo pelo administrador.

- User.ReadBasic.All
- User.Read
- User.ReadWrite
- User.Read.All
- User.ReadWrite.All
- User.ManageIdentities.All
- Directory.Read.All
- Directory.ReadWrite.All
- Directory.AccessAsUser.All

## <a name="user-and-group-search-limitations-for-guest-users-in-organizations"></a>Limitações de pesquisa de usuário e grupo para usuários convidados em organizações

Os recursos de pesquisa de usuário e grupo permitem que o aplicativo pesquise qualquer usuário ou grupo no diretório de uma organização, executando consultas no conjunto de recursos `/users` ou `/groups` (por exemplo, `https://graph.microsoft.com/v1.0/users`). Tanto administradores quanto usuários têm esse recurso. No entanto, os usuários convidados não.

Se o usuário conectado for um convidado, dependendo das permissões que recebeu um aplicativo, ele pode ler o perfil de um usuário específico ou grupo (por exemplo, `https://graph.microsoft.com/v1.0/users/241f22af-f634-44c0-9a15-c8cd2cea5531`). No entanto, o usuário não pode executar consultas no conjunto de recursos `/users` ou `/groups` que, potencialmente, retornam mais de um recurso.

Com as permissões apropriadas, o aplicativo pode ler os perfis de usuários ou grupos que ele obtém seguindo os links nas propriedades de navegação. Por exemplo, `/users/{id}/directReports` ou `/groups/{id}/members`.

Para obter mais informações sobre limitações de pesquisa para usuários convidados, consulte [Comparar permissões padrão de membro e convidado](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions).

## <a name="common-properties"></a>Propriedades comuns

| Propriedade | Descrição |
|----------|-------------|
| displayName | O nome exibido no catálogo de endereços do usuário.|
|givenName| O nome do usuário. |
|surname| O sobrenome do usuário. |
|email| O endereço de email do usuário. |
|photo| A foto de perfil do usuário. |

Para obter detalhes e uma lista de todas as propriedades, confira o objeto [user](user.md).

## <a name="common-operations"></a>Operações comuns

>**Observação:** Algumas destas operações exigem permissões adicionais.

| Caminho    | Descrição |
|---------|-------------|
|[`/users`](../api/user-list.md) | Lista os usuários na organização. |
|[`/users/{id}`](../api/user-get.md) | Obtém um usuário específico pela id. |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| Obtém a foto de perfil do usuário. |
|[`/users/{id}/manager`](../api/user-list-manager.md) | Obtém o gerente do usuário. |
|[`/users/{id}/messages`](../api/user-list-messages.md)| Lista as mensagens de email do usuário em sua caixa de entrada principal. |
|[`/users/{id}/events`](../api/user-list-events.md) | Lista os eventos futuros do usuário em seu calendário. |
|[`/users/{id}/drive`](../api/drive-get.md)| Obtém o repositório de arquivos do OneDrive do usuário. |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| Lista os grupos dos quais o usuário é membro. |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| Lista as Microsoft Teams das quais o usuário é membro. |

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.