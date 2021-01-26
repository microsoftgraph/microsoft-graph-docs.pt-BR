---
title: Tipo de recurso yammerActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 749076f407b49ff4fd408a095312ac49ea008bc1
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982394"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="88910-103">Tipo de recurso yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="88910-103">yammerActivityUserDetail resource type</span></span>

<span data-ttu-id="88910-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88910-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="88910-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88910-105">Properties</span></span>

| <span data-ttu-id="88910-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88910-106">Property</span></span>          | <span data-ttu-id="88910-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="88910-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="88910-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="88910-108">reportRefreshDate</span></span> | <span data-ttu-id="88910-109">Data</span><span class="sxs-lookup"><span data-stu-id="88910-109">Date</span></span>              |
| <span data-ttu-id="88910-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="88910-110">userPrincipalName</span></span> | <span data-ttu-id="88910-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88910-111">String</span></span>            |
| <span data-ttu-id="88910-112">displayName</span><span class="sxs-lookup"><span data-stu-id="88910-112">displayName</span></span>       | <span data-ttu-id="88910-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88910-113">String</span></span>            |
| <span data-ttu-id="88910-114">userState</span><span class="sxs-lookup"><span data-stu-id="88910-114">userState</span></span>         | <span data-ttu-id="88910-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88910-115">String</span></span>            |
| <span data-ttu-id="88910-116">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="88910-116">stateChangeDate</span></span>   | <span data-ttu-id="88910-117">Data</span><span class="sxs-lookup"><span data-stu-id="88910-117">Date</span></span>              |
| <span data-ttu-id="88910-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="88910-118">lastActivityDate</span></span>  | <span data-ttu-id="88910-119">Data</span><span class="sxs-lookup"><span data-stu-id="88910-119">Date</span></span>              |
| <span data-ttu-id="88910-120">postedCount</span><span class="sxs-lookup"><span data-stu-id="88910-120">postedCount</span></span>       | <span data-ttu-id="88910-121">Int64</span><span class="sxs-lookup"><span data-stu-id="88910-121">Int64</span></span>             |
| <span data-ttu-id="88910-122">readCount</span><span class="sxs-lookup"><span data-stu-id="88910-122">readCount</span></span>         | <span data-ttu-id="88910-123">Int64</span><span class="sxs-lookup"><span data-stu-id="88910-123">Int64</span></span>             |
| <span data-ttu-id="88910-124">likedCount</span><span class="sxs-lookup"><span data-stu-id="88910-124">likedCount</span></span>        | <span data-ttu-id="88910-125">Int64</span><span class="sxs-lookup"><span data-stu-id="88910-125">Int64</span></span>             |
| <span data-ttu-id="88910-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="88910-126">assignedProducts</span></span>  | <span data-ttu-id="88910-127">Coleção String</span><span class="sxs-lookup"><span data-stu-id="88910-127">String collection</span></span> |
| <span data-ttu-id="88910-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="88910-128">reportPeriod</span></span>      | <span data-ttu-id="88910-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88910-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="88910-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88910-130">JSON representation</span></span>

<span data-ttu-id="88910-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88910-131">The following is a JSON representation of the resource.</span></span>

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


