---
title: 'accessPackageAssignmentRequest: reprocessar'
description: Reprocessar objetos accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 36dd0d9d3e004d916e508b4f710728b214ac5a79
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58257939"
---
# <a name="accesspackageassignmentrequest-reprocess"></a>accessPackageAssignmentRequest: reprocessar

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](../resources/entitlementmanagement-root.md)os chamadores podem repetir automaticamente a solicitação de acesso de um usuário a um pacote de acesso. Ele é executado em um [objeto accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) cuja **requestState** está em `DeliveryFailed` um ou `PartiallyDelivered` estado. 

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante) | EntitlementManagement.ReadWrite.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | EntitlementManagement.ReadWrite.All |
  
## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentsRequests/{id}/reprocess  
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna  `202 Accepted` um código de resposta e recupera a solicitação. Se o [objeto accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) não existir, esse método retornará ou se a id não for válida, este método retornará um código `404 Not Found` de  `400 Bad Request` resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "ignored",
  "name": "reprocess_accesspackageassignmentsrequest"
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
