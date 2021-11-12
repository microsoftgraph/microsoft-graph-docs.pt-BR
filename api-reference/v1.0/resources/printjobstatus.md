---
title: Tipo de recurso printJobStatus
description: Representa o status atual de um trabalho de impressão.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 5b9314117218275fcb0a746247a69c281c10fab4
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60936961"
---
# <a name="printjobstatus-resource-type"></a>Tipo de recurso printJobStatus

Namespace: microsoft.graph

Representa o status atual de um trabalho de impressão.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|state|printJobProcessingState|O estado de processamento atual do trabalho de impressão. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|detalhes|Coleção printJobProcessingDetail|Detalhes adicionais para o estado do trabalho de impressão. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|description|Cadeia de caracteres|Uma descrição aceitável para humanos do estado de processamento atual do trabalho de impressão. Somente leitura.|
|isAcquiredByPrinter|Boolean|True se o trabalho foi reconhecido por uma impressora; false caso contrário. Somente leitura.|

### <a name="printjobprocessingstate-values"></a>valores printJobProcessingState

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|O estado de processamento relatado pela impressora não é reconhecido.|
|pendente|1|O trabalho de impressão está aguardando processamento pela impressora.|
|processamento|2|O trabalho de impressão está sendo processado pela impressora.|
|pausado|3|O trabalho de impressão foi pausado.|
|stopped|4|O trabalho de impressão foi interrompido porque um problema com a impressora precisa ser resolvido antes que o trabalho possa continuar. Mais informações podem ser encontradas no recurso estado da impressora.|
|completed|5|O trabalho de impressão foi concluído com êxito e nenhum processamento posterior ocorrerá.|
|cancelado|6 |O trabalho de impressão foi cancelado por um usuário e nenhum outro processamento ocorrerá.|
|abortado|7 |O trabalho de impressão foi abortado por um usuário ou pela impressora e nenhum outro processamento ocorrerá.|

### <a name="printjobprocessingdetail-values"></a>valores printJobProcessingDetail

|Membro|Valor|Descrição|
|:---|:---|:---|
|uploadPending|0|A carga do documento não foi carregada.|
|transformando|1|A carga do documento está sendo transformada.|
|completedSuccessfully|2|O trabalho foi concluído com êxito.|
|completedWithWarnings|3|O trabalho foi concluído com avisos.|
|completedWithErrors|4|O trabalho foi concluído com erros.|
|releaseWait|5|O trabalho está pendente para ser liberado.|
|interpretando|6 |O trabalho está em estado de 'processamento', mas, mais especificamente, a carga do documento está sendo interpretada.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printJobStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJobStatus",
  "state": "String",
  "description": "String",
  "isAcquiredByPrinter": "Boolean",
  "details": [
    "String"
  ]
}
```

