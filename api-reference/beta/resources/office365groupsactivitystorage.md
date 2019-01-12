---
title: tipo de recurso de office365GroupsActivityStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 180e60a52b397f969aa10cee5bc27bba934ad1e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944450"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="f3ebd-103">tipo de recurso de office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="f3ebd-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f3ebd-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3ebd-104">Properties</span></span>

| <span data-ttu-id="f3ebd-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3ebd-105">Property</span></span>                  | <span data-ttu-id="f3ebd-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3ebd-106">Type</span></span>   | <span data-ttu-id="f3ebd-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3ebd-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="f3ebd-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f3ebd-108">reportRefreshDate</span></span>         | <span data-ttu-id="f3ebd-109">Data</span><span class="sxs-lookup"><span data-stu-id="f3ebd-109">Date</span></span>   | <span data-ttu-id="f3ebd-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f3ebd-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="f3ebd-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="f3ebd-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="f3ebd-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f3ebd-112">Int64</span></span>  | <span data-ttu-id="f3ebd-113">O armazenamento utilizado na caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="f3ebd-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="f3ebd-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="f3ebd-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="f3ebd-115">Int64</span><span class="sxs-lookup"><span data-stu-id="f3ebd-115">Int64</span></span>  | <span data-ttu-id="f3ebd-116">O armazenamento usado na biblioteca de documentos do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f3ebd-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="f3ebd-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="f3ebd-117">reportDate</span></span>                | <span data-ttu-id="f3ebd-118">Data</span><span class="sxs-lookup"><span data-stu-id="f3ebd-118">Date</span></span>   | <span data-ttu-id="f3ebd-119">A data de instantâneo do Exchange e SharePoint usou o armazenamento.</span><span class="sxs-lookup"><span data-stu-id="f3ebd-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="f3ebd-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f3ebd-120">reportPeriod</span></span>              | <span data-ttu-id="f3ebd-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3ebd-121">String</span></span> | <span data-ttu-id="f3ebd-122">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="f3ebd-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="f3ebd-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3ebd-123">JSON representation</span></span>

<span data-ttu-id="f3ebd-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3ebd-124">The following is a JSON representation of the resource.</span></span>

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
