---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Cota
localization_priority: Normal
description: O recurso quota fornece detalhes sobre restrições de espaço em um recurso Drive.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ee93ddfe54e785ea8a8fa245ab3828c548928cc0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034955"
---
# <a name="quota-resource-type"></a><span data-ttu-id="1868e-103">Tipo de recurso Quota</span><span class="sxs-lookup"><span data-stu-id="1868e-103">Quota resource type</span></span>

<span data-ttu-id="1868e-104">O recurso **quota** fornece detalhes sobre restrições de espaço em um recurso [Drive](drive.md).</span><span class="sxs-lookup"><span data-stu-id="1868e-104">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1868e-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1868e-105">JSON representation</span></span>

<span data-ttu-id="1868e-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1868e-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a><span data-ttu-id="1868e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1868e-107">Properties</span></span>

| <span data-ttu-id="1868e-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="1868e-108">Property name</span></span> | <span data-ttu-id="1868e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1868e-109">Type</span></span>   | <span data-ttu-id="1868e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1868e-110">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="1868e-111">total</span><span class="sxs-lookup"><span data-stu-id="1868e-111">total</span></span>         | <span data-ttu-id="1868e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1868e-112">Int64</span></span>  | <span data-ttu-id="1868e-p101">Espaço de armazenamento permitido total, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1868e-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="1868e-115">used</span><span class="sxs-lookup"><span data-stu-id="1868e-115">used</span></span>          | <span data-ttu-id="1868e-116">Int64</span><span class="sxs-lookup"><span data-stu-id="1868e-116">Int64</span></span>  | <span data-ttu-id="1868e-p102">Espaço total, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1868e-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="1868e-119">remaining</span><span class="sxs-lookup"><span data-stu-id="1868e-119">remaining</span></span>     | <span data-ttu-id="1868e-120">Int64</span><span class="sxs-lookup"><span data-stu-id="1868e-120">Int64</span></span>  | <span data-ttu-id="1868e-p103">Espaço total restante antes de atingir o limite de cota, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1868e-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="1868e-123">deleted</span><span class="sxs-lookup"><span data-stu-id="1868e-123">deleted</span></span>       | <span data-ttu-id="1868e-124">Int64</span><span class="sxs-lookup"><span data-stu-id="1868e-124">Int64</span></span>  | <span data-ttu-id="1868e-p104">Espaço total consumido por arquivos na Lixeira, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1868e-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="1868e-127">estado</span><span class="sxs-lookup"><span data-stu-id="1868e-127">state</span></span>         | <span data-ttu-id="1868e-128">string</span><span class="sxs-lookup"><span data-stu-id="1868e-128">string</span></span> | <span data-ttu-id="1868e-p105">Valor de enumeração que indica o estado do espaço de armazenamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1868e-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |

## <a name="state-enumeration"></a><span data-ttu-id="1868e-131">Enumeração de Estado</span><span class="sxs-lookup"><span data-stu-id="1868e-131">State Enumeration</span></span>

| <span data-ttu-id="1868e-132">Valor</span><span class="sxs-lookup"><span data-stu-id="1868e-132">Value</span></span>      | <span data-ttu-id="1868e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1868e-133">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="1868e-134">A unidade tem bastante cota restante.</span><span class="sxs-lookup"><span data-stu-id="1868e-134">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="1868e-135">A cota restante é inferior a 10% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="1868e-135">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="1868e-136">A cota restante é inferior a 1% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="1868e-136">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="1868e-p106">A cota usada excedeu a cota total. Novos arquivos ou pastas não podem ser adicionadas à unidade até que ela esteja abaixo da quantidade total de cotas ou mais espaço de armazenamento seja adquirido.</span><span class="sxs-lookup"><span data-stu-id="1868e-p106">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/quota.md:
      Found potential enums in resource example that weren't defined in a table:(normal, nearing,critical,exceeded) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Quota"
} -->
