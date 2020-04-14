---
title: tipo de recurso userActivationCounts
description: Veja a seguir uma representação JSON do recurso.
author: krbain
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 91366f9d2b2308c997c111123d856581db7c00c6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43384951"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="c628e-103">tipo de recurso userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="c628e-103">userActivationCounts resource type</span></span>

<span data-ttu-id="c628e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c628e-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c628e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c628e-105">Properties</span></span>

| <span data-ttu-id="c628e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c628e-106">Property</span></span>          | <span data-ttu-id="c628e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c628e-107">Type</span></span>   | <span data-ttu-id="c628e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c628e-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="c628e-109">ProductType</span><span class="sxs-lookup"><span data-stu-id="c628e-109">productType</span></span>       | <span data-ttu-id="c628e-110">String</span><span class="sxs-lookup"><span data-stu-id="c628e-110">String</span></span> | <span data-ttu-id="c628e-111">O tipo de produto, como "Office 365 ProPlus", "Project Client" ou "Visio Pro for Office 365".</span><span class="sxs-lookup"><span data-stu-id="c628e-111">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="c628e-112">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="c628e-112">lastActivatedDate</span></span> | <span data-ttu-id="c628e-113">Data</span><span class="sxs-lookup"><span data-stu-id="c628e-113">Date</span></span>   | <span data-ttu-id="c628e-114">A data da ativação mais recente.</span><span class="sxs-lookup"><span data-stu-id="c628e-114">The date of the latest activation.</span></span>       |
| <span data-ttu-id="c628e-115">Windows</span><span class="sxs-lookup"><span data-stu-id="c628e-115">windows</span></span>           | <span data-ttu-id="c628e-116">Int64</span><span class="sxs-lookup"><span data-stu-id="c628e-116">Int64</span></span>  | <span data-ttu-id="c628e-117">A contagem de ativação no Windows.</span><span class="sxs-lookup"><span data-stu-id="c628e-117">The activation count on Windows.</span></span> <span data-ttu-id="c628e-118">Esse número inclui todas as ativações em qualquer computador Windows.</span><span class="sxs-lookup"><span data-stu-id="c628e-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="c628e-119">mac</span><span class="sxs-lookup"><span data-stu-id="c628e-119">mac</span></span>               | <span data-ttu-id="c628e-120">Int64</span><span class="sxs-lookup"><span data-stu-id="c628e-120">Int64</span></span>  | <span data-ttu-id="c628e-121">A contagem de ativação no Mac OS.</span><span class="sxs-lookup"><span data-stu-id="c628e-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="c628e-122">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="c628e-122">windows10Mobile</span></span>   | <span data-ttu-id="c628e-123">Int64</span><span class="sxs-lookup"><span data-stu-id="c628e-123">Int64</span></span>  | <span data-ttu-id="c628e-124">A contagem de ativação no Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="c628e-124">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="c628e-125">emiti</span><span class="sxs-lookup"><span data-stu-id="c628e-125">ios</span></span>               | <span data-ttu-id="c628e-126">Int64</span><span class="sxs-lookup"><span data-stu-id="c628e-126">Int64</span></span>  | <span data-ttu-id="c628e-127">A contagem de ativação no iOS.</span><span class="sxs-lookup"><span data-stu-id="c628e-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="c628e-128">Android</span><span class="sxs-lookup"><span data-stu-id="c628e-128">android</span></span>           | <span data-ttu-id="c628e-129">Int64</span><span class="sxs-lookup"><span data-stu-id="c628e-129">Int64</span></span>  | <span data-ttu-id="c628e-130">A contagem de ativação em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="c628e-130">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="c628e-131">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="c628e-131">activatedOnSharedComputer</span></span>   | <span data-ttu-id="c628e-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="c628e-132">Boolean</span></span> | <span data-ttu-id="c628e-133">True se o usuário usou o produto em um computador compartilhado antes.</span><span class="sxs-lookup"><span data-stu-id="c628e-133">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c628e-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c628e-134">JSON representation</span></span>

<span data-ttu-id="c628e-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c628e-135">The following is a JSON representation of the resource.</span></span>

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
