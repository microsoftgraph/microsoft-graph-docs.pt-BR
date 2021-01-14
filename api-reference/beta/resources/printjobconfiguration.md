---
title: Tipo de recurso printJobConfiguration
description: Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 33e2873b12cb9bb689f451bcf85b2b9305120b99
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866113"
---
# <a name="printjobconfiguration-resource-type"></a>Tipo de recurso printJobConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|pageRanges|[Coleção integerRange](integerrange.md)|Os intervalos de página a ser impresso. Somente leitura.|
|quality|printQuality|A qualidade de impressão a ser usada ao imprimir o trabalho. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|dpi|Int32|A resolução a ser usada ao imprimir o trabalho, expressa em pontos por polegada (DPI). Somente leitura.|
|feedOrientation|printerFeedOrientation|A orientação a ser usada ao alimentar mídia na impressora. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|orientation|printOrientation|A configuração de orientação que a impressora deve usar ao imprimir o trabalho. Os valores válidos são descritos na tabela a seguir.|
|duplexMode|printDuplexMode|O modo duplex que a impressora deve usar ao imprimir o trabalho. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|copies|Int32|O número de cópias que devem ser impressas. Somente leitura.|
|colorMode|printColorMode|O modo de cor que a impressora deve usar para imprimir o trabalho. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|inputBin|Cadeia de caracteres|A bandeja de entrada (bandeja) a ser usada durante a impressão. Consulte os recursos da [impressora para](printercapabilities.md) ver uma lista de compartimentos de entrada com suporte.|
|outputBin|Cadeia de caracteres|A lixeira de saída a ser colocada é impressa. Consulte os recursos da [impressora para](printercapabilities.md) ver uma lista de compartimentos de saída com suporte.|
|mediaSize|Cadeia de caracteres|O tamanho de mídia a ser usado durante a impressão. Dá suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI, juntamente com qualquer tamanho personalizado compatível com a impressora associada.|
|margin|[printMargin](printmargin.md)|As configurações de margem a usar ao imprimir.|
|mediaType|Cadeia de caracteres|O tipo de mídia padrão (como papel) na qual imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|finishings|Coleção printFinishing|Processos finais a ser usado durante a impressão.|
|pagesPerSheet|Int32|O número de páginas de documento a ser impressa em cada planilha.
|multipageLayout|printMultipageLayout|A direção para o texto das páginas quando várias páginas estão sendo impressas por folha. Os valores válidos são descritos na tabela a seguir.|
|collate|Boolean|Se a impressora deve ser colada páginas que são impressas com várias cópias de um documento de várias páginas.|
|scaling|printScaling|Especifica como a impressora deve dimensionar os dados do documento para se ajustar à mídia solicitada. Os valores válidos são descritos na tabela a seguir.|

### <a name="printquality-values"></a>Valores de printQuality

|Membro|Valor|Descrição|
|:---|:---|:---|
|low|0|A impressora imprimirá o trabalho usando baixa qualidade (normalmente conhecida como "rascunho").|
|medium|1 |A impressora imprimirá o trabalho usando a qualidade medim (normalmente conhecida como "normal").|
|high|2 |A impressora imprimirá o trabalho usando qualidade alta (normalmente conhecida como "melhor" ou "fina").|
|unknownFutureValue|3 |Valor de sentinel de enumeração evolvável. Não usar.|

### <a name="printerfeedorientation-values"></a>Valores de printerFeedOrientation

|Membro|Valor|Descrição|
|:---|:---|:---|
|longEdgeFirst|0|A impressora consumirá planilhas da bandeja ativa na orientação "paisagem", com a borda longa da planilha primeiro.|
|shortEdgeFirst|1 |A impressora consumirá planilhas da bandeja ativa na orientação "retrato", com a borda curta da planilha primeiro.|
|unknownFutureValue|2 |Valor de sentinel de enumeração evolvável. Não usar.|

### <a name="printorientation-values"></a>Valores de printOrientation

|Membro|Valor|Descrição|
|:---|:---|:---|
|retrato|3 |A impressora imprimirá impressões na orientação "retrato".|
|paisagem|4 |A impressora imprimirá impressões na orientação "paisagem".|
|reverseLandscape|5 |A impressora imprimirá impressões na orientação "paisagem inversa".|
|reversePortrait|6 |A impressora imprimirá impressões na orientação "retrato reverso".|

### <a name="printduplexmode-values"></a>Valores de printDuplexMode

|Membro|Valor|Descrição|
|:---|:---|:---|
|flipOnLongEdge|0|A impressora imprimirá com duas laterais e inverterá documentos ao longo da borda longa.|
|flipOnShortEdge|1 |A impressora imprimirá com duas laterais e inverterá documentos ao longo da borda curta.|
|oneSided|2 |A impressora imprimirá de lado único.|

### <a name="printcolormode-values"></a>Valores printColorMode

