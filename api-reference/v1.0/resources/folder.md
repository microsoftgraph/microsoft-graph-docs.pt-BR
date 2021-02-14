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
# <a name="folder-resource-type"></a><span data-ttu-id="5a52c-103">Tipo de recurso Folder</span><span class="sxs-lookup"><span data-stu-id="5a52c-103">Folder resource type</span></span>

<span data-ttu-id="5a52c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a52c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a52c-p101">O recurso **Folder** agrupa dados relacionados a pastas em um item em uma única estrutura. [**DriveItems**](driveitem.md) com uma faceta **folder** não nula são contêineres de outros DriveItems.</span><span class="sxs-lookup"><span data-stu-id="5a52c-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a52c-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a52c-107">JSON representation</span></span>

<span data-ttu-id="5a52c-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a52c-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="5a52c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a52c-109">Properties</span></span>

| <span data-ttu-id="5a52c-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a52c-110">Property</span></span>       | <span data-ttu-id="5a52c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a52c-111">Type</span></span>           | <span data-ttu-id="5a52c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a52c-112">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="5a52c-113">**childCount**</span><span class="sxs-lookup"><span data-stu-id="5a52c-113">**childCount**</span></span> | <span data-ttu-id="5a52c-114">Int32</span><span class="sxs-lookup"><span data-stu-id="5a52c-114">Int32</span></span>          | <span data-ttu-id="5a52c-115">Número de filhos imediatamente neste contêiner.</span><span class="sxs-lookup"><span data-stu-id="5a52c-115">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="5a52c-116">**view**</span><span class="sxs-lookup"><span data-stu-id="5a52c-116">**view**</span></span>       | <span data-ttu-id="5a52c-117">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="5a52c-117">[folderView][]</span></span> | <span data-ttu-id="5a52c-118">Uma coleção de propriedades que definem o modo de exibição recomendado para a pasta.</span><span class="sxs-lookup"><span data-stu-id="5a52c-118">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="5a52c-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="5a52c-119">Remarks</span></span> 

<span data-ttu-id="5a52c-120">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="5a52c-120">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->

