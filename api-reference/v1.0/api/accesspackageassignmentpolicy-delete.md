---
title: Excluir accessPackageAssignmentPolicy
description: Exclua um accessPackageAssignmentPolicy.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9ad20866326f77cf8fc869a4a8d4de79cd9ec598
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608251"
---
# <a name="delete-accesspackageassignmentpolicy"></a>Excluir accessPackageAssignmentPolicy

Namespace: microsoft.graph


No [gerenciamento de direitos do Azure AD](../resources/entitlementmanagement-overview.md), exclua [um accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | EntitlementManagement.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /identityGovernance/entitlementManagement/assignmentPolicies/{accessPackageAssignmentPolicyId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "delete_accesspackageassignmentpolicy"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentPolicies/{accessPackageAssignmentPolicyId}
```


### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


