---
title: tipo complexo printerCapabilities
description: Representa os recursos relatados por uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 26d786d61f72df48f50d8241ff689f0d398ae03f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048880"
---
# <a name="printercapabilities-complex-type"></a>tipo complexo printerCapabilities

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os recursos relatados por uma impressora.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|contentTypes|Coleção de cadeias de caracteres|Uma lista de tipos de conteúdo (MIME) com suporte que a impressora suporta. Não é garantido que o serviço de impressão universal ofereça suporte à impressão de todos esses tipos MIME.|
|isColorPrintingSupported|Booliano|True se a impressão de cores for suportada pela impressora; caso contrário, false. Somente leitura.|
|feedDirections|coleção printerFeedDirection|A lista de direções de feed que são suportadas pela impressora.|
|isPageRangeSupported|Booliano|True se a impressora oferece suporte à impressão por intervalos de página; caso contrário, false.|
|qualidades|coleção PrintQuality|As qualidades de impressão suportadas pela impressora.|
|dpis|Coleção Int32|A lista de resoluções de impressão no DPI com suporte da impressora.|
|duplexModes|coleção reduplexmode|A lista de modos duplex que são suportados pela impressora. Os valores válidos são descritos na tabela a seguir.|
|queueBufferSizeInBytes|Int32|O tamanho máximo da fila de trabalhos de impressão que pode ser armazenado pela impressora.|
|copiesPerJob|[integerRange](integerrange.md)|O intervalo de cópias por trabalho suportado pela impressora.|
|finishings|coleção de canacabados|Concluir processos a impressora oferece suporte a um documento impresso.|
|mediaColors|Coleção de cadeias de caracteres|As cores de mídia (isto é, papel) suportadas pela impressora.|
|mediaTypes|Coleção de cadeias de caracteres|Os tipos de mídia com suporte da impressora. Os valores válidos são descritos na tabela a seguir.|
|mediaSizes|Coleção de cadeias de caracteres|Os tamanhos de mídia com suporte da impressora. Dá suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI, juntamente com qualquer tamanho personalizado suportado pela impressora associada.|
|pagesPerSheet|Coleção Int32|Número de páginas de entrada com suporte para impor uma única impressão.|
|orientações|coleção reorientation|As orientações de impressão suportadas pela impressora. Os valores válidos são descritos na tabela a seguir.|
|inputBins|Coleção de cadeias de caracteres|Bandejas de entrada com suporte para a impressora.|
|outputBins|Coleção de cadeias de caracteres|Os compartimentos de saída suportados da impressora (bandejas).|
|supportsFitPdfToPage|Booliano|True se a impressora suporta o dimensionamento de páginas PDF para corresponder ao tamanho da mídia de impressão; caso contrário, false.|
|multipageLayouts|coleção printMultipageLayout|As direções de apresentação suportadas pela impressora. Os valores com suporte são descritos na tabela a seguir.|
|colorModes|coleção addcolormode|Os modos de cores suportados pela impressora. Os valores válidos são descritos na tabela a seguir.|
|topMargins|Coleção Int32|Uma lista de margens superiores suportadas (em mícrons) para a impressora.|
|bottomMargins|Coleção Int32|Uma lista de margens inferiores suportadas (em mícrons) para a impressora.|
|rightMargins|Coleção Int32|Uma lista de margens direita suportadas (em mícrons) para a impressora.|
|leftMargins|Coleção Int32|Uma lista de margens esquerdas suportadas (em mícrons) para a impressora.|
|collation|Booliano|True se a impressora suportar o Agrupamento ao imprimir muliple cópias de um documento com várias páginas; caso contrário, false.|
|scalings|coleção redimensionamento|Escalas de impressão suportadas.|

## <a name="printerfeeddirection-values"></a>valores de printerFeedDirection

|Membro|Valor|Descrição|
|:---|:---|
|longEdgeFirst|,0|A impressora consumirá planilhas da bandeja ativa na orientação "paisagem", com a borda longa da planilha primeiro.|
|shortEdgeFirst|1 |A impressora consumirá planilhas da bandeja ativa na orientação "retrato", com a borda curta da planilha primeiro.|
|unknownFutureValue|2 |Valor de sentinela de enumeração evolvable. Não usar.|

### <a name="printquality-values"></a>valores de PrintQuality

|Membro|Valor|Descrição|
|:---|:---|
|low|,0|A impressora imprimirá o trabalho usando a qualidade baixa (normalmente conhecida como "rascunho").|
|medium|1 |A impressora imprimirá o trabalho usando o medim (comumente conhecido como qualidade "normal").|
|high|2 |A impressora imprimirá o trabalho usando a qualidade alta (normalmente conhecida como "melhor" ou "boa").|
|unknownFutureValue|3 |Valor de sentinela de enumeração evolvable. Não usar.|

### <a name="printduplexmode-values"></a>valores de reduplexmode

|Membro|Valor|Descrição|
|:---|:---|:---|
|flipOnLongEdge|,0|A impressora imprimirá em frente e voltará os documentos ao longo da borda longa.|
|flipOnShortEdge|1 |A impressora imprimirá em frente e voltará os documentos ao longo da borda curta.|
|oneSided|2 |A impressora imprimirá um lado.|

### <a name="printfinishing-values"></a>valores de reconclusão de

