---
title: Tipo de recurso office365GroupsActivityStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 7ac9ca260e4723f7c4aeca8e15f837d4cd57b7c4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982177"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="83e89-103">Tipo de recurso office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="83e89-103">office365GroupsActivityStorage resource type</span></span>

<span data-ttu-id="83e89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83e89-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="83e89-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83e89-105">Properties</span></span>

| <span data-ttu-id="83e89-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83e89-106">Property</span></span>                  | <span data-ttu-id="83e89-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="83e89-107">Type</span></span>   | <span data-ttu-id="83e89-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="83e89-108">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="83e89-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="83e89-109">reportRefreshDate</span></span>         | <span data-ttu-id="83e89-110">Data</span><span class="sxs-lookup"><span data-stu-id="83e89-110">Date</span></span>   | <span data-ttu-id="83e89-111">A data mais recente do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="83e89-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="83e89-112">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="83e89-112">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="83e89-113">Int64</span><span class="sxs-lookup"><span data-stu-id="83e89-113">Int64</span></span>  | <span data-ttu-id="83e89-114">O armazenamento usado na caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="83e89-114">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="83e89-115">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="83e89-115">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="83e89-116">Int64</span><span class="sxs-lookup"><span data-stu-id="83e89-116">Int64</span></span>  | <span data-ttu-id="83e89-117">O armazenamento usado na biblioteca de documentos do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="83e89-117">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="83e89-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="83e89-118">reportDate</span></span>                | <span data-ttu-id="83e89-119">Data</span><span class="sxs-lookup"><span data-stu-id="83e89-119">Date</span></span>   | <span data-ttu-id="83e89-120">A data do instantâneo do armazenamento usado pelo Exchange e pelo SharePoint.</span><span class="sxs-lookup"><span data-stu-id="83e89-120">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="83e89-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="83e89-121">reportPeriod</span></span>              | <span data-ttu-id="83e89-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83e89-122">String</span></span> | <span data-ttu-id="83e89-123">O número de dias que o relatório abrange.</span><span class="sxs-lookup"><span data-stu-id="83e89-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="83e89-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83e89-124">JSON representation</span></span>

<span data-ttu-id="83e89-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83e89-125">The following is a JSON representation of the resource.</span></span>

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


