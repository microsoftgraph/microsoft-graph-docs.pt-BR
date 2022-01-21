---
title: Tipo de recurso richLongRunningOperation
description: Contém metadados sobre a operação de execução longa.
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 2f16e9abb8dc3a22ad7a3d3b32e707ddb595c06a
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162195"
---
# <a name="richlongrunningoperation-resource-type"></a>Tipo de recurso richLongRunningOperation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém metadados sobre a operação de execução longa.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar richLongRunningOperations em um site](../api/site-list-operations.md)|[coleção richLongRunningOperation](../resources/richlongrunningoperation.md)|Obter uma lista dos [objetos richLongRunningOperation](../resources/richlongrunningoperation.md) e suas propriedades em um site.|
|[Listar richLongRunningOperations em uma lista](../api/list-list-operations.md)|[coleção richLongRunningOperation](../resources/richlongrunningoperation.md)|Obter uma lista dos [objetos richLongRunningOperation](../resources/richlongrunningoperation.md) e suas propriedades em uma lista.|
|[Obter richLongRunningOperation](../api/richlongrunningoperation-get.md)|[richLongRunningOperation](../resources/richlongrunningoperation.md)|Leia as propriedades de [um objeto richLongRunningOperation.](../resources/richlongrunningoperation.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Hora em que essa operação foi criada.|
|erro|[publicError](../resources/publicerror.md)| Erro devido ao qual a operação falhou.|
|id|Cadeia de caracteres|Identificador de operação. Herda da [entidade](../resources/entity.md).|
|lastActionDateTime|DateTimeOffset| Hora em que a última ação foi executada nesta operação.|
|percentageComplete|Int32|Um valor entre 0 e 100 que indica o andamento da operação.|
|resourceId|Cadeia de caracteres|Um identificador exclusivo para o resultado.|
|resourceLocation|Cadeia de caracteres|Url canônica do recurso.|
|status|longRunningOperationStatus|Status do opertaion. Os valores possíveis são: `notStarted` , , , , `running` `succeeded` `failed` `unknownFutureValue` .|
|statusDetail|Cadeia de caracteres|Detalhes sobre o valor de status.|
|type|Cadeia de caracteres| Tipo da operação.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.richLongRunningOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.richLongRunningOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "resourceLocation": "String",
  "status": "String",
  "statusDetail": "String",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  },
  "percentageComplete": "Integer",
  "resourceId": "String",
  "type": "String"
}
```

