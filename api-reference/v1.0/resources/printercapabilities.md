---
title: Tipo complexo printerCapabilities
description: Representa os recursos relatados por uma impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: bda913275aff692df2f66472f61436665cbc3dd7
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944223"
---
# <a name="printercapabilities-resource-type"></a>Tipo de recurso printerCapabilities

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Representa os recursos relatados por um printer/printerShare.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|contentTypes|Coleção de cadeias de caracteres|Uma lista de tipos de conteúdo com suporte (MIME) compatíveis com a impressora. Não é garantido que o serviço Impressão Universal dá suporte à impressão de todos esses tipos mime.|
|isColorPrintingSupported|Booliano|True se a impressão de cores for suportada pela impressora; false caso contrário. Somente leitura.|
|feedOrientations|Coleção printerFeedOrientation|A lista de orientações de feed que são suportadas pela impressora.|
|isPageRangeSupported|Booliano|True se a impressora dá suporte à impressão por intervalos de página; false caso contrário.|
|qualidades|[Coleção printQuality](enums.md#printquality-values)|As qualidades de impressão suportadas pela impressora.|
|dpis|Coleção Int32|A lista de resoluções de impressão em DPI que são suportadas pela impressora.|
|duplexModes|[Coleção printDuplexMode](enums.md#printduplexmode-values)|A lista de modos duplex com suporte da impressora. Os valores válidos são descritos na tabela a seguir.|
|queueBufferSizeInBytes|Int32|O tamanho máximo da fila de trabalho de impressão que pode ser armazenado pela impressora.|
|copiesPerJob|[integerRange](integerrange.md)|O intervalo de cópias por trabalho suportado pela impressora.|
|finishings|[Coleção printFinishing](enums.md#printfinishing-values)|Processos de término que a impressora dá suporte a um documento impresso.|
|mediaColors|Coleção de cadeias de caracteres|As cores de mídia (ou seja, papel) suportadas pela impressora.|
|mediaTypes|Coleção de cadeias de caracteres|Os tipos de mídia suportados pela impressora.|
|mediaSizes|Coleção de cadeias de caracteres|Os tamanhos de mídia suportados pela impressora. Oferece suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI. Os valores válidos estão na tabela [a seguir](#mediasizes-values).|
|pagesPerSheet|Coleção Int32|Número suportado de Páginas de Entrada para impor uma única Impressão.|
|orientações|[Coleção printOrientation](enums.md#printorientation-values)|As orientações de impressão suportadas pela impressora. Os valores válidos são descritos na tabela a seguir.|
|inputBins|Coleção de cadeias de caracteres|Caixas de entrada com suporte para a impressora.|
|outputBins|Coleção de cadeias de caracteres|As caixas de saída com suporte da impressora (bandejas).|
|supportsFitPdfToPage|Booliano|True se a impressora oferece suporte ao dimensionamento de páginas PDF para corresponder ao tamanho da mídia de impressão; false caso contrário.|
|multipageLayouts|[Coleção printMultipageLayout](enums.md#printmultipagelayout-values)|As instruções de apresentação suportadas pela impressora. Os valores com suporte são descritos na tabela a seguir.|
|colorModes|[Coleção printColorMode](enums.md#printcolormode-values)|Os modos de cor suportados pela impressora. Os valores válidos são descritos na tabela a seguir.|
|topMargins|Coleção Int32|Uma lista de margens principais com suporte (em mícrons) para a impressora.|
|bottomMargins|Coleção Int32|Uma lista de margens inferior suportadas (em mícrons) para a impressora.|
|rightMargins|Coleção Int32|Uma lista de margens direitas com suporte (em mícrons) para a impressora.|
|leftMargins|Coleção Int32|Uma lista de margens esquerdas suportadas (em mícrons) para a impressora.|
|collation|Booliano|True se a impressora dá suporte à colagem ao imprimir cópias muliplas de um documento de várias páginas; false caso contrário.|
|scalings|[Coleção printScaling](enums.md#printscaling-values)|Dimensionamentos de impressão com suporte.|

### <a name="mediasizes-values"></a>mediaSizes values

|Valor|
|:---|
|A3|
|A4|
|A5|
|A6|
|JIS B4|
|JIS B5|
|JPN Hagaki|
|América do Norte 5x7in|
|Executivo da América do Norte|
|Carta de Goverment da América do Norte|
|Índice da América do Norte 3x5in|
|Índice da América do Norte 4x8in|
|Índice da América do Norte 5x8in|
|Fatura da América do Norte|
|Ledger da América do Norte|
|América do Norte Legal|
|Carta da América do Norte|
|Foto l 3.5x5in|
|Cartão de Visita|
|Photo|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerCapabilities"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerCapabilities",
  "contentTypes": [
    "String"
  ],
  "isColorPrintingSupported": "Boolean",
  "feedOrientations": [
    "String"
  ],
  "isPageRangeSupported": "Boolean",
  "qualities": [
    "String"
  ],
  "dpis": [
    "Integer"
  ],
  "duplexModes": [
    "String"
  ],
  "copiesPerJob": {
    "@odata.type": "microsoft.graph.integerRange"
  },
  "finishings": [
    "String"
  ],
  "mediaColors": [
    "String"
  ],
  "mediaTypes": [
    "String"
  ],
  "mediaSizes": [
    "String"
  ],
  "pagesPerSheet": [
    "Integer"
  ],
  "orientations": [
    "String"
  ],
  "outputBins": [
    "String"
  ],
  "supportsFitPdfToPage": "Boolean",
  "multipageLayouts": [
    "String"
  ],
  "colorModes": [
    "String"
  ],
  "inputBins": [
    "String"
  ],
  "topMargins": [
    "Integer"
  ],
  "bottomMargins": [
    "Integer"
  ],
  "rightMargins": [
    "Integer"
  ],
  "leftMargins": [
    "Integer"
  ],
  "collation": "Boolean",
  "scalings": [
    "String"
  ]
}
```

