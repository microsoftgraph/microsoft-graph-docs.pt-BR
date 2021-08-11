---
title: Tipo de recurso printOperationStatus
description: Representa o status atual de uma operação de Impressão Universal de longa duração.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 968958ef9d016b672bfe4d100cfc09f7a3b57d6c6c3ff28c36309ec6df04fe4d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54154886"
---
# <a name="printoperationstatus-resource-type"></a>Tipo de recurso printOperationStatus

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

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
|unknownFutureValue|4 |Valor de sentinela de enumeração evolvável. Não usar.|

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

