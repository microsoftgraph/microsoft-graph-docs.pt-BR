---
title: 'accessPackageAssignmentRequest: cancel'
description: Cancele os objetos accessPackageAssignmentRequest que estão em estado cancelável.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8abc80afd455c3f5057ede358f24b4a266a1e89d
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60729672"
---
# <a name="accesspackageassignmentrequest-cancel"></a>accessPackageAssignmentRequest: cancel
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Entitlement Management,](../resources/entitlementmanagement-root.md)cancele os objetos [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) que estão em estado cancelável: `accepted` , , , `pendingApproval` `pendingNotBefore` `pendingApprovalEscalated` .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|EntitlementManagement.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de um [objeto accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)

Para que um usuário não administrador cancele sua própria solicitação, a solicitação deve conter a **id** do [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) e um **requestStatus** com um valor `cancelled` de .

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK`.  Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel

{
  "id":"request-id",
  "requestStatus":"cancelled"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackageassignmentrequest-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackageassignmentrequest-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

