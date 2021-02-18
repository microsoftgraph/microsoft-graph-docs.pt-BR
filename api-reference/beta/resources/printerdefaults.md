---
title: Tipo de recurso printerDefaults
description: Representa as configurações padrão da impressora. Verifique os recursos da impressora para ver todos os valores compatíveis.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7121760cc823470a0ea7b64e57cab8f61b231be8
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292609"
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
|finishings|Coleção printFinishing|O conjunto padrão de términos a ser aplicado aos trabalhos de impressão. Os valores válidos são descritos na tabela a seguir.|
|mediaColor|String|A cor de mídia padrão (como papel) na onde imprimir o documento.
|mediaType|String|O tipo de mídia padrão (como papel) na qual imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|mediaSize|String|O tamanho de mídia padrão a ser usado. Dá suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI, juntamente com qualquer tamanho personalizado compatível com a impressora associada.
|pagesPerSheet|Int32|O número padrão de páginas de documento a ser impressa em cada planilha.
|orientation|printOrientation|A orientação padrão a ser usada ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|inputBin|String|A lixeira de entrada padrão que serve como fonte de papel.|
|outputBin|String|A lixeira de saída padrão a ser colocada é impressa. Consulte os recursos da [impressora para](printercapabilities.md) ver uma lista de compartimentos de saída com suporte.|
|fitPdfToPage|Booliano|A configuração padrão fitPdfToPage. True para ajustar cada página de um documento PDF a uma folha física de mídia; false para permitir que a impressora decida como definir impressões.|
|multipageLayout|printMultipageLayout|A direção padrão para o texto das páginas quando várias páginas estão sendo impressas por planilha. Os valores válidos são descritos na tabela a seguir.|
|colorMode|printColorMode|O modo de cor padrão a ser usado ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|quality|printQuality|A qualidade padrão a ser usada ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|duplexMode|printDuplexMode|A configuração duplex padrão (lado a lado duplo) a ser usada ao imprimir um documento. Os valores válidos são descritos na tabela a seguir.|
|dpi|Int32|A resolução padrão em DPI a ser usada ao imprimir o trabalho.|
|scaling|printScaling|Especifica como a impressora dimensiona os dados do documento para se ajustar à mídia solicitada. Os valores válidos são descritos na tabela a seguir.|

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

### <a name="printduplexmode-values"></a>Valores de printDuplexMode

|Membro|Valor|Descrição|
|:---|:---|:---|
|flipOnLongEdge|0|A impressora imprimirá com duas laterais e inverterá documentos ao longo da borda longa.|
|flipOnShortEdge|1 |A impressora imprimirá com duas laterais e inverterá documentos ao longo da borda curta.|
|oneSided|2 |A impressora imprimirá de lado único.|

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
|unknownFutureValue|32|Valor de sentinel de enumeração evolvable. Não usar.|

## <a name="printorientation-values"></a>Valores de printOrientation

|Membro|Valor|Descrição|
|:---|:---|:---|
|retrato|3 |A impressora imprimirá impressões na orientação "retrato".|
|paisagem|4 |A impressora imprimirá impressões na orientação "paisagem".|
|reverseLandscape|5 |A impressora imprimirá impressões na orientação "paisagem inversa".|
|reversePortrait|6 |A impressora imprimirá impressões na orientação "retrato reverso".|

### <a name="printquality-values"></a>Valores de printQuality

|Membro|Valor|Descrição|
|:---|:---|
|low|0|A impressora imprimirá o trabalho usando baixa qualidade (normalmente conhecida como "rascunho").|
|medium|1 |A impressora imprimirá o trabalho usando a qualidade medim (normalmente conhecida como "normal").|
|high|2 |A impressora imprimirá o trabalho usando qualidade alta (normalmente conhecida como "melhor" ou "fina").|
|unknownFutureValue|3 |Valor de sentinel de enumeração evolvable. Não usar.|

### <a name="printcolormode-values"></a>Valores de printColorMode

|Membro|Valor|Descrição|
|:---|:---|:---|
|blackAndWhite|0|Preto e branco (use apenas material de marcador preto.)|
|escala de cinza|1 |Escala de cinza (pode usar algum material de marcador de cor.)|
|color|2 |Cor (use qualquer combinação de materiais de marcador para criar uma impressão de cor).|
|auto|3 |Deixe a impressora decidir qual modo de cor usar.|

### <a name="printscaling-values"></a>Valores de printScaling

|Membro|Valor|Descrição|
|:---|:---|:---|
|auto|0|Se o documento for maior do que a mídia solicitada e as margens não são zero, a impressora dimensiona o documento como o ajuste printScaling.  Caso contrário, a impressora dimensiona o documento usando **o fill** printScaling. Se o documento for menor do que a mídia solicitada, será usado o printScaling 'none'.|
|shrinkToFit|1 |Se o documento for maior que a mídia solicitada, a impressora dimensiona o documento como o **ajuste** printScaling. Caso contrário, a impressora dimensiona o documento como **nenhum** printScaling.|
|fill|2 |A impressora dimensiona o documento para preencher o tamanho de mídia solicitado, preservando sua taxa de proporção, mas potencialmente recorte partes do documento.|
|fit|3 |A impressora dimensiona o documento para se ajustar à área de impressão do tamanho de mídia solicitado, preservando a taxa de proporção dos dados do documento sem rebaixar o documento.|
|nenhum|4 |A impressora não dimensiona o documento para se ajustar ao tamanho de mídia solicitado. Se o documento for maior que a mídia solicitada, a impressora centraliza e reclipe a saída resultante. Se o documento for menor do que a mídia solicitada, a impressora centraliza a saída resultante.|
|unknownFutureValue|5 |Valor de sentinel de enumeração evolvable. Não usar.|

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

