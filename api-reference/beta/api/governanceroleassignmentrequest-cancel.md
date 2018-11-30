---
title: Cancelar governanceRoleAssignmentRequest
description: Cancele um governanceRoleAssignmentRequest.
ms.openlocfilehash: 3e83d47b94f69b124b841f99490a012f2e39a42c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035896"
---
# <a name="cancel-governanceroleassignmentrequest"></a>Cancelar governanceRoleAssignmentRequest

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Cancele um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureResources  |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método **não** suporta [Parâmetros da Consulta OData](/graph/query-parameters).

### <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | Portador {código}|
| Content-type  | application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204 NoContent`. Não retorna nada no corpo da resposta. 

## <a name="error-codes"></a>Códigos de erro
Essa API segue o padrão dos códigos HTTP. Além disso, os códigos de erro personalizadas são mostrados abaixo.
|Código de erro     | Mensagem de erro              | Detalhes |
|:--------------------| :---------------------|:--------------------|
| 400 BadRequest | RoleAssignmentRequestNotFound | O governanceRoleAssignmentRequest não existe no sistema.
| 400 BadRequest | RequestCannotBeCancelled    | Somente as solicitações em status de `Granted`, `PendingApproval`, `PendingApprovalProvisioning` e `PendingAdminDecision` pode ser cancelado.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->