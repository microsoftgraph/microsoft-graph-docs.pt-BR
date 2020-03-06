---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Cota
localization_priority: Normal
description: O recurso quota fornece detalhes sobre restrições de espaço em um recurso Drive.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 53aad1392e66f610f85f30ae088dc6f8ca04df73
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533929"
---
# <a name="quota-resource-type"></a><span data-ttu-id="c3cf9-103">Tipo de recurso Quota</span><span class="sxs-lookup"><span data-stu-id="c3cf9-103">Quota resource type</span></span>

<span data-ttu-id="c3cf9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3cf9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c3cf9-105">O recurso **quota** fornece detalhes sobre restrições de espaço em um recurso [Drive](drive.md).</span><span class="sxs-lookup"><span data-stu-id="c3cf9-105">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3cf9-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3cf9-106">JSON representation</span></span>

<span data-ttu-id="c3cf9-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3cf9-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c3cf9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3cf9-108">Properties</span></span>

| <span data-ttu-id="c3cf9-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="c3cf9-109">Property name</span></span> | <span data-ttu-id="c3cf9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3cf9-110">Type</span></span>   | <span data-ttu-id="c3cf9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3cf9-111">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="c3cf9-112">total</span><span class="sxs-lookup"><span data-stu-id="c3cf9-112">total</span></span>         | <span data-ttu-id="c3cf9-113">Int64</span><span class="sxs-lookup"><span data-stu-id="c3cf9-113">Int64</span></span>  | <span data-ttu-id="c3cf9-p101">Espaço de armazenamento permitido total, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3cf9-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="c3cf9-116">used</span><span class="sxs-lookup"><span data-stu-id="c3cf9-116">used</span></span>          | <span data-ttu-id="c3cf9-117">Int64</span><span class="sxs-lookup"><span data-stu-id="c3cf9-117">Int64</span></span>  | <span data-ttu-id="c3cf9-p102">Espaço total, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3cf9-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="c3cf9-120">remaining</span><span class="sxs-lookup"><span data-stu-id="c3cf9-120">remaining</span></span>     | <span data-ttu-id="c3cf9-121">Int64</span><span class="sxs-lookup"><span data-stu-id="c3cf9-121">Int64</span></span>  | <span data-ttu-id="c3cf9-p103">Espaço total restante antes de atingir o limite de cota, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3cf9-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="c3cf9-124">deleted</span><span class="sxs-lookup"><span data-stu-id="c3cf9-124">deleted</span></span>       | <span data-ttu-id="c3cf9-125">Int64</span><span class="sxs-lookup"><span data-stu-id="c3cf9-125">Int64</span></span>  | <span data-ttu-id="c3cf9-p104">Espaço total consumido por arquivos na Lixeira, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3cf9-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="c3cf9-128">estado</span><span class="sxs-lookup"><span data-stu-id="c3cf9-128">state</span></span>         | <span data-ttu-id="c3cf9-129">string</span><span class="sxs-lookup"><span data-stu-id="c3cf9-129">string</span></span> | <span data-ttu-id="c3cf9-p105">Valor de enumeração que indica o estado do espaço de armazenamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3cf9-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |

## <a name="state-enumeration"></a><span data-ttu-id="c3cf9-132">Enumeração de Estado</span><span class="sxs-lookup"><span data-stu-id="c3cf9-132">State Enumeration</span></span>

| <span data-ttu-id="c3cf9-133">Valor</span><span class="sxs-lookup"><span data-stu-id="c3cf9-133">Value</span></span>      | <span data-ttu-id="c3cf9-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3cf9-134">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="c3cf9-135">A unidade tem bastante cota restante.</span><span class="sxs-lookup"><span data-stu-id="c3cf9-135">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="c3cf9-136">A cota restante é inferior a 10% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="c3cf9-136">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="c3cf9-137">A cota restante é inferior a 1% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="c3cf9-137">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="c3cf9-p106">A cota usada excedeu a cota total. Novos arquivos ou pastas não podem ser adicionadas à unidade até que ela esteja abaixo da quantidade total de cotas ou mais espaço de armazenamento seja adquirido.</span><span class="sxs-lookup"><span data-stu-id="c3cf9-p106">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

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
