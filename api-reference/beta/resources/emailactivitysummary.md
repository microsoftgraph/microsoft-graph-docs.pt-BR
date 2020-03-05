---
title: tipo de recurso emailActivitySummary
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: dd30bb496cb6591b3bde11d1c0c38b4099175891
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499586"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="573e6-103">tipo de recurso emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="573e6-103">emailActivitySummary resource type</span></span>

<span data-ttu-id="573e6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="573e6-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="573e6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="573e6-105">Properties</span></span>

| <span data-ttu-id="573e6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="573e6-106">Property</span></span>          | <span data-ttu-id="573e6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="573e6-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="573e6-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="573e6-108">reportRefreshDate</span></span> | <span data-ttu-id="573e6-109">Data</span><span class="sxs-lookup"><span data-stu-id="573e6-109">Date</span></span>   |
| <span data-ttu-id="573e6-110">Enviar</span><span class="sxs-lookup"><span data-stu-id="573e6-110">send</span></span>              | <span data-ttu-id="573e6-111">Int64</span><span class="sxs-lookup"><span data-stu-id="573e6-111">Int64</span></span>  |
| <span data-ttu-id="573e6-112">receber</span><span class="sxs-lookup"><span data-stu-id="573e6-112">receive</span></span>           | <span data-ttu-id="573e6-113">Int64</span><span class="sxs-lookup"><span data-stu-id="573e6-113">Int64</span></span>  |
| <span data-ttu-id="573e6-114">Saiba</span><span class="sxs-lookup"><span data-stu-id="573e6-114">read</span></span>              | <span data-ttu-id="573e6-115">Int64</span><span class="sxs-lookup"><span data-stu-id="573e6-115">Int64</span></span>  |
| <span data-ttu-id="573e6-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="573e6-116">reportDate</span></span>        | <span data-ttu-id="573e6-117">Data</span><span class="sxs-lookup"><span data-stu-id="573e6-117">Date</span></span>   |
| <span data-ttu-id="573e6-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="573e6-118">reportPeriod</span></span>      | <span data-ttu-id="573e6-119">String</span><span class="sxs-lookup"><span data-stu-id="573e6-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="573e6-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="573e6-120">JSON representation</span></span>

<span data-ttu-id="573e6-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="573e6-121">The following is a JSON representation of the resource.</span></span>

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
