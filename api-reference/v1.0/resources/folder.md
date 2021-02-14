---
author: JeremyKelley
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
description: 'O recurso Folder agrupa dados relacionados a pastas em um item em uma única estrutura. '
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 27ea5bc0d90d89c13fe751e78e9aef423dd099ff
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240035"
---
# <a name="folder-resource-type"></a>Tipo de recurso Folder

Namespace: microsoft.graph

O recurso **Folder** agrupa dados relacionados a pastas em um item em uma única estrutura. [**DriveItems**](driveitem.md) com uma faceta **folder** não nula são contêineres de outros DriveItems.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.folder"
}-->

```json
{
  "childCount": 1024,
  "view": { "@odata.type": "microsoft.graph.folderView" }
}
```

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo           | Descrição
|:---------------|:---------------|:-------------------------------------------
| **childCount** | Int32          | Número de filhos imediatamente neste contêiner.
| **view**       | [folderView][] | Uma coleção de propriedades que definem o modo de exibição recomendado para a pasta.

## <a name="remarks"></a>Comentários 

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem][].

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->

