---
title: Listar taskFileAttachments
description: Obtenha uma lista dos objetos taskFileAttachment e suas propriedades.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 66caaea5cf604ab85cd7e64c4a4ca088c2db2b6f
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645604"
---
# <a name="list-taskfileattachments"></a>Listar taskFileAttachments
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista dos [objetos taskFileAttachment](../resources/taskfileattachment.md) e suas propriedades. A **propriedade contentBytes** não será retornada na resposta. Use a API [Obter anexo](../api/attachment-get.md) para exibir **o contentBytes**.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Tasks.Read, Tasks.ReadWrite|
|Delegado (conta pessoal da Microsoft)|Tasks.Read, Tasks.ReadWrite|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/attachments
GET /users/{id}/todo/lists/{id}/tasks/{id}/attachments
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

Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de [objetos taskFileAttachment](../resources/taskfileattachment.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "list_taskfileattachment"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMehdkfuhgAAA=/tasks/AAMkAGUzY5QKjAAA=/attachments
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.taskFileAttachment",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.taskFileAttachment",
            "id": "AAMkADliMm=",
            "name": "flower.md",
            "size": 2814,
            "lastModifiedDateTime": "2022-06-09T10:40:52Z",
            "contentType": "application/octet-stream"
        },
        {
            "@odata.type": "#microsoft.graph.taskFileAttachment",
            "id": "AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwBGAAAAAADdOMUbUmCfTKa7OC-fqjkdBwBnu3olF7NfToRyJ2f__TNcAAAAAAESAABnu3olF7NfToRyJ2f__TNcAAHmG2K0AAABEgAQAFWmGvX71MhOrjRDhWM95yY=",
            "name": "tree.jpg",
            "size": 8591,
            "lastModifiedDateTime": "2022-06-09T10:40:59Z",
            "contentType": "image/jpeg"
        }
    ]
}
```
