---
title: Tipo de recurso printerDefaults
description: Representa as configurações padrão da impressora. Verifique os recursos da impressora para ver todos os valores compatíveis.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: efc0c59774967a1ef135c0f90ec3e5c57b97b9c5
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944132"
---
# <a name="printerdefaults-resource-type"></a>Tipo de recurso printerDefaults

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações padrão da impressora. Verifique os recursos da [impressora para](printercapabilities.md) ver todos os valores compatíveis.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|copiesPerJob|Int32|O número padrão de cópias impressas por trabalho.|
|contentType|String|O tipo de conteúdo padrão (MIME) a ser usado ao processar documentos.|
|finishings|Coleção printFinishing|O conjunto padrão de acabamentos a ser aplicado a trabalhos de impressão. Os valores válidos são descritos na tabela a seguir.|
|mediaColor|Cadeia de caracteres|A cor padrão da mídia (como papel) para imprimir o documento.|
|mediaType|Cadeia de caracteres|O tipo de mídia padrão (como papel) para imprimir o documento.|
|mediaSize|Cadeia de caracteres|O tamanho de mídia padrão a ser usado. Oferece suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI. Os valores válidos são listados no tópico [printerCapabilities.](printercapabilities.md#mediasizes-values)|
|pagesPerSheet|Int32|O número padrão de páginas de documento a ser impressa em cada planilha.
|orientation|printOrientation|A orientação padrão a ser usada ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|inputBin|Cadeia de caracteres|A lixeira de entrada padrão que serve como a fonte de papel.|
|outputBin|Cadeia de caracteres|A lixeira de saída padrão para colocar as impressões concluídas. Consulte os recursos da [impressora para](printercapabilities.md) uma lista de caixas de saída com suporte.|
|fitPdfToPage|Booliano|A configuração padrão fitPdfToPage. True para ajustar cada página de um documento PDF a uma folha física de mídia; false para permitir que a impressora decida como definir impressões.|
|multipageLayout|printMultipageLayout|A direção padrão para colocar as páginas quando várias páginas estão sendo impressas por planilha. Os valores válidos são descritos na tabela a seguir.|
|colorMode|printColorMode|O modo de cor padrão a ser usado ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|quality|printQuality|A qualidade padrão a ser usada ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|duplexMode|printDuplexMode|A configuração duplex padrão (com duas laterais) a ser usada ao imprimir um documento. Os valores válidos são descritos na tabela a seguir.|
|dpi|Int32|A resolução padrão no DPI a ser usada ao imprimir o trabalho.|
|scaling|printScaling|Especifica como a impressora dimensiona os dados do documento para se ajustar à mídia solicitada. Os valores válidos são descritos na tabela a seguir.|

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

### <a name="printquality-values"></a>valores printQuality

|Membro|Valor|Descrição|
|:---|:---|
|low|0|A impressora imprimirá o trabalho usando qualidade baixa (comumente conhecida como "rascunho").|
|medium|1|A impressora imprimirá o trabalho usando a qualidade medim (comumente conhecida como "normal").|
|high|2|A impressora imprimirá o trabalho usando qualidade alta (comumente conhecida como "melhor" ou "bem").|
|unknownFutureValue|3|Valor de sentinela de enumeração evolvável. Não usar.|

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

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerDefaults"
}-->

```json
{
  "copiesPerJob": 123456,
  "contentType": "String",
  "finishings": ["String"],
  "mediaColor": "String",
  "mediaSize": "String",
  "pagesPerSheet": 123456,
  "orientation": "String",
  "outputBin": "String",
  "fitPdfToPage": true,
  "multipageLayout": "String",
  "colorMode": "String",
  "quality": "String",
  "duplexMode": "String"
}

```

## <a name="see-also"></a>Confira também

* [restoreFactoryDefaults](../api/printer-restorefactorydefaults.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerDefaults resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

