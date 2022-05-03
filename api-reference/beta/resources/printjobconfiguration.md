---
title: Tipo de recurso printJobConfiguration
description: Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 3579a8ca5e8bc7fa238456fc3d368d3c101acdca
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176952"
---
# <a name="printjobconfiguration-resource-type"></a>Tipo de recurso printJobConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|pageRanges|[Coleção integerRange](integerrange.md)|Os intervalos de páginas a serem impressos. Somente leitura.|
|Qualidade|Printquality|A qualidade de impressão a ser usada ao imprimir o trabalho. Os valores válidos são descritos na tabela abaixo. Somente leitura.|
|dpi|Int32|A resolução a ser usada ao imprimir o trabalho, expressa em pontos por polegada (DPI). Somente leitura.|
|feedOrientation|printerFeedOrientation|A orientação a ser usada ao alimentar a mídia na impressora. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|orientation|printOrientation|A configuração de orientação que a impressora deve usar ao imprimir o trabalho. Os valores válidos são descritos na tabela a seguir.|
|duplexMode|printDuplexMode|O modo duplex que a impressora deve usar ao imprimir o trabalho. Os valores válidos são descritos na tabela abaixo. Somente leitura.|
|Cópias|Int32|O número de cópias que devem ser impressas. Somente leitura.|
|Colormode|printColorMode|O modo de cor que a impressora deve usar para imprimir o trabalho. Os valores válidos são descritos na tabela abaixo. Somente leitura.|
|inputBin|Cadeia de Caracteres|A bandeja de entrada (bandeja) a ser usada durante a impressão. Consulte as funcionalidades [da impressora para](printercapabilities.md) obter uma lista de compartimentos de entrada com suporte.|
|outputBin|Cadeia de Caracteres|O compartimento de saída no qual colocar as impressões concluídas. Consulte as funcionalidades [da impressora para](printercapabilities.md) obter uma lista de compartimentos de saída com suporte.|
|mediaSize|Cadeia de Caracteres|O tamanho da mídia a ser usado durante a impressão. Dá suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI. Os valores válidos são listados no tópico [printerCapabilities](printercapabilities.md#mediasizes-values) .|
|margin|[printMargin](printmargin.md)|As configurações de margem a serem usadas durante a impressão.|
|mediaType|Cadeia de Caracteres|O tipo de mídia padrão (como papel) no qual imprimir o documento.|
|finishings|coleção printFinishing|Concluir processos a serem usados ao imprimir.|
|pagesPerSheet|Int32|O número de páginas de documento a serem impressas em cada planilha.
|multipageLayout|printMultipageLayout|A direção para dispor páginas quando várias páginas estão sendo impressas por planilha. Os valores válidos são descritos na tabela a seguir.|
|collate|Booliano|Se a impressora deve agrupar páginas para imprimir várias cópias de um documento de várias páginas.|
|escala|printScaling|Especifica como a impressora deve dimensionar os dados do documento para se ajustar à mídia solicitada. Os valores válidos são descritos na tabela a seguir.|

### <a name="printquality-values"></a>valores printQuality

|Membro|Valor|Descrição|
|:---|:---|:---|
|low|0|A impressora imprimirá o trabalho usando baixa qualidade (normalmente conhecida como "rascunho").|
|medium|1|A impressora imprimirá o trabalho usando a qualidade medim (normalmente conhecida como "normal").|
|high|2|A impressora imprimirá o trabalho usando a qualidade alta (normalmente conhecida como "melhor" ou "fina").|
|unknownFutureValue|3|Valor de sentinel de enumeração evolvável. Não usar.|

### <a name="printerfeedorientation-values"></a>Valores printerFeedOrientation

|Membro|Valor|Descrição|
|:---|:---|:---|
|longEdgeFirst|0|A impressora consumirá planilhas da bandeja ativa na orientação "paisagem", com a borda longa da planilha primeiro.|
|shortEdgeFirst|1|A impressora consumirá planilhas da bandeja ativa na orientação "retrato", com a borda curta da planilha primeiro.|
|unknownFutureValue|2|Valor de sentinel de enumeração evolvável. Não usar.|

### <a name="printorientation-values"></a>Valores printOrientation

|Membro|Valor|Descrição|
|:---|:---|:---|
|Retrato|3|A impressora imprimirá impressões na orientação "retrato".|
|Paisagem|4|A impressora imprimirá impressões na orientação "paisagem".|
|reverseLandscape|5|A impressora imprimirá impressões na orientação "paisagem inversa".|
|reversePortrait|6 |A impressora imprimirá impressões na orientação "retrato reverso".|

### <a name="printduplexmode-values"></a>Valores printDuplexMode

|Membro|Valor|Descrição|
|:---|:---|:---|
|flipOnLongEdge|0|A impressora imprimirá em dois lados e inverterá os documentos ao longo da borda longa.|
|flipOnShortEdge|1|A impressora imprimirá em dois lados e inverterá os documentos ao longo da borda curta.|
|oneSided|2|A impressora imprimirá em um único lado.|

### <a name="printcolormode-values"></a>Valores printColorMode

|Membro|Valor|Descrição|
|:---|:---|:---|
|blackAndWhite|0|Preto e branco (use somente material de marcador preto.)|
|Cinza|1|Escala de cinza (pode usar algum material de marcador de cor.)|
|color|2|Cor (use qualquer combinação de materiais de marcador para criar uma impressão de cor).|
|Automático|3|Deixe a impressora decidir qual modo de cor usar.|

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

### <a name="printmultipagelayout-values"></a>Valores printMultipageLayout

|Membro|Valor|Descrição|
|:---|:---|:---|
|clockwiseFromTopLeft|0|Organize as páginas em uma grade no sentido horário começando no canto superior esquerdo.|
|counterClockwiseFromTopLeft|1|Organize as páginas em uma grade no sentido anti-horário começando no canto superior esquerdo.|
|counterClockwiseFromTopRight|2|Organize as páginas em uma grade no sentido anti-horário começando no canto superior direito.|
|clockwiseFromTopRight|3|Organize as páginas em uma grade no sentido horário começando no canto superior direito.|
|counterClockwiseFromBottomLeft|4|Organize as páginas em uma grade no sentido anti-horário começando na parte inferior esquerda.|
|clockwiseFromBottomLeft|5|Organize as páginas em uma grade no sentido horário começando na parte inferior esquerda.|
|counterClockwiseFromBottomRight|6 |Organize as páginas em uma grade no sentido anti-horário começando no canto inferior direito.|
|clockwiseFromBottomRight|7 |Organize as páginas em uma grade no sentido horário começando no canto inferior direito.|

### <a name="printscaling-values"></a>Valores printScaling

|Membro|Valor|Descrição|
|:---|:---|:---|
|Automático|0|Se o documento for maior que a mídia solicitada e as margens forem diferentes de zero, a impressora dimensiona o documento como o **ajuste** printScaling. Caso contrário, a impressora dimensiona o documento usando **o fill** printScaling. Se o documento for menor do que a mídia solicitada, 'none' printScaling será usado.|
|Shrinktofit|1|Se o documento for maior que a mídia solicitada, a impressora dimensiona o documento como o **ajuste** printScaling. Caso contrário, a impressora dimensiona o documento como **nenhum** printScaling.|
|fill|2|A impressora dimensiona o documento para preencher o tamanho de mídia solicitado, preservando sua taxa de proporção, mas potencialmente cortando partes do documento.|
|Caber|3|A impressora dimensiona o documento para se ajustar à área imprimível do tamanho de mídia solicitado, preservando a taxa de proporção dos dados do documento sem cortar o documento.|
|none|4|A impressora não dimensiona o documento para se ajustar ao tamanho de mídia solicitado. Se o documento for maior que a mídia solicitada, a impressora centraliza e clipes a saída resultante. Se o documento for menor que a mídia solicitada, a impressora centraliza a saída resultante.|
|unknownFutureValue|5|Valor de sentinel de enumeração evolvável. Não usar.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJobConfiguration"
}-->

```json
{
  "pageRanges": [{"@odata.type": "microsoft.graph.integerRange"}],
  "quality": {"@odata.type": "microsoft.graph.printQuality"},
  "dpi": 12345,
  "feedOrientation": {"@odata.type": "microsoft.graph.printerFeedOrientation"},
  "orientation": {"@odata.type": "microsoft.graph.printOrientation"},
  "duplexMode": {"@odata.type": "microsoft.graph.printDuplexMode"},
  "copies": 12345,
  "colorMode": {"@odata.type": "microsoft.graph.printColorMode"},
  "inputBin": "",
  "outputBin": "",
  "mediaSize": "",
  "margin": {"@odata.type": "microsoft.graph.printMargin"},
  "mediaType": "",
  "finishings": [{"@odata.type": "microsoft.graph.printFinishing"}],
  "pagesPerSheet": 12345,
  "multipageLayout": {"@odata.type": "microsoft.graph.printMultipageLayout"},
  "collate": true,
  "scaling": {"@odata.type": "microsoft.graph.printScaling"}
}
```


