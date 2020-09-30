---
title: tipo de recurso directorySizeQuota
description: Representa a cota de diretório total usada e de uma empresa.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 8f5f172cb8f090b71b7e0fd3c89151668c167afd
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315595"
---
# <a name="directorysizequota-resource-type"></a><span data-ttu-id="6d209-103">tipo de recurso directorySizeQuota</span><span class="sxs-lookup"><span data-stu-id="6d209-103">directorySizeQuota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d209-104">Representa a cota de diretório total usada e de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="6d209-104">Represents a company's used and total directory quota.</span></span>

## <a name="properties"></a><span data-ttu-id="6d209-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d209-105">Properties</span></span>
| <span data-ttu-id="6d209-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d209-106">Property</span></span>   | <span data-ttu-id="6d209-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d209-107">Type</span></span>|<span data-ttu-id="6d209-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d209-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d209-109">usado</span><span class="sxs-lookup"><span data-stu-id="6d209-109">used</span></span>|<span data-ttu-id="6d209-110">Int32</span><span class="sxs-lookup"><span data-stu-id="6d209-110">Int32</span></span>| <span data-ttu-id="6d209-111">Valor usado da cota de diretório.</span><span class="sxs-lookup"><span data-stu-id="6d209-111">Used amount of the directory quota.</span></span> |
|<span data-ttu-id="6d209-112">total</span><span class="sxs-lookup"><span data-stu-id="6d209-112">total</span></span>|<span data-ttu-id="6d209-113">Int32</span><span class="sxs-lookup"><span data-stu-id="6d209-113">Int32</span></span>| <span data-ttu-id="6d209-114">Valor total da cota de diretório.</span><span class="sxs-lookup"><span data-stu-id="6d209-114">Total amount of the directory quota.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d209-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d209-115">JSON representation</span></span>

<span data-ttu-id="6d209-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d209-116">The following is a JSON representation of the resource.</span></span>

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
