---
title: tipo de recurso office365ActivationCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: ef612173b8b78d4e87e07e66995ea6cb9ac0dc16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021214"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="27916-103">tipo de recurso office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="27916-103">office365ActivationCounts resource type</span></span>

<span data-ttu-id="27916-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27916-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="27916-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27916-105">Properties</span></span>

| <span data-ttu-id="27916-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27916-106">Property</span></span>          | <span data-ttu-id="27916-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="27916-107">Type</span></span>   | <span data-ttu-id="27916-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="27916-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="27916-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="27916-109">reportRefreshDate</span></span> | <span data-ttu-id="27916-110">Data</span><span class="sxs-lookup"><span data-stu-id="27916-110">Date</span></span>   | <span data-ttu-id="27916-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="27916-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="27916-112">ProductType</span><span class="sxs-lookup"><span data-stu-id="27916-112">productType</span></span>       | <span data-ttu-id="27916-113">String</span><span class="sxs-lookup"><span data-stu-id="27916-113">String</span></span> | <span data-ttu-id="27916-114">O tipo de produto, como "Microsoft 365 ProPlus" ou "Project Client".</span><span class="sxs-lookup"><span data-stu-id="27916-114">The product type, such as "Microsoft 365 ProPlus" or "Project Client".</span></span> |
| <span data-ttu-id="27916-115">Windows</span><span class="sxs-lookup"><span data-stu-id="27916-115">windows</span></span>           | <span data-ttu-id="27916-116">Int64</span><span class="sxs-lookup"><span data-stu-id="27916-116">Int64</span></span>  | <span data-ttu-id="27916-117">A contagem de ativação no Windows.</span><span class="sxs-lookup"><span data-stu-id="27916-117">The activation count on Windows.</span></span> <span data-ttu-id="27916-118">Esse número inclui todas as ativações em qualquer computador Windows.</span><span class="sxs-lookup"><span data-stu-id="27916-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="27916-119">mac</span><span class="sxs-lookup"><span data-stu-id="27916-119">mac</span></span>               | <span data-ttu-id="27916-120">Int64</span><span class="sxs-lookup"><span data-stu-id="27916-120">Int64</span></span>  | <span data-ttu-id="27916-121">A contagem de ativação no Mac OS.</span><span class="sxs-lookup"><span data-stu-id="27916-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="27916-122">Android</span><span class="sxs-lookup"><span data-stu-id="27916-122">android</span></span>           | <span data-ttu-id="27916-123">Int64</span><span class="sxs-lookup"><span data-stu-id="27916-123">Int64</span></span>  | <span data-ttu-id="27916-124">A contagem de ativação em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="27916-124">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="27916-125">emiti</span><span class="sxs-lookup"><span data-stu-id="27916-125">ios</span></span>               | <span data-ttu-id="27916-126">Int64</span><span class="sxs-lookup"><span data-stu-id="27916-126">Int64</span></span>  | <span data-ttu-id="27916-127">A contagem de ativação no iOS.</span><span class="sxs-lookup"><span data-stu-id="27916-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="27916-128">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="27916-128">windows10Mobile</span></span>   | <span data-ttu-id="27916-129">Int64</span><span class="sxs-lookup"><span data-stu-id="27916-129">Int64</span></span>  | <span data-ttu-id="27916-130">A contagem de ativação no Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="27916-130">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="27916-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27916-131">JSON representation</span></span>

<span data-ttu-id="27916-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="27916-132">The following is a JSON representation of the resource.</span></span>

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


