---
title: tipo de recurso oneDriveActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 24f6b9da0fb4e4a141872bd00b423b799b880aa6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048859"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="bcc58-103">tipo de recurso oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="bcc58-103">oneDriveActivityUserDetail resource type</span></span>

<span data-ttu-id="bcc58-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcc58-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="bcc58-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bcc58-105">Properties</span></span>

| <span data-ttu-id="bcc58-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bcc58-106">Property</span></span>                  | <span data-ttu-id="bcc58-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcc58-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="bcc58-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bcc58-108">reportRefreshDate</span></span>         | <span data-ttu-id="bcc58-109">Data</span><span class="sxs-lookup"><span data-stu-id="bcc58-109">Date</span></span>              |
| <span data-ttu-id="bcc58-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bcc58-110">userPrincipalName</span></span>         | <span data-ttu-id="bcc58-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bcc58-111">String</span></span>            |
| <span data-ttu-id="bcc58-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="bcc58-112">isDeleted</span></span>                 | <span data-ttu-id="bcc58-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="bcc58-113">Boolean</span></span>           |
| <span data-ttu-id="bcc58-114">deletedDate</span><span class="sxs-lookup"><span data-stu-id="bcc58-114">deletedDate</span></span>               | <span data-ttu-id="bcc58-115">Data</span><span class="sxs-lookup"><span data-stu-id="bcc58-115">Date</span></span>              |
| <span data-ttu-id="bcc58-116">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="bcc58-116">lastActivityDate</span></span>          | <span data-ttu-id="bcc58-117">Data</span><span class="sxs-lookup"><span data-stu-id="bcc58-117">Date</span></span>              |
| <span data-ttu-id="bcc58-118">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="bcc58-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="bcc58-119">Int64</span><span class="sxs-lookup"><span data-stu-id="bcc58-119">Int64</span></span>             |
| <span data-ttu-id="bcc58-120">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="bcc58-120">syncedFileCount</span></span>           | <span data-ttu-id="bcc58-121">Int64</span><span class="sxs-lookup"><span data-stu-id="bcc58-121">Int64</span></span>             |
| <span data-ttu-id="bcc58-122">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="bcc58-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="bcc58-123">Int64</span><span class="sxs-lookup"><span data-stu-id="bcc58-123">Int64</span></span>             |
| <span data-ttu-id="bcc58-124">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="bcc58-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="bcc58-125">Int64</span><span class="sxs-lookup"><span data-stu-id="bcc58-125">Int64</span></span>             |
| <span data-ttu-id="bcc58-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="bcc58-126">assignedProducts</span></span>          | <span data-ttu-id="bcc58-127">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bcc58-127">String collection</span></span> |
| <span data-ttu-id="bcc58-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bcc58-128">reportPeriod</span></span>              | <span data-ttu-id="bcc58-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bcc58-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="bcc58-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bcc58-130">JSON representation</span></span>

<span data-ttu-id="bcc58-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bcc58-131">The following is a JSON representation of the resource.</span></span>

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


