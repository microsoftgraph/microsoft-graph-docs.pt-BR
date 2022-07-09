---
title: 'accessPackageAssignment: reprocessar'
description: Reprocesse objetos accesspackageassignment.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 75d221efa4c740eadb132ef429ac5d193512f3c6
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698521"
---
# <a name="accesspackageassignment-reprocess"></a>accessPackageAssignment: reprocessar

Namespace: microsoft.graph

No [Azure AD](../resources/entitlementmanagement-overview.md) de direitos, os chamadores podem reavaliar e impor automaticamente um objeto [accessPackageAssignment](../resources/accesspackageassignment.md) das atribuições de um usuário para um pacote de acesso específico. O **assignmentState** do pacote de acesso deve ser `Delivered` para o administrador reprocessar a atribuição do usuário. Somente administradores com a função Gerenciador de Atribuição de Pacote de Acesso, ou superior, Azure AD gerenciamento de direitos podem executar essa ação.

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

Se bem-sucedido, este método retorna um código de resposta e reavalia e impõe as atribuições `202 Accepted` do usuário do objeto [accessPackageAssignment](../resources/accesspackageassignment.md) , o que significa que o status do pacote de acesso será alterado para Entregue. Se a atribuição não existir, esse `404 Not Found` método retornará ou, se a **ID** não for válida, esse método retornará um código `400 Bad Request` de resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "ignored",
  "name": "reprocess_accesspackageassignments"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackageAssignments/d82eb508-acc4-43cc-bcf1-7c1c4a2c073b/reprocess
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