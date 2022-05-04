---
title: Tipo de recurso richLongRunningOperation
description: Representa o status de uma operação de execução longa em um site ou uma lista.
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 73f57e5daaf2f55aca6fa03f0958d19d8323bdf8
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191818"
---
# <a name="richlongrunningoperation-resource-type"></a>Tipo de recurso richLongRunningOperation

Namespace: microsoft.graph

Representa o status de uma operação de execução longa em um [site](../resources/site.md) ou uma [lista](../resources/list.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter richLongRunningOperation](../api/richlongrunningoperation-get.md)|[richLongRunningOperation](../resources/richlongrunningoperation.md)|Obtenha o status de uma [operação de execução longa avançada](../resources/richlongrunningoperation.md) em um [site](../resources/site.md) ou uma [lista](../resources/list.md).|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|A data e a hora em que essa operação foi criada.|
|erro|[publicError](../resources/publicerror.md)| Erro que causou a falha da operação.|
|id|Cadeia de caracteres|Identificador exclusivo para a operação. Herdado da [entidade](../resources/entity.md).|
|lastActionDateTime|DateTimeOffset| A data e a hora em que a última ação foi executada nesta operação.|
|percentageComplete|Int32|Um valor entre 0 e 100 que indica o progresso da operação.|
|resourceId|Cadeia de caracteres|O identificador exclusivo do resultado.|
|Resourcelocation|Cadeia de Caracteres|A URL canônica do recurso.|
|status|Longrunningoperationstatus|O status da operação de execução longa. Os valores possíveis são: `notStarted`, `running`, `succeeded`, `failed`, `unknownFutureValue`.|
|statusDetail|Cadeia de Caracteres|Os detalhes sobre o valor de status.|
|type|Cadeia de caracteres| O tipo da operação.|

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
  "createdDateTime": "String (timestamp)",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  },
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "percentageComplete": "Integer",
  "resourceId": "String",
  "resourceLocation": "String",
  "status": "String",
  "statusDetail": "String",
  "type": "String"
}
```

