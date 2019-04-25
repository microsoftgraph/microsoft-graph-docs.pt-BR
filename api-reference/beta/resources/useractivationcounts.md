---
title: tipo de recurso userActivationCounts
description: Veja a seguir uma representação JSON do recurso.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 535355d6be3f6b617d7eb293890aa05a517cfc3b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581279"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="e1eda-103">tipo de recurso userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="e1eda-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e1eda-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1eda-104">Properties</span></span>

| <span data-ttu-id="e1eda-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1eda-105">Property</span></span>          | <span data-ttu-id="e1eda-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1eda-106">Type</span></span>   | <span data-ttu-id="e1eda-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1eda-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="e1eda-108">ProductType</span><span class="sxs-lookup"><span data-stu-id="e1eda-108">productType</span></span>       | <span data-ttu-id="e1eda-109">String</span><span class="sxs-lookup"><span data-stu-id="e1eda-109">String</span></span> | <span data-ttu-id="e1eda-110">O tipo de produto, como "Office 365 proPlus", "Project Client" ou "Visio Pro for Office 365".</span><span class="sxs-lookup"><span data-stu-id="e1eda-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="e1eda-111">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="e1eda-111">lastActivatedDate</span></span> | <span data-ttu-id="e1eda-112">Data</span><span class="sxs-lookup"><span data-stu-id="e1eda-112">Date</span></span>   | <span data-ttu-id="e1eda-113">A data da ativação mais recente.</span><span class="sxs-lookup"><span data-stu-id="e1eda-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="e1eda-114">Windows</span><span class="sxs-lookup"><span data-stu-id="e1eda-114">windows</span></span>           | <span data-ttu-id="e1eda-115">Int64</span><span class="sxs-lookup"><span data-stu-id="e1eda-115">Int64</span></span>  | <span data-ttu-id="e1eda-116">A contagem de ativação no Windows.</span><span class="sxs-lookup"><span data-stu-id="e1eda-116">The activation count on Windows.</span></span> <span data-ttu-id="e1eda-117">Esse número inclui todas as ativações em qualquer computador Windows.</span><span class="sxs-lookup"><span data-stu-id="e1eda-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="e1eda-118">mac</span><span class="sxs-lookup"><span data-stu-id="e1eda-118">mac</span></span>               | <span data-ttu-id="e1eda-119">Int64</span><span class="sxs-lookup"><span data-stu-id="e1eda-119">Int64</span></span>  | <span data-ttu-id="e1eda-120">A contagem de ativação no Mac OS.</span><span class="sxs-lookup"><span data-stu-id="e1eda-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="e1eda-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="e1eda-121">windows10Mobile</span></span>   | <span data-ttu-id="e1eda-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e1eda-122">Int64</span></span>  | <span data-ttu-id="e1eda-123">A contagem de ativação no Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="e1eda-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="e1eda-124">emiti</span><span class="sxs-lookup"><span data-stu-id="e1eda-124">ios</span></span>               | <span data-ttu-id="e1eda-125">Int64</span><span class="sxs-lookup"><span data-stu-id="e1eda-125">Int64</span></span>  | <span data-ttu-id="e1eda-126">A contagem de ativação no iOS.</span><span class="sxs-lookup"><span data-stu-id="e1eda-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="e1eda-127">Android</span><span class="sxs-lookup"><span data-stu-id="e1eda-127">android</span></span>           | <span data-ttu-id="e1eda-128">Int64</span><span class="sxs-lookup"><span data-stu-id="e1eda-128">Int64</span></span>  | <span data-ttu-id="e1eda-129">A contagem de ativação em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="e1eda-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="e1eda-130">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="e1eda-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="e1eda-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="e1eda-131">Boolean</span></span> | <span data-ttu-id="e1eda-132">True se o usuário usou o produto em um computador compartilhado antes.</span><span class="sxs-lookup"><span data-stu-id="e1eda-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e1eda-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1eda-133">JSON representation</span></span>

<span data-ttu-id="e1eda-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1eda-134">The following is a JSON representation of the resource.</span></span>

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
