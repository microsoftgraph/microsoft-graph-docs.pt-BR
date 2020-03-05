---
title: tipo de recurso connectionOperation
description: Descreve o status de uma solicitação assíncrona para criar um esquema de conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 21d962bbbfee64c51f11cf1ac3f5e7de2c0497e9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507482"
---
# <a name="connectionoperation-resource-type"></a>tipo de recurso connectionOperation

Namespace: Microsoft. Graph

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
