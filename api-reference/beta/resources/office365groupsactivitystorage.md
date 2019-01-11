---
title: tipo de recurso de office365GroupsActivityStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 9824d3d172a8578f8a25a049c2d0d3b407bbc47e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862248"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="050ad-103">tipo de recurso de office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="050ad-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="050ad-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="050ad-104">Properties</span></span>

| <span data-ttu-id="050ad-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="050ad-105">Property</span></span>                  | <span data-ttu-id="050ad-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="050ad-106">Type</span></span>   | <span data-ttu-id="050ad-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="050ad-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="050ad-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="050ad-108">reportRefreshDate</span></span>         | <span data-ttu-id="050ad-109">Data</span><span class="sxs-lookup"><span data-stu-id="050ad-109">Date</span></span>   | <span data-ttu-id="050ad-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="050ad-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="050ad-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="050ad-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="050ad-112">Int64</span><span class="sxs-lookup"><span data-stu-id="050ad-112">Int64</span></span>  | <span data-ttu-id="050ad-113">O armazenamento utilizado na caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="050ad-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="050ad-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="050ad-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="050ad-115">Int64</span><span class="sxs-lookup"><span data-stu-id="050ad-115">Int64</span></span>  | <span data-ttu-id="050ad-116">O armazenamento usado na biblioteca de documentos do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="050ad-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="050ad-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="050ad-117">reportDate</span></span>                | <span data-ttu-id="050ad-118">Data</span><span class="sxs-lookup"><span data-stu-id="050ad-118">Date</span></span>   | <span data-ttu-id="050ad-119">A data de instantâneo do Exchange e SharePoint usou o armazenamento.</span><span class="sxs-lookup"><span data-stu-id="050ad-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="050ad-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="050ad-120">reportPeriod</span></span>              | <span data-ttu-id="050ad-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="050ad-121">String</span></span> | <span data-ttu-id="050ad-122">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="050ad-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="050ad-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="050ad-123">JSON representation</span></span>

<span data-ttu-id="050ad-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="050ad-124">The following is a JSON representation of the resource.</span></span>

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
