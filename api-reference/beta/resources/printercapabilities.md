---
title: tipo complexo printerCapabilities
description: Representa os recursos relatados por uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 42ae340e349b282d5480520ed118d049c77cf8bc
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895501"
---
# <a name="printercapabilities-complex-type"></a>tipo complexo printerCapabilities

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os recursos relatados por uma impressora.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|isColorPrintingSupported|Boolean|True se a impressão de cores for suportada pela impressora; caso contrário, false. Somente leitura.|
|supportsFitPdfToPage|Boolean|True se a impressora suporta o dimensionamento de páginas PDF para corresponder ao tamanho da mídia de impressão; caso contrário, false.|
|supportedCopiesPerJob|[integerRange](integerrange.md)|O intervalo de cópias por trabalho suportado pela impressora.|
|supportedDocumentMimeTypes|Coleção de cadeias de caracteres|Os tipos MIME de documento que são suportados pela impressora.|
|supportedFinishings|coleção de canacabados|As finalidades suportadas pela impressora.|
|supportedMediaColors|Coleção de cadeias de caracteres|As cores de mídia (isto é, papel) suportadas pela impressora.|
|supportedMediaTypes|coleção multimediatype|Os tipos de mídia com suporte da impressora. Os valores válidos são descritos na tabela a seguir.|
|supportedDuplexConfigurations|coleção printDuplexConfiguration|As configurações de duplex com suporte da impressora. Os valores válidos são descritos na tabela a seguir.|
|supportedMediaSizes|Coleção de cadeias de caracteres|Os tamanhos de mídia com suporte da impressora. Dá suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI, juntamente com qualquer tamanho personalizado suportado pela impressora associada.|
|supportedPagesPerSheet|[integerRange](integerrange.md)|Os valores de pagesPerSheet aceitos pela impressora.|
|supportedOrientations|coleção reorientation|As orientações de impressão suportadas pela impressora. Os valores válidos são descritos na tabela a seguir.|
|supportedOutputBins|Coleção de cadeias de caracteres|Os compartimentos de saída suportados da impressora (bandejas).|
|supportedPresentationDirections|coleção printPresentationDirection|As direções de apresentação suportadas pela impressora. Os valores com suporte são descritos na tabela a seguir.|
|supportedColorConfigurations|coleção printColorConfiguration|Os modos de cores suportados pela impressora. Os valores válidos são descritos na tabela a seguir.|
|supportedPrintQualities|coleção PrintQuality|As qualidades de impressão suportadas pela impressora.|

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

### <a name="printduplexconfiguration-values"></a>valores de printDuplexConfiguration

|Membro|Valor|Descrição|
|:---|:---|:---|
|twoSidedLongEdge|,0|A impressora imprimirá em frente e voltará os documentos ao longo da borda longa.|
|twoSidedShortEdge|1|A impressora imprimirá em frente e voltará os documentos ao longo da borda curta.|
|oneSided|duas|A impressora imprimirá um lado.|

## <a name="printorientation-values"></a>valores de reorientação

|Membro|Valor|Descrição|
|:---|:---|:---|
|modos|3D|A impressora imprimirá impressões na orientação "retrato".|
|paisagens|4 |A impressora imprimirá impressões na orientação "paisagem".|
|reverseLandscape|5 |A impressora imprimirá impressões na orientação "paisagem reversa".|
|reversePortrait|6 |A impressora imprimirá impressões na orientação "retrato reverso".|

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
  "@odata.type": "microsoft.graph.printerCapabilities"
}-->

```json
{
  "isColorPrintingSupported": true,
  "supportsFitPdfToPage": true,
  "supportedCopiesPerJob": {"@odata.type": "microsoft.graph.integerRange"},
  "supportedDocumentMimeTypes": ["String"],
  "supportedFinishings": ["String"],
  "supportedMediaColors": ["String"],
  "supportedMediaTypes": ["String"],
  "supportedDuplexConfigurations": ["String"],
  "supportedMediaSizes": ["String"],
  "supportedPagesPerSheet": {"@odata.type": "microsoft.graph.integerRange"},
  "supportedOrientations": ["String"],
  "supportedOutputBins": ["String"],
  "supportedPresentationDirections": ["String"],
  "supportedColorConfigurations": ["String"],
  "supportedPrintQualities": ["String"]
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