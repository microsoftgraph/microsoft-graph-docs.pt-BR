---
title: Atualizar linkedResource_v2
description: Atualize as propriedades de um linkedResource_v2 objeto.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 70554d1d64be0d3c497225ee25a124b3d52681d5
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526125"
---
# <a name="update-linkedresource_v2"></a>Atualizar linkedResource_v2
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [linkedResource_v2](../resources/linkedresource_v2.md) objeto.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Tasks.ReadWrite|
|Delegada (conta pessoal da Microsoft)|Tasks.ReadWrite|
|Aplicativo|Tasks.ReadWrite|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/tasks/lists/{baseTaskListId}/tasks/{baseTaskId}/linkedResources/{linkedResourceId}
PATCH /users/{id | userPrincipalName}/tasks/lists/{baseTaskListId}/tasks/{baseTaskId}/linkedResources/{linkedResourceId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|applicationName|Cadeia de caracteres|Campo indicando o nome do aplicativo da fonte que está enviando **o linkedResource**.|
|displayName|Cadeia de caracteres|Campo que indica o título do **linkedResource**.|
|externalId|Cadeia de caracteres|ID do objeto associado a essa tarefa no sistema de terceiros/parceiro.|
|webUrl|String|Link profundo para **o linkedResource**.|


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto linkedResource_v2](../resources/linkedresource_v2.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_linkedresource_v2"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/tasks/lists/AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA/linkedResources/e2c5ed75-7aa4-4f8e-84ab-98b5e0b56ee8
Content-Type: application/json

{
    "webUrl": "https://microsoft.com",
    "applicationName": "Microsoft",
    "displayName": "Microsoft Web page",
    "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-linkedresource-v2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.linkedResource_v2"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('6f9a2a92-8527-4d64-937e-b5312852f35d')/tasks/lists('AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA%3D')/tasks('AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA')/linkedResources/$entity",
    "webUrl": "https://microsoft.com",
    "applicationName": "Microsoft",
    "displayName": "Microsoft Web page",
    "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9",
    "id": "e2c5ed75-7aa4-4f8e-84ab-98b5e0b56ee8"
}
```

