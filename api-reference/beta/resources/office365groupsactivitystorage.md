---
title: tipo de recurso office365GroupsActivityStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0485fd95046bc83350983bc1333dba83c79139d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505547"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="f0c64-103">tipo de recurso office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="f0c64-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f0c64-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0c64-104">Properties</span></span>

| <span data-ttu-id="f0c64-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0c64-105">Property</span></span>                  | <span data-ttu-id="f0c64-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0c64-106">Type</span></span>   | <span data-ttu-id="f0c64-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0c64-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="f0c64-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f0c64-108">reportRefreshDate</span></span>         | <span data-ttu-id="f0c64-109">Data</span><span class="sxs-lookup"><span data-stu-id="f0c64-109">Date</span></span>   | <span data-ttu-id="f0c64-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f0c64-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="f0c64-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="f0c64-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="f0c64-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f0c64-112">Int64</span></span>  | <span data-ttu-id="f0c64-113">O armazenamento usado na caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="f0c64-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="f0c64-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="f0c64-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="f0c64-115">Int64</span><span class="sxs-lookup"><span data-stu-id="f0c64-115">Int64</span></span>  | <span data-ttu-id="f0c64-116">O armazenamento usado na biblioteca de documentos do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f0c64-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="f0c64-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="f0c64-117">reportDate</span></span>                | <span data-ttu-id="f0c64-118">Data</span><span class="sxs-lookup"><span data-stu-id="f0c64-118">Date</span></span>   | <span data-ttu-id="f0c64-119">A data do instantâneo para o armazenamento usado pelo Exchange e pelo SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f0c64-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="f0c64-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f0c64-120">reportPeriod</span></span>              | <span data-ttu-id="f0c64-121">String</span><span class="sxs-lookup"><span data-stu-id="f0c64-121">String</span></span> | <span data-ttu-id="f0c64-122">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="f0c64-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="f0c64-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0c64-123">JSON representation</span></span>

<span data-ttu-id="f0c64-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0c64-124">The following is a JSON representation of the resource.</span></span>

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
