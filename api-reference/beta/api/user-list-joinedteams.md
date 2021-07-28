---
title: Listar joinedTeams
description: Obtenha as equipes do Microsoft Teams das quais o usuário é um membro direto.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0f340b92dc0da0cdceedb3cd5b6a15019e0ab386
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580923"
---
# <a name="list-joinedteams"></a>Listar joinedTeams

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha as [equipes](../resources/team.md) do Microsoft Teams das quais o usuário é um membro direto.
 
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

> **Observação:** atualmente, com as permissões delegadas pelo usuário, essa operação só funcionará para o usuário `me`. Com as permissões de aplicativo, ela funciona para todos os usuários especificando a ID de usuário específica (a alias`me` não é suportada com as permissões de aplicativo). Para mais detalhes, confira [Problemas conhecidos](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview).

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
GET /users/{id | user-principal-name}/joinedTeams
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
No momento, esse método não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Aceitar  | application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos da[equipe](../resources/team.md) no corpo da resposta.

> [!Note]
> Atualmente, essa chamada à API retorna apenas as propriedades **ID**, **displayName** e **description** de uma [equipe](../resources/team.md). Para obter todas as propriedades, use a operação[Obter equipe](../api/team-get.md). Para saber mais, confira [problemas conhecidos](/graph/known-issues#unable-to-return-all-values-for-properties-for-a-user-joined-teams).

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
O exemplo a seguir mostra uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/joinedTeams
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-joinedteams-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-joinedteams-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-joinedteams-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-joinedteams-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Resposta
O exemplo a seguir mostra a resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "172b0cce-e65d-44ce-9a49-91d9f2e8493a",
      "displayName": "Contoso Team",
      "description": "This is a Contoso team, used to showcase the range of properties supported by this API"
    }
  ]
}
```

## <a name="see-also"></a>Confira também
- [Listar todas as equipes](/graph/teams-list-all-teams)
- [Obter equipe](../api/team-get.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
