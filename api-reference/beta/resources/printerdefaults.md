---
title: tipo de recurso printerDefaults
description: Representa as configurações padrão da impressora. Verifique os recursos da impressora para ver todos os valores que ele suporta.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 66357689b843be8783b888ab863e8e4382185ba9
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895488"
---
# <a name="printerdefaults-resource-type"></a>tipo de recurso printerDefaults

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações padrão da impressora. Verifique os [recursos](../api/printer-getcapabilities.md) da impressora para ver todos os valores que ele suporta.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|copiesPerJob|Int32|O número padrão de cópias impressas por trabalho.|
|documentMimeType|String|O tipo MIME padrão a ser usado durante o processamento de documentos.|
|término|coleção de canacabados|O conjunto de finalidades padrão a ser aplicado aos trabalhos de impressão. Os valores válidos são descritos na tabela a seguir.|
|mediaColor|String|A mídia padrão (como papel) em que a cor será impressa.
|Mídia|Arquivo de MediaType|O tipo de mídia padrão (como papel) para imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|mediaSize|String|O tamanho de mídia padrão a ser usado. Dá suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI, juntamente com qualquer tamanho personalizado suportado pela impressora associada.
|pagesPerSheet|Int32|O número padrão de páginas de documento a ser impresso em cada folha.
|orientation|a reorientação|A orientação padrão a ser usada ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|outputBin|String|O compartimento de saída padrão a ser inserido é impresso no. Confira os [recursos](../api/printer-getcapabilities.md) da impressora para obter uma lista de bandejas de saída suportadas.|
|pdfFitToPage|Boolean|A configuração padrão do pdfFitToPage. True para ajustar cada página de um documento PDF a uma folha física de mídia; false para permitir que a impressora decida como dispor as impressões.|
|presentationDirection|printPresentationDirection|A direção padrão para dispor páginas quando várias páginas estão sendo impressas por folha. Os valores válidos são descritos na tabela a seguir.|
|printColorConfiguration|printColorConfiguration|O modo de cor padrão a ser usado ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|printQuality|printQuality|A qualidade padrão a ser usada ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|duplexConfiguration|printDuplexConfiguration|A configuração duplex padrão (frente e verso) a ser usada ao imprimir um documento. Os valores válidos são descritos na tabela a seguir.|

### <a name="printpresentationdirection-values"></a>valores de printPresentationDirection

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

### <a name="printduplexconfiguration-values"></a>valores de printDuplexConfiguration

|Membro|Valor|Descrição|
|:---|:---|:---|
|twoSidedLongEdge|,0|A impressora imprimirá em frente e voltará os documentos ao longo da borda longa.|
|twoSidedShortEdge|1|A impressora imprimirá em frente e voltará os documentos ao longo da borda curta.|
|oneSided|duas|A impressora imprimirá um lado.|

### <a name="printfinishing-values"></a>valores de reconclusão de

|Membro|Valor|Descrição|
|:---|:---|:---|
|none|3D|Nenhuma conclusão. Incluir esse valor equivale a fornecer uma coleção vazia de finalidades.|
|grampo|4 |Grampear o documento usando a configuração de associação padrão da impressora.|
|relógio|5 |Perfuração o documento usando a configuração de perfuração padrão da impressora.|
|visa|6 |Aplicar uma capa ao documento.|
|associá|7 |Vincule o documento usando a configuração de associação padrão da impressora.|
|saddleStitch|8 |Lombada-Stich o documento usando a configuração de costura padrão da impressora.|
|edgeStitch|9 |Borda-costura o documento usando a configuração de costura padrão da impressora.|
|stapleTopLeft|508|Grampear o documento no canto superior esquerdo.|
|stapleBottomLeft|21|Grampear o documento no canto inferior esquerdo.|
|stapleTopRight|22|Grampear o documento no canto superior direito.|
|stapleBottomRight|23|Grampo o documento no canto inferior direito.|
|edgeStitchLeft|dia|Borda-costura o documento ao longo da borda esquerda.|
|edgeStitchTop|25|Borda-costura o documento ao longo da borda superior.|
|edgeStitchRight|660|Borda-costura o documento ao longo da borda direita.|
|edgeStitchBottom|27|Borda-costura o documento ao longo da borda inferior.|
|stapleDualLeft|28|Grampear o documento duas vezes ao longo da borda esquerda.|
|stapleDualTop|anos|Grampear o documento duas vezes ao longo da borda superior.|
|stapleDualRight|até|Grampear o documento duas vezes ao longo da borda direita.|
|stapleDualBottom|31|Grampear o documento duas vezes ao longo da borda inferior.|

## <a name="printorientation-values"></a>valores de reorientação

|Membro|Valor|Descrição|
|:---|:---|:---|
|modos|3D|A impressora imprimirá impressões na orientação "retrato".|
|paisagens|4 |A impressora imprimirá impressões na orientação "paisagem".|
|reverseLandscape|5 |A impressora imprimirá impressões na orientação "paisagem reversa".|
|reversePortrait|6 |A impressora imprimirá impressões na orientação "retrato reverso".|

### <a name="printmediatype-values"></a>valores de multimediatype

|Membro|Valor|Descrição|
|:---|:---|:---|
|carta|,0|Folhas de papel padrão.|
|transparência|1|Filme de transparência usado com projetores de sobrecarga.|
|envelope|duas|Um envelope.|
|envelopePlain|3D|Um envelope simples.|
|permanente|4 |Um rolo de papel contínuo.|
|tela|5 |Uma tela digital.|
|screenPaged|6 |Uma tela digital com suporte para paginação.|
|continuousLong|7 |Um longo lançamento de papel contínuo.|
|continuousShort|8 |Um pequeno rolo contínuo de papel.|
|envelopeWindow|9 |Um envelope com um corte de janela transparente.|
|multiPartForm|10 |Um formulário de várias partes perfurado.|
|Multilayer|11|Uma média de várias camadas.|
|Legendas|12 |Uma planilha com recortes de rótulo.|

### <a name="printquality-values"></a>valores de PrintQuality

|Member|Descrição|
|:---|:---|
|low|A impressora imprimirá o trabalho usando a qualidade baixa (normalmente conhecida como "rascunho").|
|medium|A impressora imprimirá o trabalho usando o medim (comumente conhecido como qualidade "normal").|
|high|A impressora imprimirá o trabalho usando a qualidade alta (normalmente conhecida como "melhor" ou "boa").|

### <a name="printcolorconfiguration-values"></a>valores de printColorConfiguration

|Membro|Valor|Descrição|
|:---|:---|:---|
|blackAndWhite|,0|Preto e branco (Use apenas o material de marcador preto).|
|escala|1|Escala de cinza (pode usar algum material de marcador de cor.)|
|color|duas|Color (use qualquer combinação de materiais de marcador para criar uma impressão colorida).|
|Automático|3D|Permitir que a impressora decida qual modo de cor usar.|

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
  "documentMimeType": "String",
  "finishings": ["String"],
  "mediaColor": "String",
  "mediaSize": "String",
  "pagesPerSheet": 123456,
  "orientation": "String",
  "outputBin": "String",
  "pdfFitToPage": true,
  "presentationDirection": "String",
  "printColorConfiguration": "String",
  "printQuality": "String",
  "duplexConfiguration": "String"
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