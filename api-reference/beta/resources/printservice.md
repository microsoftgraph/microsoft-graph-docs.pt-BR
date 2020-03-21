---
title: tipo de recurso de serviço de serviço
description: Representa uma descrição específica do locatário do Azure AD de uma instância de serviço de impressão. Existem serviços para cada componente da infraestrutura de impressão (por exemplo, descoberta, notificações, registro e IPP) e ter um ou mais pontos de extremidade.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: fd8641f7fe9fd361e131f0978c8f677a6395e405
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895500"
---
# <a name="printservice-resource-type"></a>tipo de recurso de serviço de serviço

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma descrição específica do locatário do Azure AD de uma instância de serviço de impressão. Os serviços existem para cada componente da infraestrutura de impressão (descoberta, notificações, registro e IPP) e ter um ou mais pontos de extremidade.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar serviços](../api/print-list-services.md) | coleção de [serviços de multiserviço](printservice.md) | Obtenha uma lista de serviços de impressão universal. |
| [Obter serviço](../api/printservice-get.md) | [Serviço de serviço](printservice.md) | Leia as propriedades e as relações do objeto de serviço. |
| [Listar pontos de extremidade](../api/printservice-list-endpoints.md) | coleção [Barserviceendpoint](printserviceendpoint.md) | Obter uma lista de pontos de extremidade que um serviço fornece. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O identificador do serviço. Somente leitura.|

## <a name="relationships"></a>Relacionamento
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|pontos de extremidade|coleção [Barserviceendpoint](printserviceendpoint.md)| Pontos de extremidade que podem ser usados para acessar o serviço. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printService",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "endpoints": [ {"@odata.type": "microsoft.graph.printServiceEndpoint"} ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->