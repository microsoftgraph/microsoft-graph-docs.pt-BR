---
title: tipo de recurso oneDriveActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 4021d1bdfb9322dbef75264ab88bb8b3a71c20e7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812145"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="2bdb3-103">tipo de recurso oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="2bdb3-103">oneDriveActivityUserDetail resource type</span></span>

<span data-ttu-id="2bdb3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bdb3-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="2bdb3-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2bdb3-105">Properties</span></span>

| <span data-ttu-id="2bdb3-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2bdb3-106">Property</span></span>                  | <span data-ttu-id="2bdb3-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bdb3-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="2bdb3-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2bdb3-108">reportRefreshDate</span></span>         | <span data-ttu-id="2bdb3-109">Data</span><span class="sxs-lookup"><span data-stu-id="2bdb3-109">Date</span></span>              |
| <span data-ttu-id="2bdb3-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2bdb3-110">userPrincipalName</span></span>         | <span data-ttu-id="2bdb3-111">String</span><span class="sxs-lookup"><span data-stu-id="2bdb3-111">String</span></span>            |
| <span data-ttu-id="2bdb3-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="2bdb3-112">isDeleted</span></span>                 | <span data-ttu-id="2bdb3-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="2bdb3-113">Boolean</span></span>           |
| <span data-ttu-id="2bdb3-114">deletedDate</span><span class="sxs-lookup"><span data-stu-id="2bdb3-114">deletedDate</span></span>               | <span data-ttu-id="2bdb3-115">Data</span><span class="sxs-lookup"><span data-stu-id="2bdb3-115">Date</span></span>              |
| <span data-ttu-id="2bdb3-116">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="2bdb3-116">lastActivityDate</span></span>          | <span data-ttu-id="2bdb3-117">Data</span><span class="sxs-lookup"><span data-stu-id="2bdb3-117">Date</span></span>              |
| <span data-ttu-id="2bdb3-118">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="2bdb3-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="2bdb3-119">Int64</span><span class="sxs-lookup"><span data-stu-id="2bdb3-119">Int64</span></span>             |
| <span data-ttu-id="2bdb3-120">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="2bdb3-120">syncedFileCount</span></span>           | <span data-ttu-id="2bdb3-121">Int64</span><span class="sxs-lookup"><span data-stu-id="2bdb3-121">Int64</span></span>             |
| <span data-ttu-id="2bdb3-122">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="2bdb3-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="2bdb3-123">Int64</span><span class="sxs-lookup"><span data-stu-id="2bdb3-123">Int64</span></span>             |
| <span data-ttu-id="2bdb3-124">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="2bdb3-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="2bdb3-125">Int64</span><span class="sxs-lookup"><span data-stu-id="2bdb3-125">Int64</span></span>             |
| <span data-ttu-id="2bdb3-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="2bdb3-126">assignedProducts</span></span>          | <span data-ttu-id="2bdb3-127">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bdb3-127">String collection</span></span> |
| <span data-ttu-id="2bdb3-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2bdb3-128">reportPeriod</span></span>              | <span data-ttu-id="2bdb3-129">String</span><span class="sxs-lookup"><span data-stu-id="2bdb3-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="2bdb3-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2bdb3-130">JSON representation</span></span>

<span data-ttu-id="2bdb3-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-131">The following is a JSON representation of the resource.</span></span>

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
