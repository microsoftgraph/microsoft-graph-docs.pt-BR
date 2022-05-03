---
title: Tipo de recurso printerDefaults
description: Representa as configurações padrão da impressora. Verifique os recursos da impressora para ver todos os valores compatíveis.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: b6450b1293a1b5f5b5a7a019df01b9cfb4dd4ef8
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176690"
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
|finishings|coleção printFinishing|O conjunto padrão de acabamentos a serem aplicados a trabalhos de impressão. Os valores válidos são descritos na tabela a seguir.|
|mediaColor|Cadeia de Caracteres|A cor de mídia padrão (como papel) na qual imprimir o documento.|
|mediaType|Cadeia de Caracteres|O tipo de mídia padrão (como papel) no qual imprimir o documento.|
|mediaSize|Cadeia de Caracteres|O tamanho de mídia padrão a ser usado. Dá suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI. Os valores válidos são listados no tópico [printerCapabilities](printercapabilities.md#mediasizes-values) .|
|pagesPerSheet|Int32|O número padrão de páginas de documento a serem impressas em cada planilha.
|orientation|printOrientation|A orientação padrão a ser usada ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|inputBin|Cadeia de Caracteres|O compartimento de entrada padrão que serve como a fonte de papel.|
|outputBin|Cadeia de Caracteres|O compartimento de saída padrão no qual colocar as impressões concluídas. Consulte as funcionalidades [da impressora para](printercapabilities.md) obter uma lista de compartimentos de saída com suporte.|
|fitPdfToPage|Booliano|A configuração fitPdfToPage padrão. True para ajustar cada página de um documento PDF a uma folha física de mídia; false para permitir que a impressora decida como dispor impressões.|
|multipageLayout|printMultipageLayout|A direção padrão para dispor páginas quando várias páginas estão sendo impressas por planilha. Os valores válidos são descritos na tabela a seguir.|
|Colormode|printColorMode|O modo de cor padrão a ser usado ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|Qualidade|Printquality|A qualidade padrão a ser usada ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|duplexMode|printDuplexMode|A configuração duplex padrão (frente e verso) a ser usada ao imprimir um documento. Os valores válidos são descritos na tabela a seguir.|
|dpi|Int32|A resolução padrão no DPI a ser usada ao imprimir o trabalho.|
|escala|printScaling|Especifica como a impressora dimensiona os dados do documento para se ajustar à mídia solicitada. Os valores válidos são descritos na tabela a seguir.|

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

### <a name="printquality-values"></a>valores printQuality

|Membro|Valor|Descrição|
|:---|:---|
|low|0|A impressora imprimirá o trabalho usando baixa qualidade (normalmente conhecida como "rascunho").|
|medium|1|A impressora imprimirá o trabalho usando a qualidade medim (normalmente conhecida como "normal").|
|high|2|A impressora imprimirá o trabalho usando a qualidade alta (normalmente conhecida como "melhor" ou "fina").|
|unknownFutureValue|3|Valor de sentinel de enumeração evolvável. Não usar.|

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

