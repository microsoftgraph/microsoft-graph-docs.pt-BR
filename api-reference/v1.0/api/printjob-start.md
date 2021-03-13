---
title: 'printJob: start'
description: Envia o trabalho de impressão para a impressora ou printerShare associada. Ele será impresso depois que quaisquer trabalhos pendentes existentes são concluídos, cancelados ou cancelados.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: dd264c395538ee3d77fe22829edca27a6d7ad4b1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775917"
---
# <a name="printjob-start"></a>printJob: start
Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Envia o trabalho de impressão para a impressora [associada](../resources/printer.md) ou [printerShare](../resources/printershare.md). Ele será impresso depois que quaisquer trabalhos pendentes existentes **são** concluídos, abortados ou cancelados.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda [Obter](printer-get.md) impressora ou [Obter printerShare,](printershare-get.md) dependendo se a impressora ou impressoraShare está sendo usada.

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegada (conta corporativa ou de estudante)| PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares/{printerShareId}/jobs/{printJobId}/start
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printJobStatus](../resources/printjobstatus.md) no corpo.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob_start"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/jobs/{printJobId}/start
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJobStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```

