---
title: Tipo de recurso printService
description: Representa uma descrição específica do locatário do Azure AD de uma instância de serviço de impressão. Os serviços existem para cada componente da infraestrutura de impressão (por exemplo, descoberta, notificações, registro e IPP) e têm um ou mais pontos de extremidade.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 08b5a0857a62e91f545c6678398f54c4585436be
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2021
ms.locfileid: "60355236"
---
# <a name="printservice-resource-type"></a>Tipo de recurso printService

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma descrição específica do locatário do Azure AD de uma instância de serviço de impressão. Os serviços existem para cada componente da infraestrutura de impressão (descoberta, notificações, registro e IPP) e têm um ou mais pontos de extremidade.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar serviços](../api/print-list-services.md) | [Coleção printService](printservice.md) | Obter uma lista de serviços de Impressão Universal. |
| [Obter serviço](../api/printservice-get.md) | [printService](printservice.md) | Leia as propriedades e as relações do objeto service. |
| [Listar pontos de extremidade](../api/printservice-list-endpoints.md) | [Coleção printServiceEndpoint](printserviceendpoint.md) | Obter uma lista de pontos de extremidade que um serviço fornece. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O identificador do serviço. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|pontos de extremidade|[Coleção printServiceEndpoint](printserviceendpoint.md)| Pontos de extremidade que podem ser usados para acessar o serviço. Somente leitura. Anulável.|

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

