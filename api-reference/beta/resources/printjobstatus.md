---
title: tipo de recurso printJobStatus
description: Representa o status atual de um trabalho de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bb3221eb12946d58664211731a31993e540aaf00
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728932"
---
# <a name="printjobstatus-resource-type"></a>tipo de recurso printJobStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status atual de um trabalho de impressão.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|state|printJobProcessingState|O estado atual de processamento do trabalho de impressão. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|detalhes|coleção printJobProcessingDetail|Detalhes adicionais para o estado do trabalho de impressão. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|description|String|Uma descrição legível do estado de processamento atual do trabalho de impressão. Somente leitura.|
|isAcquiredByPrinter|Booliano|True se o trabalho foi confirmado por uma impressora; caso contrário, false. Somente leitura.|

### <a name="printjobprocessingstate-values"></a>valores de printJobProcessingState

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O estado de processamento relatado pela impressora não é reconhecido.|
|função|1|O trabalho de impressão está aguardando o processamento da impressora.|
|processe|duas|O trabalho de impressão está sendo processado pela impressora no momento.|
|pausado|3D|O trabalho de impressão foi pausado.|
|parar|4 |O trabalho de impressão foi interrompido porque um problema com a impressora precisa ser resolvido para que o trabalho possa continuar. Mais informações podem ser encontradas no recurso de estado da impressora.|
|Completed|5 |O trabalho de impressão foi concluído com êxito e nenhum processamento adicional ocorrerá.|
|foi|6 |O trabalho de impressão foi cancelado por um usuário e nenhum processamento adicional ocorrerá.|
|anulada|7 |O trabalho de impressão foi anulado por um usuário ou pela impressora e nenhum processamento adicional ocorrerá.|

### <a name="printjobprocessingdetail-values"></a>valores de printJobProcessingDetail

|Membro|Valor|Descrição|
|:---|:---|:---|
|uploadPending|,0|A carga do documento não foi carregada.|
|transformar|1|A carga do documento está sendo transformada.|
|completedSuccessfully|duas|O trabalho foi concluído com êxito.|
|completedWithWarnings|3D|O trabalho foi concluído com avisos.|
|completedWithErrors|4 |O trabalho foi concluído com erros.|
|releaseWait|5 |O trabalho está pendente para ser liberado.|
|interpretar|6 |O trabalho está no estado de "processamento", mas, mais especificamente, a carga do documento está sendo interpretada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJobStatus"
}-->

```json
{
    "state": "String",
    "description": "String",
    "isAcquiredByPrinter": true,    
    "details": ["String"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJobStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

