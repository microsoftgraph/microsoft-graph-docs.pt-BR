---
title: tipo de recurso printerStatus
description: Representa o status de processamento da impressora, incluindo erros.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: b07c450a258d7cd672dada974180e0ed0589dda7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048754"
---
# <a name="printerstatus-resource-type"></a>tipo de recurso printerStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status de processamento da impressora, incluindo erros.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|ProcessingState|printerProcessingState|O estado de processamento atual. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|processingStateReasons|coleção printerProcessingStateReason|A lista de motivos que descrevem por que a impressora está no estado atual. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|processingStateDescription|Cadeia de caracteres|Uma descrição legível do estado de processamento atual da impressora. Somente leitura.|

### <a name="printerprocessingstate-values"></a>valores de printerProcessingState

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O estado de processamento relatado pela impressora é desconhecido.|
|Estado|1 |A impressora está ociosa e pronta para aceitar novos trabalhos de impressão.|
|processe|2 |Atualmente, a impressora está processando um trabalho de impressão e processará qualquer trabalho pendente após a conclusão.|
|parar|3 |A impressora encontrou um problema (por exemplo, ficou sem papel na bandeja ativa) e não pode continuar o trabalho de impressão atual até que o problema seja resolvido. Confira o (s) valor (es) **printerProcessingStateReasons** ou o valor de **printerProcessingStateDescription** para obter mais informações.|
|unknownFutureValue|4 |Valor de sentinela de enumeração evolvable. Não usar.|

### <a name="printerprocessingstatereason-values"></a>valores de printerProcessingStateReason

|Membro|Valor|Descrição|
|:---|:---|:---|
|pausado|,0| Um trabalho de impressão em andamento foi pausado.|
|estava|1 |A conexão com a impressora foi perdida ou não pode ser estabelecida.|
|mediaJam|2 |Mídia em uma ou mais bandejas está obstruída.|
|mediaNeeded|3 |A mídia na bandeja de entrada usada no momento precisa ser substituída para que o trabalho possa continuar.|
|mediaLow|4 |Mídia em uma ou mais bandejas está quase esgotada.|
|mediaEmpty|5 |A mídia em uma ou mais bandejas está esgotada.|
|coverOpen|6 |Uma ou mais capas estão abertas.|
|interlockOpen|7 |Um ou mais dispositivos de travamento estão abertos.|
|queueFull|8 |A fila de spooler da impressora está cheia e novos trabalhos não podem ser enfileirados.|
|outputTrayMissing|9 |Uma ou mais bandejas de saída estão ausentes.|
|outputAreaFull|10 |Uma ou mais bandejas de saída estão cheias e não podem aceitar mais mídias.|
|markerSupplyLow|11 |Uma ou mais fontes de marcador (por exemplo, tinta, toner ou faixa de opções) são baixas.|
|markerSupplyEmpty|12 |Uma ou mais fontes de marcador (por exemplo, tinta, toner ou faixa de opções) estão esgotadas.|
|inputTrayMissing|13 |Uma ou mais bandejas de entrada não estão no dispositivo.|
|outputAlmostFull|14 |Uma ou mais áreas de saída estão quase cheia (por exemplo, Tray, Stacker, COLLATE).|
|markerWasteAlmostFull|15 |O marcador de dispositivo suprimento de resíduos está quase cheio.|
|markerWasteFull|16 |O marcador de dispositivo fornecendo receptáculo de lixo está cheio.|
|fuserOverTemp|17 |A temperatura do fusor está acima do normal.|
|fuserUnderTemp|18 |A temperatura do fusor está abaixo da normal.|
|outro|19|Qualquer outro motivo que não esteja no restante dos motivos.|
|unknownFutureValue|508|Valor de sentinela de enumeração evolvable. Não usar.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerStatus"
}-->

```json
{
    "processingState": "String",
    "processingStateReasons": ["String"],
    "processingStateDescription": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