|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|3 |Nenhuma conclusão. Incluir esse valor equivale a fornecer uma coleção vazia de finalidades.|
|grampo|4 |Grampear o documento usando a configuração de associação padrão da impressora.|
|relógio|5 |Perfuração o documento usando a configuração de perfuração padrão da impressora.|
|visa|6 |Aplicar uma capa ao documento.|
|associá|7 |Vincule o documento usando a configuração de associação padrão da impressora.|
|saddleStitch|8 |Lombada-Stich o documento usando a configuração de costura padrão da impressora.|
|stitchEdge|9 |Borda-costura o documento usando a configuração de costura padrão da impressora.|
|stapleTopLeft|508|Grampear o documento no canto superior esquerdo.|
|stapleBottomLeft| 21 |Grampear o documento no canto inferior esquerdo.|
|stapleTopRight|22|Grampear o documento no canto superior direito.|
|stapleBottomRight|23|Grampo o documento no canto inferior direito.|
|stitchLeftEdge|dia|Borda-costura o documento ao longo da borda esquerda.|
|stitchTopEdge|25|Borda-costura o documento ao longo da borda superior.|
|stitchRightEdge|660|Borda-costura o documento ao longo da borda direita.|
|stitchBottomEdge|27|Borda-costura o documento ao longo da borda inferior.|
|stapleDualLeft|28|Grampear o documento duas vezes ao longo da borda esquerda.|
|stapleDualTop|anos|Grampear o documento duas vezes ao longo da borda superior.|
|stapleDualRight|até|Grampear o documento duas vezes ao longo da borda direita.|
|stapleDualBottom|31|Grampear o documento duas vezes ao longo da borda inferior.|
|unknownFutureValue|32|Valor de sentinela de enumeração evolvable. Não usar.|

## <a name="printorientation-values"></a>valores de reorientação

|Membro|Valor|Descrição|
|:---|:---|:---|
|modos|3 |A impressora imprimirá impressões na orientação "retrato".|
|paisagens|4 |A impressora imprimirá impressões na orientação "paisagem".|
|reverseLandscape|5 |A impressora imprimirá impressões na orientação "paisagem reversa".|
|reversePortrait|6 |A impressora imprimirá impressões na orientação "retrato reverso".|

### <a name="printmultipagelayout-values"></a>valores de printMultipageLayout

|Membro|Valor|Descrição|
|:---|:---|:---|
|clockwiseFromTopLeft|,0|Organiza as páginas em uma grade no sentido horário que começa no canto superior esquerdo.|
|counterclockwiseFromTopLeft|1 |Organiza as páginas em uma grade no sentido anti-horário que começa no canto superior esquerdo.|
|counterclockwiseFromTopRight|2 |Organiza as páginas em uma grade no sentido anti-horário que começa no canto superior direito.|
|clockwiseFromTopRight|3 |Organizar as páginas em uma grade no sentido horário começando no canto superior direito.|
|counterclockwiseFromBottomLeft|4 |Organiza as páginas em uma grade no sentido anti-horário que começa no canto inferior esquerdo.|
|clockwiseFromBottomLeft|5 |Organiza as páginas em uma grade no sentido horário que começa no canto inferior esquerdo.|
|counterclockwiseFromBottomRight|6 |Organiza as páginas em uma grade no sentido anti-horário que começa no canto inferior direito.|
|clockwiseFromBottomRight|7 |Organizar as páginas em uma grade no sentido horário começando no canto inferior direito.|

### <a name="printcolormode-values"></a>valores de addcolormode

|Membro|Valor|Descrição|
|:---|:---|:---|
|blackAndWhite|,0|Preto e branco (Use apenas o material de marcador preto).|
|escala|1 |Escala de cinza (pode usar algum material de marcador de cor.)|
|color|2 |Color (use qualquer combinação de materiais de marcador para criar uma impressão colorida).|
|Automático|3 |Permitir que a impressora decida qual modo de cor usar.|

### <a name="printscaling-values"></a>valores de redimensionamento

|Membro|Valor|Descrição|
|:---|:---|:---|
|Automático|,0|Se o documento for maior do que a mídia solicitada e as margens forem diferentes de zero, a impressora dimensionará o documento como o **ajuste** à escala. Caso contrário, a impressora dimensionará o documento usando o **preenchimento** de redimensionamento. Se o documento for menor do que a mídia solicitada, a escala de impressões ' nenhum ' será usada.|
|shrinkToFit|1 |Se o documento for maior do que a mídia solicitada, a impressora dimensionará o documento como o **ajuste** à escala. Caso contrário, a impressora dimensionará o documento como o formato **nenhum** .|
|fill|2 |A impressora dimensiona o documento para preencher o tamanho de mídia solicitado, preservando a taxa de proporção, mas pode cortar partes do documento.|
|contida|3 |A impressora dimensiona o documento para caber na área imprimível do tamanho de mídia solicitado, preservando a taxa de proporção dos dados do documento sem cortar o documento.|
|Nenhuma|4 |A impressora não dimensiona o documento para se ajustar ao tamanho de mídia solicitado. Se o documento for maior do que a mídia solicitada, a impressora centralizará e cortará a saída resultante. Se o documento for menor do que a mídia solicitada, a impressora centralizará a saída resultante.|
|unknownFutureValue|5 |Valor de sentinela de enumeração evolvable. Não usar.|

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
  "feedDirections": [{"@odata.type": "microsoft.graph.printerFeedDirection"}],
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

