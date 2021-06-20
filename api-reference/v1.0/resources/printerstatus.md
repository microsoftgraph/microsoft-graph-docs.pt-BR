---
title: Tipo de recurso printerStatus
description: Representa o status de processamento da impressora, incluindo quaisquer erros.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 55374ff2cdb2ad26100fbc3440e4b542e763248b
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030961"
---
# <a name="printerstatus-resource-type"></a>Tipo de recurso printerStatus

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Representa o status de processamento da impressora, incluindo quaisquer erros.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|state|printerProcessingState|O estado de processamento atual. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|detalhes|Coleção printerProcessingStateDetail|A lista de detalhes que descrevem por que a impressora está no estado atual. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|description|String|Uma descrição aceitável para humanos do estado de processamento atual da impressora. Somente leitura.|

### <a name="printerprocessingstate-values"></a>printerProcessingState values

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|O estado de processamento relatado pela impressora é desconhecido.|
|idle|1|A impressora está ociosa e pronta para aceitar novos trabalhos de impressão.|
|processamento|2|No momento, a impressora está mediante o processamento de um trabalho de impressão e processará todos os trabalhos pendentes após a conclusão.|
|stopped|3|A impressora encontrou um problema (por exemplo, ficou sem papel na bandeja ativa) e não pode continuar o trabalho de impressão atual até que o problema seja resolvido. Confira os **valores** de detalhes ou o valor **de descrição** para obter mais informações.|
|unknownFutureValue|4 |Valor de sentinela de enumeração evolvável. Não usar.|

### <a name="printerprocessingstatedetail-values"></a>printerProcessingStateDetail values

|Membro|Valor|Descrição|
|:---|:---|:---|
|pausado|0| Um trabalho de impressão em andamento foi pausado.|
|mediaJam|2|A mídia em uma ou mais bandejas está emperrada.|
|mediaNeededed|3|A mídia na bandeja de entrada usada no momento precisa ser substituída antes que o trabalho possa continuar.|
|mediaLow|4 |A mídia em uma ou mais bandejas está quase esgotada.|
|mediaEmpty|5 |A mídia em uma ou mais bandejas está esgotada.|
|coverOpen|6 |Uma ou mais capas estão abertas.|
|interlockOpen|7 |Um ou mais dispositivos de bloqueio estão abertos.|
|outputTrayMissing|9 |Uma ou mais bandejas de saída estão ausentes.|
|outputAreaFull|10 |Uma ou mais bandejas de saída estão cheias e não podem aceitar mais mídia.|
|markerSupplyLow|11|Uma ou mais fontes de marcador (por exemplo, tinta, toner ou faixa de opções) estão baixas.|
|markerSupplyEmpty|12 |Uma ou mais fontes de marcador (por exemplo, tinta, toner ou faixa de opções) estão esgotadas.|
|inputTrayMissing|13|Uma ou mais bandejas de entrada não estão no dispositivo.|
|outputAreaAlmostFull|14 |Uma ou mais área de saída está quase cheia (por exemplo, bandeja, empilhador, colator).|
|markerWasteAlmostFull|15|O recipiente de lixo de fornecimento de marcador de dispositivo está quase cheio.|
|markerWasteFull|16 |O recipiente de lixo de fornecimento de marcador de dispositivo está cheio.|
|fuserOverTemp|17 |A temperatura do fusor está acima do normal.|
|fuserUnderTemp|18 |A temperatura do fusor está abaixo do normal.|
|other|19|Qualquer outro motivo que não se enquadra no restante dos motivos.|
|nenhuma|20|Sem motivos.|
|movingToPaused| 21 |Alguém fez uma pausa na impressora usando a Pause-Printer de usuário.|
|shutdown|22|Alguém removeu um objeto Printer do serviço e o dispositivo pode ser desligado ou removido fisicamente.|
|connectingToDevice|23|A impressora está no processo de conexão com um Dispositivo de Saída de Rede Compartilhada.|
|timedOut|24|O servidor não conseguiu obter uma resposta do dispositivo de saída.|
|stopping|25|O objeto Printer está em processo de interrupção do dispositivo.|
|stoppedPartially|26|Um ou mais dispositivos de saída são interrompidos.|
|tonerLow|27|O dispositivo está com pouca toner.|
|tonerEmpty|28|O dispositivo está sem toner.|
|spoolAreaFull|29|O limite de armazenamento persistente alocado para o spooling foi atingido.|
|doorOpen|30|Uma ou mais portas no dispositivo estão abertas.|
|opticalPhotoConductorNearEndOfLife|31|O condutor de fotos óptico está quase no fim da vida útil.|
|opticalPhotoConductorLifeOver|32|O condutor óptico de fotos não está mais funcionando.|
|developerLow|33|O dispositivo está com pouco desenvolvedor.|
|developerEmpty|34|O dispositivo está fora do desenvolvedor.|
|interpreterResourceUnavailable|35|Um recurso de intérprete não está disponível (por exemplo, fonte, formulário).|
|unknownFutureValue|36|Valor de sentinela de enumeração evolvável. Não usar.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerStatus",
  "state": "String",
  "details": [
    "String"
  ],
  "description": "String"
}
```
