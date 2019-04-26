---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Cota
localization_priority: Normal
ms.openlocfilehash: 7cafff3162c7cdc4435df1cde522b42998398693
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563270"
---
# <a name="quota-resource-type"></a><span data-ttu-id="87da1-102">tipo de recurso quota</span><span class="sxs-lookup"><span data-stu-id="87da1-102">quota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87da1-103">O recurso **quota** fornece detalhes sobre restrições de espaço em um recurso [drive](drive.md) .</span><span class="sxs-lookup"><span data-stu-id="87da1-103">The **quota** resource provides details about space constrains on a [drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="87da1-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87da1-104">JSON representation</span></span>

<span data-ttu-id="87da1-105">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87da1-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="87da1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87da1-106">Properties</span></span>

| <span data-ttu-id="87da1-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="87da1-107">Property name</span></span> | <span data-ttu-id="87da1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="87da1-108">Type</span></span>   | <span data-ttu-id="87da1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="87da1-109">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="87da1-110">total</span><span class="sxs-lookup"><span data-stu-id="87da1-110">total</span></span>         | <span data-ttu-id="87da1-111">Int64</span><span class="sxs-lookup"><span data-stu-id="87da1-111">Int64</span></span>  | <span data-ttu-id="87da1-p101">Espaço de armazenamento permitido total, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87da1-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="87da1-114">used</span><span class="sxs-lookup"><span data-stu-id="87da1-114">used</span></span>          | <span data-ttu-id="87da1-115">Int64</span><span class="sxs-lookup"><span data-stu-id="87da1-115">Int64</span></span>  | <span data-ttu-id="87da1-p102">Espaço total, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87da1-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="87da1-118">remaining</span><span class="sxs-lookup"><span data-stu-id="87da1-118">remaining</span></span>     | <span data-ttu-id="87da1-119">Int64</span><span class="sxs-lookup"><span data-stu-id="87da1-119">Int64</span></span>  | <span data-ttu-id="87da1-p103">Espaço total restante antes de atingir o limite de cota, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87da1-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="87da1-122">deleted</span><span class="sxs-lookup"><span data-stu-id="87da1-122">deleted</span></span>       | <span data-ttu-id="87da1-123">Int64</span><span class="sxs-lookup"><span data-stu-id="87da1-123">Int64</span></span>  | <span data-ttu-id="87da1-p104">Espaço total consumido por arquivos na Lixeira, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87da1-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="87da1-126">estado</span><span class="sxs-lookup"><span data-stu-id="87da1-126">state</span></span>         | <span data-ttu-id="87da1-127">string</span><span class="sxs-lookup"><span data-stu-id="87da1-127">string</span></span> | <span data-ttu-id="87da1-p105">Valor de enumeração que indica o estado do espaço de armazenamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87da1-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="87da1-130">Adicionadostorageplaninformation</span><span class="sxs-lookup"><span data-stu-id="87da1-130">storagePlanInformation</span></span>  | [<span data-ttu-id="87da1-131">Adicionadostorageplaninformation</span><span class="sxs-lookup"><span data-stu-id="87da1-131">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="87da1-132">Informações sobre os planos de cota de armazenamento da unidade.</span><span class="sxs-lookup"><span data-stu-id="87da1-132">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="87da1-133">Somente no OneDrive pessoal.</span><span class="sxs-lookup"><span data-stu-id="87da1-133">Only in Personal OneDrive.</span></span>|

### <a name="state-enumeration-values"></a><span data-ttu-id="87da1-134">Valores de enumeração de estado</span><span class="sxs-lookup"><span data-stu-id="87da1-134">State enumeration values</span></span>

| <span data-ttu-id="87da1-135">Valor</span><span class="sxs-lookup"><span data-stu-id="87da1-135">Value</span></span>      | <span data-ttu-id="87da1-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="87da1-136">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="87da1-137">A unidade tem bastante cota restante.</span><span class="sxs-lookup"><span data-stu-id="87da1-137">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="87da1-138">A cota restante é inferior a 10% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="87da1-138">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="87da1-139">A cota restante é inferior a 1% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="87da1-139">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="87da1-p107">A cota usada excedeu a cota total. Novos arquivos ou pastas não podem ser adicionadas à unidade até que ela esteja abaixo da quantidade total de cotas ou mais espaço de armazenamento seja adquirido.</span><span class="sxs-lookup"><span data-stu-id="87da1-p107">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

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
