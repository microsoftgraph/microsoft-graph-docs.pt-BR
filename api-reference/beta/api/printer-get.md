---
title: Obter impressora
description: Recupere as propriedades e os relacionamentos de um objeto printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: bfd3f6e71e8fd56c630cfcaa5b56cc32eff4e148
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034048"
---
# <a name="get-printer"></a>Obter impressora

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades e os relacionamentos de um [objeto printer.](../resources/printer.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Para usar o serviço de Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir. O usuário assinado deve ser um Administrador [de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| Printer.Read.All, Printer.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}
GET /print/shares/{id}/printer
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método dá suporte a alguns dos parâmetros de consulta OData, incluindo $select, $expand para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

por exemplo, 
```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.
## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto [printer](../resources/printer.md) no corpo da resposta.
Por padrão, a resposta não conterá [printerCapabilities](../resources/printerCapabilities.md). Para obter **printerCapabilities**, use `$select` o parâmetro de consulta. 

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1313

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "name": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "acceptingJobs": true,
  "status": {
    "processingState": "stopped",
    "processingStateReasons": ["disconnected"],
    "processingStateDescription": ""
  },
  "defaults": {
    "copiesPerJob":1,
    "documentMimeType": "application/oxps",
    "finishings": ["none"],
    "mediaType": "stationery"
  },
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3,
    "streetAddress": "One Microsoft Way",
    "subUnit": [
        "Main Plaza",
        "Unit 400"
    ],
    "city": "Redmond",
    "postalCode": "98052",
    "countryOrRegion": "USA",
    "site": "Puget Sound",
    "building": "Studio E",
    "floorNumber": 1,
    "floorDescription": "First Floor",
    "roomNumber": 1234,
    "roomDescription": "First floor copy room",
    "organization": [
        "C+AI",
        "Microsoft Graph"
    ],
    "subdivision": [
        "King County",
        "Red West"
    ],
    "stateOrProvince": "Washington"
  }
}
```

A seguir está um exemplo da resposta, ao usar $select=id,displayName,capabilities
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1313

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "displayName": "PrinterName",
  "capabilities": {
    "isColorPrintingSupported": true,
    "supportsFitPdfToPage": false,
    "contentTypes": [
      "application/pdf",
      "image/pwg-raster",
      "application/PCLm"
    ],
    "isPageRangeSupported": false,
    "qualities": [
      "medium"
    ],
    "dpis": [
      600
    ],
    "duplexModes": [
      "oneSided",
      "flipOnLongEdge",
      "flipOnShortEdge"
    ],
    "finishings": [
      "none"
    ],
    "mediaTypes": [
      "stationery"
    ],
    "mediaSizes": [
      "North America Letter"
    ],
    "outputBins": [
      "tray-1"
    ],
    "colorModes": [
      "grayscale",
      "color"
    ],
    "inputBins": [
      "tray-1"
    ],
    "collation": true,
    "scalings": [
      "fill"
    ],
    "copiesPerJob": {
      "start": 1,
      "end": 38
    }
  }
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
