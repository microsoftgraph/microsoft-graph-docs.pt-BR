---
title: tipo de recurso office365ActivationCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: d396ee84e4af6606cfde3e5fc17ef02c0a9594f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966577"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="fec7a-103">tipo de recurso office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="fec7a-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fec7a-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fec7a-104">Properties</span></span>

| <span data-ttu-id="fec7a-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fec7a-105">Property</span></span>          | <span data-ttu-id="fec7a-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="fec7a-106">Type</span></span>   | <span data-ttu-id="fec7a-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="fec7a-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="fec7a-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fec7a-108">reportRefreshDate</span></span> | <span data-ttu-id="fec7a-109">Data</span><span class="sxs-lookup"><span data-stu-id="fec7a-109">Date</span></span>   | <span data-ttu-id="fec7a-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="fec7a-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="fec7a-111">ProductType</span><span class="sxs-lookup"><span data-stu-id="fec7a-111">productType</span></span>       | <span data-ttu-id="fec7a-112">String</span><span class="sxs-lookup"><span data-stu-id="fec7a-112">String</span></span> | <span data-ttu-id="fec7a-113">O tipo de produto, como "Office 365 ProPlus", "Project Client" ou "Visio Pro for Office 365".</span><span class="sxs-lookup"><span data-stu-id="fec7a-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="fec7a-114">Windows</span><span class="sxs-lookup"><span data-stu-id="fec7a-114">windows</span></span>           | <span data-ttu-id="fec7a-115">Int64</span><span class="sxs-lookup"><span data-stu-id="fec7a-115">Int64</span></span>  | <span data-ttu-id="fec7a-116">A contagem de ativação no Windows.</span><span class="sxs-lookup"><span data-stu-id="fec7a-116">The activation count on Windows.</span></span> <span data-ttu-id="fec7a-117">Esse número inclui todas as ativações em qualquer computador Windows.</span><span class="sxs-lookup"><span data-stu-id="fec7a-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="fec7a-118">mac</span><span class="sxs-lookup"><span data-stu-id="fec7a-118">mac</span></span>               | <span data-ttu-id="fec7a-119">Int64</span><span class="sxs-lookup"><span data-stu-id="fec7a-119">Int64</span></span>  | <span data-ttu-id="fec7a-120">A contagem de ativação no Mac OS.</span><span class="sxs-lookup"><span data-stu-id="fec7a-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="fec7a-121">Android</span><span class="sxs-lookup"><span data-stu-id="fec7a-121">android</span></span>           | <span data-ttu-id="fec7a-122">Int64</span><span class="sxs-lookup"><span data-stu-id="fec7a-122">Int64</span></span>  | <span data-ttu-id="fec7a-123">A contagem de ativação em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="fec7a-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="fec7a-124">emiti</span><span class="sxs-lookup"><span data-stu-id="fec7a-124">ios</span></span>               | <span data-ttu-id="fec7a-125">Int64</span><span class="sxs-lookup"><span data-stu-id="fec7a-125">Int64</span></span>  | <span data-ttu-id="fec7a-126">A contagem de ativação no iOS.</span><span class="sxs-lookup"><span data-stu-id="fec7a-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="fec7a-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="fec7a-127">windows10Mobile</span></span>   | <span data-ttu-id="fec7a-128">Int64</span><span class="sxs-lookup"><span data-stu-id="fec7a-128">Int64</span></span>  | <span data-ttu-id="fec7a-129">A contagem de ativação no Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="fec7a-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fec7a-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fec7a-130">JSON representation</span></span>

<span data-ttu-id="fec7a-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fec7a-131">The following is a JSON representation of the resource.</span></span>

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
