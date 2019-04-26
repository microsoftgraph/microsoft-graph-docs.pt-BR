---
title: tipo de recurso oneDriveActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 29c9c8b723d4f87fa9858e26906878c973b37b09
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582245"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="70563-103">tipo de recurso oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="70563-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="70563-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70563-104">Properties</span></span>

| <span data-ttu-id="70563-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70563-105">Property</span></span>                  | <span data-ttu-id="70563-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="70563-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="70563-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="70563-107">reportRefreshDate</span></span>         | <span data-ttu-id="70563-108">Data</span><span class="sxs-lookup"><span data-stu-id="70563-108">Date</span></span>              |
| <span data-ttu-id="70563-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="70563-109">userPrincipalName</span></span>         | <span data-ttu-id="70563-110">String</span><span class="sxs-lookup"><span data-stu-id="70563-110">String</span></span>            |
| <span data-ttu-id="70563-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="70563-111">isDeleted</span></span>                 | <span data-ttu-id="70563-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="70563-112">Boolean</span></span>           |
| <span data-ttu-id="70563-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="70563-113">deletedDate</span></span>               | <span data-ttu-id="70563-114">Data</span><span class="sxs-lookup"><span data-stu-id="70563-114">Date</span></span>              |
| <span data-ttu-id="70563-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="70563-115">lastActivityDate</span></span>          | <span data-ttu-id="70563-116">Data</span><span class="sxs-lookup"><span data-stu-id="70563-116">Date</span></span>              |
| <span data-ttu-id="70563-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="70563-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="70563-118">Int64</span><span class="sxs-lookup"><span data-stu-id="70563-118">Int64</span></span>             |
| <span data-ttu-id="70563-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="70563-119">syncedFileCount</span></span>           | <span data-ttu-id="70563-120">Int64</span><span class="sxs-lookup"><span data-stu-id="70563-120">Int64</span></span>             |
| <span data-ttu-id="70563-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="70563-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="70563-122">Int64</span><span class="sxs-lookup"><span data-stu-id="70563-122">Int64</span></span>             |
| <span data-ttu-id="70563-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="70563-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="70563-124">Int64</span><span class="sxs-lookup"><span data-stu-id="70563-124">Int64</span></span>             |
| <span data-ttu-id="70563-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="70563-125">assignedProducts</span></span>          | <span data-ttu-id="70563-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="70563-126">String collection</span></span> |
| <span data-ttu-id="70563-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="70563-127">reportPeriod</span></span>              | <span data-ttu-id="70563-128">String</span><span class="sxs-lookup"><span data-stu-id="70563-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="70563-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70563-129">JSON representation</span></span>

<span data-ttu-id="70563-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70563-130">The following is a JSON representation of the resource.</span></span>

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
