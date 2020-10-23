---
title: tipo de recurso printJobConfiguration
description: Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: a8d15d5b1666081f3a3ae054c209dd43a3b6eae7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728934"
---
# <a name="printjobconfiguration-resource-type"></a>tipo de recurso printJobConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|pageRanges|coleção [integerRange](integerrange.md)|Os intervalos de páginas a serem impressos. Somente leitura.|
|qualidade|printQuality|A qualidade de impressão a ser usada ao imprimir o trabalho. Os valores válidos são descritos na tabela abaixo. Somente leitura.|
|dpi|Int32|A resolução a ser usada ao imprimir o trabalho, expresso em pontos por polegada (DPI). Somente leitura.|
|feedOrientation|printerFeedOrientation|A orientação a ser usada ao alimentar mídia na impressora. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|orientation|a reorientação|A configuração de orientação que a impressora deve usar ao imprimir o trabalho. Os valores válidos são descritos na tabela a seguir.|
|duplexmode|o defaultduplexmode|O modo duplex que a impressora deve usar ao imprimir o trabalho. Os valores válidos são descritos na tabela abaixo. Somente leitura.|
|Copia|Int32|O número de cópias que devem ser impressas. Somente leitura.|
|colorMode|addcolormode|O modo de cor que a impressora deve usar para imprimir o trabalho. Os valores válidos são descritos na tabela abaixo. Somente leitura.|
|inputBin|String|O compartimento de entrada (bandeja) a ser usado ao imprimir. Confira os [recursos](../api/printer-getcapabilities.md) da impressora para obter uma lista de bandejas de entrada suportadas.|
|outputBin|String|O compartimento de saída para fazer a impressão foi concluída no. Confira os [recursos](../api/printer-getcapabilities.md) da impressora para obter uma lista de bandejas de saída suportadas.|
|mediaSize|String|O tamanho da mídiapara usar ao imprimir. Dá suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI, juntamente com qualquer tamanho personalizado suportado pela impressora associada.|
|margin|[Margem da](printmargin.md)|As configurações de margem a serem usadas ao imprimir.|
|mediaType|String|O tipo de mídia padrão (como papel) para imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|finishings|coleção de canacabados|Concluir os processos a serem usados ao imprimir.|
|pagesPerSheet|Int32|O número de páginas do documento a ser impresso em cada folha.
|multipageLayout|printMultipageLayout|A direção para dispor páginas quando várias páginas estão sendo impressas por folha. Os valores válidos são descritos na tabela a seguir.|
|collate|Booliano|Se a impressora deve agrupar páginas Wehen imprimir várias cópias de um documento com várias páginas.|
|scaling|redimensionamento|Especifica como a impressora deve dimensionar os dados do documento para se ajustarem à mídia solicitada. Os valores válidos são descritos na tabela a seguir.|

### <a name="printquality-values"></a>valores de PrintQuality

|Membro|Valor|Descrição|
|:---|:---|:---|
|low|,0|A impressora imprimirá o trabalho usando a qualidade baixa (normalmente conhecida como "rascunho").|
|medium|1|A impressora imprimirá o trabalho usando o medim (comumente conhecido como qualidade "normal").|
|high|duas|A impressora imprimirá o trabalho usando a qualidade alta (normalmente conhecida como "melhor" ou "boa").|
|unknownFutureValue|3D|Valor de sentinela de enumeração evolvable. Não usar.|

### <a name="printerfeedorientation-values"></a>valores de printerFeedOrientation

|Membro|Valor|Descrição|
|:---|:---|:---|
|longEdgeFirst|,0|A impressora consumirá planilhas da bandeja ativa na orientação "paisagem", com a borda longa da planilha primeiro.|
|shortEdgeFirst|1|A impressora consumirá planilhas da bandeja ativa na orientação "retrato", com a borda curta da planilha primeiro.|
|unknownFutureValue|duas|Valor de sentinela de enumeração evolvable. Não usar.|

### <a name="printorientation-values"></a>valores de reorientação

