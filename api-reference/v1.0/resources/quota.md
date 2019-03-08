---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Cota
localization_priority: Normal
ms.openlocfilehash: a9a5da54aeef3c9666c22c7a2f9bc0d92fc7a405
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481451"
---
# <a name="quota-resource-type"></a><span data-ttu-id="ccc5b-102">Tipo de recurso Quota</span><span class="sxs-lookup"><span data-stu-id="ccc5b-102">Quota resource type</span></span>

<span data-ttu-id="ccc5b-103">O recurso **quota** fornece detalhes sobre restrições de espaço em um recurso [Drive](drive.md).</span><span class="sxs-lookup"><span data-stu-id="ccc5b-103">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccc5b-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ccc5b-104">JSON representation</span></span>

<span data-ttu-id="ccc5b-105">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ccc5b-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ccc5b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ccc5b-106">Properties</span></span>

| <span data-ttu-id="ccc5b-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ccc5b-107">Property name</span></span> | <span data-ttu-id="ccc5b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccc5b-108">Type</span></span>   | <span data-ttu-id="ccc5b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccc5b-109">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="ccc5b-110">total</span><span class="sxs-lookup"><span data-stu-id="ccc5b-110">total</span></span>         | <span data-ttu-id="ccc5b-111">Int64</span><span class="sxs-lookup"><span data-stu-id="ccc5b-111">Int64</span></span>  | <span data-ttu-id="ccc5b-p101">Espaço de armazenamento permitido total, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc5b-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="ccc5b-114">used</span><span class="sxs-lookup"><span data-stu-id="ccc5b-114">used</span></span>          | <span data-ttu-id="ccc5b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ccc5b-115">Int64</span></span>  | <span data-ttu-id="ccc5b-p102">Espaço total, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc5b-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="ccc5b-118">remaining</span><span class="sxs-lookup"><span data-stu-id="ccc5b-118">remaining</span></span>     | <span data-ttu-id="ccc5b-119">Int64</span><span class="sxs-lookup"><span data-stu-id="ccc5b-119">Int64</span></span>  | <span data-ttu-id="ccc5b-p103">Espaço total restante antes de atingir o limite de cota, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc5b-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="ccc5b-122">deleted</span><span class="sxs-lookup"><span data-stu-id="ccc5b-122">deleted</span></span>       | <span data-ttu-id="ccc5b-123">Int64</span><span class="sxs-lookup"><span data-stu-id="ccc5b-123">Int64</span></span>  | <span data-ttu-id="ccc5b-p104">Espaço total consumido por arquivos na Lixeira, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc5b-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="ccc5b-126">estado</span><span class="sxs-lookup"><span data-stu-id="ccc5b-126">state</span></span>         | <span data-ttu-id="ccc5b-127">string</span><span class="sxs-lookup"><span data-stu-id="ccc5b-127">string</span></span> | <span data-ttu-id="ccc5b-p105">Valor de enumeração que indica o estado do espaço de armazenamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccc5b-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |

## <a name="state-enumeration"></a><span data-ttu-id="ccc5b-130">Enumeração de Estado</span><span class="sxs-lookup"><span data-stu-id="ccc5b-130">State Enumeration</span></span>

| <span data-ttu-id="ccc5b-131">Valor</span><span class="sxs-lookup"><span data-stu-id="ccc5b-131">Value</span></span>      | <span data-ttu-id="ccc5b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccc5b-132">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="ccc5b-133">A unidade tem bastante cota restante.</span><span class="sxs-lookup"><span data-stu-id="ccc5b-133">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="ccc5b-134">A cota restante é inferior a 10% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="ccc5b-134">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="ccc5b-135">A cota restante é inferior a 1% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="ccc5b-135">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="ccc5b-p106">A cota usada excedeu a cota total. Novos arquivos ou pastas não podem ser adicionadas à unidade até que ela esteja abaixo da quantidade total de cotas ou mais espaço de armazenamento seja adquirido.</span><span class="sxs-lookup"><span data-stu-id="ccc5b-p106">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

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
