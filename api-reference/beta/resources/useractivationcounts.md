---
title: tipo de recurso userActivationCounts
description: Veja a seguir uma representação JSON do recurso.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 65554254260d640638e7cbbbb2d0a0076e209f22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519544"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="2a896-103">tipo de recurso userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="2a896-103">userActivationCounts resource type</span></span>

<span data-ttu-id="2a896-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2a896-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="2a896-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2a896-105">Properties</span></span>

| <span data-ttu-id="2a896-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a896-106">Property</span></span>          | <span data-ttu-id="2a896-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a896-107">Type</span></span>   | <span data-ttu-id="2a896-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a896-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="2a896-109">ProductType</span><span class="sxs-lookup"><span data-stu-id="2a896-109">productType</span></span>       | <span data-ttu-id="2a896-110">String</span><span class="sxs-lookup"><span data-stu-id="2a896-110">String</span></span> | <span data-ttu-id="2a896-111">O tipo de produto, como "Office 365 ProPlus", "Project Client" ou "Visio Pro for Office 365".</span><span class="sxs-lookup"><span data-stu-id="2a896-111">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="2a896-112">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="2a896-112">lastActivatedDate</span></span> | <span data-ttu-id="2a896-113">Data</span><span class="sxs-lookup"><span data-stu-id="2a896-113">Date</span></span>   | <span data-ttu-id="2a896-114">A data da ativação mais recente.</span><span class="sxs-lookup"><span data-stu-id="2a896-114">The date of the latest activation.</span></span>       |
| <span data-ttu-id="2a896-115">Windows</span><span class="sxs-lookup"><span data-stu-id="2a896-115">windows</span></span>           | <span data-ttu-id="2a896-116">Int64</span><span class="sxs-lookup"><span data-stu-id="2a896-116">Int64</span></span>  | <span data-ttu-id="2a896-117">A contagem de ativação no Windows.</span><span class="sxs-lookup"><span data-stu-id="2a896-117">The activation count on Windows.</span></span> <span data-ttu-id="2a896-118">Esse número inclui todas as ativações em qualquer computador Windows.</span><span class="sxs-lookup"><span data-stu-id="2a896-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="2a896-119">mac</span><span class="sxs-lookup"><span data-stu-id="2a896-119">mac</span></span>               | <span data-ttu-id="2a896-120">Int64</span><span class="sxs-lookup"><span data-stu-id="2a896-120">Int64</span></span>  | <span data-ttu-id="2a896-121">A contagem de ativação no Mac OS.</span><span class="sxs-lookup"><span data-stu-id="2a896-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="2a896-122">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="2a896-122">windows10Mobile</span></span>   | <span data-ttu-id="2a896-123">Int64</span><span class="sxs-lookup"><span data-stu-id="2a896-123">Int64</span></span>  | <span data-ttu-id="2a896-124">A contagem de ativação no Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="2a896-124">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="2a896-125">emiti</span><span class="sxs-lookup"><span data-stu-id="2a896-125">ios</span></span>               | <span data-ttu-id="2a896-126">Int64</span><span class="sxs-lookup"><span data-stu-id="2a896-126">Int64</span></span>  | <span data-ttu-id="2a896-127">A contagem de ativação no iOS.</span><span class="sxs-lookup"><span data-stu-id="2a896-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="2a896-128">Android</span><span class="sxs-lookup"><span data-stu-id="2a896-128">android</span></span>           | <span data-ttu-id="2a896-129">Int64</span><span class="sxs-lookup"><span data-stu-id="2a896-129">Int64</span></span>  | <span data-ttu-id="2a896-130">A contagem de ativação em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="2a896-130">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="2a896-131">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="2a896-131">activatedOnSharedComputer</span></span>   | <span data-ttu-id="2a896-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a896-132">Boolean</span></span> | <span data-ttu-id="2a896-133">True se o usuário usou o produto em um computador compartilhado antes.</span><span class="sxs-lookup"><span data-stu-id="2a896-133">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2a896-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2a896-134">JSON representation</span></span>

<span data-ttu-id="2a896-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2a896-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userActivationCounts"
} -->

```json
{
  "productType": "String", 
  "lastActivatedDate": "Date", 
  "windows": 1024, 
  "mac": 1024, 
  "windows10Mobile": 1024, 
  "ios": 1024, 
  "android": 1024,
  "activatedOnSharedComputer": true 
}
```
