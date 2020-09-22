---
title: tipo de recurso de esquema
description: O esquema de conexão determina como o conteúdo adicionado a uma conexão será usado em várias experiências do Microsoft Graph.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: ff14f04adb31d99aadec15cb9368e09a098c7a26
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192865"
---
# <a name="schema-resource-type"></a>tipo de recurso de esquema

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O esquema de [conexão](externalconnection.md) determina como o conteúdo externo será usado em várias experiências do Microsoft Graph. Schema é uma lista simples de todas as propriedades que você planeja adicionar à conexão junto com seus atributos, rótulos e aliases. Você deve registrar o esquema antes de adicionar itens à conexão.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Methods

| Método                                                    | Tipo de retorno                   | Descrição |
|:----------------------------------------------------------|:------------------------------|:--|
| [Criar esquema](../api/externalconnection-post-schema.md) | Nenhum *ou* [esquema](schema.md) | Registrar o esquema de conexão. |
| [Obter esquema](../api/schema-get.md)                        | [schema](schema.md)           | Ler as propriedades de um objeto Schema. |

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo                               | Descrição                |
|:-----------|:-----------------------------------|:---------------------------|
| baseType   | String                             | Deve ser definida como `microsoft.graph.externalItem`. Obrigatório. |
| properties | coleção [Property](property.md) | As propriedades definidas para os itens na conexão. O número mínimo de propriedades é um, o máximo é 128. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schema",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "baseType": "String",
  "id": "String (identifier)",
  "properties": [{"@odata.type": "microsoft.graph.property"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "schema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


