---
title: Atualizar printJob
description: Atualizar trabalho de impressão
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 3fd3109f914e08d0dd152b2e22ce5f20a84b2d96
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516897"
---
# <a name="update-printjob"></a>Atualizar printJob
Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Atualizar um [trabalho de impressão](../resources/printjob.md). Somente a **propriedade de** configuração pode ser atualizada.

A atualização de um trabalho de impressão só terá êxito se houver [um printTask](../resources/printTask.md) em um estado no trabalho de impressão associado, iniciado por um gatilho criado pelo aplicativo `processing` solicitante. Para obter detalhes sobre como registrar um gatilho de tarefas, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Para usar o serviço impressão universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, a permissão Printer.Read.All ou Printer.ReadWrite.All e uma das permissões listadas na tabela a seguir.

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| Sem suporte. |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/printers/{printerId}/jobs/{printJobId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece os valores dos campos [printJob relevantes.](../resources/printjob.md) As propriedades existentes que não estão incluídas no corpo da solicitação manterão seus valores anteriores. 

Somente a **propriedade de** configuração pode ser atualizada.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta com um objeto [printJob](../resources/printjob.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_printjob"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}
Content-Type: application/json
Content-length: 376

{
  "configuration": {
    "feedOrientation": "longEdgeFirst",
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "quality": "medium",
    "dpi": 600,
    "orientation": "landscape",
    "copies": 1,
    "duplexMode": "oneSided",
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    },
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false
  }
}
```

### <a name="response"></a>Resposta
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('d5ef6ec4-07ca-4212-baf9-d45be126bfbb')/jobs/$entity",
  "id": "44353",
  "createdDateTime": "2020-06-26T04:20:06.5715544Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "userPrincipalName": ""
  },
  "status": {
    "state": "paused",
    "description": "The job is not a candidate for processing yet."
  },
  "configuration": {
    "feedOrientation": "longEdgeFirst",
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "quality": "medium",
    "dpi": 600,
    "orientation": "landscape",
    "copies": 1,
    "duplexMode": "oneSided",
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    },
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false
  }
}
```

