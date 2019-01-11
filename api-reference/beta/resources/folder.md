---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Pasta
localization_priority: Normal
ms.openlocfilehash: 98c477ebeda436c57db3eaac5cb062639a2447d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856494"
---
# <a name="folder-resource-type"></a><span data-ttu-id="b94fa-102">Tipo de recurso Folder</span><span class="sxs-lookup"><span data-stu-id="b94fa-102">Folder resource type</span></span>

> <span data-ttu-id="b94fa-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b94fa-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b94fa-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b94fa-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b94fa-p102">O recurso **Folder** agrupa dados relacionados a pastas em um item em uma única estrutura. [**DriveItems**](driveitem.md) com uma faceta **folder** não nula são contêineres de outros DriveItems.</span><span class="sxs-lookup"><span data-stu-id="b94fa-p102">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b94fa-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b94fa-107">JSON representation</span></span>

<span data-ttu-id="b94fa-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b94fa-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="b94fa-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b94fa-109">Properties</span></span>

| <span data-ttu-id="b94fa-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b94fa-110">Property</span></span>       | <span data-ttu-id="b94fa-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b94fa-111">Type</span></span>           | <span data-ttu-id="b94fa-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b94fa-112">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="b94fa-113">**childCount**</span><span class="sxs-lookup"><span data-stu-id="b94fa-113">**childCount**</span></span> | <span data-ttu-id="b94fa-114">Int64</span><span class="sxs-lookup"><span data-stu-id="b94fa-114">Int64</span></span>          | <span data-ttu-id="b94fa-115">Número de filhos imediatamente neste contêiner.</span><span class="sxs-lookup"><span data-stu-id="b94fa-115">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="b94fa-116">**view**</span><span class="sxs-lookup"><span data-stu-id="b94fa-116">**view**</span></span>       | <span data-ttu-id="b94fa-117">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="b94fa-117">[folderView][]</span></span> | <span data-ttu-id="b94fa-118">Uma coleção de propriedades que definem o modo de exibição recomendado para a pasta.</span><span class="sxs-lookup"><span data-stu-id="b94fa-118">A collection of properties defining the recommended view for the folder.</span></span>


## <a name="remarks"></a><span data-ttu-id="b94fa-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="b94fa-119">Remarks</span></span> 

<span data-ttu-id="b94fa-120">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="b94fa-120">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
