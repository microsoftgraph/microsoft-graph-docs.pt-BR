---
title: tipo de recurso sharePointActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a7dc324d821dca26ff1083f1e48c258e1955d72f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583974"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="71afe-103">tipo de recurso sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="71afe-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="71afe-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71afe-104">Properties</span></span>

| <span data-ttu-id="71afe-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71afe-105">Property</span></span>                  | <span data-ttu-id="71afe-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="71afe-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="71afe-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="71afe-107">reportRefreshDate</span></span>         | <span data-ttu-id="71afe-108">Data</span><span class="sxs-lookup"><span data-stu-id="71afe-108">Date</span></span>              |
| <span data-ttu-id="71afe-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="71afe-109">userPrincipalName</span></span>         | <span data-ttu-id="71afe-110">String</span><span class="sxs-lookup"><span data-stu-id="71afe-110">String</span></span>            |
| <span data-ttu-id="71afe-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="71afe-111">isDeleted</span></span>                 | <span data-ttu-id="71afe-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="71afe-112">Boolean</span></span>           |
| <span data-ttu-id="71afe-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="71afe-113">deletedDate</span></span>               | <span data-ttu-id="71afe-114">Data</span><span class="sxs-lookup"><span data-stu-id="71afe-114">Date</span></span>              |
| <span data-ttu-id="71afe-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="71afe-115">lastActivityDate</span></span>          | <span data-ttu-id="71afe-116">Data</span><span class="sxs-lookup"><span data-stu-id="71afe-116">Date</span></span>              |
| <span data-ttu-id="71afe-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="71afe-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="71afe-118">Int64</span><span class="sxs-lookup"><span data-stu-id="71afe-118">Int64</span></span>             |
| <span data-ttu-id="71afe-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="71afe-119">syncedFileCount</span></span>           | <span data-ttu-id="71afe-120">Int64</span><span class="sxs-lookup"><span data-stu-id="71afe-120">Int64</span></span>             |
| <span data-ttu-id="71afe-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="71afe-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="71afe-122">Int64</span><span class="sxs-lookup"><span data-stu-id="71afe-122">Int64</span></span>             |
| <span data-ttu-id="71afe-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="71afe-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="71afe-124">Int64</span><span class="sxs-lookup"><span data-stu-id="71afe-124">Int64</span></span>             |
| <span data-ttu-id="71afe-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="71afe-125">visitedPageCount</span></span>          | <span data-ttu-id="71afe-126">Int64</span><span class="sxs-lookup"><span data-stu-id="71afe-126">Int64</span></span>             |
| <span data-ttu-id="71afe-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="71afe-127">assignedProducts</span></span>          | <span data-ttu-id="71afe-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="71afe-128">String collection</span></span> |
| <span data-ttu-id="71afe-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="71afe-129">reportPeriod</span></span>              | <span data-ttu-id="71afe-130">String</span><span class="sxs-lookup"><span data-stu-id="71afe-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="71afe-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71afe-131">JSON representation</span></span>

<span data-ttu-id="71afe-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71afe-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "viewedOrEditedFileCount": 1024, 
  "syncedFileCount": 1024, 
  "sharedInternallyFileCount": 1024, 
  "sharedExternallyFileCount": 1024, 
  "visitedPageCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
