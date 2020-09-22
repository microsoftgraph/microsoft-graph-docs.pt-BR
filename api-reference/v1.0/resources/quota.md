---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Cota
localization_priority: Normal
description: O recurso quota fornece detalhes sobre restrições de espaço em um recurso Drive.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 833093569de75af450f325384f29d001e50da000
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037099"
---
# <a name="quota-resource-type"></a><span data-ttu-id="76010-103">Tipo de recurso Quota</span><span class="sxs-lookup"><span data-stu-id="76010-103">Quota resource type</span></span>

<span data-ttu-id="76010-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76010-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="76010-105">O recurso **quota** fornece detalhes sobre restrições de espaço em um recurso [Drive](drive.md).</span><span class="sxs-lookup"><span data-stu-id="76010-105">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76010-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76010-106">JSON representation</span></span>

<span data-ttu-id="76010-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="76010-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="76010-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76010-108">Properties</span></span>

| <span data-ttu-id="76010-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="76010-109">Property name</span></span> | <span data-ttu-id="76010-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="76010-110">Type</span></span>   | <span data-ttu-id="76010-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="76010-111">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="76010-112">total</span><span class="sxs-lookup"><span data-stu-id="76010-112">total</span></span>         | <span data-ttu-id="76010-113">Int64</span><span class="sxs-lookup"><span data-stu-id="76010-113">Int64</span></span>  | <span data-ttu-id="76010-p101">Espaço de armazenamento permitido total, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76010-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="76010-116">used</span><span class="sxs-lookup"><span data-stu-id="76010-116">used</span></span>          | <span data-ttu-id="76010-117">Int64</span><span class="sxs-lookup"><span data-stu-id="76010-117">Int64</span></span>  | <span data-ttu-id="76010-p102">Espaço total, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76010-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="76010-120">remaining</span><span class="sxs-lookup"><span data-stu-id="76010-120">remaining</span></span>     | <span data-ttu-id="76010-121">Int64</span><span class="sxs-lookup"><span data-stu-id="76010-121">Int64</span></span>  | <span data-ttu-id="76010-p103">Espaço total restante antes de atingir o limite de cota, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76010-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="76010-124">deleted</span><span class="sxs-lookup"><span data-stu-id="76010-124">deleted</span></span>       | <span data-ttu-id="76010-125">Int64</span><span class="sxs-lookup"><span data-stu-id="76010-125">Int64</span></span>  | <span data-ttu-id="76010-p104">Espaço total consumido por arquivos na Lixeira, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76010-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="76010-128">estado</span><span class="sxs-lookup"><span data-stu-id="76010-128">state</span></span>         | <span data-ttu-id="76010-129">string</span><span class="sxs-lookup"><span data-stu-id="76010-129">string</span></span> | <span data-ttu-id="76010-p105">Valor de enumeração que indica o estado do espaço de armazenamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76010-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="76010-132">Adicionadostorageplaninformation</span><span class="sxs-lookup"><span data-stu-id="76010-132">storagePlanInformation</span></span>  | [<span data-ttu-id="76010-133">Adicionadostorageplaninformation</span><span class="sxs-lookup"><span data-stu-id="76010-133">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="76010-134">Informações sobre os planos de cota de armazenamento da unidade.</span><span class="sxs-lookup"><span data-stu-id="76010-134">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="76010-135">Somente no OneDrive pessoal.</span><span class="sxs-lookup"><span data-stu-id="76010-135">Only in Personal OneDrive.</span></span>|

## <a name="state-enumeration"></a><span data-ttu-id="76010-136">Enumeração de Estado</span><span class="sxs-lookup"><span data-stu-id="76010-136">State Enumeration</span></span>

| <span data-ttu-id="76010-137">Valor</span><span class="sxs-lookup"><span data-stu-id="76010-137">Value</span></span>      | <span data-ttu-id="76010-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="76010-138">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="76010-139">A unidade tem bastante cota restante.</span><span class="sxs-lookup"><span data-stu-id="76010-139">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="76010-140">A cota restante é inferior a 10% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="76010-140">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="76010-141">A cota restante é inferior a 1% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="76010-141">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="76010-p107">A cota usada excedeu a cota total. Novos arquivos ou pastas não podem ser adicionadas à unidade até que ela esteja abaixo da quantidade total de cotas ou mais espaço de armazenamento seja adquirido.</span><span class="sxs-lookup"><span data-stu-id="76010-p107">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

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

