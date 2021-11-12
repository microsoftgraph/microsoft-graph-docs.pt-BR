---
title: Tipo de recurso printOperationStatus
description: Representa o status atual de uma operação de Impressão Universal de longa duração.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: dd5e7e912ea6810a4a0d501d47a8711830e91ae0
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944890"
---
# <a name="printoperationstatus-resource-type"></a>Tipo de recurso printOperationStatus

Namespace: microsoft.graph

Representa o status atual de uma operação de Impressão Universal de longa duração.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|state|printOperationProcessingState|O estado de processamento atual da printOperation. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|description|Cadeia de caracteres|Uma descrição aceitável para humanos do estado de processamento atual do printOperation. Somente leitura.|

### <a name="printoperationprocessingstate-values"></a>valores printOperationProcessingState

|Membro|Valor|Descrição|
|:---|:---|:---|
|notStarted|0|A operação ainda não foi iniciada.|
|running|1|A operação está em execução.|
|bem-sucedido|2|A operação foi concluída com êxito.|
|failed|3|Falha na operação.|
|unknownFutureValue|4|Valor de sentinela de enumeração evolvável. Não usar.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printOperationStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printOperationStatus",
  "state": "String",
  "description": "String"
}
```

