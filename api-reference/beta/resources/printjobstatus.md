---
title: tipo de recurso printJobStatus
description: Representa o status atual de um trabalho de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bebf2081dafe6412a22b66b8a371b67ba0e53548
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048734"
---
# <a name="printjobstatus-resource-type"></a>tipo de recurso printJobStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status atual de um trabalho de impressão.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|ProcessingState|printJobProcessingState|O estado atual de processamento do trabalho de impressão. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|processingStateDescription|Cadeia de caracteres|Uma descrição legível do estado de processamento atual do trabalho de impressão. Somente leitura.|
|acquiredByPrinter|Booliano|True se o trabalho foi confirmado por uma impressora; caso contrário, false. Somente leitura.|

### <a name="printjobprocessingstate-values"></a>valores de printJobProcessingState

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O estado de processamento relatado pela impressora não é reconhecido.|
|função|1 |O trabalho de impressão está aguardando o processamento da impressora.|
|pendingHeld|2 |O trabalho ainda não é um candidato para processamento. Certifique-se de que não haja erros ou limitações de recursos que impeçam o início do trabalho.|
|processe|3 |O trabalho de impressão está sendo processado pela impressora no momento.|
|pausado|4 |O trabalho de impressão foi pausado por um usuário.|
|parar|5 |O trabalho de impressão foi interrompido porque um problema com a impressora precisa ser resolvido para que o trabalho possa continuar. Mais informações podem ser encontradas no recurso de estado da impressora.|
|Completed|6 |O trabalho de impressão foi concluído com êxito e nenhum processamento adicional ocorrerá.|
|foi|7 |O trabalho de impressão foi cancelado por um usuário e nenhum processamento adicional ocorrerá.|
|anulada|8 |O trabalho de impressão foi anulado por um usuário ou pela impressora e nenhum processamento adicional ocorrerá.|

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
    "processingState": "String",
    "processingStateDescription": "String",
    "acquiredByPrinter": true
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

