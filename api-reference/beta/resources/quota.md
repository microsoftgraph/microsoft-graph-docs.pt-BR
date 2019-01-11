---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Cota
localization_priority: Normal
ms.openlocfilehash: a63b41253569dbb3d666a76b0a7495839ef61b12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882408"
---
# <a name="quota-resource-type"></a><span data-ttu-id="c8fdc-102">tipo de recurso de cota</span><span class="sxs-lookup"><span data-stu-id="c8fdc-102">quota resource type</span></span>

> <span data-ttu-id="c8fdc-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c8fdc-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8fdc-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c8fdc-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8fdc-105">O recurso de **cota** fornece detalhes sobre o espaço restringe em um recurso de [unidade](drive.md) .</span><span class="sxs-lookup"><span data-stu-id="c8fdc-105">The **quota** resource provides details about space constrains on a [drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8fdc-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8fdc-106">JSON representation</span></span>

<span data-ttu-id="c8fdc-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8fdc-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c8fdc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8fdc-108">Properties</span></span>

| <span data-ttu-id="c8fdc-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="c8fdc-109">Property name</span></span> | <span data-ttu-id="c8fdc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8fdc-110">Type</span></span>   | <span data-ttu-id="c8fdc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8fdc-111">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="c8fdc-112">total</span><span class="sxs-lookup"><span data-stu-id="c8fdc-112">total</span></span>         | <span data-ttu-id="c8fdc-113">Int64</span><span class="sxs-lookup"><span data-stu-id="c8fdc-113">Int64</span></span>  | <span data-ttu-id="c8fdc-p102">Espaço de armazenamento permitido total, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c8fdc-p102">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="c8fdc-116">used</span><span class="sxs-lookup"><span data-stu-id="c8fdc-116">used</span></span>          | <span data-ttu-id="c8fdc-117">Int64</span><span class="sxs-lookup"><span data-stu-id="c8fdc-117">Int64</span></span>  | <span data-ttu-id="c8fdc-p103">Espaço total, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c8fdc-p103">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="c8fdc-120">remaining</span><span class="sxs-lookup"><span data-stu-id="c8fdc-120">remaining</span></span>     | <span data-ttu-id="c8fdc-121">Int64</span><span class="sxs-lookup"><span data-stu-id="c8fdc-121">Int64</span></span>  | <span data-ttu-id="c8fdc-p104">Espaço total restante antes de atingir o limite de cota, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c8fdc-p104">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="c8fdc-124">deleted</span><span class="sxs-lookup"><span data-stu-id="c8fdc-124">deleted</span></span>       | <span data-ttu-id="c8fdc-125">Int64</span><span class="sxs-lookup"><span data-stu-id="c8fdc-125">Int64</span></span>  | <span data-ttu-id="c8fdc-p105">Espaço total consumido por arquivos na Lixeira, em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c8fdc-p105">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="c8fdc-128">estado</span><span class="sxs-lookup"><span data-stu-id="c8fdc-128">state</span></span>         | <span data-ttu-id="c8fdc-129">string</span><span class="sxs-lookup"><span data-stu-id="c8fdc-129">string</span></span> | <span data-ttu-id="c8fdc-p106">Valor de enumeração que indica o estado do espaço de armazenamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c8fdc-p106">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="c8fdc-132">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="c8fdc-132">storagePlanInformation</span></span>  | [<span data-ttu-id="c8fdc-133">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="c8fdc-133">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="c8fdc-134">Informações sobre planos de cota de armazenamento da unidade.</span><span class="sxs-lookup"><span data-stu-id="c8fdc-134">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="c8fdc-135">Somente no OneDrive pessoal.</span><span class="sxs-lookup"><span data-stu-id="c8fdc-135">Only in Personal OneDrive.</span></span>|

### <a name="state-enumeration-values"></a><span data-ttu-id="c8fdc-136">Valores de enumeração State</span><span class="sxs-lookup"><span data-stu-id="c8fdc-136">State enumeration values</span></span>

| <span data-ttu-id="c8fdc-137">Valor</span><span class="sxs-lookup"><span data-stu-id="c8fdc-137">Value</span></span>      | <span data-ttu-id="c8fdc-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8fdc-138">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="c8fdc-139">A unidade tem bastante cota restante.</span><span class="sxs-lookup"><span data-stu-id="c8fdc-139">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="c8fdc-140">A cota restante é inferior a 10% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="c8fdc-140">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="c8fdc-141">A cota restante é inferior a 1% do espaço de cota total.</span><span class="sxs-lookup"><span data-stu-id="c8fdc-141">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="c8fdc-p108">A cota usada excedeu a cota total. Novos arquivos ou pastas não podem ser adicionadas à unidade até que ela esteja abaixo da quantidade total de cotas ou mais espaço de armazenamento seja adquirido.</span><span class="sxs-lookup"><span data-stu-id="c8fdc-p108">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota"
} -->
