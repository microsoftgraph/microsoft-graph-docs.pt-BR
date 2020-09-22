---
title: tipo de recurso printerDefaults
description: Representa as configurações padrão da impressora. Verifique os recursos da impressora para ver todos os valores que ele suporta.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: ace8b39358a5fea1645fd0ed46984d6d672897b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048838"
---
# <a name="printerdefaults-resource-type"></a>tipo de recurso printerDefaults

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações padrão da impressora. Verifique os [recursos](../api/printer-getcapabilities.md) da impressora para ver todos os valores que ele suporta.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|copiesPerJob|Int32|O número padrão de cópias impressas por trabalho.|
|contentType|String|O tipo de conteúdo padrão (MIME) a ser usado durante o processamento de documentos.|
|finishings|coleção de canacabados|O conjunto de finalidades padrão a ser aplicado aos trabalhos de impressão. Os valores válidos são descritos na tabela a seguir.|
|mediaColor|Cadeia de caracteres|A mídia padrão (como papel) em que a cor será impressa.
|mediaType|Cadeia de caracteres|O tipo de mídia padrão (como papel) para imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|mediaSize|Cadeia de caracteres|O tamanho de mídia padrão a ser usado. Dá suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI, juntamente com qualquer tamanho personalizado suportado pela impressora associada.
|pagesPerSheet|Int32|O número padrão de páginas de documento a ser impresso em cada folha.
|orientation|a reorientação|A orientação padrão a ser usada ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|outputBin|Cadeia de caracteres|O compartimento de saída padrão a ser inserido é impresso no. Confira os [recursos](../api/printer-getcapabilities.md) da impressora para obter uma lista de bandejas de saída suportadas.|
|fitPdfToPage|Booliano|A configuração padrão do fitPdfToPage. True para ajustar cada página de um documento PDF a uma folha física de mídia; false para permitir que a impressora decida como dispor as impressões.|
|multipageLayout|printMultipageLayout|A direção padrão para dispor páginas quando várias páginas estão sendo impressas por folha. Os valores válidos são descritos na tabela a seguir.|
|colorMode|addcolormode|O modo de cor padrão a ser usado ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|qualidade|printQuality|A qualidade padrão a ser usada ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|duplexmode|o defaultduplexmode|A configuração duplex padrão (frente e verso) a ser usada ao imprimir um documento. Os valores válidos são descritos na tabela a seguir.|
|dpi|Int32|A resolução padrão em DPI para usar ao imprimir o trabalho.|
|scaling|redimensionamento|Especifica como a impressora dimensiona os dados do documento para se ajustarem à mídia solicitada. Os valores válidos são descritos na tabela a seguir.|

### <a name="printmultipagelayout-values"></a>valores de printMultipageLayout

|Membro|Valor|Descrição|
|:---|:---|:---|
|clockwiseFromTopLeft|,0|Organiza as páginas em uma grade no sentido horário que começa no canto superior esquerdo.|
|counterClockwiseFromTopLeft|1 |Organiza as páginas em uma grade no sentido anti-horário que começa no canto superior esquerdo.|
|counterClockwiseFromTopRight|2 |Organiza as páginas em uma grade no sentido anti-horário que começa no canto superior direito.|
|clockwiseFromTopRight|3 |Organizar as páginas em uma grade no sentido horário começando no canto superior direito.|
|counterClockwiseFromBottomLeft|4 |Organiza as páginas em uma grade no sentido anti-horário que começa no canto inferior esquerdo.|
|clockwiseFromBottomLeft|5 |Organiza as páginas em uma grade no sentido horário que começa no canto inferior esquerdo.|
|counterClockwiseFromBottomRight|6 |Organiza as páginas em uma grade no sentido anti-horário que começa no canto inferior direito.|
|clockwiseFromBottomRight|7 |Organizar as páginas em uma grade no sentido horário começando no canto inferior direito.|

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

### <a name="printquality-values"></a>valores de PrintQuality

|Membro|Valor|Descrição|
|:---|:---|
|low|,0|A impressora imprimirá o trabalho usando a qualidade baixa (normalmente conhecida como "rascunho").|
|medium|1 |A impressora imprimirá o trabalho usando o medim (comumente conhecido como qualidade "normal").|
|high|2 |A impressora imprimirá o trabalho usando a qualidade alta (normalmente conhecida como "melhor" ou "boa").|
|unknownFutureValue|3 |Valor de sentinela de enumeração evolvable. Não usar.|

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

* [resetDefaults](../api/printer-resetdefaults.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerDefaults resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

