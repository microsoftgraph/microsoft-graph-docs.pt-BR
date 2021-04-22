---
title: Tipo de recurso printJobConfiguration
description: Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5eeee682ca5e854fdcb2589089b873900b598f4e
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944258"
---
# <a name="printjobconfiguration-resource-type"></a>Tipo de recurso printJobConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|pageRanges|[Coleção integerRange](integerrange.md)|A página varia para imprimir. Somente leitura.|
|quality|printQuality|A qualidade de impressão a ser usada ao imprimir o trabalho. Os valores válidos são descritos na tabela abaixo. Somente leitura.|
|dpi|Int32|A resolução a ser usada ao imprimir o trabalho, expressa em pontos por polegada (DPI). Somente leitura.|
|feedOrientation|printerFeedOrientation|A orientação a ser usada ao alimentar mídia na impressora. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|orientation|printOrientation|A configuração de orientação que a impressora deve usar ao imprimir o trabalho. Os valores válidos são descritos na tabela a seguir.|
|duplexMode|printDuplexMode|O modo duplex que a impressora deve usar ao imprimir o trabalho. Os valores válidos são descritos na tabela abaixo. Somente leitura.|
|copies|Int32|O número de cópias que devem ser impressas. Somente leitura.|
|colorMode|printColorMode|O modo de cor que a impressora deve usar para imprimir o trabalho. Os valores válidos são descritos na tabela abaixo. Somente leitura.|
|inputBin|Cadeia de caracteres|A bandeja de entrada (bandeja) a ser usada durante a impressão. Consulte os recursos da [impressora para](printercapabilities.md) uma lista de caixas de entrada com suporte.|
|outputBin|Cadeia de caracteres|A lixeira de saída para colocar as impressões concluídas. Consulte os recursos da [impressora para](printercapabilities.md) uma lista de caixas de saída com suporte.|
|mediaSize|Cadeia de caracteres|O tamanho da mídia a ser usado ao imprimir. Oferece suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI. Os valores válidos são listados no tópico [printerCapabilities.](printercapabilities.md#mediasizes-values)|
|margin|[printMargin](printmargin.md)|As configurações de margem a ser usadas ao imprimir.|
|mediaType|Cadeia de caracteres|O tipo de mídia padrão (como papel) para imprimir o documento.|
|finishings|Coleção printFinishing|Processos de término a ser usado ao imprimir.|
|pagesPerSheet|Int32|O número de páginas de documento a ser impressa em cada planilha.
|multipageLayout|printMultipageLayout|A direção para colocar as páginas quando várias páginas estão sendo impressas por planilha. Os valores válidos são descritos na tabela a seguir.|
|collate|Booliano|Se a impressora deve colá-los para imprimir várias cópias de um documento de várias páginas.|
|scaling|printScaling|Especifica como a impressora deve dimensionar os dados do documento para se ajustar à mídia solicitada. Os valores válidos são descritos na tabela a seguir.|

### <a name="printquality-values"></a>valores printQuality

|Membro|Valor|Descrição|
|:---|:---|:---|
|low|0|A impressora imprimirá o trabalho usando qualidade baixa (comumente conhecida como "rascunho").|
|medium|1|A impressora imprimirá o trabalho usando a qualidade medim (comumente conhecida como "normal").|
|high|2|A impressora imprimirá o trabalho usando qualidade alta (comumente conhecida como "melhor" ou "bem").|
|unknownFutureValue|3|Valor de sentinela de enumeração evolvável. Não usar.|

### <a name="printerfeedorientation-values"></a>PrinterFeedOrientation values

|Membro|Valor|Descrição|
|:---|:---|:---|
|longEdgeFirst|0|A impressora consumirá folhas da bandeja ativa na orientação "paisagem", com a borda longa da planilha primeiro.|
|shortEdgeFirst|1|A impressora consumirá folhas da bandeja ativa na orientação "retrato", com a borda curta da planilha primeiro.|
|unknownFutureValue|2|Valor de sentinela de enumeração evolvável. Não usar.|

### <a name="printorientation-values"></a>valores printOrientation

|Membro|Valor|Descrição|
|:---|:---|:---|
|portrait|3|A impressora imprimirá impressões na orientação "retrato".|
|landscape|4 |A impressora imprimirá impressões na orientação "paisagem".|
|reverseLandscape|5 |A impressora imprimirá impressões na orientação "paisagem inversa".|
|reversePortrait|6 |A impressora imprimirá impressões na orientação "retrato reverso".|

### <a name="printduplexmode-values"></a>Valores printDuplexMode

|Membro|Valor|Descrição|
|:---|:---|:---|
|flipOnLongEdge|0|A impressora imprimirá de lado duplo e inverterá documentos ao longo da borda longa.|
|flipOnShortEdge|1|A impressora imprimirá de lado duplo e inverterá documentos ao longo da borda curta.|
|oneSided|2|A impressora imprimirá de lado único.|

### <a name="printcolormode-values"></a>valores printColorMode

|Membro|Valor|Descrição|
|:---|:---|:---|
|blackAndWhite|0|Preto e branco (use somente material de marcador preto.)|
|grayscale|1|Escala de cinza (pode usar algum material de marcador de cor.)|
|color|2|Cor (use qualquer combinação de materiais de marcador para criar uma impressão de cor).|
|Automático|3|Deixe a impressora decidir qual modo de cor usar.|

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

### <a name="printmultipagelayout-values"></a>valores printMultipageLayout

|Membro|Valor|Descrição|
|:---|:---|:---|
|clockwiseFromTopLeft|0|Organize as páginas em uma grade no sentido horário começando na parte superior esquerda.|
|counterClockwiseFromTopLeft|1|Organize as páginas em uma grade no sentido anti-horário começando na parte superior esquerda.|
|counterClockwiseFromTopRight|2|Organize as páginas em uma grade no sentido anti-horário começando na parte superior direita.|
|clockwiseFromTopRight|3|Organize as páginas em uma grade no sentido horário começando na parte superior direita.|
|counterClockwiseFromBottomLeft|4 |Organize as páginas em uma grade no sentido anti-horário começando na parte inferior esquerda.|
|clockwiseFromBottomLeft|5 |Organize as páginas em uma grade no sentido horário começando na parte inferior esquerda.|
|counterClockwiseFromBottomRight|6 |Organize as páginas em uma grade no sentido anti-horário começando na parte inferior direita.|
|clockwiseFromBottomRight|7 |Organize as páginas em uma grade no sentido horário começando na parte inferior direita.|

### <a name="printscaling-values"></a>valores printScaling

|Membro|Valor|Descrição|
|:---|:---|:---|
|Automático|0|Se o documento for maior que a mídia solicitada e as margens não são zero, a impressora dimensiona o documento como o **ajuste** printScaling. Caso contrário, a impressora dimensiona o documento usando **o fill** printScaling. Se o documento for menor que a mídia solicitada, o printScaling 'none' será usado.|
|shrinkToFit|1|Se o documento for maior do que a mídia solicitada, a impressora dimensiona o documento como o **ajuste** printScaling. Caso contrário, a impressora dimensiona o documento como **nenhum** printScaling.|
|fill|2|A impressora dimensiona o documento para preencher o tamanho de mídia solicitado, preservando sua taxa de proporção, mas potencialmente recorte partes do documento.|
|fit|3|A impressora dimensiona o documento para se ajustar à área imprimível do tamanho de mídia solicitado, preservando a proporção dos dados do documento sem o recorte do documento.|
|nenhuma|4 |A impressora não dimensiona o documento para se ajustar ao tamanho de mídia solicitado. Se o documento for maior que a mídia solicitada, a impressora centraliza e clipes a saída resultante. Se o documento for menor que a mídia solicitada, a impressora centraliza a saída resultante.|
|unknownFutureValue|5 |Valor de sentinela de enumeração evolvável. Não usar.|

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


