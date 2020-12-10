---
title: tipo de recurso printerStatus
description: Representa o status de processamento da impressora, incluindo erros.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 726fba10b91edb98d41eac47779c86749a173e48
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617000"
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
|description|Cadeia de caracteres|Uma descrição legível do estado de processamento atual da impressora. Somente leitura.|

### <a name="printerprocessingstate-values"></a>valores de printerProcessingState

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O estado de processamento relatado pela impressora é desconhecido.|
|Estado|1 |A impressora está ociosa e pronta para aceitar novos trabalhos de impressão.|
|processe|2 |Atualmente, a impressora está processando um trabalho de impressão e processará qualquer trabalho pendente após a conclusão.|
|parar|3 |A impressora encontrou um problema (por exemplo, ficou sem papel na bandeja ativa) e não pode continuar o trabalho de impressão atual até que o problema seja resolvido. Confira o (s) valor (es) de **detalhes** ou o valor de **Descrição** para obter mais informações.|
|unknownFutureValue|4 |Valor de sentinela de enumeração evolvable. Não usar.|

### <a name="printerprocessingstatedetail-values"></a>valores de printerProcessingStateDetail

|Membro|Valor|Descrição|
|:---|:---|:---|
|pausado|,0| Um trabalho de impressão em andamento foi pausado.|
|mediaJam|2 |Mídia em uma ou mais bandejas está obstruída.|
|mediaNeeded|3 |A mídia na bandeja de entrada usada no momento precisa ser substituída para que o trabalho possa continuar.|
|mediaLow|4 |Mídia em uma ou mais bandejas está quase esgotada.|
|mediaEmpty|5 |A mídia em uma ou mais bandejas está esgotada.|
|coverOpen|6 |Uma ou mais capas estão abertas.|
|interlockOpen|7 |Um ou mais dispositivos de travamento estão abertos.|
|outputTrayMissing|9 |Uma ou mais bandejas de saída estão ausentes.|
|outputAreaFull|10 |Uma ou mais bandejas de saída estão cheias e não podem aceitar mais mídias.|
|markerSupplyLow|11 |Uma ou mais fontes de marcador (por exemplo, tinta, toner ou faixa de opções) são baixas.|
|markerSupplyEmpty|12 |Uma ou mais fontes de marcador (por exemplo, tinta, toner ou faixa de opções) estão esgotadas.|
|inputTrayMissing|13 |Uma ou mais bandejas de entrada não estão no dispositivo.|
|outputAreaAlmostFull|14 |Uma ou mais áreas de saída estão quase cheia (por exemplo, Tray, Stacker, COLLATE).|
|markerWasteAlmostFull|15 |O marcador de dispositivo suprimento de resíduos está quase cheio.|
|markerWasteFull|16 |O marcador de dispositivo fornecendo receptáculo de lixo está cheio.|
|fuserOverTemp|17 |A temperatura do fusor está acima do normal.|
|fuserUnderTemp|18 |A temperatura do fusor está abaixo da normal.|
|outro|19|Qualquer outro motivo que não esteja no restante dos motivos.|
|Nenhuma|508|Nenhum motivo.|
|movingToPaused| 21 |Alguém pausou a impressora usando a operação Pause-Printer.|
|parada|22|Alguém removeu um objeto Printer do serviço e o dispositivo pode estar desligado ou fisicamente removido.|
|connectingToDevice|23|A impressora está em processo de conexão com um dispositivo de saída de rede compartilhado.|
|timedOut|dia|O servidor não pôde obter uma resposta do dispositivo de saída.|
|interrompendo|25|O objeto Printer está no processo de interrupção do dispositivo.|
|stoppedPartially|660|Um ou mais dispositivos de saída são interrompidos.|
|tonerLow|27|O dispositivo está com pouco toner.|
|tonerEmpty|28|O dispositivo está sem toner.|
|spoolAreaFull|anos|O limite de armazenamento persistente alocado para o spool foi atingido.|
|doorOpen|até|Uma ou mais portas no dispositivo estão abertas.|
|opticalPhotoConductorNearEndOfLife|31|O condutor de fotos óptica está próximo do fim da vida útil.|
|opticalPhotoConductorLifeOver|32|O condutor de fotos óptica não está mais funcionando.|
|developerLow|33|O dispositivo é de baixo desenvolvedor.|
|developerEmpty|34|O dispositivo está fora do desenvolvedor.|
|interpreterResourceUnavailable|35|Um recurso de intérprete não está disponível (por exemplo, Font, Form).|
|unknownFutureValue|36|Valor de sentinela de enumeração evolvable. Não usar.|

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

