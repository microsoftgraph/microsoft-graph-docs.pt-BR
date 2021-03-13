---
title: Get printJob
description: Recupere as propriedades e as relações de um trabalho de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 976624807ab6cbf8a104790665c481e3f54f9750
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776001"
---
# <a name="get-printjob"></a>Get printJob
Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Recupere as propriedades e as relações de um trabalho de impressão.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma [](printer-get.md) assinatura de Impressão Universal ativa e ter uma permissão que conceda Obter impressora ou Obter acesso a [PrinterShare,](printershare-get.md) dependendo se a impressora ou impressoraShare está sendo usada.

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegada (conta corporativa ou de estudante)| PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All |

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
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printJob](../resources/printjob.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-print-job"></a>Exemplo 1: Obter trabalho de impressão

#### <a name="request"></a>Solicitação
A seguir, um exemplo de uma solicitação para obter metadados para um trabalho de impressão.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}
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
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {    
  },
  "configuration": {    
  },
  "status": {
    "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ],
    "isAcquiredByPrinter": true
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false
}
```

### <a name="example-2-get-print-job-with-task-list"></a>Exemplo 2: Obter trabalho de impressão com lista de tarefas

#### <a name="request"></a>Solicitação
A seguir está uma solicitação para [](../resources/printtask.md) obter um trabalho de impressão e todas as tarefas que estão sendo executadas ou executadas em relação a ele.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob_withtasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}?$expand=tasks
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-withtasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-withtasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-withtasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printjob-withtasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {    
  },
  "configuration": {    
  },
  "status": {
    "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ],
    "isAcquiredByPrinter": true
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false,
  "tasks": [
    {
      "id": "d036638b-1272-4bba-9227-732463823ed3",
      "parentUrl": "https://graph.microsoft.com/v1.0/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182",
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
A seguir, um exemplo de uma solicitação para obter um trabalho de impressão e seus dados de documento associados.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob_withdocumentdata"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}?$expand=documents
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


#### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {    
  },
  "configuration": {    
  },
  "status": {
    "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ],
    "isAcquiredByPrinter": true
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false,
  "documents@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs('5182')/documents",
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
