---
title: 'accessPackageAssignmentRequest: reprocessar'
description: Reprocessar objetos accessPackageAssignmentRequest.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
---

# <a name="accesspackageassignmentrequest-reprocess"></a>accessPackageAssignmentRequest: reprocessar

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [gerenciamento de direitos do Azure AD](../resources/entitlementmanagement-overview.md), os chamadores podem repetir automaticamente a solicitação de acesso de um usuário a um pacote de acesso. Ele é executado em um [objeto accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) cuja **requestState** está em um `DeliveryFailed` ou `PartiallyDelivered` estado. 

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | EntitlementManagement.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | EntitlementManagement.ReadWrite.All |
  
## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/reprocess
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um  `202 Accepted` código de resposta e recupera a solicitação. Se o [objeto accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) não existir, `404 Not Found` esse método retornará ou se a **id** não for válida, este método retornará um `400 Bad Request` código de resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "ignored",
  "name": "reprocess_accesspackageassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/d82eb508-acc4-43cc-bcf1-7c1c4a2c073b/reprocess
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted  
```
