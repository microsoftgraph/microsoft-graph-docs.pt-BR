---
title: Tipo de recurso office365ActivationCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 7ac3b6bb14b347f4ab273bbf65ce767f1ae6e1a2
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983200"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="d649a-103">Tipo de recurso office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="d649a-103">office365ActivationCounts resource type</span></span>

<span data-ttu-id="d649a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d649a-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d649a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d649a-105">Properties</span></span>

| <span data-ttu-id="d649a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d649a-106">Property</span></span>          | <span data-ttu-id="d649a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d649a-107">Type</span></span>   | <span data-ttu-id="d649a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d649a-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="d649a-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d649a-109">reportRefreshDate</span></span> | <span data-ttu-id="d649a-110">Data</span><span class="sxs-lookup"><span data-stu-id="d649a-110">Date</span></span>   | <span data-ttu-id="d649a-111">A data mais recente do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d649a-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="d649a-112">productType</span><span class="sxs-lookup"><span data-stu-id="d649a-112">productType</span></span>       | <span data-ttu-id="d649a-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d649a-113">String</span></span> | <span data-ttu-id="d649a-114">O tipo de produto, como "Microsoft 365 ProPlus" ou "Project Client".</span><span class="sxs-lookup"><span data-stu-id="d649a-114">The product type, such as "Microsoft 365 ProPlus" or "Project Client".</span></span> |
| <span data-ttu-id="d649a-115">windows</span><span class="sxs-lookup"><span data-stu-id="d649a-115">windows</span></span>           | <span data-ttu-id="d649a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="d649a-116">Int64</span></span>  | <span data-ttu-id="d649a-117">A contagem de ativação no Windows.</span><span class="sxs-lookup"><span data-stu-id="d649a-117">The activation count on Windows.</span></span> <span data-ttu-id="d649a-118">Esse número inclui todas as ativações em qualquer computador Windows.</span><span class="sxs-lookup"><span data-stu-id="d649a-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="d649a-119">mac</span><span class="sxs-lookup"><span data-stu-id="d649a-119">mac</span></span>               | <span data-ttu-id="d649a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="d649a-120">Int64</span></span>  | <span data-ttu-id="d649a-121">A contagem de ativação no Mac OS.</span><span class="sxs-lookup"><span data-stu-id="d649a-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="d649a-122">android</span><span class="sxs-lookup"><span data-stu-id="d649a-122">android</span></span>           | <span data-ttu-id="d649a-123">Int64</span><span class="sxs-lookup"><span data-stu-id="d649a-123">Int64</span></span>  | <span data-ttu-id="d649a-124">A contagem de ativação em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="d649a-124">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="d649a-125">ios</span><span class="sxs-lookup"><span data-stu-id="d649a-125">ios</span></span>               | <span data-ttu-id="d649a-126">Int64</span><span class="sxs-lookup"><span data-stu-id="d649a-126">Int64</span></span>  | <span data-ttu-id="d649a-127">A contagem de ativação no iOS.</span><span class="sxs-lookup"><span data-stu-id="d649a-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="d649a-128">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="d649a-128">windows10Mobile</span></span>   | <span data-ttu-id="d649a-129">Int64</span><span class="sxs-lookup"><span data-stu-id="d649a-129">Int64</span></span>  | <span data-ttu-id="d649a-130">A contagem de ativação no Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="d649a-130">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d649a-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d649a-131">JSON representation</span></span>

<span data-ttu-id="d649a-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d649a-132">The following is a JSON representation of the resource.</span></span>

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


