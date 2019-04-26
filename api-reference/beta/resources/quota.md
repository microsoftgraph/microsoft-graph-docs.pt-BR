---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Cota
localization_priority: Normal
ms.openlocfilehash: b7357eba3cdf7a9f01c983016c6890232c3d5bbf
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344048"
---
# <a name="quota-resource-type"></a><span data-ttu-id="25088-102">tipo de recurso quota</span><span class="sxs-lookup"><span data-stu-id="25088-102">quota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25088-103">O recurso **quota** fornece detalhes sobre restrições de espaço em um recurso [drive](drive.md) .</span><span class="sxs-lookup"><span data-stu-id="25088-103">The **quota** resource provides details about space constrains on a [drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="25088-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25088-104">JSON representation</span></span>

<span data-ttu-id="25088-105">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25088-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="25088-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25088-106">Properties</span></span>

| <span data-ttu-id="25088-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="25088-107">Property name</span></span> | <span data-ttu-id="25088-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="25088-108">Type</span></span>   | <span data-ttu-id="25088-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="25088-109">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="25088-110">total</span><span class="sxs-lookup"><span data-stu-id="25088-110">total</span></span>         | <span data-ttu-id="25088-111">Int64</span><span class="sxs-lookup"><span data-stu-id="25088-111">Int64</span></span>  | <span data-ttu-id="25088-p101">Espaço de armazenamento permitido total, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25088-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="25088-114">used</span><span class="sxs-lookup"><span data-stu-id="25088-114">used</span></span>          | <span data-ttu-id="25088-115">Int64</span><span class="sxs-lookup"><span data-stu-id="25088-115">Int64</span></span>  | <span data-ttu-id="25088-p102">Espaço total, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25088-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="25088-118">remaining</span><span class="sxs-lookup"><span data-stu-id="25088-118">remaining</span></span>     | <span data-ttu-id="25088-119">Int64</span><span class="sxs-lookup"><span data-stu-id="25088-119">Int64</span></span>  | <span data-ttu-id="25088-p103">Espaço total restante antes de atingir o limite de cota, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25088-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="25088-122">deleted</span><span class="sxs-lookup"><span data-stu-id="25088-122">deleted</span></span>       | <span data-ttu-id="25088-123">Int64</span><span class="sxs-lookup"><span data-stu-id="25088-123">Int64</span></span>  | <span data-ttu-id="25088-p104">Espaço total consumido por arquivos na Lixeira, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25088-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="25088-126">estado</span><span class="sxs-lookup"><span data-stu-id="25088-126">state</span></span>         | <span data-ttu-id="25088-127">string</span><span class="sxs-lookup"><span data-stu-id="25088-127">string</span></span> | <span data-ttu-id="25088-p105">Valor de enumeração que indica o estado do espaço de armazenamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25088-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="25088-130">Adicionadostorageplaninformation</span><span class="sxs-lookup"><span data-stu-id="25088-130">storagePlanInformation</span></span>  | [<span data-ttu-id="25088-131">Adicionadostorageplaninformation</span><span class="sxs-lookup"><span data-stu-id="25088-131">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="25088-132">Informações sobre os planos de cota de armazenamento da unidade.</span><span class="sxs-lookup"><span data-stu-id="25088-132">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="25088-133">Somente no OneDrive pessoal.</span><span class="sxs-lookup"><span data-stu-id="25088-133">Only in Personal OneDrive.</span></span>|

### <a name="state-enumeration-values"></a><span data-ttu-id="25088-134">Valores de enumeração de estado</span><span class="sxs-lookup"><span data-stu-id="25088-134">State enumeration values</span></span>

| <span data-ttu-id="25088-135">Valor</span><span class="sxs-lookup"><span data-stu-id="25088-135">Value</span></span>      | <span data-ttu-id="25088-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="25088-136">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="25088-137">A unidade tem bastante cota restante.</span><span class="sxs-lookup"><span data-stu-id="25088-137">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="25088-138">A cota restante é inferior a 10% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="25088-138">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="25088-139">A cota restante é inferior a 1% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="25088-139">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="25088-p107">A cota usada excedeu a cota total. Novos arquivos ou pastas não podem ser adicionadas à unidade até que ela esteja abaixo da quantidade total de cotas ou mais espaço de armazenamento seja adquirido.</span><span class="sxs-lookup"><span data-stu-id="25088-p107">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota",
  "suppressions": []
}
-->
