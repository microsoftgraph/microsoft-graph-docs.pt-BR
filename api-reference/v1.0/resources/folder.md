---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Pasta
ms.openlocfilehash: 664597297700f7af096ef30cfbd5342a45a6c157
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="folder-resource-type"></a><span data-ttu-id="10e1d-102">Tipo de recurso Folder</span><span class="sxs-lookup"><span data-stu-id="10e1d-102">Folder resource type</span></span>

<span data-ttu-id="10e1d-103">O recurso **Folder** agrupa dados relacionados a pastas em um item em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="10e1d-103">The **Folder** resource groups folder-related data on an item into a single structure. DriveItems with a non-null folder facet are containers for other DriveItems.</span></span> 
<span data-ttu-id="10e1d-104">[**DriveItems**](driveitem.md) com uma faceta **folder** não nula são contêineres de outros DriveItems.</span><span class="sxs-lookup"><span data-stu-id="10e1d-104">The Folder resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="10e1d-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10e1d-105">JSON representation</span></span>

<span data-ttu-id="10e1d-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10e1d-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="10e1d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10e1d-107">Properties</span></span>

| <span data-ttu-id="10e1d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10e1d-108">Property</span></span>       | <span data-ttu-id="10e1d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="10e1d-109">Type</span></span>           | <span data-ttu-id="10e1d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="10e1d-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="10e1d-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="10e1d-111">**childCount**</span></span> | <span data-ttu-id="10e1d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="10e1d-112">Int64</span></span>          | <span data-ttu-id="10e1d-113">Número de filhos imediatamente neste contêiner.</span><span class="sxs-lookup"><span data-stu-id="10e1d-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="10e1d-114">**view**</span><span class="sxs-lookup"><span data-stu-id="10e1d-114">**view**</span></span>       | <span data-ttu-id="10e1d-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="10e1d-115">[folderView facet][]</span></span> | <span data-ttu-id="10e1d-116">Uma coleção de propriedades que definem o modo de exibição recomendado para a pasta.</span><span class="sxs-lookup"><span data-stu-id="10e1d-116">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="10e1d-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="10e1d-117">Remarks</span></span> 

<span data-ttu-id="10e1d-118">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="10e1d-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderView.md
[DriveItem]: driveItem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
