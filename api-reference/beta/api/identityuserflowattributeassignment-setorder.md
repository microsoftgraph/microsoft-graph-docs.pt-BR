---
title: 'identityUserFlowAttributeAssignment: SetOrder'
description: Definir a ordem de identityUserFlowAttributeAssignments que está sendo coletada dentro de um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cc1487246f5a3370ce1b88f50eafcce7029baf4f
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752729"
---
# <a name="identityuserflowattributeassignment-setorder"></a>identityUserFlowAttributeAssignment: SetOrder

Namespace: microsoft.graph

Definir a ordem de identityUserFlowAttributeAssignments que está sendo coletada dentro de um fluxo de usuário.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|IdentityUserFlow.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|IdentityUserFlow.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/setOrder
POST /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/setOrder
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|newAssignmentOrder|[assignmentOrder](../resources/assignmentorder.md)|Usado para definir a ordem dos atributos que estão sendo coletados dentro de um fluxo de usuário.|

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_setorder"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/setOrder
Content-Type: application/json
Content-length: 90

{
  "newAssignmentOrder": {
    "order": [
        "City",
        "extension_GUID_ShoeSize"
    ]
  }
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityuserflowattributeassignment-setorder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityuserflowattributeassignment-setorder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityuserflowattributeassignment-setorder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityuserflowattributeassignment-setorder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
