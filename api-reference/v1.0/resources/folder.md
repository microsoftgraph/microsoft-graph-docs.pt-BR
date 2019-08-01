---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
description: 'O recurso Folder agrupa dados relacionados a pastas em um item em uma única estrutura. '
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f4b43c672b297ce50a5a6aa3dbb3f3d83a1d53be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030328"
---
# <a name="folder-resource-type"></a><span data-ttu-id="5e6a4-103">Tipo de recurso Folder</span><span class="sxs-lookup"><span data-stu-id="5e6a4-103">Folder resource type</span></span>

<span data-ttu-id="5e6a4-p101">O recurso **Folder** agrupa dados relacionados a pastas em um item em uma única estrutura. [**DriveItems**](driveitem.md) com uma faceta **folder** não nula são contêineres de outros DriveItems.</span><span class="sxs-lookup"><span data-stu-id="5e6a4-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e6a4-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e6a4-106">JSON representation</span></span>

<span data-ttu-id="5e6a4-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e6a4-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="5e6a4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e6a4-108">Properties</span></span>

| <span data-ttu-id="5e6a4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e6a4-109">Property</span></span>       | <span data-ttu-id="5e6a4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e6a4-110">Type</span></span>           | <span data-ttu-id="5e6a4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e6a4-111">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="5e6a4-112">**childCount**</span><span class="sxs-lookup"><span data-stu-id="5e6a4-112">**childCount**</span></span> | <span data-ttu-id="5e6a4-113">Int32</span><span class="sxs-lookup"><span data-stu-id="5e6a4-113">Int32</span></span>          | <span data-ttu-id="5e6a4-114">Número de filhos imediatamente neste contêiner.</span><span class="sxs-lookup"><span data-stu-id="5e6a4-114">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="5e6a4-115">**view**</span><span class="sxs-lookup"><span data-stu-id="5e6a4-115">**view**</span></span>       | <span data-ttu-id="5e6a4-116">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="5e6a4-116">[folderView][]</span></span> | <span data-ttu-id="5e6a4-117">Uma coleção de propriedades que definem o modo de exibição recomendado para a pasta.</span><span class="sxs-lookup"><span data-stu-id="5e6a4-117">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="5e6a4-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="5e6a4-118">Remarks</span></span> 

<span data-ttu-id="5e6a4-119">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="5e6a4-119">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
