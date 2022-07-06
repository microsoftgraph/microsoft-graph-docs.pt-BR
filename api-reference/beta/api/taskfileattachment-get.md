---
title: Obter taskFileAttachment
description: Leia as propriedades e as relações de um objeto taskFileAttachment.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0a269e67fd3305aa12e3492609d8d672f6c49f69
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645606"
---
# <a name="get-taskfileattachment"></a>Obter taskFileAttachment
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto taskFileAttachment](../resources/taskfileattachment.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Tasks.Read, Tasks.ReadWrite|
|Delegado (conta pessoal da Microsoft)|Tasks.Read, Tasks.ReadWrite|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
Para obter um arquivo anexado a um [todoTask](../resources/todotask.md):
 
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /me/todo/lists/{id}/tasks/{id}/attachments/{id}
GET /users/{id}/todo/lists/{id}/tasks/{id}/attachments/{id}
```

Para obter o conteúdo bruto de um anexo de arquivo (o tipo de conteúdo é baseado no tipo de conteúdo original do arquivo):
<!-- {
  "blockType": "ignored"
}
-->
``http
GET /me/todo/lists/{id}/tasks/{id}/attachments/{id}/$value
GET /users/{id}/todo/lists/{id}/tasks/{id}/attachments/{id}/$value
``

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um [objeto taskFileAttachment](../resources/taskfileattachment.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "get_taskfileattachment"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMehdkfuhgAAA=/tasks/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.taskFileAttachment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.taskFileAttachment",
    "id": "AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=",
    "lastModifiedDateTime": "2021-04-02T03:41:29Z",
    "name": "Q1 Planning.docx",
    "contentType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
    "size": 29068,
    "contentBytes": "UEsDBBQABgAIAAAAIQ4AAAAA"
  }
}
```

