---
title: tipo de recurso personWebsite
description: tipo de recurso personWebsite
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0be7c3863f9c764e7b6a0c0a4d0d8b2e9dc30717
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939590"
---
# <a name="personwebsite-resource-type"></a>tipo de recurso personWebsite

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre sites que o usuário tenha associado a si mesmos em vários serviços.

Herda de [Myfacet](itemfacet.md).

## <a name="methods"></a>Métodos

| Método                                           | Tipo de retorno                       | Descrição                                                |
|:-------------------------------------------------|:----------------------------------|:-----------------------------------------------------------|
| [Obter personWebsite](../api/personwebsite-get.md) | [personWebsite](personwebsite.md) | Leia as propriedades e os relacionamentos do objeto personWebsite. |
| [Update](../api/personwebsite-update.md)         | [personWebsite](personwebsite.md) | Atualize o objeto personWebsite.                               |
| [Delete](../api/personwebsite-delete.md)         | None                              | Exclua o objeto personWebsite.                               |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo              | Descrição                                                                         |
|:-------------|:------------------|:------------------------------------------------------------------------------------|
|categories    |String collection  | Contém categorias que um usuário associou ao site (por exemplo: pessoal, receitas)  |
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