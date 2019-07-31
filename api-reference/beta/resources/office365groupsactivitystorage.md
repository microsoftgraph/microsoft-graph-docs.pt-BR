---
title: tipo de recurso office365GroupsActivityStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: a3168ad417f246017ba1018aca265ec0363c951e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009458"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="4b955-103">tipo de recurso office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="4b955-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4b955-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b955-104">Properties</span></span>

| <span data-ttu-id="4b955-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b955-105">Property</span></span>                  | <span data-ttu-id="4b955-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b955-106">Type</span></span>   | <span data-ttu-id="4b955-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b955-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="4b955-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4b955-108">reportRefreshDate</span></span>         | <span data-ttu-id="4b955-109">Data</span><span class="sxs-lookup"><span data-stu-id="4b955-109">Date</span></span>   | <span data-ttu-id="4b955-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4b955-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="4b955-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="4b955-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="4b955-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4b955-112">Int64</span></span>  | <span data-ttu-id="4b955-113">O armazenamento usado na caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="4b955-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="4b955-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="4b955-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="4b955-115">Int64</span><span class="sxs-lookup"><span data-stu-id="4b955-115">Int64</span></span>  | <span data-ttu-id="4b955-116">O armazenamento usado na biblioteca de documentos do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4b955-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="4b955-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="4b955-117">reportDate</span></span>                | <span data-ttu-id="4b955-118">Data</span><span class="sxs-lookup"><span data-stu-id="4b955-118">Date</span></span>   | <span data-ttu-id="4b955-119">A data do instantâneo para o armazenamento usado pelo Exchange e pelo SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4b955-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="4b955-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4b955-120">reportPeriod</span></span>              | <span data-ttu-id="4b955-121">String</span><span class="sxs-lookup"><span data-stu-id="4b955-121">String</span></span> | <span data-ttu-id="4b955-122">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="4b955-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="4b955-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b955-123">JSON representation</span></span>

<span data-ttu-id="4b955-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b955-124">The following is a JSON representation of the resource.</span></span>

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
