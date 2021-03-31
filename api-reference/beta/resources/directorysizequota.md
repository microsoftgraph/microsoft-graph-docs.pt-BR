---
title: Tipo de recurso directorySizeQuota
description: Representa a cota de diretório total e usada de uma empresa.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: Jumaodhiss
ms.openlocfilehash: 54e2280fdb416e5ccfd0853ee77a2ef3f90ddf37
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469371"
---
# <a name="directorysizequota-resource-type"></a><span data-ttu-id="3d841-103">Tipo de recurso directorySizeQuota</span><span class="sxs-lookup"><span data-stu-id="3d841-103">directorySizeQuota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d841-104">Representa a cota de diretório total e usada de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="3d841-104">Represents a company's used and total directory quota.</span></span>

## <a name="properties"></a><span data-ttu-id="3d841-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d841-105">Properties</span></span>
| <span data-ttu-id="3d841-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d841-106">Property</span></span>   | <span data-ttu-id="3d841-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d841-107">Type</span></span>|<span data-ttu-id="3d841-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d841-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d841-109">usado</span><span class="sxs-lookup"><span data-stu-id="3d841-109">used</span></span>|<span data-ttu-id="3d841-110">Int32</span><span class="sxs-lookup"><span data-stu-id="3d841-110">Int32</span></span>| <span data-ttu-id="3d841-111">Quantidade usada da cota de diretório.</span><span class="sxs-lookup"><span data-stu-id="3d841-111">Used amount of the directory quota.</span></span> |
|<span data-ttu-id="3d841-112">total</span><span class="sxs-lookup"><span data-stu-id="3d841-112">total</span></span>|<span data-ttu-id="3d841-113">Int32</span><span class="sxs-lookup"><span data-stu-id="3d841-113">Int32</span></span>| <span data-ttu-id="3d841-114">Quantidade total da cota de diretório.</span><span class="sxs-lookup"><span data-stu-id="3d841-114">Total amount of the directory quota.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d841-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d841-115">JSON representation</span></span>

<span data-ttu-id="3d841-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d841-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySizeQuota"
}-->

```json
{
  "used": 123,
  "total": 1234
}
```
