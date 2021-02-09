---
title: Tipo de recurso connectionOperation
description: Descreve o status de uma solicitação assíncrona para criar um esquema de conexão da Pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e17b1f55b00fd7b9bdc69eb7a7a34d3453ab332d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158300"
---
# <a name="connectionoperation-resource-type"></a>Tipo de recurso connectionOperation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o status de uma solicitação assíncrona para criar um esquema de conexão da Pesquisa [da](schema.md)Microsoft.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter connectionOperation](../api/connectionoperation-get.md) | [connectionOperation](connectionoperation.md) | Leia as propriedades de um objeto connectionOperation. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo                          | Descrição                       |
|:---------|:------------------------------|:----------------------------------|
| erro    | [errorDetail](errordetail.md) | Se `status` `failed` for, fornece mais informações sobre o erro que causou a falha. |
| id       | String                        | Identificador exclusivo da connectionOperation. Somente leitura. |
| status   | cadeia de caracteres                        | Indica o status da operação assíncrona. Os valores possíveis são: `unspecified`, `inprogress`, `completed`, `failed`. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectionOperation",
  "keyProperty": "id"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.errorDetail"},
  "id": "String (identifier)",
  "status": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectionOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