|Membro|Valor|Descrição|
|:---|:---|:---|
|blackAndWhite|0|Preto e branco (use apenas material de marcador preto.)|
|escala de cinza|1 |Escala de cinza (pode usar algum material de marcador de cor.)|
|color|2 |Cor (use qualquer combinação de materiais de marcador para criar uma impressão de cor).|
|auto|3 |Deixe a impressora decidir qual modo de cor usar.|

### <a name="printfinishing-values"></a>Valores printFinishing

|Membro|Valor|Descrição|
|:---|:---|:---|
|nenhum|3 |Sem finalização. Incluir esse valor é equivalente a fornecer uma coleção vazia de terminações.|
|grampeador|4 |Grampee o documento usando a configuração de apling padrão da impressora.|
|olh|5 |Fazer o buraco no documento usando a configuração padrão do buraco da impressora.|
|cover|6 |Aplique uma capa ao documento.|
|bind|7 |Vinque o documento usando a configuração de associação padrão da impressora.|
|itchOstitch|8 |Stich-stich o documento usando a configuração de pontos padrão da impressora.|
|stitchEdge|9 |Costure o documento usando a configuração de pontos padrão da impressora.|
|stapleTopLeft|20|Grampee o documento no canto superior esquerdo.|
|stapleBottomLeft| 21 |Grampee o documento no canto inferior esquerdo.|
|stapleTopRight|22|Grampee o documento no canto superior direito.|
|stapleBottomRight|23|Grampee o documento no canto inferior direito.|
|stitchLeftEdge|24|Costure o documento na borda esquerda.|
|stitchTopEdge|25|Costure o documento na borda superior.|
|stitchRightEdge|26|Costure o documento na borda direita.|
|stitchBottomEdge|27|Costure o documento ao longo da borda inferior.|
|grampeadoDualLeft|28|Grampee o documento duas vezes ao longo da borda esquerda.|
|grampeadoDualTop|29|Grampee o documento duas vezes ao longo da borda superior.|
|grampeadoDualRight|30|Grampee o documento duas vezes ao longo da borda direita.|
|grampeadoDualBottom|31|Grampee o documento duas vezes ao longo da borda inferior.|
|unknownFutureValue|32|Valor de sentinel de enumeração evolvável. Não usar.|

### <a name="printmultipagelayout-values"></a>Valores de printMultipageLayout

|Membro|Valor|Descrição|
|:---|:---|:---|
|clockwiseFromTopLeft|0|Organize as páginas em uma grade no sentido horário começando na parte superior esquerda.|
|counterClockwiseFromTopLeft|1 |Organize as páginas em uma grade no sentido anti-horário começando na parte superior esquerda.|
|counterClockwiseFromTopRight|2 |Organize as páginas em uma grade no sentido anti-horário começando no canto superior direito.|
|clockwiseFromTopRight|3 |Organize as páginas em uma grade no sentido horário começando no canto superior direito.|
|counterClockwiseFromBottomLeft|4 |Organize as páginas em uma grade no sentido anti-horário começando na parte inferior esquerda.|
|clockwiseFromBottomLeft|5 |Organize as páginas em uma grade no sentido horário começando na parte inferior esquerda.|
|counterClockwiseFromBottomRight|6 |Organize as páginas em uma grade no sentido anti-horário começando na parte inferior direita.|
|clockwiseFromBottomRight|7 |Organize as páginas em uma grade no sentido horário começando na parte inferior direita.|

### <a name="printscaling-values"></a>Valores de printScaling

|Membro|Valor|Descrição|
|:---|:---|:---|
|auto|0|Se o documento for maior do que a mídia solicitada e as margens não são zero, a impressora dimensiona o documento como o **fit** printScaling. Caso contrário, a impressora dimensiona o documento usando **o fill** printScaling. Se o documento for menor do que a mídia solicitada, será usado o printScaling 'none'.|
|shrinkToFit|1 |Se o documento for maior que a mídia solicitada, a impressora dimensiona o documento como o **ajuste** printScaling. Caso contrário, a impressora dimensiona o documento como **nenhum** printScaling.|
|fill|2 |A impressora dimensiona o documento para preencher o tamanho de mídia solicitado, preservando sua taxa de proporção, mas potencialmente recorte partes do documento.|
|fit|3 |A impressora dimensiona o documento para se ajustar à área de impressão do tamanho de mídia solicitado, preservando a taxa de proporção dos dados do documento sem rebaixar o documento.|
|nenhum|4 |A impressora não dimensiona o documento para se ajustar ao tamanho de mídia solicitado. Se o documento for maior do que a mídia solicitada, a impressora centraliza e reclipe a saída resultante. Se o documento for menor do que a mídia solicitada, a impressora centraliza a saída resultante.|
|unknownFutureValue|5 |Valor de sentinel de enumeração evolvável. Não usar.|

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


