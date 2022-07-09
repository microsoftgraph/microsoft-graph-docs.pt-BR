---
title: 'accessPackageAssignmentRequest: reprocessar'
description: Reprocesse objetos accessPackageAssignmentRequest.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0ec27bd2dc451f95b3c001188924fa8c0077211b
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698517"
---
# <a name="accesspackageassignmentrequest-reprocess"></a>accessPackageAssignmentRequest: reprocessar

Namespace: microsoft.graph

No [Azure AD de](../resources/entitlementmanagement-overview.md) direitos, os chamadores podem repetir automaticamente a solicitação de acesso de um usuário a um pacote de acesso. Ele é executado em um [objeto accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) cujo **requestState** está em um `DeliveryFailed` ou `PartiallyDelivered` estado. 

Você só pode reprocessar uma solicitação dentro de 14 dias a partir do momento em que a solicitação original foi concluída. Para solicitações concluídas por mais de 14 dias, você precisará solicitar que os usuários cancelem as solicitações e façam uma nova solicitação no portal [do MyAccess](https://myaccess.microsoft.com/) .

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

Se tiver êxito, este método retornará um  `202 Accepted` código de resposta e tentará novamente a solicitação. Se o [objeto accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) não existir, `404 Not Found` esse método retornará ou se a `400 Bad Request` **ID** não for válida, esse método retornará um código de resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "ignored",
  "name": "reprocess_accesspackageassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/d82eb508-acc4-43cc-bcf1-7c1c4a2c073b/reprocess
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
