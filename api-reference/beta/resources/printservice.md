---
title: Tipo de recurso printService
description: Representa uma descrição Azure AD específica do locatário de uma instância de serviço de impressão. Os serviços existem para cada componente da infraestrutura de impressão (por exemplo, descoberta, notificações, registro e IPP) e têm um ou mais pontos de extremidade.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: df904704f6efb9d069832a6b9767ab1314e261ee
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176760"
---
# <a name="printservice-resource-type"></a>Tipo de recurso printService

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma descrição Azure AD específica do locatário de uma instância de serviço de impressão. Os serviços existem para cada componente da infraestrutura de impressão (descoberta, notificações, registro e IPP) e têm um ou mais pontos de extremidade.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar serviços](../api/print-list-services.md) | [coleção printService](printservice.md) | Obter uma lista de serviços de Impressão Universal. |
| [Obter serviço](../api/printservice-get.md) | [printService](printservice.md) | Leia as propriedades e as relações do objeto de serviço. |
| [Listar pontos de extremidade](../api/printservice-list-endpoints.md) | [coleção printServiceEndpoint](printserviceendpoint.md) | Obtenha uma lista de pontos de extremidade que um serviço fornece. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|O identificador do serviço. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|pontos de extremidade|[coleção printServiceEndpoint](printserviceendpoint.md)| Pontos de extremidade que podem ser usados para acessar o serviço. Somente leitura. Anulável.|

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

