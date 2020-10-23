---
title: tipo de recurso printerStatus
description: Representa o status de processamento da impressora, incluindo erros.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c6e6f756c91af14d4a5c17dbf873e52fb1d553b7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726287"
---
# <a name="printerstatus-resource-type"></a>tipo de recurso printerStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status de processamento da impressora, incluindo erros.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|state|printerProcessingState|O estado de processamento atual. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|detalhes|coleção printerProcessingStateDetail|A lista de detalhes que descrevem por que a impressora está no estado atual. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|description|String|Uma descrição legível do estado de processamento atual da impressora. Somente leitura.|

### <a name="printerprocessingstate-values"></a>valores de printerProcessingState

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O estado de processamento relatado pela impressora é desconhecido.|
|Estado|1|A impressora está ociosa e pronta para aceitar novos trabalhos de impressão.|
|processe|duas|Atualmente, a impressora está processando um trabalho de impressão e processará qualquer trabalho pendente após a conclusão.|
|parar|3D|A impressora encontrou um problema (por exemplo, ficou sem papel na bandeja ativa) e não pode continuar o trabalho de impressão atual até que o problema seja resolvido. Confira o (s) valor (es) de **detalhes** ou o valor de **Descrição** para obter mais informações.|
|unknownFutureValue|4 |Valor de sentinela de enumeração evolvable. Não usar.|

### <a name="printerprocessingstatedetail-values"></a>valores de printerProcessingStateDetail

|Membro|Valor|Descrição|
|:---|:---|:---|
|pausado|,0| Um trabalho de impressão em andamento foi pausado.|
|estava|1|A conexão com a impressora foi perdida ou não pode ser estabelecida.|
|mediaJam|duas|Mídia em uma ou mais bandejas está obstruída.|
|mediaNeeded|3D|A mídia na bandeja de entrada usada no momento precisa ser substituída para que o trabalho possa continuar.|
|mediaLow|4 |Mídia em uma ou mais bandejas está quase esgotada.|
|mediaEmpty|5 |A mídia em uma ou mais bandejas está esgotada.|
|coverOpen|6 |Uma ou mais capas estão abertas.|
|interlockOpen|7 |Um ou mais dispositivos de travamento estão abertos.|
|queueFull|8 |A fila de spooler da impressora está cheia e novos trabalhos não podem ser enfileirados.|
|outputTrayMissing|9 |Uma ou mais bandejas de saída estão ausentes.|
|outputAreaFull|10 |Uma ou mais bandejas de saída estão cheias e não podem aceitar mais mídias.|
|markerSupplyLow|11|Uma ou mais fontes de marcador (por exemplo, tinta, toner ou faixa de opções) são baixas.|
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
    "state": "String",
    "details": ["String"],
    "description": "String"
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

