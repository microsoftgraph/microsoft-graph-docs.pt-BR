---
title: Obter checklistItem
description: Leia as propriedades e as relações de um objeto checklistItem.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 44391ca98a8b83030c80e08a1d825b4e0b10042a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440738"
---
# <a name="get-checklistitem"></a>Obter checklistItem
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi-sharedfeature](../includes/todo-deprecate-basetaskapi-sharedfeature.md)]

Leia as propriedades e as relações de um [objeto checklistItem](../resources/checklistitem.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Tasks.Read, Tasks.ReadWrite|
|Delegada (conta pessoal da Microsoft)|Tasks.Read, Tasks.ReadWrite|
|Aplicativo|Tasks.Read, Tasks.ReadWrite|

## <a name="http-request"></a>Solicitação HTTP

Esta seção lista a sintaxe de cada um dos dois `GET` cenários descritos acima.

### <a name="get-a-checklistitem-associated-to-a-specified-todotask"></a>Obter um checklistItem associado a um todoTask especificado

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/checklistItems/{checklistItemId}
GET /users/{id | userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/checklistItems/{checklistItemId}
```

### <a name="get-a-checklistitem-associated-to-a-specified-basetask-deprecated"></a>Obter um checklistItem associado a uma baseTask especificada (preterida)

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/tasks/lists/{baseTaskListId}/tasks/{baseTaskId}/checklistItems/{checklistItemId}
GET /users/{id | userPrincipalName}/tasks/lists/{baseTaskListId}/tasks/{baseTaskId}/checklistItems/{checklistItemId}
```


## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um [objeto checklistItem](../resources/checklistitem.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request-1"></a>Solicitação 1 

Aqui está um exemplo para obter **um checklistItem** associado a um **todoTask**.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_checklistitem_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA/checklistitems/51d8a471-2e9d-4f53-9937-c33a8742d28f
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-checklistitem-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-checklistitem-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-checklistitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-checklistitem-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-checklistitem-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-checklistitem-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.checklistItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('6f9a2a92-8527-4d64-937e-b5312852f35d')/todo/lists('AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA%3D')/tasks('AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA')/checklistItems/$entity",
    "displayName": "Create draft",
    "createdDateTime": "2021-11-17T05:22:14.2207813Z",
    "isChecked": false,
    "id": "51d8a471-2e9d-4f53-9937-c33a8742d28f"
}
```


### <a name="request-2"></a>Solicitação 2

Aqui está um exemplo para obter um **checklistItem** associado a uma **baseTask** (preterido).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_checklistitem_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/tasks/lists/AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA/checklistitems/51d8a471-2e9d-4f53-9937-c33a8742d28f
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-checklistitem-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-checklistitem-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-checklistitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-checklistitem-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-checklistitem-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.checklistItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('6f9a2a92-8527-4d64-937e-b5312852f35d')/tasks/lists('AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA%3D')/tasks('AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA')/checklistItems/$entity",
    "displayName": "Create draft",
    "createdDateTime": "2021-11-17T05:22:14.2207813Z",
    "isChecked": false,
    "id": "51d8a471-2e9d-4f53-9937-c33a8742d28f"
}
```
