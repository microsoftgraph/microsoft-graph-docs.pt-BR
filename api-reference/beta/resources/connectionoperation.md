---
title: tipo de recurso connectionOperation
description: Descreve o status de uma solicitação assíncrona para criar um esquema de conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9ced1c9bd00e3e865c3663ed6ade936747b9dded
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704140"
---
# <a name="connectionoperation-resource-type"></a>tipo de recurso connectionOperation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o status de uma solicitação assíncrona para criar um [esquema](schema.md)de conexão de pesquisa da Microsoft.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter connectionOperation](../api/connectionoperation-get.md) | [connectionOperation](connectionoperation.md) | Ler as propriedades de um objeto connectionOperation. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo                          | Descrição                       |
|:---------|:------------------------------|:----------------------------------|
| erro    | [errorDetail](errordetail.md) | Se `status` for `failed`, fornecerá mais informações sobre o erro que causou a falha. |
| id       | Cadeia de caracteres                        | Identificador exclusivo para o connectionOperation. Somente leitura. |
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
  "baseType": "",
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
