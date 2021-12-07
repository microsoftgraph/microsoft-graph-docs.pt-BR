---
title: Criar accessPackageAssignmentRequest
description: Crie um novo accessPackageAssignmentRequest.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 269045dd629974bfde3b060082657d28a6a36d75
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322330"
---
# <a name="create-accesspackageassignmentrequest"></a>Criar accessPackageAssignmentRequest

Namespace: microsoft.graph


No [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), crie um novo [objeto accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)


## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | EntitlementManagement.ReadWrite.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/assignmentRequests
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | \{token\} de portador. Obrigatório. |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON [do objeto accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)

Para que um administrador solicite a remoção de uma atribuição, o valor da propriedade **requestType** é , e a propriedade assignment contém a propriedade id que identifica `AdminRemove` o [accessPackageAssignment sendo](../resources/accesspackageassignment.md) removido.  

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta de 200 séries e um novo [objeto accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-remove-an-assignment"></a>Exemplo 1: Remover uma atribuição

Para remover atribuições, crie um novo objeto accessPackageAssignmentRequest com as seguintes configurações:

+ O valor da **propriedade requestType** definida como `AdminRemove` .
+ Na propriedade assignment, inclua um objeto com o identificador do objeto accessPackageAssignment a ser excluído.

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra como remover uma atribuição.

<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
}-->

```http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentRequests
Content-type: application/json

{
    "requestType": "AdminRemove",
    "assignment":{
     "id": "a6bb6942-3ae1-4259-9908-0133aaee9377"
    }
}
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#accessPackageAssignmentRequests/$entity",

    "id": "78eaee8c-e6cf-48c9-8f99-aae44c35e379",
    "requestType": "AdminRemove",
    "requestState": "Submitted",
    "requestStatus": "Accepted"
}
```

