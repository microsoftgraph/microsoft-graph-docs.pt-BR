---
title: 'accessPackageAssignment: reprocessamento'
description: Reprocessar objetos accesspackageassignment.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 66356cd856906ba73b107c06cfd36cc52bf85acb
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650864"
---
# <a name="accesspackageassignment-reprocess"></a>accessPackageAssignment: reprocessamento

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](../resources/entitlementmanagement-overview.md)os chamadores podem reavaliar automaticamente e impor um objeto [accessPackageAssignment](../resources/accesspackageassignment.md) das atribuições de um usuário para um pacote de acesso específico. O **assignmentState** do pacote de acesso deve ser para `Delivered` o administrador reprocessar a atribuição do usuário. Somente os administradores com a função Gerenciador de Atribuição de Pacote do Access, ou superior, no gerenciamento de direitos do Azure AD podem executar essa ação.

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
POST /identityGovernance/entitlementManagement/accessPackageAssignments/{id}/reprocess 
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e reavalia e impõe as atribuições do usuário do `202 Accepted` [objeto accessPackageAssignment,](../resources/accesspackageassignment.md) o que significa que o status do pacote de acesso será alterado para Entregue. Se a atribuição não existir, esse método retornará ou se a id não for válida, este `404 Not Found` método retornará um código de  `400 Bad Request` resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "ignored",
  "name": "reprocess_accesspackageassignments"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments/d82eb508-acc4-43cc-bcf1-7c1c4a2c073b/reprocess
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
