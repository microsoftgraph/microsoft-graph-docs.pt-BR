---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Pasta
localization_priority: Normal
ms.openlocfilehash: af22487f017830481af6f39e113b80009f2e567f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512749"
---
# <a name="folder-resource-type"></a><span data-ttu-id="3722d-102">Tipo de recurso Folder</span><span class="sxs-lookup"><span data-stu-id="3722d-102">Folder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3722d-p101">O recurso **Folder** agrupa dados relacionados a pastas em um item em uma única estrutura. [**DriveItems**](driveitem.md) com uma faceta **folder** não nula são contêineres de outros DriveItems.</span><span class="sxs-lookup"><span data-stu-id="3722d-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3722d-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3722d-105">JSON representation</span></span>

<span data-ttu-id="3722d-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3722d-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3722d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3722d-107">Properties</span></span>

| <span data-ttu-id="3722d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3722d-108">Property</span></span>       | <span data-ttu-id="3722d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3722d-109">Type</span></span>           | <span data-ttu-id="3722d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3722d-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="3722d-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="3722d-111">**childCount**</span></span> | <span data-ttu-id="3722d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="3722d-112">Int64</span></span>          | <span data-ttu-id="3722d-113">Número de filhos imediatamente neste contêiner.</span><span class="sxs-lookup"><span data-stu-id="3722d-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="3722d-114">**view**</span><span class="sxs-lookup"><span data-stu-id="3722d-114">**view**</span></span>       | <span data-ttu-id="3722d-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="3722d-115">[folderView][]</span></span> | <span data-ttu-id="3722d-116">Uma coleção de propriedades que definem o modo de exibição recomendado para a pasta.</span><span class="sxs-lookup"><span data-stu-id="3722d-116">A collection of properties defining the recommended view for the folder.</span></span>


## <a name="remarks"></a><span data-ttu-id="3722d-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="3722d-117">Remarks</span></span> 

<span data-ttu-id="3722d-118">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="3722d-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/folder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
