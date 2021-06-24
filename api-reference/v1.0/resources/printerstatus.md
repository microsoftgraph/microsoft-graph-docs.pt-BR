---
title: Tipo de recurso printerStatus
description: Representa o status de processamento da impressora, incluindo quaisquer erros.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: b1fec030433734d29e5557fe238eb41a6ca545c1
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107722"
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
|idle|1 |A impressora está ociosa e pronta para aceitar novos trabalhos de impressão.|
|processamento|2 |No momento, a impressora está mediante o processamento de um trabalho de impressão e processará todos os trabalhos pendentes após a conclusão.|
|stopped|3 |A impressora encontrou um problema (por exemplo, ficou sem papel na bandeja ativa) e não pode continuar o trabalho de impressão atual até que o problema seja resolvido. Confira os **valores** de detalhes ou o valor **de descrição** para obter mais informações.|
|unknownFutureValue|4 |Valor de sentinela de enumeração evolvável. Não usar.|

### <a name="printerprocessingstatedetail-values"></a>printerProcessingStateDetail values

|Membro|Valor|Descrição|
|:---|:---|:---|
|pausado|0| Um trabalho de impressão em andamento foi pausado.|
|mediaJam|2 |A mídia em uma ou mais bandejas está emperrada.|
|mediaNeededed|3 |A mídia na bandeja de entrada usada no momento precisa ser substituída antes que o trabalho possa continuar.|
|mediaLow|4 |A mídia em uma ou mais bandejas está quase esgotada.|
|mediaEmpty|5 |A mídia em uma ou mais bandejas está esgotada.|
|coverOpen|6 |Uma ou mais capas estão abertas.|
|interlockOpen|7 |Um ou mais dispositivos de bloqueio estão abertos.|
|outputTrayMissing|9 |Uma ou mais bandejas de saída estão ausentes.|
|outputAreaFull|10 |Uma ou mais bandejas de saída estão cheias e não podem aceitar mais mídia.|
|markerSupplyLow|11 |Uma ou mais fontes de marcador (por exemplo, tinta, toner ou faixa de opções) estão baixas.|
|markerSupplyEmpty|12 |Uma ou mais fontes de marcador (por exemplo, tinta, toner ou faixa de opções) estão esgotadas.|
|inputTrayMissing|13 |Uma ou mais bandejas de entrada não estão no dispositivo.|
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
|alertRemovalOfBinaryChangeEntry|36|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderAdded|37|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderAlmostEmpty|38|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderAlmostFull|39|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderAtLimit|40|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderClosed|41|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderConfigurationChange|42|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderCoverClosed|43|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderCoverOpen|44|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderEmpty|45|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderFull|46|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderInterlockClosed|47|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderInterlockOpen|48|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderJam|49|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderLifeAlmostOver|50|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderLifeOver|51|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderMemoryExhausted|52|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderMissing|53|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderMotorFailure|54|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderNearLimit|55|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderOffline|56|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderOpened|57|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderOverTemperature|58|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderPowerSaver|59|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderRecoverableFailure|60|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderRecoverableStorage|61|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderRemoved|62|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderResourceAdded|63|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderResourceRemoved|64|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderThermistorFailure|65|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderTimingFailure|66|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderTurnedOff|67|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderTurnedOn|68|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderUnderTemperature|69|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderUnrecoverableFailure|70|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderUnrecoverableStorageError|71|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|banderWarmingUp|72|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderAdded|73|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderAlmostEmpty|74|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderAlmostFull|75|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderAtLimit|76|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderClosed|77|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderConfigurationChange|78|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderCoverClosed|79|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderCoverOpen|80|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderEmpty|81|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderFull|82|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderInterlockClosed|83|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderInterlockOpen|84|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderJam|85|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderLifeAlmostOver|86|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderLifeOver|87|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderMemoryExhausted|88|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderMissing|89|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderMotorFailure|90|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderNearLimit|91|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderOffline|92|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderOpened|93|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderOverTemperature|94|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderPowerSaver|95|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderRecoverableFailure|96|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderRecoverableStorage|97|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderRemoved|98|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderResourceAdded|99|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderResourceRemoved|100|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderThermistorFailure|101|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderTimingFailure|102|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderTurnedOff|103|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderTurnedOn|104|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderUnderTemperature|105|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderUnrecoverableFailure|106|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderUnrecoverableStorageError|107|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|binderWarmingUp|108|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|cameraFailure|109|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|chamberCooling|110|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|chamberFailure|111|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|chamberHeating|112|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|chamberTemperatureHigh|113|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|chamberTemperatureLow|114|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|cleanerLifeAlmostOver|115|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.13.|
|cleanerLifeOver|116|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.13.|
|configurationChange|117|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|desativado|118|Este é um valor padrão de Atributo de Impressora IPP descrito em RFC3998.|
|deleted|119|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.22.|
|dieCutterAdded|120|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterAlmostEmpty|121|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterAlmostFull|122|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterAtLimit|123|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterClosed|124|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterConfigurationChange|125|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterCoverClosed|126|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterCoverOpen|127|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterEmpty|128|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterFull|129|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterInterlockClosed|130|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterInterlockOpen|131|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterJam|132|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterLifeAlmostOver|133|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterLifeOver|134|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterMemoryExhausted|135|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterMissing|136|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterMotorFailure|137|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterNearLimit|138|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterOffline|139|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterOpened|140|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterOverTemperature|141|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterPowerSaver|142|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterRecoverableFailure|143|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterRecoverableStorage|144|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterRemoved|145|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterResourceAdded|146|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterResourceRemoved|147|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterThermistorFailure|148|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterTimingFailure|149|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterTurnedOff|150|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterTurnedOn|151|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterUnderTemperature|152|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterUnrecoverableFailure|153|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterUnrecoverableStorageError|154|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dieCutterWarmingUp|155|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|extruderCooling|156|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|extruderFailure|157|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|extruderHeating|158|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|extruderJam|159|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|extruderTemperatureHigh|160|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|extruderTemperatureLow|161|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|fanFailure|162|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|faxModemLifeAlmostOver|163|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|faxModemLifeOver|164|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|faxModemMissing|165|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|faxModemTurnedOff|166|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|faxModemTurnedOn|167|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|folderAdded|168|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderAlmostEmpty|169|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderAlmostFull|170|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderAtLimit|171|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderClosed|172|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderConfigurationChange|173|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderCoverClosed|174|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderCoverOpen|175|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderEmpty|176|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderFull|177|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderInterlockClosed|178|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderInterlockOpen|179|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderJam|180|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderLifeAlmostOver|181|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderLifeOver|182|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderMemoryExhausted|183|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderMissing|184|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderMotorFailure|185|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderNearLimit|186|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderOffline|187|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderOpened|188|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderOverTemperature|189|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderPowerSaver|190|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderRecoverableFailure|191|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderRecoverableStorage|192|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderRemoved|193|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderResourceAdded|194|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderResourceRemoved|195|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderThermistorFailure|196|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderTimingFailure|197|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderTurnedOff|198|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderTurnedOn|199|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderUnderTemperature|200|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderUnrecoverableFailure|201|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderUnrecoverableStorageError|202|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|folderWarmingUp|203|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|hibernar|204|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5106.4.|
|holdNewJobs|205|Este é um valor padrão de Atributo de Impressora IPP descrito em RFC3998.|
|identifyPrinterRequested|206|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.18.|
|imprinterAdded|207|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterAlmostEmpty|208|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterAlmostFull|209|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterAtLimit|210|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterClosed|211|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterConfigurationChange|212|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterCoverClosed|213|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterCoverOpen|214|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterEmpty|215|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterFull|216|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterInterlockClosed|217|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterInterlockOpen|218|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterJam|219|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterLifeAlmostOver|220|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterLifeOver|221|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterMemoryExhausted|222|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterMissing|223|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterMotorFailure|224|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterNearLimit|225|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterOffline|226|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterOpened|227|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterOverTemperature|228|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterPowerSaver|229|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterRecoverableFailure|230|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterRecoverableStorage|231|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterRemoved|232|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterResourceAdded|233|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterResourceRemoved|234|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterThermistorFailure|235|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterTimingFailure|236|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterTurnedOff|237|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterTurnedOn|238|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterUnderTemperature|239|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterUnrecoverableFailure|240|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterUnrecoverableStorageError|241|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|imprinterWarmingUp|242|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inputCannotFeedSizeSelected|243|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inputManualInputRequest|244|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inputMediaColorChange|245|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inputMediaFormPartsChange|246|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inputMediaSizeChange|247|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inputMediaTrayFailure|248|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|inputMediaTrayFeedError|249|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|inputMediaTrayJam|250|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|inputMediaTypeChange|251|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inputMediaWeightChange|252|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inputPickRollerFailure|253|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|inputPickRollerLifeOver|254|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|inputPickRollerLifeWarn|255|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|inputPickRollerMissing|256|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|inputTrayElevationFailure|257|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inputTrayPositionFailure|258|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterAdded|259|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterAlmostEmpty|260|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterAlmostFull|261|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterAtLimit|262|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterClosed|263|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterConfigurationChange|264|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterCoverClosed|265|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterCoverOpen|266|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterEmpty|267|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterFull|268|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterInterlockClosed|269|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterInterlockOpen|270|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterJam|271|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterLifeAlmostOver|272|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterLifeOver|273|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterMemoryExhausted|274|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterMissing|275|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterMotorFailure|276|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterNearLimit|277|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterOffline|278|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterOpened|279|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterOverTemperature|280|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterPowerSaver|281|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterRecoverableFailure|282|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterRecoverableStorage|283|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterRemoved|284|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterResourceAdded|285|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterResourceRemoved|286|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterThermistorFailure|287|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterTimingFailure|288|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterTurnedOff|289|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterTurnedOn|290|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterUnderTemperature|291|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterUnrecoverableFailure|292|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterUnrecoverableStorageError|293|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|inserterWarmingUp|294|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|interlockClosed|295|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|interpreterCartrichAdded|296|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|interpreterCartrichDeleted|297|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|interpreterComplexPageEncountered|298|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|interpreterMemoryDecrease|299|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|interpreterMemoryIncrease|300|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|interpreterResourceAdded|301|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|interpreterResourceDeleted|302|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|lampAtEol|303|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|lampFailure|304|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|lampNearEol|305|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|laserAtEol|306|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|laserFailure|307|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|laserNearEol|308|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|makeEnvelopeAdded|309|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeAlmostEmpty|310|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeAlmostFull|311|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeAtLimit|312|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeClosed|313|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeConfigurationChange|314|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeCoverClosed|315|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeCoverOpen|316|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeEmpty|317|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeFull|318|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeInterlockClosed|319|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeInterlockOpen|320|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeJam|321|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeLifeAlmostOver|322|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeLifeOver|323|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeMemoryExhausted|324|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeMissing|325|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeMotorFailure|326|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeNearLimit|327|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeOffline|328|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeOpened|329|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeOverTemperature|330|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopePowerSaver|331|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeRecoverableFailure|332|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeRecoverableStorage|333|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeRemoved|334|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeResourceAdded|335|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeResourceRemoved|336|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeThermistorFailure|337|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeTimingFailure|338|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeTurnedOff|339|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeTurnedOn|340|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeUnderTemperature|341|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeUnrecoverableFailure|342|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeUnrecoverableStorageError|343|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|makeEnvelopeWarmingUp|344|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|markerAdjustingPrintQuality|345|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|markerCleanerMissing|346|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|markerDeveloperAlmostEmpty|347|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|markerDeveloperEmpty|348|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|markerDeveloperMissing|349|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|markerFuserMissing|350|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|markerFuserThermistorFailure|351|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|markerFuserTimingFailure|352|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|markerInkAlmostEmpty|353|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|markerInkEmpty|354|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|markerInkMissing|355|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|markerOpcMissing|356|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|markerPrintRibbonAlmostEmpty|357|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|markerPrintRibbonEmpty|358|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|markerPrintRibbonMissing|359|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|markerSupplyAlmostEmpty|360|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|markerSupplyMissing|361|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|markerTonerCartrichMissing|362|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|markerTonerMissing|363|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|markerWasteInkReceptacleAlmostFull|364|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|markerWasteInkReceptacleFull|365|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|markerWasteInkReceptacleMissing|366|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|markerWasteMissing|367|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|markerWasteTonerReceptacleAlmostFull|368|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|markerWasteTonerReceptacleFull|369|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|markerWasteTonerReceptacleMissing|370|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|materialEmpty|371|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|materialLow|372|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|materialNeededed|373|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|mediaDrying|374|Este é um valor padrão de Atributo de Impressora IPP descrito em HP20181213.|
|mediaPathCannotDuplexMediaSelected|375|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|mediaPathFailure|376|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|mediaPathInputEmpty|377|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|mediaPathInputFeedError|378|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|mediaPathInputJam|379|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|mediaPathInputRequest|380|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|mediaPathJam|381|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|mediaPathMediaTrayAlmostFull|382|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|mediaPathMediaTrayFull|383|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|mediaPathMediaTrayMissing|384|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|mediaPathOutputFeedError|385|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|mediaPathOutputFull|386|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|mediaPathOutputJam|387|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|mediaPathPickRollerFailure|388|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|mediaPathPickRollerLifeOver|389|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|mediaPathPickRollerLifeWarn|390|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|mediaPathPickRollerMissing|391|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|motorFailure|392|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|outputMailboxSelectFailure|393|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|outputMediaTrayFailure|394|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|outputMediaTrayFeedError|395|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|outputMediaTrayJam|396|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|aduladorAdded|397|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016|398|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016|399|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016|400|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|queerClosed|401|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016|402|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|queerCoverClosed|403|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016|404|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|queerEmpty|405|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|queerFull|406|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|oerInterlockClosed|407|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016|408|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|queerJam|409|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016|410|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|de acordo com o trabalho do 21 de outubro de 2|411|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dememoryExhausted|412|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|100% de 2016.|413|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016.|414|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|queerNearLimit|415|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|queerOffline|416|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016|417|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|dooerOverTemperature|418|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|300000.000.000|419|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016.|420|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016|421|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|queerRemoved|422|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016.|423|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016.|424|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016.|425|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016|426|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|100% de 100%.|427|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|100% de 2006|428|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|queerUnderTemperature|429|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016|430|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|100%.|431|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|2016|432|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|platformCooling|433|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|platformFailure|434|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|platformHeating|435|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|platformTemperatureHigh|436|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|platformTemperatureLow|437|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.21.|
|powerDown|438|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|powerUp|439|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|printerManualReset|440|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|printerNmsReset|441|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|printerReadyToPrint|442|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherAdded|443|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherAlmostEmpty|444|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherAlmostFull|445|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherAtLimit|446|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherClosed|447|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherConfigurationChange|448|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherCoverClosed|449|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherCoverOpen|450|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherEmpty|451|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherFull|452|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherInterlockClosed|453|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherInterlockOpen|454|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherJam|455|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherLifeAlmostOver|456|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherLifeOver|457|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherMemoryExhausted|458|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherMissing|459|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherMotorFailure|460|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherNearLimit|461|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherOffline|462|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherOpened|463|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherOverTemperature|464|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherPowerSaver|465|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherRecoverableFailure|466|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherRecoverableStorage|467|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherRemoved|468|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherResourceAdded|469|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherResourceRemoved|470|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherThermistorFailure|471|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherTimingFailure|472|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherTurnedOff|473|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherTurnedOn|474|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherUnderTemperature|475|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherUnrecoverableFailure|476|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherUnrecoverableStorageError|477|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|puncherWarmingUp|478|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|retomada|479|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.22.|
|scanMediaPathFailure|480|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scanMediaPathInputEmpty|481|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scanMediaPathInputFeedError|482|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scanMediaPathInputJam|483|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scanMediaPathInputRequest|484|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scanMediaPathJam|485|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scanMediaPathOutputFeedError|486|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scanMediaPathOutputFull|487|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scanMediaPathOutputJam|488|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scanMediaPathPickRollerFailure|489|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scanMediaPathPickRollerLifeOver|490|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scanMediaPathPickRollerLifeWarn|491|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scanMediaPathPickRollerMissing|492|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scanMediaPathTrayAlmostFull|493|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scanMediaPathTrayFull|494|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scanMediaPathTrayMissing|495|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scannerLightFailure|496|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scannerLightLifeAlmostOver|497|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scannerLightLifeOver|498|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scannerLightMissing|499|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scannerSensorFailure|500|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scannerSensorLifeAlmostOver|501|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scannerSensorLifeOver|502|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|scannerSensorMissing|503|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5107.3.|
|separationCutterAdded|504|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterAlmostEmpty|505|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterAlmostFull|506|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterAtLimit|507|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterClosed|508|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterConfigurationChange|509|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterCoverClosed|510|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterCoverOpen|511|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterEmpty|512|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterFull|513|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterInterlockClosed|514|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterInterlockOpen|515|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterJam|516|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterLifeAlmostOver|517|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterLifeOver|518|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterMemoryExhausted|519|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterMissing|520|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterMotorFailure|521|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterNearLimit|522|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterOffline|523|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterOpened|524|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterOverTemperature|525|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterPowerSaver|526|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterRecoverableFailure|527|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterRecoverableStorage|528|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterRemoved|529|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterResourceAdded|530|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterResourceRemoved|531|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterThermistorFailure|532|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterTimingFailure|533|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterTurnedOff|534|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterTurnedOn|535|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterUnderTemperature|536|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterUnrecoverableFailure|537|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterUnrecoverableStorageError|538|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|separationCutterWarmingUp|539|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorAdded|540|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorAlmostEmpty|541|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorAlmostFull|542|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorAtLimit|543|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorClosed|544|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorConfigurationChange|545|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorCoverClosed|546|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorCoverOpen|547|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorEmpty|548|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorFull|549|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorInterlockClosed|550|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorInterlockOpen|551|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorJam|552|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorLifeAlmostOver|553|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorLifeOver|554|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorMemoryExhausted|555|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorMissing|556|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorMotorFailure|557|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorNearLimit|558|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorOffline|559|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorOpened|560|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorOverTemperature|561|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorPowerSaver|562|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorRecoverableFailure|563|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorRecoverableStorage|564|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorRemoved|565|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorResourceAdded|566|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorResourceRemoved|567|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorThermistorFailure|568|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorTimingFailure|569|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorTurnedOff|570|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorTurnedOn|571|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorUnderTemperature|572|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorUnrecoverableFailure|573|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorUnrecoverableStorageError|574|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|sheetRotatorWarmingUp|575|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterAdded|576|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterAlmostEmpty|577|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterAlmostFull|578|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterAtLimit|579|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterClosed|580|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterConfigurationChange|581|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterCoverClosed|582|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterCoverOpen|583|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterEmpty|584|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterFull|585|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterInterlockClosed|586|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterInterlockOpen|587|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterJam|588|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterLifeAlmostOver|589|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterLifeOver|590|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterMemoryExhausted|591|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterMissing|592|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterMotorFailure|593|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterNearLimit|594|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterOffline|595|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterOpened|596|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterOverTemperature|597|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterPowerSaver|598|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterRecoverableFailure|599|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterRecoverableStorage|600|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterRemoved|601|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterResourceAdded|602|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterResourceRemoved|603|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterThermistorFailure|604|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterTimingFailure|605|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterTurnedOff|606|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterTurnedOn|607|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterUnderTemperature|608|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterUnrecoverableFailure|609|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterUnrecoverableStorageError|610|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|slitterWarmingUp|611|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerAdded|612|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerAlmostEmpty|613|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerAlmostFull|614|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerAtLimit|615|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerClosed|616|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerConfigurationChange|617|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerCoverClosed|618|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerCoverOpen|619|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerEmpty|620|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerFull|621|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerInterlockClosed|622|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerInterlockOpen|623|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerJam|624|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerLifeAlmostOver|625|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerLifeOver|626|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerMemoryExhausted|627|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerMissing|628|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerMotorFailure|629|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerNearLimit|630|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerOffline|631|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerOpened|632|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerOverTemperature|633|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerPowerSaver|634|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerRecoverableFailure|635|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerRecoverableStorage|636|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerRemoved|637|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerResourceAdded|638|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerResourceRemoved|639|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerThermistorFailure|640|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerTimingFailure|641|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerTurnedOff|642|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerTurnedOn|643|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerUnderTemperature|644|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerUnrecoverableFailure|645|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerUnrecoverableStorageError|646|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stackerWarmingUp|647|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|standby|648|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5106.4.|
|staplerAdded|649|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerAlmostEmpty|650|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerAlmostFull|651|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerAtLimit|652|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerClosed|653|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerConfigurationChange|654|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerCoverClosed|655|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerCoverOpen|656|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerEmpty|657|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerFull|658|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerInterlockClosed|659|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerInterlockOpen|660|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerJam|661|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerLifeAlmostOver|662|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerLifeOver|663|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerMemoryExhausted|664|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerMissing|665|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerMotorFailure|666|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerNearLimit|667|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerOffline|668|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerOpened|669|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerOverTemperature|670|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerPowerSaver|671|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerRecoverableFailure|672|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerRecoverableStorage|673|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerRemoved|674|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerResourceAdded|675|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerResourceRemoved|676|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerThermistorFailure|677|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerTimingFailure|678|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerTurnedOff|679|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerTurnedOn|680|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerUnderTemperature|681|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerUnrecoverableFailure|682|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerUnrecoverableStorageError|683|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|staplerWarmingUp|684|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherAdded|685|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherAlmostEmpty|686|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherAlmostFull|687|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherAtLimit|688|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherClosed|689|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherConfigurationChange|690|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherCoverClosed|691|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherCoverOpen|692|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherEmpty|693|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherFull|694|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherInterlockClosed|695|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherInterlockOpen|696|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherJam|697|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherLifeAlmostOver|698|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherLifeOver|699|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherMemoryExhausted|700|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherMissing|701|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherMotorFailure|702|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherNearLimit|703|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherOffline|704|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherOpened|705|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherOverTemperature|706|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherPowerSaver|707|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherRecoverableFailure|708|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherRecoverableStorage|709|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherRemoved|710|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherResourceAdded|711|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherResourceRemoved|712|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherThermistorFailure|713|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherTimingFailure|714|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherTurnedOff|715|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherTurnedOn|716|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherUnderTemperature|717|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherUnrecoverableFailure|718|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherUnrecoverableStorageError|719|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|stitcherWarmingUp|720|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitAdded|721|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitAlmostEmpty|722|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitAlmostFull|723|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitAtLimit|724|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitClosed|725|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitCoolingDown|726|Este é um valor padrão de Atributo de Impressora IPP descrito no HPINC20180215.|
|subunitEmpty|727|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitFull|728|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitLifeAlmostOver|729|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitLifeOver|730|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitMemoryExhausted|731|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitMissing|732|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitMotorFailure|733|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitNearLimit|734|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitOffline|735|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitOpened|736|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitOverTemperature|737|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitPowerSaver|738|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitRecoverableFailure|739|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitRecoverableStorage|740|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitRemoved|741|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitResourceAdded|742|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitResourceRemoved|743|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitThermistorFailure|744|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitTimingFailure|745|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitTurnedOff|746|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitTurnedOn|747|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitUnderTemperature|748|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitUnrecoverableFailure|749|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitUnrecoverableStorage|750|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|subunitWarmingUp|751|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|suspend|752|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5106.4.|
|testing|753|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.22.|
|trimmerAdded|754|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerAlmostEmpty|755|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerAlmostFull|756|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerAtLimit|757|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerClosed|758|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerConfigurationChange|759|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerCoverClosed|760|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerCoverOpen|761|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerEmpty|762|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerFull|763|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerInterlockClosed|764|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerInterlockOpen|765|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerJam|766|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerLifeAlmostOver|767|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerLifeOver|768|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerMemoryExhausted|769|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerMissing|770|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerMotorFailure|771|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerNearLimit|772|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerOffline|773|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerOpened|774|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerOverTemperature|775|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerPowerSaver|776|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerRecoverableFailure|777|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerRecoverableStorage|778|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerRemoved|779|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerResourceAdded|780|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerResourceRemoved|781|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerThermistorFailure|782|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerTimingFailure|783|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerTurnedOff|784|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerTurnedOn|785|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerUnderTemperature|786|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerUnrecoverableFailure|787|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerUnrecoverableStorageError|788|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|trimmerWarmingUp|789|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|desconhecido|790|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperAdded|791|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperAlmostEmpty|792|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperAlmostFull|793|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperAtLimit|794|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperClosed|795|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperConfigurationChange|796|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperCoverClosed|797|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperCoverOpen|798|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperEmpty|799|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperFull|800|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperInterlockClosed|801|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperInterlockOpen|802|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperJam|803|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperLifeAlmostOver|804|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperLifeOver|805|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperMemoryExhausted|806|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperMissing|807|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperMotorFailure|808|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperNearLimit|809|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperOffline|810|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperOpened|811|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperOverTemperature|812|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperPowerSaver|813|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperRecoverableFailure|814|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperRecoverableStorage|815|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperRemoved|816|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperResourceAdded|817|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperResourceRemoved|818|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperThermistorFailure|819|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperTimingFailure|820|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperTurnedOff|821|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperTurnedOn|822|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperUnderTemperature|823|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperUnrecoverableFailure|824|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperUnrecoverableStorageError|825|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|wrapperWarmingUp|826|Este é um valor padrão de Atributo de Impressora IPP descrito em PWG5100.9.|
|unknownFutureValue|827|Valor de sentinela de enumeração evolvável. Não usar.|

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
