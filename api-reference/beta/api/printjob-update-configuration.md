---
title: Atualizar configuração de printJob
description: Atualizar a configuração de um trabalho de impressão
author: tomsato-ms
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 23d61d24367bc5c69d4613ac30deed9244a5ac08
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706219"
---
# <a name="update-printjob-configuration"></a>Atualizar configuração de printJob

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize a propriedade de [configuração](../resources/printjobconfiguration.md) de um [trabalho de impressão](../resources/printjob.md).

Atualizar uma configuração de trabalho de impressão requer que o trabalho de impressão esteja em estado mantido registrando um gatilho de tarefa para a impressora. Para obter detalhes sobre como registrar um disparador de tarefas, consulte [estendendo a impressão universal para dar suporte à impressão pull](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura universal de impressão ativa, uma permissão que conceda obter acesso à [impressora](printer-get.md) e uma das permissões listadas na tabela a seguir.

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| Sem suporte. |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| PrintJob.Manage.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}/jobs/{id}/configuration
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores dos campos [printJobConfiguration](../resources/printjobconfiguration.md) relevantes. As propriedades existentes que não estão incluídas no corpo da solicitação manterão seus valores anteriores.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API.
### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "printjob-update-configuration"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/configuration

{
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
```

### <a name="response"></a>Resposta
Este é um exemplo de resposta. 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update print job configuration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


