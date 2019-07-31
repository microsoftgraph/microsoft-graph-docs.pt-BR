---
author: JeremyKelley
description: 'O recurso Folder agrupa dados relacionados a pastas em um item em uma única estrutura. '
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f9cbbba6ae20c56800a5f6f492319f47b7d8017c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971988"
---
# <a name="folder-resource-type"></a><span data-ttu-id="0775b-103">Tipo de recurso Folder</span><span class="sxs-lookup"><span data-stu-id="0775b-103">Folder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0775b-p101">O recurso **Folder** agrupa dados relacionados a pastas em um item em uma única estrutura. [**DriveItems**](driveitem.md) com uma faceta **folder** não nula são contêineres de outros DriveItems.</span><span class="sxs-lookup"><span data-stu-id="0775b-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0775b-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0775b-106">JSON representation</span></span>

<span data-ttu-id="0775b-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0775b-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="0775b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0775b-108">Properties</span></span>

| <span data-ttu-id="0775b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0775b-109">Property</span></span>       | <span data-ttu-id="0775b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0775b-110">Type</span></span>           | <span data-ttu-id="0775b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0775b-111">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="0775b-112">**childCount**</span><span class="sxs-lookup"><span data-stu-id="0775b-112">**childCount**</span></span> | <span data-ttu-id="0775b-113">Int64</span><span class="sxs-lookup"><span data-stu-id="0775b-113">Int64</span></span>          | <span data-ttu-id="0775b-114">Número de filhos imediatamente neste contêiner.</span><span class="sxs-lookup"><span data-stu-id="0775b-114">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="0775b-115">**view**</span><span class="sxs-lookup"><span data-stu-id="0775b-115">**view**</span></span>       | <span data-ttu-id="0775b-116">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="0775b-116">[folderView][]</span></span> | <span data-ttu-id="0775b-117">Uma coleção de propriedades que definem o modo de exibição recomendado para a pasta.</span><span class="sxs-lookup"><span data-stu-id="0775b-117">A collection of properties defining the recommended view for the folder.</span></span>


## <a name="remarks"></a><span data-ttu-id="0775b-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="0775b-118">Remarks</span></span> 

<span data-ttu-id="0775b-119">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="0775b-119">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

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
