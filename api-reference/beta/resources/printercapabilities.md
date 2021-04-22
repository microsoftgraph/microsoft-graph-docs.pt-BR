---
title: Tipo complexo printerCapabilities
description: Representa os recursos relatados por uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 37e011eedfe00d905f4bf862327e948787207270
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944137"
---
# <a name="printercapabilities-complex-type"></a>Tipo complexo printerCapabilities

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os recursos relatados por uma impressora.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|contentTypes|Coleção de cadeias de caracteres|Uma lista de tipos de conteúdo com suporte (MIME) compatíveis com a impressora. Não é garantido que o serviço Impressão Universal dá suporte à impressão de todos esses tipos mime.|
|isColorPrintingSupported|Booliano|True se a impressão de cores for suportada pela impressora; false caso contrário. Somente leitura.|
|feedOrientations|Coleção printerFeedOrientation|A lista de orientações de feed que são suportadas pela impressora.|
|isPageRangeSupported|Booliano|True se a impressora dá suporte à impressão por intervalos de página; false caso contrário.|
|qualidades|Coleção printQuality|As qualidades de impressão suportadas pela impressora.|
|dpis|Coleção Int32|A lista de resoluções de impressão em DPI que são suportadas pela impressora.|
|duplexModes|Coleção printDuplexMode|A lista de modos duplex com suporte da impressora. Os valores válidos são descritos na tabela a seguir.|
|queueBufferSizeInBytes|Int32|O tamanho máximo da fila de trabalho de impressão que pode ser armazenado pela impressora.|
|copiesPerJob|[integerRange](integerrange.md)|O intervalo de cópias por trabalho suportado pela impressora.|
|finishings|Coleção printFinishing|Processos de término que a impressora dá suporte a um documento impresso.|
|mediaColors|Coleção de cadeias de caracteres|As cores de mídia (ou seja, papel) suportadas pela impressora.|
|mediaTypes|Coleção de cadeias de caracteres|Os tipos de mídia suportados pela impressora.|
|mediaSizes|Coleção de cadeias de caracteres|Os tamanhos de mídia suportados pela impressora. Oferece suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI. Os valores válidos estão na tabela [a seguir](#mediasizes-values).|
|pagesPerSheet|Coleção Int32|Número suportado de Páginas de Entrada para impor uma única Impressão.|
|orientações|Coleção printOrientation|As orientações de impressão suportadas pela impressora. Os valores válidos são descritos na tabela a seguir.|
|inputBins|Coleção de cadeias de caracteres|Caixas de entrada com suporte para a impressora.|
|outputBins|Coleção de cadeias de caracteres|As caixas de saída com suporte da impressora (bandejas).|
|supportsFitPdfToPage|Booliano|True se a impressora oferece suporte ao dimensionamento de páginas PDF para corresponder ao tamanho da mídia de impressão; false caso contrário.|
|multipageLayouts|Coleção printMultipageLayout|As instruções de apresentação suportadas pela impressora. Os valores com suporte são descritos na tabela a seguir.|
|colorModes|Coleção printColorMode|Os modos de cor suportados pela impressora. Os valores válidos são descritos na tabela a seguir.|
|topMargins|Coleção Int32|Uma lista de margens principais com suporte (em mícrons) para a impressora.|
|bottomMargins|Coleção Int32|Uma lista de margens inferior suportadas (em mícrons) para a impressora.|
|rightMargins|Coleção Int32|Uma lista de margens direitas com suporte (em mícrons) para a impressora.|
|leftMargins|Coleção Int32|Uma lista de margens esquerdas suportadas (em mícrons) para a impressora.|
|collation|Booliano|True se a impressora dá suporte à colagem ao imprimir cópias muliplas de um documento de várias páginas; false caso contrário.|
|scalings|Coleção printScaling|Dimensionamentos de impressão com suporte.|

## <a name="printerfeedorientation-values"></a>PrinterFeedOrientation values

|Membro|Valor|Descrição|
|:---|:---|
|longEdgeFirst|0|A impressora consumirá folhas da bandeja ativa na orientação "paisagem", com a borda longa da planilha primeiro.|
|shortEdgeFirst|1|A impressora consumirá folhas da bandeja ativa na orientação "retrato", com a borda curta da planilha primeiro.|
|unknownFutureValue|2|Valor de sentinela de enumeração evolvável. Não usar.|

### <a name="printquality-values"></a>valores printQuality

|Membro|Valor|Descrição|
|:---|:---|
|low|0|A impressora imprimirá o trabalho usando qualidade baixa (comumente conhecida como "rascunho").|
|medium|1|A impressora imprimirá o trabalho usando a qualidade medim (comumente conhecida como "normal").|
|high|2|A impressora imprimirá o trabalho usando qualidade alta (comumente conhecida como "melhor" ou "bem").|
|unknownFutureValue|3|Valor de sentinela de enumeração evolvável. Não usar.|

### <a name="printduplexmode-values"></a>Valores printDuplexMode

|Membro|Valor|Descrição|
|:---|:---|:---|
|flipOnLongEdge|0|A impressora imprimirá de lado duplo e inverterá documentos ao longo da borda longa.|
|flipOnShortEdge|1|A impressora imprimirá de lado duplo e inverterá documentos ao longo da borda curta.|
|oneSided|2|A impressora imprimirá de lado único.|

### <a name="printfinishing-values"></a>printFinishing values

|Membro|Valor|Descrição|
|:---|:---|:---|
|nenhuma|3|Sem acabamentos. Incluir esse valor equivale a fornecer uma coleção vazia de acabamentos.|
|staple|4 |Grampeia o documento usando a configuração de estaplagem padrão da impressora.|
|punch|5 |Fure o documento usando a configuração de buraco padrão da impressora.|
|cover|6 |Aplique uma capa ao documento.|
|bind|7 |Vinque o documento usando a configuração de associação padrão da impressora.|
|saddleStitch|8 |Estique o documento usando a configuração de ponto padrão da impressora.|
|stitchEdge|9 |Costure o documento usando a configuração de ponto padrão da impressora.|
|stapleTopLeft|20|Grampeia o documento no canto superior esquerdo.|
|stapleBottomLeft| 21 |Grampeia o documento no canto inferior esquerdo.|
|stapleTopRight|22|Grampeia o documento no canto superior direito.|
|stapleBottomRight|23|Grampeia o documento no canto inferior direito.|
|stitchLeftEdge|24|Costure o documento ao longo da borda esquerda.|
|stitchTopEdge|25|Costure o documento na borda superior.|
|stitchRightEdge|26|Costure o documento na borda direita.|
|stitchBottomEdge|27|Costure o documento na borda inferior.|
|stapleDualLeft|28|Grampeia o documento duas vezes ao longo da borda esquerda.|
|stapleDualTop|29|Grampeia o documento duas vezes ao longo da borda superior.|
|stapleDualRight|30|Grampeia o documento duas vezes ao longo da borda direita.|
|stapleDualBottom|31|Grampeia o documento duas vezes ao longo da borda inferior.|
|unknownFutureValue|32|Valor de sentinela de enumeração evolvável. Não usar.|

## <a name="printorientation-values"></a>valores printOrientation

|Membro|Valor|Descrição|
|:---|:---|:---|
|portrait|3|A impressora imprimirá impressões na orientação "retrato".|
|landscape|4 |A impressora imprimirá impressões na orientação "paisagem".|
|reverseLandscape|5 |A impressora imprimirá impressões na orientação "paisagem inversa".|
|reversePortrait|6 |A impressora imprimirá impressões na orientação "retrato reverso".|

### <a name="printmultipagelayout-values"></a>valores printMultipageLayout

|Membro|Valor|Descrição|
|:---|:---|:---|
|clockwiseFromTopLeft|0|Organize as páginas em uma grade no sentido horário começando na parte superior esquerda.|
|counterclockwiseFromTopLeft|1|Organize as páginas em uma grade no sentido anti-horário começando na parte superior esquerda.|
|counterclockwiseFromTopRight|2|Organize as páginas em uma grade no sentido anti-horário começando na parte superior direita.|
|clockwiseFromTopRight|3|Organize as páginas em uma grade no sentido horário começando na parte superior direita.|
|counterclockwiseFromBottomLeft|4 |Organize as páginas em uma grade no sentido anti-horário começando na parte inferior esquerda.|
|clockwiseFromBottomLeft|5 |Organize as páginas em uma grade no sentido horário começando na parte inferior esquerda.|
|counterclockwiseFromBottomRight|6 |Organize as páginas em uma grade no sentido anti-horário começando na parte inferior direita.|
|clockwiseFromBottomRight|7 |Organize as páginas em uma grade no sentido horário começando na parte inferior direita.|

### <a name="printcolormode-values"></a>valores printColorMode

|Membro|Valor|Descrição|
|:---|:---|:---|
|blackAndWhite|0|Preto e branco (use somente material de marcador preto.)|
|grayscale|1|Escala de cinza (pode usar algum material de marcador de cor.)|
|color|2|Cor (use qualquer combinação de materiais de marcador para criar uma impressão de cor).|
|Automático|3|Deixe a impressora decidir qual modo de cor usar.|

### <a name="printscaling-values"></a>valores printScaling

|Membro|Valor|Descrição|
|:---|:---|:---|
|Automático|0|Se o documento for maior que a mídia solicitada e as margens não são zero, a impressora dimensiona o documento como o **ajuste** printScaling. Caso contrário, a impressora dimensiona o documento usando **o fill** printScaling. Se o documento for menor que a mídia solicitada, o printScaling 'none' será usado.|
|shrinkToFit|1|Se o documento for maior do que a mídia solicitada, a impressora dimensiona o documento como o **ajuste** printScaling. Caso contrário, a impressora dimensiona o documento como **nenhum** printScaling.|
|fill|2|A impressora dimensiona o documento para preencher o tamanho de mídia solicitado, preservando sua taxa de proporção, mas potencialmente recorte partes do documento.|
|fit|3|A impressora dimensiona o documento para se ajustar à área imprimível do tamanho de mídia solicitado, preservando a proporção dos dados do documento sem o recorte do documento.|
|nenhuma|4 |A impressora não dimensiona o documento para se ajustar ao tamanho de mídia solicitado. Se o documento for maior que a mídia solicitada, a impressora centraliza e clipes a saída resultante. Se o documento for menor que a mídia solicitada, a impressora centraliza a saída resultante.|
|unknownFutureValue|5 |Valor de sentinela de enumeração evolvável. Não usar.|

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

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerCapabilities"
}-->

