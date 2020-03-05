---
author: JeremyKelley
description: 'O recurso Folder agrupa dados relacionados a pastas em um item em uma única estrutura. '
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b7950008a3bcd310e90f604becb865d130781b34
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497892"
---
# <a name="folder-resource-type"></a><span data-ttu-id="fa649-103">Tipo de recurso Folder</span><span class="sxs-lookup"><span data-stu-id="fa649-103">Folder resource type</span></span>

<span data-ttu-id="fa649-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fa649-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa649-p101">O recurso **Folder** agrupa dados relacionados a pastas em um item em uma única estrutura. [**DriveItems**](driveitem.md) com uma faceta **folder** não nula são contêineres de outros DriveItems.</span><span class="sxs-lookup"><span data-stu-id="fa649-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa649-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa649-107">JSON representation</span></span>

<span data-ttu-id="fa649-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa649-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="fa649-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa649-109">Properties</span></span>

| <span data-ttu-id="fa649-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa649-110">Property</span></span>       | <span data-ttu-id="fa649-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa649-111">Type</span></span>           | <span data-ttu-id="fa649-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa649-112">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="fa649-113">**childCount**</span><span class="sxs-lookup"><span data-stu-id="fa649-113">**childCount**</span></span> | <span data-ttu-id="fa649-114">Int64</span><span class="sxs-lookup"><span data-stu-id="fa649-114">Int64</span></span>          | <span data-ttu-id="fa649-115">Número de filhos imediatamente neste contêiner.</span><span class="sxs-lookup"><span data-stu-id="fa649-115">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="fa649-116">**view**</span><span class="sxs-lookup"><span data-stu-id="fa649-116">**view**</span></span>       | <span data-ttu-id="fa649-117">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="fa649-117">[folderView][]</span></span> | <span data-ttu-id="fa649-118">Uma coleção de propriedades que definem o modo de exibição recomendado para a pasta.</span><span class="sxs-lookup"><span data-stu-id="fa649-118">A collection of properties defining the recommended view for the folder.</span></span>


## <a name="remarks"></a><span data-ttu-id="fa649-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="fa649-119">Remarks</span></span> 

<span data-ttu-id="fa649-120">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="fa649-120">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

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
