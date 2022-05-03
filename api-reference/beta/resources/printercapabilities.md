---
title: Tipo complexo printerCapabilities
description: Representa os recursos relatados por uma impressora.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 045fd0b29b1cf6c1baa0d70659556d2f49a3391c
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176360"
---
# <a name="printercapabilities-complex-type"></a>Tipo complexo printerCapabilities

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os recursos relatados por uma impressora.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|contentTypes|Coleção de cadeias de caracteres|Uma lista de tipos de conteúdo com suporte (MIME) compatíveis com a impressora. Não há garantia de que o serviço de Impressão Universal dê suporte à impressão de todos esses tipos MIME.|
|isColorPrintingSupported|Booliano|True se a impressão de cores é compatível com a impressora; caso contrário, false. Somente leitura.|
|feedOrientations|Coleção printerFeedOrientation|A lista de orientações de feed compatíveis com a impressora.|
|isPageRangeSupported|Booliano|True se a impressora dá suporte à impressão por intervalos de páginas; caso contrário, false.|
|Qualidades|coleção printQuality|As qualidades de impressão compatíveis com a impressora.|
|dpis|Coleção Int32|A lista de resoluções de impressão em DPI compatíveis com a impressora.|
|duplexModes|Coleção printDuplexMode|A lista de modos duplex compatíveis com a impressora. Os valores válidos são descritos na tabela a seguir.|
|queueBufferSizeInBytes|Int32|O tamanho máximo da fila de trabalhos de impressão que pode ser armazenado pela impressora.|
|copiesPerJob|[integerRange](integerrange.md)|O intervalo de cópias por trabalho compatível com a impressora.|
|finishings|coleção printFinishing|Processos de conclusão aos quais a impressora dá suporte para um documento impresso.|
|mediaColors|Conjunto de cadeias de caracteres|As cores de mídia (ou seja, papel) compatíveis com a impressora.|
|mediaTypes|Coleção de cadeias de caracteres|Os tipos de mídia compatíveis com a impressora.|
|mediaSizes|Conjunto de cadeias de caracteres|Os tamanhos de mídia compatíveis com a impressora. Dá suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI. Os valores válidos estão na tabela a [seguir](#mediasizes-values).|
|pagesPerSheet|Coleção Int32|Número com suporte de Páginas de Entrada para impor uma única Impressão.|
|Orientações|Coleção printOrientation|As orientações de impressão compatíveis com a impressora. Os valores válidos são descritos na tabela a seguir.|
|inputBins|Coleção de cadeias de caracteres|Compartimentos de entrada com suporte para a impressora.|
|outputBins|Conjunto de cadeias de caracteres|Os compartimentos de saída com suporte da impressora (bandejas).|
|supportsFitPdfToPage|Booliano|True se a impressora dá suporte ao dimensionamento de páginas PDF para corresponder ao tamanho da mídia de impressão; caso contrário, false.|
|multipageLayouts|Coleção printMultipageLayout|As instruções de apresentação compatíveis com a impressora. Os valores com suporte são descritos na tabela a seguir.|
|colorModes|coleção printColorMode|Os modos de cor compatíveis com a impressora. Os valores válidos são descritos na tabela a seguir.|
|topMargins|Coleção Int32|Uma lista de margens principais com suporte (em mícrons) para a impressora.|
|bottomMargins|Coleção Int32|Uma lista de margens  inferior com suporte (em mícrons) para a impressora.|
|rightMargins|Coleção Int32|Uma lista de margens direitas com suporte (em mícrons) para a impressora.|
|leftMargins|Coleção Int32|Uma lista de margens esquerdas com suporte (em mícrons) para a impressora.|
|ordenação|Boolean|True se a impressora dá suporte à colagem ao imprimir cópias muliplas de um documento de várias páginas; caso contrário, false.|
|scalings|Coleção printScaling|Dimensionamentos de impressão com suporte.|

## <a name="printerfeedorientation-values"></a>Valores printerFeedOrientation

|Membro|Valor|Descrição|
|:---|:---|
|longEdgeFirst|0|A impressora consumirá planilhas da bandeja ativa na orientação "paisagem", com a borda longa da planilha primeiro.|
|shortEdgeFirst|1|A impressora consumirá planilhas da bandeja ativa na orientação "retrato", com a borda curta da planilha primeiro.|
|unknownFutureValue|2|Valor de sentinel de enumeração evolvável. Não usar.|

### <a name="printquality-values"></a>valores printQuality

|Membro|Valor|Descrição|
|:---|:---|
|low|0|A impressora imprimirá o trabalho usando baixa qualidade (normalmente conhecida como "rascunho").|
|medium|1|A impressora imprimirá o trabalho usando a qualidade medim (normalmente conhecida como "normal").|
|high|2|A impressora imprimirá o trabalho usando a qualidade alta (normalmente conhecida como "melhor" ou "fina").|
|unknownFutureValue|3|Valor de sentinel de enumeração evolvável. Não usar.|

### <a name="printduplexmode-values"></a>Valores printDuplexMode

|Membro|Valor|Descrição|
|:---|:---|:---|
|flipOnLongEdge|0|A impressora imprimirá em dois lados e inverterá os documentos ao longo da borda longa.|
|flipOnShortEdge|1|A impressora imprimirá em dois lados e inverterá os documentos ao longo da borda curta.|
|oneSided|2|A impressora imprimirá em um único lado.|

### <a name="printfinishing-values"></a>valores printFinishing

|Membro|Valor|Descrição|
|:---|:---|:---|
|none|3|Sem acabamentos. Incluir esse valor é equivalente a fornecer uma coleção vazia de acabamentos.|
|Grampo|4|Grampeia o documento usando a configuração de grampeamento padrão da impressora.|
|Soco|5|O furo esburaça o documento usando a configuração de furo padrão da impressora.|
|Cobrir|6 |Aplique uma capa ao documento.|
|Ligar|7 |Associe o documento usando a configuração de associação padrão da impressora.|
|saddleStitch|8 |Sele o documento usando a configuração de costura padrão da impressora.|
|stitchEdge|9 |Costure o documento usando a configuração de costura padrão da impressora.|
|stapleTopLeft|20|Grampeia o documento no canto superior esquerdo.|
|stapleBottomLeft| 21 |Grampeia o documento no canto inferior esquerdo.|
|stapleTopRight|22|Grampeia o documento no canto superior direito.|
|stapleBottomRight|23|Grampeia o documento no canto inferior direito.|
|stitchLeftEdge|24|Costure o documento na borda esquerda.|
|stitchTopEdge|25|Costure o documento na borda superior.|
|stitchRightEdge|26|Costure o documento na borda direita.|
|stitchBottomEdge|27|Costure o documento na borda inferior.|
|stapleDualLeft|28|Grampeia o documento duas vezes ao longo da borda esquerda.|
|stapleDualTop|29|Grampeia o documento duas vezes ao longo da borda superior.|
|stapleDualRight|30|Grampeia o documento duas vezes ao longo da borda direita.|
|stapleDualBottom|31|Grampeia o documento duas vezes ao longo da borda inferior.|
|unknownFutureValue|32|Valor de sentinel de enumeração evolvável. Não usar.|

## <a name="printorientation-values"></a>Valores printOrientation

|Membro|Valor|Descrição|
|:---|:---|:---|
|Retrato|3|A impressora imprimirá impressões na orientação "retrato".|
|Paisagem|4|A impressora imprimirá impressões na orientação "paisagem".|
|reverseLandscape|5|A impressora imprimirá impressões na orientação "paisagem inversa".|
|reversePortrait|6 |A impressora imprimirá impressões na orientação "retrato reverso".|

### <a name="printmultipagelayout-values"></a>Valores printMultipageLayout

|Membro|Valor|Descrição|
|:---|:---|:---|
|clockwiseFromTopLeft|0|Organize as páginas em uma grade no sentido horário começando no canto superior esquerdo.|
|counterclockwiseFromTopLeft|1|Organize as páginas em uma grade no sentido anti-horário começando no canto superior esquerdo.|
|counterclockwiseFromTopRight|2|Organize as páginas em uma grade no sentido anti-horário começando no canto superior direito.|
|clockwiseFromTopRight|3|Organize as páginas em uma grade no sentido horário começando no canto superior direito.|
|counterclockwiseFromBottomLeft|4|Organize as páginas em uma grade no sentido anti-horário começando na parte inferior esquerda.|
|clockwiseFromBottomLeft|5|Organize as páginas em uma grade no sentido horário começando na parte inferior esquerda.|
|counterclockwiseFromBottomRight|6 |Organize as páginas em uma grade no sentido anti-horário começando no canto inferior direito.|
|clockwiseFromBottomRight|7 |Organize as páginas em uma grade no sentido horário começando no canto inferior direito.|

### <a name="printcolormode-values"></a>Valores printColorMode

|Membro|Valor|Descrição|
|:---|:---|:---|
|blackAndWhite|0|Preto e branco (use somente material de marcador preto.)|
|Cinza|1|Escala de cinza (pode usar algum material de marcador de cor.)|
|color|2|Cor (use qualquer combinação de materiais de marcador para criar uma impressão de cor).|
|Automático|3|Deixe a impressora decidir qual modo de cor usar.|

### <a name="printscaling-values"></a>Valores printScaling

|Membro|Valor|Descrição|
|:---|:---|:---|
|Automático|0|Se o documento for maior que a mídia solicitada e as margens forem diferentes de zero, a impressora dimensiona o documento como o **ajuste** printScaling. Caso contrário, a impressora dimensiona o documento usando **o fill** printScaling. Se o documento for menor do que a mídia solicitada, 'none' printScaling será usado.|
|Shrinktofit|1|Se o documento for maior que a mídia solicitada, a impressora dimensiona o documento como o **ajuste** printScaling. Caso contrário, a impressora dimensiona o documento como **nenhum** printScaling.|
|fill|2|A impressora dimensiona o documento para preencher o tamanho de mídia solicitado, preservando sua taxa de proporção, mas potencialmente cortando partes do documento.|
|Caber|3|A impressora dimensiona o documento para se ajustar à área imprimível do tamanho de mídia solicitado, preservando a taxa de proporção dos dados do documento sem cortar o documento.|
|none|4|A impressora não dimensiona o documento para se ajustar ao tamanho de mídia solicitado. Se o documento for maior que a mídia solicitada, a impressora centraliza e clipes a saída resultante. Se o documento for menor que a mídia solicitada, a impressora centraliza a saída resultante.|
|unknownFutureValue|5|Valor de sentinel de enumeração evolvável. Não usar.|

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
|América do Norte Executivo|
|América do Norte Carta de Confirmação|
|América do Norte índice 3x5in|
|América do Norte índice 4x8in|
|América do Norte índice 5x8in|
|América do Norte fatura|
|América do Norte Razão|
|América do Norte Legal|
|América do Norte carta|
|Foto l 3.5x5in|
|Cartão de visita|
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

