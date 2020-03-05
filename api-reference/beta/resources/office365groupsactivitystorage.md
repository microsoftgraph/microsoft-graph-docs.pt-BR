---
title: tipo de recurso office365GroupsActivityStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: ba81621a819bb38f2d5d48e118729fc4476b5806
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522425"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="64d7a-103">tipo de recurso office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="64d7a-103">office365GroupsActivityStorage resource type</span></span>

<span data-ttu-id="64d7a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="64d7a-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="64d7a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64d7a-105">Properties</span></span>

| <span data-ttu-id="64d7a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64d7a-106">Property</span></span>                  | <span data-ttu-id="64d7a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="64d7a-107">Type</span></span>   | <span data-ttu-id="64d7a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="64d7a-108">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="64d7a-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="64d7a-109">reportRefreshDate</span></span>         | <span data-ttu-id="64d7a-110">Data</span><span class="sxs-lookup"><span data-stu-id="64d7a-110">Date</span></span>   | <span data-ttu-id="64d7a-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="64d7a-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="64d7a-112">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="64d7a-112">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="64d7a-113">Int64</span><span class="sxs-lookup"><span data-stu-id="64d7a-113">Int64</span></span>  | <span data-ttu-id="64d7a-114">O armazenamento usado na caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="64d7a-114">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="64d7a-115">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="64d7a-115">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="64d7a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="64d7a-116">Int64</span></span>  | <span data-ttu-id="64d7a-117">O armazenamento usado na biblioteca de documentos do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="64d7a-117">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="64d7a-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="64d7a-118">reportDate</span></span>                | <span data-ttu-id="64d7a-119">Data</span><span class="sxs-lookup"><span data-stu-id="64d7a-119">Date</span></span>   | <span data-ttu-id="64d7a-120">A data do instantâneo para o armazenamento usado pelo Exchange e pelo SharePoint.</span><span class="sxs-lookup"><span data-stu-id="64d7a-120">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="64d7a-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="64d7a-121">reportPeriod</span></span>              | <span data-ttu-id="64d7a-122">String</span><span class="sxs-lookup"><span data-stu-id="64d7a-122">String</span></span> | <span data-ttu-id="64d7a-123">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="64d7a-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="64d7a-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64d7a-124">JSON representation</span></span>

<span data-ttu-id="64d7a-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64d7a-125">The following is a JSON representation of the resource.</span></span>

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
