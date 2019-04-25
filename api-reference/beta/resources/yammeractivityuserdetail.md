---
title: tipo de recurso yammerActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: eea520e6024bb050001461fb5ada5c90ea2b2125
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541182"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="696ec-103">tipo de recurso yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="696ec-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="696ec-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="696ec-104">Properties</span></span>

| <span data-ttu-id="696ec-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="696ec-105">Property</span></span>          | <span data-ttu-id="696ec-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="696ec-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="696ec-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="696ec-107">reportRefreshDate</span></span> | <span data-ttu-id="696ec-108">Data</span><span class="sxs-lookup"><span data-stu-id="696ec-108">Date</span></span>              |
| <span data-ttu-id="696ec-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="696ec-109">userPrincipalName</span></span> | <span data-ttu-id="696ec-110">String</span><span class="sxs-lookup"><span data-stu-id="696ec-110">String</span></span>            |
| <span data-ttu-id="696ec-111">displayName</span><span class="sxs-lookup"><span data-stu-id="696ec-111">displayName</span></span>       | <span data-ttu-id="696ec-112">String</span><span class="sxs-lookup"><span data-stu-id="696ec-112">String</span></span>            |
| <span data-ttu-id="696ec-113">userState</span><span class="sxs-lookup"><span data-stu-id="696ec-113">userState</span></span>         | <span data-ttu-id="696ec-114">String</span><span class="sxs-lookup"><span data-stu-id="696ec-114">String</span></span>            |
| <span data-ttu-id="696ec-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="696ec-115">stateChangeDate</span></span>   | <span data-ttu-id="696ec-116">Data</span><span class="sxs-lookup"><span data-stu-id="696ec-116">Date</span></span>              |
| <span data-ttu-id="696ec-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="696ec-117">lastActivityDate</span></span>  | <span data-ttu-id="696ec-118">Data</span><span class="sxs-lookup"><span data-stu-id="696ec-118">Date</span></span>              |
| <span data-ttu-id="696ec-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="696ec-119">postedCount</span></span>       | <span data-ttu-id="696ec-120">Int64</span><span class="sxs-lookup"><span data-stu-id="696ec-120">Int64</span></span>             |
| <span data-ttu-id="696ec-121">readCount</span><span class="sxs-lookup"><span data-stu-id="696ec-121">readCount</span></span>         | <span data-ttu-id="696ec-122">Int64</span><span class="sxs-lookup"><span data-stu-id="696ec-122">Int64</span></span>             |
| <span data-ttu-id="696ec-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="696ec-123">likedCount</span></span>        | <span data-ttu-id="696ec-124">Int64</span><span class="sxs-lookup"><span data-stu-id="696ec-124">Int64</span></span>             |
| <span data-ttu-id="696ec-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="696ec-125">assignedProducts</span></span>  | <span data-ttu-id="696ec-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="696ec-126">String collection</span></span> |
| <span data-ttu-id="696ec-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="696ec-127">reportPeriod</span></span>      | <span data-ttu-id="696ec-128">String</span><span class="sxs-lookup"><span data-stu-id="696ec-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="696ec-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="696ec-129">JSON representation</span></span>

<span data-ttu-id="696ec-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="696ec-130">The following is a JSON representation of the resource.</span></span>

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
