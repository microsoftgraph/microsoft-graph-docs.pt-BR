---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Pasta
ms.openlocfilehash: dc90624b14a88d06b45302f421a7e3fcfa802a67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003486"
---
# <a name="folder-resource-type"></a><span data-ttu-id="9ae76-102">Tipo de recurso Folder</span><span class="sxs-lookup"><span data-stu-id="9ae76-102">Folder resource type</span></span>

<span data-ttu-id="9ae76-p101">O recurso **Folder** agrupa dados relacionados a pastas em um item em uma única estrutura. [**DriveItems**](driveitem.md) com uma faceta **folder** não nula são contêineres de outros DriveItems.</span><span class="sxs-lookup"><span data-stu-id="9ae76-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ae76-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ae76-105">JSON representation</span></span>

<span data-ttu-id="9ae76-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ae76-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="9ae76-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ae76-107">Properties</span></span>

| <span data-ttu-id="9ae76-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ae76-108">Property</span></span>       | <span data-ttu-id="9ae76-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ae76-109">Type</span></span>           | <span data-ttu-id="9ae76-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ae76-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="9ae76-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="9ae76-111">**childCount**</span></span> | <span data-ttu-id="9ae76-112">Int32</span><span class="sxs-lookup"><span data-stu-id="9ae76-112">Int32</span></span>          | <span data-ttu-id="9ae76-113">Número de filhos imediatamente neste contêiner.</span><span class="sxs-lookup"><span data-stu-id="9ae76-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="9ae76-114">**view**</span><span class="sxs-lookup"><span data-stu-id="9ae76-114">**view**</span></span>       | <span data-ttu-id="9ae76-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="9ae76-115">[folderView][]</span></span> | <span data-ttu-id="9ae76-116">Uma coleção de propriedades que definem o modo de exibição recomendado para a pasta.</span><span class="sxs-lookup"><span data-stu-id="9ae76-116">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="9ae76-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="9ae76-117">Remarks</span></span> 

<span data-ttu-id="9ae76-118">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="9ae76-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
