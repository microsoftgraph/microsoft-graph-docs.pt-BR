---
title: Get printJob
description: Recupere as propriedades e as relações de um trabalho de impressão.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 8a1c843410e4d2f01ea3da5458d11a835d2163b8
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160409"
---
# <a name="get-printjob"></a>Get printJob

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades e as relações de um trabalho de impressão.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o locatário do usuário ou do aplicativo deve ter uma assinatura de Impressão Universal ativa.

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application| PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All |

Para um aplicativo com permissões delegadas para recuperar trabalhos de outros usuários, o usuário conectado deve ser membro de uma das seguintes funções de administrador:
- Administrador Global
- Administrador da impressora

Para um aplicativo com permissões de aplicativo para recuperar trabalhos dos usuários, o aplicativo precisa de uma permissão que conceda acesso à impressora, juntamente com uma das permissões de aplicativo [descritas](#permissions) na tabela Permissões.[](printer-get.md)

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->

Para obter um trabalho de uma impressora:
```http
GET /print/printers/{id}/jobs/{id}
```

Para obter um trabalho de um compartilhamento de impressora:
```http
GET /print/shares/{id}/jobs/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.
## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código `200 OK` de resposta e um [objeto printJob](../resources/printjob.md) no corpo da resposta.
## <a name="examples"></a>Exemplos

### <a name="example-1-get-print-job"></a>Exemplo 1: Obter trabalho de impressão

#### <a name="request"></a>Solicitação
A seguir está um exemplo de uma solicitação para obter metadados para um trabalho de impressão.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {},
  "status": {
    "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ]
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false
}
```

### <a name="example-2-get-print-job-with-task-list"></a>Exemplo 2: Obter trabalho de impressão com a lista de tarefas

#### <a name="request"></a>Solicitação
A seguir está uma solicitação para obter um trabalho de impressão [](../resources/printtask.md) e todas as tarefas que estão sendo executadas ou executadas nele.

<!-- {
  "blockType": "request",
  "name": "get_printjob_withtasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182?$expand=tasks
```

#### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs(tasks())/$entity",
  "id": "5182",
  "createdDateTime": "2020-06-30T17:18:52.3930472Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "userPrincipalName": ""
  },
  "status": {
    "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ]
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false,
  "configuration": {    
  },
  "tasks": [
    {
      "id": "d036638b-1272-4bba-9227-732463823ed3",
      "parentUrl": "https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182",
      "status": {
        "state": "processing",
        "description": "The task is being processed."
      }
    }
  ]
}
```

### <a name="example-3-get-a-print-job-and-its-associated-document-data"></a>Exemplo 3: Obter um trabalho de impressão e seus dados de documento associados

#### <a name="request"></a>Solicitação
A seguir está um exemplo de uma solicitação para obter um trabalho de impressão e seus dados de documento associados.
# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob_withdocumentdata"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/86b6d420-7e6b-4797-a05c-af4e56cd81bd/jobs/31216?$expand=documents
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-withdocumentdata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-withdocumentdata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-withdocumentdata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printjob-withdocumentdata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('86b6d420-7e6b-4797-a05c-af4e56cd81bd')/jobs(documents())/$entity",
  "id": "31216",
  "createdDateTime": "2020-06-26T04:20:06.5715544Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "ipAddress": null,
    "userPrincipalName": "",
    "oDataType": null
  },
  "status": {
  "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ]
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false,
  "configuration": {    
  },
  "documents": [
    {
      "id": "ca96c367-c3ad-478a-bbce-fbd1cd856e73",
      "displayName": "",
      "contentType": "application/oxps",
      "size": 276604
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


