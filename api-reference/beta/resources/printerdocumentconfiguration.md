---
title: tipo de recurso printerDocumentConfiguration
description: Um grupo de configurações que uma impressora deve usar para imprimir um documento.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: ff1da92894f8854bcdee2ce24d7a9d5cef6288e7
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895484"
---
# <a name="printerdocumentconfiguration-resource-type"></a>tipo de recurso printerDocumentConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um grupo de configurações que uma impressora deve usar para imprimir um documento.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|pageRanges|coleção [printPageRange](printpagerange.md)|Os intervalos de páginas a serem impressos. Somente leitura.|
|printQuality|printQuality|A qualidade de impressão a ser usada ao imprimir o trabalho. Os valores válidos são descritos na tabela abaixo. Somente leitura.|
|printResolutionInDpi|Int32|A resolução a ser usada ao imprimir o trabalho, expresso em pontos por polegada (DPI). Somente leitura.|
|feedDirection|printerFeedDirection|A direção a ser usada ao alimentar mídia na impressora. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|orientation|a reorientação|A configuração de orientação que a impressora deve usar ao imprimir o trabalho. Os valores válidos são descritos na tabela a seguir.|
|duplexConfiguration|printDuplexConfiguration|A configuração duplex que a impressora deve usar ao imprimir o trabalho. Os valores válidos são descritos na tabela abaixo. Somente leitura.|
|Copia|Int32|O número de cópias que devem ser impressas. Somente leitura.|
|colorConfiguration|printColorConfiguration|A configuração de cor que a impressora deve usar para imprimir o trabalho. Os valores válidos são descritos na tabela abaixo. Somente leitura.|

### <a name="printduplexconfiguration-values"></a>valores de printDuplexConfiguration

|Membro|Valor|Descrição|
|:---|:---|:---|
|twoSidedLongEdge|,0|A impressora imprimirá em frente e voltará os documentos ao longo da borda longa.|
|twoSidedShortEdge|1|A impressora imprimirá em frente e voltará os documentos ao longo da borda curta.|
|oneSided|duas|A impressora imprimirá um lado.|

### <a name="printquality-values"></a>valores de PrintQuality

|Member|Descrição|
|:---|:---|
|low|A impressora imprimirá o trabalho usando a qualidade baixa (normalmente conhecida como "rascunho").|
|medium|A impressora imprimirá o trabalho usando o medim (comumente conhecido como qualidade "normal").|
|high|A impressora imprimirá o trabalho usando a qualidade alta (normalmente conhecida como "melhor" ou "boa").|

## <a name="printerfeeddirection-values"></a>valores de printerFeedDirection

|Member|Descrição|
|:---|:---|
|longEdgeFirst|A impressora consumirá planilhas da bandeja ativa na orientação "paisagem", com a borda longa da planilha primeiro.|
|shortEdgeFirst|A impressora consumirá planilhas da bandeja ativa na orientação "retrato", com a borda curta da planilha primeiro.|

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
  "@odata.type": "microsoft.graph.printerDocumentConfiguration"
}-->

```json
{
  "pageRanges": [{"@odata.type": "microsoft.graph.printPageRange"}],
  "printQuality": "String",
  "printResolutionInDpi": 123456,
  "feedDirection": "String",
  "orientation": "String",
  "duplexConfiguration": "String",
  "copies": 123456,
  "colorConfiguration": "String",
}

```
