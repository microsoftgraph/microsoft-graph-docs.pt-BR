---
title: tipo de recurso office365GroupsActivityStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 0b14e6981a193ad1698303d2762d0321de430b73
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092388"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="58a98-103">tipo de recurso office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="58a98-103">office365GroupsActivityStorage resource type</span></span>

<span data-ttu-id="58a98-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58a98-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="58a98-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58a98-105">Properties</span></span>

| <span data-ttu-id="58a98-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58a98-106">Property</span></span>                  | <span data-ttu-id="58a98-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="58a98-107">Type</span></span>   | <span data-ttu-id="58a98-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="58a98-108">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="58a98-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="58a98-109">reportRefreshDate</span></span>         | <span data-ttu-id="58a98-110">Data</span><span class="sxs-lookup"><span data-stu-id="58a98-110">Date</span></span>   | <span data-ttu-id="58a98-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="58a98-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="58a98-112">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="58a98-112">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="58a98-113">Int64</span><span class="sxs-lookup"><span data-stu-id="58a98-113">Int64</span></span>  | <span data-ttu-id="58a98-114">O armazenamento usado na caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="58a98-114">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="58a98-115">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="58a98-115">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="58a98-116">Int64</span><span class="sxs-lookup"><span data-stu-id="58a98-116">Int64</span></span>  | <span data-ttu-id="58a98-117">O armazenamento usado na biblioteca de documentos do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="58a98-117">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="58a98-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="58a98-118">reportDate</span></span>                | <span data-ttu-id="58a98-119">Data</span><span class="sxs-lookup"><span data-stu-id="58a98-119">Date</span></span>   | <span data-ttu-id="58a98-120">A data do instantâneo para o armazenamento usado pelo Exchange e pelo SharePoint.</span><span class="sxs-lookup"><span data-stu-id="58a98-120">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="58a98-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="58a98-121">reportPeriod</span></span>              | <span data-ttu-id="58a98-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58a98-122">String</span></span> | <span data-ttu-id="58a98-123">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="58a98-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="58a98-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58a98-124">JSON representation</span></span>

<span data-ttu-id="58a98-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="58a98-125">The following is a JSON representation of the resource.</span></span>

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


