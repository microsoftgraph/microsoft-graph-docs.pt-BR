---
title: Conceder um appRoleAssignment a um grupo
description: Conceder uma atribuição de função de aplicativo a um grupo.
ms.localizationpriority: high
doc_type: apiPageType
ms.prod: groups
author: psignoret
ms.openlocfilehash: 542fa5608096e5c46f0f0dc2691870b63f2ef332
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015220"
---
# <a name="grant-an-approleassignment-to-a-group"></a>Conceder um appRoleAssignment a um grupo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use esta API para atribuir uma função de aplicativo a um grupo. Todos os membros diretos do grupo serão considerados atribuídos. Para conceder uma atribuição de função de aplicativo a um grupo, você precisa de três identificadores:

- `principalId`: A `id` do grupo ao qual você está atribuindo a função de aplicativo.
- `resourceId`: A `id` do recurso `servicePrincipal` que definiu a função do aplicativo.
- `appRoleId`: A `id` do `appRole` (definido na entidade de serviço do recurso) para atribuir ao grupo.

Licenças adicionais podem ser necessárias para [usar um grupo para gerenciar o acesso aos aplicativos](/azure/active-directory/users-groups-roles/groups-saasapps).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | AppRoleAssignment.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/appRoleAssignments
```

> [!NOTE]
> Como prática recomendada, recomendamos que você crie atribuições de função de aplicativo por meio da `appRoleAssignedTo`relação do _recurso_ da entidade de serviço, em vez da `appRoleAssignments`relação do usuário, grupo ou entidade de serviço atribuída.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:----------|
| Autorização | {token} de portador. Obrigatório.  |
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON de um objeto [appRoleAssignment](../resources/approleassignment.md).

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment_1"
}-->

```http
POST https://graph.microsoft.com/beta/groups/7679d9a4-2323-44cd-b5c2-673ec88d8b12/appRoleAssignments
Content-Type: application/json

{
  "principalId": "7679d9a4-2323-44cd-b5c2-673ec88d8b12",
  "resourceId": "076e8b57-bac8-49d7-9396-e3449b685055",
  "appRoleId": "00000000-0000-0000-0000-000000000000"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-create-approleassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-create-approleassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-create-approleassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-create-approleassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-create-approleassignment-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


Neste exemplo, `{id}` e `{principalId-value}` seriam os `id` do grupo atribuído.

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('7679d9a4-2323-44cd-b5c2-673ec88d8b12')/appRoleAssignments/$entity",
  "id": "pNl5diMjzUS1wmc-yI2LEkGgWqFFrFdLhG2Ly2CysL4",
  "deletedDateTime": null,
  "appRoleId": "00000000-0000-0000-0000-000000000000",
  "creationTimestamp": "2021-02-19T17:55:08.3369542Z",
  "principalDisplayName": "Young techmakers",
  "principalId": "7679d9a4-2323-44cd-b5c2-673ec88d8b12",
  "principalType": "Group",
  "resourceDisplayName": "Yammer",
  "resourceId": "076e8b57-bac8-49d7-9396-e3449b685055"
}
```

Neste exemplo, observe que o valor usado como a **id** do usuário na URL de solicitação (`cde330e5-2150-4c11-9c5b-14bfdc948c79`) é o mesmo que a propriedade **principalId** no corpo.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
