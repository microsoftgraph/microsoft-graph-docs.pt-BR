---
title: tipo de recurso de esquema
description: Descreve o tipo de conteúdo e como indexar cada propriedade em itens em uma conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 2a13d797ff3b695250f7dd5cfef3bc077afe505b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870114"
---
# <a name="schema-resource-type"></a>tipo de recurso de esquema

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o tipo de conteúdo e como indexar cada propriedade em itens em uma [conexão](externalconnection.md)de pesquisa da Microsoft.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Métodos

| Método                                                    | Tipo de retorno                   | Descrição |
|:----------------------------------------------------------|:------------------------------|:--|
| [Criar esquema](../api/externalconnection-post-schema.md) | Nenhum *ou* [esquema](schema.md) | Registrar o esquema de conexão. |
| [Obter esquema](../api/schema-get.md)                        | [schema](schema.md)           | Ler as propriedades de um objeto Schema. |

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo                               | Descrição                |
|:-----------|:-----------------------------------|:---------------------------|
| baseType   | String                             | Os valores possíveis são: `microsoft.graph.externalItem` e `microsoft.graph.externalFile`. Obrigatório. |
| properties | coleção [Property](property.md) | As propriedades definidas para os itens na conexão. O número mínimo de propriedades é um, o máximo é 64. Obrigatório quando `baseType` está definido como `microsoft.graph.externalItem`. Ignorado quando `baseType` está definido como `microsoft.graph.externalFile`. |

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
