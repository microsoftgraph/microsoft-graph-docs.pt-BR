---
title: tipo de recurso de oneDriveActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 679ec9b8452d388fe311e67d88bcfffd6fe73d93
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035852"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="2eb5c-103">tipo de recurso de oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="2eb5c-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2eb5c-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2eb5c-104">Properties</span></span>

| <span data-ttu-id="2eb5c-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2eb5c-105">Property</span></span>                  | <span data-ttu-id="2eb5c-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="2eb5c-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="2eb5c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2eb5c-107">reportRefreshDate</span></span>         | <span data-ttu-id="2eb5c-108">Data</span><span class="sxs-lookup"><span data-stu-id="2eb5c-108">Date</span></span>              |
| <span data-ttu-id="2eb5c-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2eb5c-109">userPrincipalName</span></span>         | <span data-ttu-id="2eb5c-110">String</span><span class="sxs-lookup"><span data-stu-id="2eb5c-110">String</span></span>            |
| <span data-ttu-id="2eb5c-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="2eb5c-111">isDeleted</span></span>                 | <span data-ttu-id="2eb5c-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="2eb5c-112">Boolean</span></span>           |
| <span data-ttu-id="2eb5c-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="2eb5c-113">deletedDate</span></span>               | <span data-ttu-id="2eb5c-114">Data</span><span class="sxs-lookup"><span data-stu-id="2eb5c-114">Date</span></span>              |
| <span data-ttu-id="2eb5c-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="2eb5c-115">lastActivityDate</span></span>          | <span data-ttu-id="2eb5c-116">Data</span><span class="sxs-lookup"><span data-stu-id="2eb5c-116">Date</span></span>              |
| <span data-ttu-id="2eb5c-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="2eb5c-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="2eb5c-118">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb5c-118">Int64</span></span>             |
| <span data-ttu-id="2eb5c-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="2eb5c-119">syncedFileCount</span></span>           | <span data-ttu-id="2eb5c-120">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb5c-120">Int64</span></span>             |
| <span data-ttu-id="2eb5c-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="2eb5c-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="2eb5c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb5c-122">Int64</span></span>             |
| <span data-ttu-id="2eb5c-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="2eb5c-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="2eb5c-124">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb5c-124">Int64</span></span>             |
| <span data-ttu-id="2eb5c-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="2eb5c-125">assignedProducts</span></span>          | <span data-ttu-id="2eb5c-126">String collection</span><span class="sxs-lookup"><span data-stu-id="2eb5c-126">String collection</span></span> |
| <span data-ttu-id="2eb5c-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2eb5c-127">reportPeriod</span></span>              | <span data-ttu-id="2eb5c-128">String</span><span class="sxs-lookup"><span data-stu-id="2eb5c-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="2eb5c-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2eb5c-129">JSON representation</span></span>

<span data-ttu-id="2eb5c-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2eb5c-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
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
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