```json
{
  "contentTypes": [""],
  "isColorPrintingSupported": true,
  "feedOrientations": [{"@odata.type": "microsoft.graph.printerFeedOrientation"}],
  "isPageRangeSupported": true,
  "qualities": [{"@odata.type": "microsoft.graph.printQuality"}],
  "dpis": [12345],
  "duplexModes": [{"@odata.type": "microsoft.graph.printDuplexMode"}],
  "queueBufferSizeInBytes": 12345,
  "copiesPerJob": {"@odata.type": "microsoft.graph.integerRange"},
  "finishings": [{"@odata.type": "microsoft.graph.printFinishing"}],
  "mediaColors": [""],
  "mediaTypes": [""],
  "mediaSizes": [""],
  "pagesPerSheet": [12345],
  "orientations": [{"@odata.type": "microsoft.graph.printOrientation"}],
  "inputBins": [""],
  "outputBins": [""],
  "supportsFitPdfToPage": true,
  "multipageLayouts": [{"@odata.type": "microsoft.graph.printMultipageLayout"}],
  "colorModes": [{"@odata.type": "microsoft.graph.printColorMode"}],
  "topMargins": [12345],
  "bottomMargins": [12345],
  "rightMargins": [12345],
  "leftMargins": [12345],
  "collation": true,
  "scalings": [{"@odata.type": "microsoft.graph.printScaling"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerCapabilities resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

