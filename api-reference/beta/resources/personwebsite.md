---
title: tipo de recurso personWebsite
description: tipo de recurso personWebsite
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: b5e6b8c3013c647087ab3d8db28b0196d0c79036
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949493"
---
# <a name="personwebsite-resource-type"></a>tipo de recurso personWebsite

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre sites associados a um usuário em vários serviços.

Herda de [Myfacet](itemfacet.md).

## <a name="methods"></a>Métodos

| Método                                           | Tipo de retorno                       | Descrição                                                |
|:-------------------------------------------------|:----------------------------------|:-----------------------------------------------------------|
| [Obter personWebsite](../api/personwebsite-get.md) | [personWebsite](personwebsite.md) | Leia as propriedades e os relacionamentos de um objeto **personWebsite** . |
| [Atualizar personWebsite](../api/personwebsite-update.md)         | [personWebsite](personwebsite.md) | Atualizar um objeto **personWebsite** .                               |
| [Excluir personWebsite](../api/personwebsite-delete.md)         | Nenhum                              | Excluir um objeto **personWebsite** .                               |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo              | Descrição                                                                         |
|:-------------|:------------------|:------------------------------------------------------------------------------------|
|categories    |String collection  | Contém categorias que um usuário associou ao site (por exemplo, pessoal, receitas).  |
|description   |String             | Contém uma descrição do site.                                              |
|displayName   |Cadeia de caracteres             | Contém um nome amigável para o site.                                           |
|webUrl        |String             | Contém um link para o próprio site.                                              |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso. 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personWebsite",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "description": "String",
  "displayName": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personWebsite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
