---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Cota
localization_priority: Normal
description: O recurso quota fornece detalhes sobre restrições de espaço em um recurso Drive.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 293daf950beb5cdf3cbd791a1e8bf0d4b92a220b
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864207"
---
# <a name="quota-resource-type"></a><span data-ttu-id="1c9a3-103">Tipo de recurso Quota</span><span class="sxs-lookup"><span data-stu-id="1c9a3-103">Quota resource type</span></span>

<span data-ttu-id="1c9a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c9a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c9a3-105">O recurso **quota** fornece detalhes sobre restrições de espaço em um recurso [Drive](drive.md).</span><span class="sxs-lookup"><span data-stu-id="1c9a3-105">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c9a3-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1c9a3-106">JSON representation</span></span>

<span data-ttu-id="1c9a3-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-107">Here is a JSON representation of the resource.</span></span>

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
  "storagePlanInformation": {
    "upgradeAvailable": true
  },
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a><span data-ttu-id="1c9a3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1c9a3-108">Properties</span></span>

| <span data-ttu-id="1c9a3-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="1c9a3-109">Property name</span></span> | <span data-ttu-id="1c9a3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c9a3-110">Type</span></span>   | <span data-ttu-id="1c9a3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c9a3-111">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="1c9a3-112">total</span><span class="sxs-lookup"><span data-stu-id="1c9a3-112">total</span></span>         | <span data-ttu-id="1c9a3-113">Int64</span><span class="sxs-lookup"><span data-stu-id="1c9a3-113">Int64</span></span>  | <span data-ttu-id="1c9a3-114">Total allowed storage space, in bytes.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-114">Total allowed storage space, in bytes.</span></span> <span data-ttu-id="1c9a3-115">Read-only.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-115">Read-only.</span></span>                           |
| <span data-ttu-id="1c9a3-116">used</span><span class="sxs-lookup"><span data-stu-id="1c9a3-116">used</span></span>          | <span data-ttu-id="1c9a3-117">Int64</span><span class="sxs-lookup"><span data-stu-id="1c9a3-117">Int64</span></span>  | <span data-ttu-id="1c9a3-118">Total space used, in bytes.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-118">Total space used, in bytes.</span></span> <span data-ttu-id="1c9a3-119">Read-only.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-119">Read-only.</span></span>                                      |
| <span data-ttu-id="1c9a3-120">remaining</span><span class="sxs-lookup"><span data-stu-id="1c9a3-120">remaining</span></span>     | <span data-ttu-id="1c9a3-121">Int64</span><span class="sxs-lookup"><span data-stu-id="1c9a3-121">Int64</span></span>  | <span data-ttu-id="1c9a3-122">Total space remaining before reaching the quota limit, in bytes.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-122">Total space remaining before reaching the quota limit, in bytes.</span></span> <span data-ttu-id="1c9a3-123">Read-only.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-123">Read-only.</span></span> |
| <span data-ttu-id="1c9a3-124">deleted</span><span class="sxs-lookup"><span data-stu-id="1c9a3-124">deleted</span></span>       | <span data-ttu-id="1c9a3-125">Int64</span><span class="sxs-lookup"><span data-stu-id="1c9a3-125">Int64</span></span>  | <span data-ttu-id="1c9a3-126">Total space consumed by files in the recycle bin, in bytes.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-126">Total space consumed by files in the recycle bin, in bytes.</span></span> <span data-ttu-id="1c9a3-127">Read-only.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-127">Read-only.</span></span>      |
| <span data-ttu-id="1c9a3-128">estado</span><span class="sxs-lookup"><span data-stu-id="1c9a3-128">state</span></span>         | <span data-ttu-id="1c9a3-129">string</span><span class="sxs-lookup"><span data-stu-id="1c9a3-129">string</span></span> | <span data-ttu-id="1c9a3-130">Enumeration value that indicates the state of the storage space.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-130">Enumeration value that indicates the state of the storage space.</span></span> <span data-ttu-id="1c9a3-131">Read-only.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-131">Read-only.</span></span> |
| <span data-ttu-id="1c9a3-132">Adicionadostorageplaninformation</span><span class="sxs-lookup"><span data-stu-id="1c9a3-132">storagePlanInformation</span></span>  | [<span data-ttu-id="1c9a3-133">Adicionadostorageplaninformation</span><span class="sxs-lookup"><span data-stu-id="1c9a3-133">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="1c9a3-134">Informações sobre os planos de cota de armazenamento da unidade.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-134">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="1c9a3-135">Somente no OneDrive pessoal.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-135">Only in Personal OneDrive.</span></span>|

## <a name="state-enumeration"></a><span data-ttu-id="1c9a3-136">Enumeração de Estado</span><span class="sxs-lookup"><span data-stu-id="1c9a3-136">State Enumeration</span></span>

| <span data-ttu-id="1c9a3-137">Valor</span><span class="sxs-lookup"><span data-stu-id="1c9a3-137">Value</span></span>      | <span data-ttu-id="1c9a3-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c9a3-138">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="1c9a3-139">A unidade tem bastante cota restante.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-139">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="1c9a3-140">A cota restante é inferior a 10% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-140">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="1c9a3-141">A cota restante é inferior a 1% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-141">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="1c9a3-142">The used quota has exceeded the total quota.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-142">The used quota has exceeded the total quota.</span></span> <span data-ttu-id="1c9a3-143">New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span><span class="sxs-lookup"><span data-stu-id="1c9a3-143">New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

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
