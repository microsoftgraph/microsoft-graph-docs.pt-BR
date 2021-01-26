---
title: Tipo de recurso emailActivitySummary
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9b3bb1d05c57874497d536de332f85b462335b5d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981869"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="8377f-103">Tipo de recurso emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="8377f-103">emailActivitySummary resource type</span></span>

<span data-ttu-id="8377f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8377f-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="8377f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8377f-105">Properties</span></span>

| <span data-ttu-id="8377f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8377f-106">Property</span></span>          | <span data-ttu-id="8377f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8377f-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="8377f-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8377f-108">reportRefreshDate</span></span> | <span data-ttu-id="8377f-109">Data</span><span class="sxs-lookup"><span data-stu-id="8377f-109">Date</span></span>   |
| <span data-ttu-id="8377f-110">send</span><span class="sxs-lookup"><span data-stu-id="8377f-110">send</span></span>              | <span data-ttu-id="8377f-111">Int64</span><span class="sxs-lookup"><span data-stu-id="8377f-111">Int64</span></span>  |
| <span data-ttu-id="8377f-112">receive</span><span class="sxs-lookup"><span data-stu-id="8377f-112">receive</span></span>           | <span data-ttu-id="8377f-113">Int64</span><span class="sxs-lookup"><span data-stu-id="8377f-113">Int64</span></span>  |
| <span data-ttu-id="8377f-114">leitura</span><span class="sxs-lookup"><span data-stu-id="8377f-114">read</span></span>              | <span data-ttu-id="8377f-115">Int64</span><span class="sxs-lookup"><span data-stu-id="8377f-115">Int64</span></span>  |
| <span data-ttu-id="8377f-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="8377f-116">reportDate</span></span>        | <span data-ttu-id="8377f-117">Data</span><span class="sxs-lookup"><span data-stu-id="8377f-117">Date</span></span>   |
| <span data-ttu-id="8377f-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8377f-118">reportPeriod</span></span>      | <span data-ttu-id="8377f-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8377f-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8377f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8377f-120">JSON representation</span></span>

<span data-ttu-id="8377f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8377f-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


