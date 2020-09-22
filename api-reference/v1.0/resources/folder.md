---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
description: 'O recurso Folder agrupa dados relacionados a pastas em um item em uma única estrutura. '
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8b883a263833380d415d3b3878b48423e5566e64
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018309"
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

