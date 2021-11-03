---
title: tipo de recurso de esquema
description: O esquema de conexão determina como o conteúdo adicionado a uma conexão será usado em várias experiências Graph Microsoft.
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8dbf6a4df47f9afb3e24effbf9d90759dc87d677
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60729203"
---
# <a name="schema-resource-type"></a>tipo de recurso de esquema

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O [esquema](externalconnectors-externalconnection.md) de conexão determina como seu conteúdo externo será usado em várias experiências Graph Microsoft. O esquema é uma lista simples de todas as propriedades que você planeja adicionar à conexão, juntamente com seus atributos, rótulos e aliases. Você deve registrá-lo antes de adicionar itens na conexão.

## <a name="methods"></a>Métodos

| Método                                                    | Tipo de retorno                   | Descrição |
|:----------------------------------------------------------|:------------------------------|:--|
| [Criar esquema](../api/externalconnectors-externalconnection-post-schema.md) | Nenhum *ou* [esquema](externalconnectors-schema.md) | Registrar esquema de conexão. |
| [Obter esquema](../api/externalconnectors-schema-get.md)                        | [schema](externalconnectors-schema.md)           | Ler propriedades de um objeto de esquema. |

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo                               | Descrição                |
|:-----------|:-----------------------------------|:---------------------------|
| baseType   | String                             | Tem que ser definida como `microsoft.graph.externalItem`. Obrigatório. |
| properties | [coleção property](externalconnectors-property.md) | As propriedades definidas para os itens na conexão. O número mínimo de propriedades é um, o máximo é 128. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.externalConnectors.schema",
  "keyProperty": "id"
}-->

```json
{
  "baseType": "String",
  "id": "String (identifier)",
  "properties": [
    {
      "name": "String",
      "type": "String"
    }
  ]
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
