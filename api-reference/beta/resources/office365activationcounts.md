---
title: tipo de recurso office365ActivationCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 1e514eb538b1edc4d9681b9937fe8cfeecc40b23
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896886"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="d94c8-103">tipo de recurso office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="d94c8-103">office365ActivationCounts resource type</span></span>

<span data-ttu-id="d94c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d94c8-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d94c8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d94c8-105">Properties</span></span>

| <span data-ttu-id="d94c8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d94c8-106">Property</span></span>          | <span data-ttu-id="d94c8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d94c8-107">Type</span></span>   | <span data-ttu-id="d94c8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d94c8-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="d94c8-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d94c8-109">reportRefreshDate</span></span> | <span data-ttu-id="d94c8-110">Data</span><span class="sxs-lookup"><span data-stu-id="d94c8-110">Date</span></span>   | <span data-ttu-id="d94c8-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d94c8-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="d94c8-112">ProductType</span><span class="sxs-lookup"><span data-stu-id="d94c8-112">productType</span></span>       | <span data-ttu-id="d94c8-113">String</span><span class="sxs-lookup"><span data-stu-id="d94c8-113">String</span></span> | <span data-ttu-id="d94c8-114">O tipo de produto, como "Microsoft 365 ProPlus" ou "Project Client".</span><span class="sxs-lookup"><span data-stu-id="d94c8-114">The product type, such as "Microsoft 365 ProPlus" or "Project Client".</span></span> |
| <span data-ttu-id="d94c8-115">Windows</span><span class="sxs-lookup"><span data-stu-id="d94c8-115">windows</span></span>           | <span data-ttu-id="d94c8-116">Int64</span><span class="sxs-lookup"><span data-stu-id="d94c8-116">Int64</span></span>  | <span data-ttu-id="d94c8-117">A contagem de ativação no Windows.</span><span class="sxs-lookup"><span data-stu-id="d94c8-117">The activation count on Windows.</span></span> <span data-ttu-id="d94c8-118">Esse número inclui todas as ativações em qualquer computador Windows.</span><span class="sxs-lookup"><span data-stu-id="d94c8-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="d94c8-119">mac</span><span class="sxs-lookup"><span data-stu-id="d94c8-119">mac</span></span>               | <span data-ttu-id="d94c8-120">Int64</span><span class="sxs-lookup"><span data-stu-id="d94c8-120">Int64</span></span>  | <span data-ttu-id="d94c8-121">A contagem de ativação no Mac OS.</span><span class="sxs-lookup"><span data-stu-id="d94c8-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="d94c8-122">Android</span><span class="sxs-lookup"><span data-stu-id="d94c8-122">android</span></span>           | <span data-ttu-id="d94c8-123">Int64</span><span class="sxs-lookup"><span data-stu-id="d94c8-123">Int64</span></span>  | <span data-ttu-id="d94c8-124">A contagem de ativação em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="d94c8-124">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="d94c8-125">emiti</span><span class="sxs-lookup"><span data-stu-id="d94c8-125">ios</span></span>               | <span data-ttu-id="d94c8-126">Int64</span><span class="sxs-lookup"><span data-stu-id="d94c8-126">Int64</span></span>  | <span data-ttu-id="d94c8-127">A contagem de ativação no iOS.</span><span class="sxs-lookup"><span data-stu-id="d94c8-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="d94c8-128">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="d94c8-128">windows10Mobile</span></span>   | <span data-ttu-id="d94c8-129">Int64</span><span class="sxs-lookup"><span data-stu-id="d94c8-129">Int64</span></span>  | <span data-ttu-id="d94c8-130">A contagem de ativação no Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="d94c8-130">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d94c8-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d94c8-131">JSON representation</span></span>

<span data-ttu-id="d94c8-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d94c8-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "windows": 1024, 
  "mac": 1024, 
  "android": 1024, 
  "ios": 1024, 
  "windows10Mobile": 1024
}
```
