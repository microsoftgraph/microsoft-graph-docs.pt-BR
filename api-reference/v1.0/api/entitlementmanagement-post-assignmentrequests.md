---
title: Criar accessPackageAssignmentRequest
description: Crie um novo accessPackageAssignmentRequest.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 827020fd3da1c4b52dd95f67bb0550fbfcb9253a
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2022
ms.locfileid: "64607894"
---
# <a name="create-accesspackageassignmentrequest"></a>Criar accessPackageAssignmentRequest

Namespace: microsoft.graph


No [Azure AD Entitlement Management](../resources/entitlementmanagement-overview.md), crie um novo [objeto accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) .  Essa operação é usada para atribuir um usuário a um pacote de acesso ou para remover uma atribuição de pacote de acesso.


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
POST /identityGovernance/entitlementManagement/assignmentRequests
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | \{token\} de portador. Obrigatório. |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON [do objeto accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) .

Para que um administrador solicite a criação de uma atribuição para um usuário, o valor da propriedade **requestType** `AdminAdd`é ,  `targetId` e a propriedade assignment contém o do usuário que está sendo atribuído, a propriedade **assignmentPolicyId** que identifica o accessPackageAssignmentPolicy e a propriedade **accessPackageId** que identifica [o accessPackage](../resources/accesspackage.md).

Para que um administrador solicite a remoção de uma atribuição, o valor da propriedade **requestType** `AdminRemove`é , e a propriedade **assignment** contém a propriedade **id** que identifica [o accessPackageAssignment sendo](../resources/accesspackageassignment.md) removido.

Para um usuário não administrador solicitar a criação de sua própria atribuição para uma primeira atribuição ou renovação de atribuição, o valor da **propriedade requestType** é `UserAdd`. A **propriedade** assignment contém um objeto com `targetId` o `id` do usuário. A **propriedade assignmentPolicyId** identifica accessPackageAssignmentPolicy. A **propriedade accessPackageId** identifica [o accessPackage](../resources/accesspackage.md). O usuário que faz a solicitação já deve existir no diretório.

Para um usuário que não seja administrador solicitar estender suas próprias atribuições, o valor da **propriedade requestType** é `UserExtend`. A **propriedade** assignment contém o `targetId` com o `id` dos usuários. A **propriedade assignmentPolicyId** identifica accessPackageAssignmentPolicy. A **propriedade accessPackageId** identifica [o accessPackage](../resources/accesspackage.md). O usuário que faz a solicitação já deve existir no diretório.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta de 200 séries e um novo [objeto accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) no corpo da resposta.

Se isso for uma `AdminAdd` solicitação, em seguida, um [accessPackageAssignment](../resources/accesspackageassignment.md) e, se necessário, um [accessPackageSubject](../resources/accesspackagesubject.md) também serão criados. Você pode localizá-los usando os parâmetros de consulta ao [listar accessPackageAssignments](entitlementmanagement-list-assignments.md).

## <a name="examples"></a>Exemplos

### <a name="example-1-admin-requests-a-direct-assignment-for-a-user-already-in-the-directory"></a>Exemplo 1: o administrador solicita uma atribuição direta para um usuário que já está no diretório
#### <a name="request"></a>Solicitação

A seguir está um exemplo da solicitação de uma atribuição direta, na qual o administrador está solicitando a criação de uma atribuição para o usuário. Como o [accessPackageSubject](../resources/accesspackagesubject.md) pode ainda não existir, o valor do **targetID** é a ID do objeto do usuário que está sendo atribuído, o valor do **accessPackageId** é o pacote de acesso desejado para esse usuário, e o valor de **assignmentPolicyId** é uma política de atribuição direta nesse pacote de acesso.


<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests_1"
}-->

```http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentRequests
Content-type: application/json

{
  "requestType": "AdminAdd",
  "assignment":{
     "targetId":"46184453-e63b-4f20-86c2-c557ed5d5df9",
     "assignmentPolicyId":"2264bf65-76ba-417b-a27d-54d291f0cbc8",
     "accessPackageId":"a914b616-e04e-476b-aa37-91038f0b165b"
  }
}
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{

  "id": "7e382d02-4454-436b-b700-59c7dd77f466",
  "requestType": "AdminAdd",
  "requestState": "Submitted",
  "requestStatus": "Accepted"
}
```

### <a name="example-2-remove-an-assignment"></a>Exemplo 2: Remover uma atribuição

Para remover atribuições, crie um novo objeto accessPackageAssignmentRequest com as seguintes configurações:

+ O valor da **propriedade requestType** definida como `AdminRemove`.
+ Na propriedade assignment, inclua um objeto com o identificador do objeto accessPackageAssignment a ser excluído.

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra como remover uma atribuição.


# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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

