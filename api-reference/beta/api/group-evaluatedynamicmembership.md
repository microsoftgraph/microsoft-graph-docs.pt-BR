---
title: 'group: evaluateDynamicMembership'
description: Avalie se um usuário ou dispositivo é ou seria membro de um grupo dinâmico.
author: Jordanndahl
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2ca43d71c14cd8468b387444651d79d56f298bd4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034352"
---
# <a name="group-evaluatedynamicmembership"></a>group: evaluateDynamicMembership

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Avaliar se um usuário ou dispositivo é ou seria membro de um grupo dinâmico. A regra de associação é retornada juntamente com outros detalhes que foram usados na avaliação. Você pode concluir essa operação das seguintes maneiras: 

- Avalie se um usuário ou dispositivo é membro de um grupo dinâmico especificado.  
- Avalie se um usuário ou dispositivo seria membro de um grupo dinâmico com base na ID do usuário ou dispositivo e uma regra de associação.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

### <a name="evaluate-dynamic-membership-with-member-id-and-group-id"></a>Avaliar a associação dinâmica com a ID do membro e a ID do grupo

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
| :-------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante) | Para usuário: Group.Read.All e User.Read.All, Directory.Read.All<br>Para dispositivo: Group.Read.All e Device.Read.All, Directory.Read.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

### <a name="evaluate-dynamic-membership-with-member-id-and-membership-rule"></a>Avaliar a associação dinâmica com a ID do membro e a regra de associação

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
| :-------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante) | Para usuário: User.Read.All, Directory.Read.All<br>Para dispositivo: Device.Read.All, Directory.Read.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/evaluateDynamicMembership
POST /groups/evaluateDynamicMembership
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome | Descrição |
| :--- | :---------- |
| Autorização | Portador {token} |
| Content-type  | application/json |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece as propriedades necessárias.

A tabela a seguir lista as propriedades necessárias ao avaliar a associação ao grupo.

| Parâmetro | Tipo | Descrição |
| :-------- | :--- | :---------- |
| memberId | Conjunto de cadeias de caracteres | memberId é a ID do objeto do usuário ou dispositivo a ser avaliado. |
| membershipRule | Conjunto de cadeias de caracteres | A regra usada para avaliação de associação. Se essa propriedade não for fornecida, a regra do grupo existente será avaliada. Se essa propriedade for fornecida, o usuário ou dispositivo será avaliado para possível associação em um grupo com a mesma regra. Para obter mais informações, consulte [Regras de associação dinâmicas para grupos em Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership).|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [evaluateDynamicMembershipResult.](../resources/evaluatedynamicmembershipresult.md)

## <a name="examples"></a>Exemplos

### <a name="example-1-evaluate-if-a-user-or-device-is-a-member-of-an-existing-group"></a>Exemplo 1: Avaliar se um usuário ou dispositivo é membro de um grupo existente

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership_1"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/evaluateDynamicMembership 
Content-type: application/json

{ 
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-evaluatedynamicmembership-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")",
  "membershipRuleEvaluationResult": true,
  "membershipRuleEvaluationDetails": {
    "expressionResult": true,
    "expression": "user.displayName -startsWith \"EndTestUser\"",
    "propertyToEvaluate": {
      "propertyName": "displayName",
      "propertyValue": "EndTestUser001"
    }
  }
}

```

### <a name="example-2-evaluate-if-a-user-or-device-would-be-a-member-of-a-group-based-on-a-membership-rule"></a>Exemplo 2: Avaliar se um usuário ou dispositivo seria um membro de um grupo com base em uma regra de associação

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership_2"
}-->

```http
POST https://graph.microsoft.com/beta/groups/evaluateDynamicMembership 
Content-type: application/json

{ 
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33",
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-evaluatedynamicmembership-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")",
  "membershipRuleEvaluationResult": true,
  "membershipRuleEvaluationDetails": {
    "expressionResult": true,
    "expression": "user.displayName -startsWith \"EndTestUser\"",
    "propertyToEvaluate": {
      "propertyName": "displayName",
      "propertyValue": "EndTestUser001"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "group: evaluateDynamicMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
