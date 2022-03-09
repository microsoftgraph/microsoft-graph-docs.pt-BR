---
title: Atualizar approvalStage
description: Aplicar aprovar ou negar decisão em um objeto approvalStage.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 62aafeda3d6f04ffd1f195ea8f1cdb9ac8d89891
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63398079"
---
# <a name="update-approvalstage"></a>Atualizar approvalStage

Namespace: microsoft.graph

No [gerenciamento de direitos do Azure AD](../resources/entitlementmanagement-overview.md), aprove ou negue um objeto [approvalStage](../resources/approvalstage.md) em uma [aprovação](../resources/approval.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | EntitlementManagement.ReadWrite.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{accessPackageAssignmentRequestId}/stages/{approvalStageId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

A tabela a seguir mostra as propriedades necessárias para este método.

| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
| reviewResult | Cadeia de caracteres | Decisão do aprovador. Os valores possíveis são: `Approve` e `Deny`. Obrigatório.|
| justification | Cadeia de caracteres | Justificativa relacionada à decisão do aprovador. |


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `204 No Content` código de resposta no corpo da resposta. IOf the caller does not the right permissions, the method returns a `403 Forbidden` response code, or if the approval id is not found, the method returns `404 Not found`. Se a solicitação já tiver sido aprovada por outro aprovador no mesmo estágio de aprovação, o método retornará o `409 Conflict` código de resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "patch_approvalstage"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/stages/d4fa4045-4716-436d-aec5-57b0a713f095

{
 "reviewResult":"Approve",
 "justification":"OK"
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patch approvalStage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
