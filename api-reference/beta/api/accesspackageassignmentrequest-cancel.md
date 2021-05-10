---
title: 'accessPackageAssignmentRequest: cancel'
description: Cancele os objetos accessPackageAssignmentRequest que estão em estado cancelável.
localization_priority: Normal
author: sbounouh
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5079de33f7ef3c7536baf50a876a84d5ca3711b4
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299014"
---
# <a name="accesspackageassignmentrequest-cancel"></a>accessPackageAssignmentRequest: cancel
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Entitlement Management,](../resources/entitlementmanagement-root.md)cancele os objetos [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) que estão em estado cancelável: `accepted` , , , `pendingApproval` `pendingNotBefore` `pendingApprovalEscalated` .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|EntitlementManagement.ReadWrite.All |
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
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


### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

