---
title: Criar linkedResource
description: Crie um novo objeto linkedResource.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e79db0afdcf223e7619fa45612a5e6971fa1771f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128249"
---
# <a name="create-linkedresource"></a>Criar linkedResource
Namespace: microsoft.graph

Crie um [objeto linkedResource](../resources/linkedresource.md) para associar uma tarefa [especificada](../resources/todotask.md) a um item em um aplicativo parceiro. Por exemplo, você pode associar uma tarefa a um item de email no Outlook que estimulou a tarefa e pode criar um **objeto linkedResource** para rastrear sua associação.

Você também pode criar um **objeto linkedResource** ao [criar uma tarefa](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Tasks.ReadWrite|
|Delegado (conta pessoal da Microsoft)|Tasks.ReadWrite|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto linkedResource.](../resources/linkedresource.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o linkedResource](../resources/linkedresource.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID gerada do servidor para a entidade vinculada Herdada da [entidade](../resources/entity.md)|
|webUrl|String|Deeplink para a entidade vinculada |
|applicationName|Cadeia de caracteres|Campo indicando o nome do aplicativo da fonte que está enviando a entidade vinculada |
|displayName|Cadeia de caracteres|Campo indicando o título da entidade vinculada. |
|externalId|Cadeia de caracteres|ID do objeto associado a essa tarefa no sistema de terceiros/parceiro |



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto linkedResource](../resources/linkedresource.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "create_linkedresource_from_linkedresources"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
Content-Type: application/json

{
  "webUrl": "https://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-linkedresource-from-linkedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-linkedresource-from-linkedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-linkedresource-from-linkedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-linkedresource-from-linkedresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-linkedresource-from-linkedresources-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-linkedresource-from-linkedresources-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.linkedResource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
  "webUrl": "http:://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```



