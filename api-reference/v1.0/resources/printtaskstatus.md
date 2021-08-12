---
title: Tipo de recurso printTaskStatus
description: Representa o status de execução atual de um printTask.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7f07ee889cb8f04edff66416ebc6ce49f7e7a3ab67a07119170929fdc12cdf8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229014"
---
# <a name="printtaskstatus-resource-type"></a>Tipo de recurso printTaskStatus

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Representa o status de execução atual de [um printTask](printtask.md). 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|state|printTaskProcessingState|O estado de processamento atual do [printTask](printtask.md). Os valores válidos são descritos na tabela a seguir.|
|description|Cadeia de caracteres|Uma descrição aceitável para humanos do estado de processamento atual do [printTask](printtask.md).|

### <a name="printtaskprocessingstate-values"></a>valores printTaskProcessingState

|Membro|Valor|Descrição|
|:---|:---|:---|
|pendente|0|A execução da tarefa está pendente.|
|processamento|1|A execução da tarefa está em andamento.|
|completed|2|A execução da tarefa foi concluída.|
|abortado|3|A execução da tarefa foi abortada.|
|unknownFutureValue|4 |Valor de sentinela de enumeração evolvável. Não usar.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printTaskStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskStatus",
  "state": "String",
  "description": "String"
}
```

