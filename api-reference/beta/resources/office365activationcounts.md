---
title: tipo de recurso office365ActivationCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 1a45aa058a5186e87d11eed5199b51abf709879b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522488"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="20f3d-103">tipo de recurso office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="20f3d-103">office365ActivationCounts resource type</span></span>

<span data-ttu-id="20f3d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="20f3d-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="20f3d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20f3d-105">Properties</span></span>

| <span data-ttu-id="20f3d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20f3d-106">Property</span></span>          | <span data-ttu-id="20f3d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="20f3d-107">Type</span></span>   | <span data-ttu-id="20f3d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="20f3d-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="20f3d-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="20f3d-109">reportRefreshDate</span></span> | <span data-ttu-id="20f3d-110">Data</span><span class="sxs-lookup"><span data-stu-id="20f3d-110">Date</span></span>   | <span data-ttu-id="20f3d-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="20f3d-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="20f3d-112">ProductType</span><span class="sxs-lookup"><span data-stu-id="20f3d-112">productType</span></span>       | <span data-ttu-id="20f3d-113">String</span><span class="sxs-lookup"><span data-stu-id="20f3d-113">String</span></span> | <span data-ttu-id="20f3d-114">O tipo de produto, como "Office 365 ProPlus", "Project Client" ou "Visio Pro for Office 365".</span><span class="sxs-lookup"><span data-stu-id="20f3d-114">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="20f3d-115">Windows</span><span class="sxs-lookup"><span data-stu-id="20f3d-115">windows</span></span>           | <span data-ttu-id="20f3d-116">Int64</span><span class="sxs-lookup"><span data-stu-id="20f3d-116">Int64</span></span>  | <span data-ttu-id="20f3d-117">A contagem de ativação no Windows.</span><span class="sxs-lookup"><span data-stu-id="20f3d-117">The activation count on Windows.</span></span> <span data-ttu-id="20f3d-118">Esse número inclui todas as ativações em qualquer computador Windows.</span><span class="sxs-lookup"><span data-stu-id="20f3d-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="20f3d-119">mac</span><span class="sxs-lookup"><span data-stu-id="20f3d-119">mac</span></span>               | <span data-ttu-id="20f3d-120">Int64</span><span class="sxs-lookup"><span data-stu-id="20f3d-120">Int64</span></span>  | <span data-ttu-id="20f3d-121">A contagem de ativação no Mac OS.</span><span class="sxs-lookup"><span data-stu-id="20f3d-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="20f3d-122">Android</span><span class="sxs-lookup"><span data-stu-id="20f3d-122">android</span></span>           | <span data-ttu-id="20f3d-123">Int64</span><span class="sxs-lookup"><span data-stu-id="20f3d-123">Int64</span></span>  | <span data-ttu-id="20f3d-124">A contagem de ativação em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="20f3d-124">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="20f3d-125">emiti</span><span class="sxs-lookup"><span data-stu-id="20f3d-125">ios</span></span>               | <span data-ttu-id="20f3d-126">Int64</span><span class="sxs-lookup"><span data-stu-id="20f3d-126">Int64</span></span>  | <span data-ttu-id="20f3d-127">A contagem de ativação no iOS.</span><span class="sxs-lookup"><span data-stu-id="20f3d-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="20f3d-128">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="20f3d-128">windows10Mobile</span></span>   | <span data-ttu-id="20f3d-129">Int64</span><span class="sxs-lookup"><span data-stu-id="20f3d-129">Int64</span></span>  | <span data-ttu-id="20f3d-130">A contagem de ativação no Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="20f3d-130">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="20f3d-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20f3d-131">JSON representation</span></span>

<span data-ttu-id="20f3d-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20f3d-132">The following is a JSON representation of the resource.</span></span>

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
