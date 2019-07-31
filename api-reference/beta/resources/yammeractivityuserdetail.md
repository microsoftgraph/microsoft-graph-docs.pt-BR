---
title: tipo de recurso yammerActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 960945d72db1cc347228983b9567968dfcfc52d7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963784"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="13fc6-103">tipo de recurso yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="13fc6-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="13fc6-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13fc6-104">Properties</span></span>

| <span data-ttu-id="13fc6-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13fc6-105">Property</span></span>          | <span data-ttu-id="13fc6-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="13fc6-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="13fc6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="13fc6-107">reportRefreshDate</span></span> | <span data-ttu-id="13fc6-108">Data</span><span class="sxs-lookup"><span data-stu-id="13fc6-108">Date</span></span>              |
| <span data-ttu-id="13fc6-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="13fc6-109">userPrincipalName</span></span> | <span data-ttu-id="13fc6-110">String</span><span class="sxs-lookup"><span data-stu-id="13fc6-110">String</span></span>            |
| <span data-ttu-id="13fc6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="13fc6-111">displayName</span></span>       | <span data-ttu-id="13fc6-112">String</span><span class="sxs-lookup"><span data-stu-id="13fc6-112">String</span></span>            |
| <span data-ttu-id="13fc6-113">userState</span><span class="sxs-lookup"><span data-stu-id="13fc6-113">userState</span></span>         | <span data-ttu-id="13fc6-114">String</span><span class="sxs-lookup"><span data-stu-id="13fc6-114">String</span></span>            |
| <span data-ttu-id="13fc6-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="13fc6-115">stateChangeDate</span></span>   | <span data-ttu-id="13fc6-116">Data</span><span class="sxs-lookup"><span data-stu-id="13fc6-116">Date</span></span>              |
| <span data-ttu-id="13fc6-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="13fc6-117">lastActivityDate</span></span>  | <span data-ttu-id="13fc6-118">Data</span><span class="sxs-lookup"><span data-stu-id="13fc6-118">Date</span></span>              |
| <span data-ttu-id="13fc6-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="13fc6-119">postedCount</span></span>       | <span data-ttu-id="13fc6-120">Int64</span><span class="sxs-lookup"><span data-stu-id="13fc6-120">Int64</span></span>             |
| <span data-ttu-id="13fc6-121">readCount</span><span class="sxs-lookup"><span data-stu-id="13fc6-121">readCount</span></span>         | <span data-ttu-id="13fc6-122">Int64</span><span class="sxs-lookup"><span data-stu-id="13fc6-122">Int64</span></span>             |
| <span data-ttu-id="13fc6-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="13fc6-123">likedCount</span></span>        | <span data-ttu-id="13fc6-124">Int64</span><span class="sxs-lookup"><span data-stu-id="13fc6-124">Int64</span></span>             |
| <span data-ttu-id="13fc6-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="13fc6-125">assignedProducts</span></span>  | <span data-ttu-id="13fc6-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="13fc6-126">String collection</span></span> |
| <span data-ttu-id="13fc6-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="13fc6-127">reportPeriod</span></span>      | <span data-ttu-id="13fc6-128">String</span><span class="sxs-lookup"><span data-stu-id="13fc6-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="13fc6-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13fc6-129">JSON representation</span></span>

<span data-ttu-id="13fc6-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13fc6-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
