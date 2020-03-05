---
title: tipo de recurso personWebsite
description: tipo de recurso personWebsite
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: cf4386cf70179715880a1ae07db3dfbb5f07c224
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521894"
---
# <a name="personwebsite-resource-type"></a>tipo de recurso personWebsite

Namespace: Microsoft. Graph

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
