---
title: Excluir permissionGrantConditionSet da coleção de inclusões de permissionGrantPolicy
description: Exclui um conjunto de condições incluídas da política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: ca7a37c0cbcb67aa2bf8fc961c8f3211a85a4256
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377114"
---
# <a name="delete-permissiongrantconditionset-from-includes-collection-of-permissiongrantpolicy"></a>Excluir permissionGrantConditionSet da coleção de inclusões de permissionGrantPolicy

Namespace: microsoft.graph

Exclui um [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) da coleção de **inclusões** de um [permissionGrantPolicy](../resources/permissiongrantpolicy.md).

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
| Delegado (conta corporativa ou de estudante) | PermissionGrantPolicy. ReadWrite. All |
| Delegado (conta pessoal da Microsoft) | Sem suporte.    |
| Application | PermissionGrantPolicy. ReadWrite. All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/includes/{include-id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_includes"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy/includes/198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5
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
