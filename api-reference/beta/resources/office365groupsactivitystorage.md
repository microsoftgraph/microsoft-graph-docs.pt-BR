---
title: tipo de recurso de office365GroupsActivityStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0485fd95046bc83350983bc1333dba83c79139d6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576378"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="43cff-103">tipo de recurso de office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="43cff-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="43cff-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43cff-104">Properties</span></span>

| <span data-ttu-id="43cff-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43cff-105">Property</span></span>                  | <span data-ttu-id="43cff-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="43cff-106">Type</span></span>   | <span data-ttu-id="43cff-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="43cff-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="43cff-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="43cff-108">reportRefreshDate</span></span>         | <span data-ttu-id="43cff-109">Data</span><span class="sxs-lookup"><span data-stu-id="43cff-109">Date</span></span>   | <span data-ttu-id="43cff-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="43cff-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="43cff-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="43cff-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="43cff-112">Int64</span><span class="sxs-lookup"><span data-stu-id="43cff-112">Int64</span></span>  | <span data-ttu-id="43cff-113">O armazenamento utilizado na caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="43cff-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="43cff-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="43cff-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="43cff-115">Int64</span><span class="sxs-lookup"><span data-stu-id="43cff-115">Int64</span></span>  | <span data-ttu-id="43cff-116">O armazenamento usado na biblioteca de documentos do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="43cff-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="43cff-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="43cff-117">reportDate</span></span>                | <span data-ttu-id="43cff-118">Data</span><span class="sxs-lookup"><span data-stu-id="43cff-118">Date</span></span>   | <span data-ttu-id="43cff-119">A data de instantâneo do Exchange e SharePoint usou o armazenamento.</span><span class="sxs-lookup"><span data-stu-id="43cff-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="43cff-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="43cff-120">reportPeriod</span></span>              | <span data-ttu-id="43cff-121">String</span><span class="sxs-lookup"><span data-stu-id="43cff-121">String</span></span> | <span data-ttu-id="43cff-122">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="43cff-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="43cff-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43cff-123">JSON representation</span></span>

<span data-ttu-id="43cff-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43cff-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailboxStorageUsedInBytes": 1024, 
  "siteStorageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
