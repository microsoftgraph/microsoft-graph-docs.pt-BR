---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
ms.openlocfilehash: 77c13d980590e908de5c7f0a8a7cbf67d1cf031e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340224"
---
# <a name="folder-resource-type"></a><span data-ttu-id="528b6-102">Tipo de recurso Folder</span><span class="sxs-lookup"><span data-stu-id="528b6-102">Folder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="528b6-p101">O recurso **Folder** agrupa dados relacionados a pastas em um item em uma única estrutura. [**DriveItems**](driveitem.md) com uma faceta **folder** não nula são contêineres de outros DriveItems.</span><span class="sxs-lookup"><span data-stu-id="528b6-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="528b6-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="528b6-105">JSON representation</span></span>

<span data-ttu-id="528b6-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="528b6-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="528b6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="528b6-107">Properties</span></span>

| <span data-ttu-id="528b6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="528b6-108">Property</span></span>       | <span data-ttu-id="528b6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="528b6-109">Type</span></span>           | <span data-ttu-id="528b6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="528b6-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="528b6-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="528b6-111">**childCount**</span></span> | <span data-ttu-id="528b6-112">Int64</span><span class="sxs-lookup"><span data-stu-id="528b6-112">Int64</span></span>          | <span data-ttu-id="528b6-113">Número de filhos imediatamente neste contêiner.</span><span class="sxs-lookup"><span data-stu-id="528b6-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="528b6-114">**view**</span><span class="sxs-lookup"><span data-stu-id="528b6-114">**view**</span></span>       | <span data-ttu-id="528b6-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="528b6-115">[folderView][]</span></span> | <span data-ttu-id="528b6-116">Uma coleção de propriedades que definem o modo de exibição recomendado para a pasta.</span><span class="sxs-lookup"><span data-stu-id="528b6-116">A collection of properties defining the recommended view for the folder.</span></span>


## <a name="remarks"></a><span data-ttu-id="528b6-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="528b6-117">Remarks</span></span> 

<span data-ttu-id="528b6-118">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="528b6-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