|Membro|Valor|Descrição|
|:---|:---|:---|
|modos|3D|A impressora imprimirá impressões na orientação "retrato".|
|paisagens|4 |A impressora imprimirá impressões na orientação "paisagem".|
|reverseLandscape|5 |A impressora imprimirá impressões na orientação "paisagem reversa".|
|reversePortrait|6 |A impressora imprimirá impressões na orientação "retrato reverso".|

### <a name="printduplexmode-values"></a>valores de reduplexmode

|Membro|Valor|Descrição|
|:---|:---|:---|
|flipOnLongEdge|,0|A impressora imprimirá em frente e voltará os documentos ao longo da borda longa.|
|flipOnShortEdge|1|A impressora imprimirá em frente e voltará os documentos ao longo da borda curta.|
|oneSided|duas|A impressora imprimirá um lado.|

### <a name="printcolormode-values"></a>valores de addcolormode

|Membro|Valor|Descrição|
|:---|:---|:---|
|blackAndWhite|,0|Preto e branco (Use apenas o material de marcador preto).|
|escala|1|Escala de cinza (pode usar algum material de marcador de cor.)|
|color|duas|Color (use qualquer combinação de materiais de marcador para criar uma impressão colorida).|
|Automático|3D|Permitir que a impressora decida qual modo de cor usar.|

### <a name="printfinishing-values"></a>valores de reconclusão de

|Membro|Valor|Descrição|
|:---|:---|:---|
|none|3D|Nenhuma conclusão. Incluir esse valor equivale a fornecer uma coleção vazia de finalidades.|
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

### <a name="printmultipagelayout-values"></a>valores de printMultipageLayout

|Membro|Valor|Descrição|
|:---|:---|:---|
|clockwiseFromTopLeft|,0|Organiza as páginas em uma grade no sentido horário que começa no canto superior esquerdo.|
|counterClockwiseFromTopLeft|1|Organiza as páginas em uma grade no sentido anti-horário que começa no canto superior esquerdo.|
|counterClockwiseFromTopRight|duas|Organiza as páginas em uma grade no sentido anti-horário que começa no canto superior direito.|
|clockwiseFromTopRight|3D|Organizar as páginas em uma grade no sentido horário começando no canto superior direito.|
|counterClockwiseFromBottomLeft|4 |Organiza as páginas em uma grade no sentido anti-horário que começa no canto inferior esquerdo.|
|clockwiseFromBottomLeft|5 |Organiza as páginas em uma grade no sentido horário que começa no canto inferior esquerdo.|
|counterClockwiseFromBottomRight|6 |Organiza as páginas em uma grade no sentido anti-horário que começa no canto inferior direito.|
|clockwiseFromBottomRight|7 |Organizar as páginas em uma grade no sentido horário começando no canto inferior direito.|

### <a name="printscaling-values"></a>valores de redimensionamento

|Membro|Valor|Descrição|
|:---|:---|:---|
|Automático|,0|Se o documento for maior do que a mídia solicitada e as margens forem diferentes de zero, a impressora dimensionará o documento como o **ajuste** à escala. Caso contrário, a impressora dimensionará o documento usando o **preenchimento** de redimensionamento. Se o documento for menor do que a mídia solicitada, a escala de impressões ' nenhum ' será usada.|
|shrinkToFit|1|Se o documento for maior do que a mídia solicitada, a impressora dimensionará o documento como o **ajuste** à escala. Caso contrário, a impressora dimensionará o documento como o formato **nenhum** .|
|fill|duas|A impressora dimensiona o documento para preencher o tamanho de mídia solicitado, preservando a taxa de proporção, mas pode cortar partes do documento.|
|contida|3D|A impressora dimensiona o documento para caber na área imprimível do tamanho de mídia solicitado, preservando a taxa de proporção dos dados do documento sem cortar o documento.|
|none|4 |A impressora não dimensiona o documento para se ajustar ao tamanho de mídia solicitado. Se o documento for maior do que a mídia solicitada, a impressora centralizará e cortará a saída resultante. Se o documento for menor do que a mídia solicitada, a impressora centralizará a saída resultante.|
|unknownFutureValue|5 |Valor de sentinela de enumeração evolvable. Não usar.|

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


