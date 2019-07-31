---
title: tipo de recurso userActivationCounts
description: Veja a seguir uma representação JSON do recurso.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9c1dbbaa6a429a90a54f8af5f3b380ff58c86dab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007491"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="03379-103">tipo de recurso userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="03379-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="03379-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03379-104">Properties</span></span>

| <span data-ttu-id="03379-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03379-105">Property</span></span>          | <span data-ttu-id="03379-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="03379-106">Type</span></span>   | <span data-ttu-id="03379-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="03379-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="03379-108">ProductType</span><span class="sxs-lookup"><span data-stu-id="03379-108">productType</span></span>       | <span data-ttu-id="03379-109">String</span><span class="sxs-lookup"><span data-stu-id="03379-109">String</span></span> | <span data-ttu-id="03379-110">O tipo de produto, como "Office 365 ProPlus", "Project Client" ou "Visio Pro for Office 365".</span><span class="sxs-lookup"><span data-stu-id="03379-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="03379-111">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="03379-111">lastActivatedDate</span></span> | <span data-ttu-id="03379-112">Data</span><span class="sxs-lookup"><span data-stu-id="03379-112">Date</span></span>   | <span data-ttu-id="03379-113">A data da ativação mais recente.</span><span class="sxs-lookup"><span data-stu-id="03379-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="03379-114">Windows</span><span class="sxs-lookup"><span data-stu-id="03379-114">windows</span></span>           | <span data-ttu-id="03379-115">Int64</span><span class="sxs-lookup"><span data-stu-id="03379-115">Int64</span></span>  | <span data-ttu-id="03379-116">A contagem de ativação no Windows.</span><span class="sxs-lookup"><span data-stu-id="03379-116">The activation count on Windows.</span></span> <span data-ttu-id="03379-117">Esse número inclui todas as ativações em qualquer computador Windows.</span><span class="sxs-lookup"><span data-stu-id="03379-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="03379-118">mac</span><span class="sxs-lookup"><span data-stu-id="03379-118">mac</span></span>               | <span data-ttu-id="03379-119">Int64</span><span class="sxs-lookup"><span data-stu-id="03379-119">Int64</span></span>  | <span data-ttu-id="03379-120">A contagem de ativação no Mac OS.</span><span class="sxs-lookup"><span data-stu-id="03379-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="03379-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="03379-121">windows10Mobile</span></span>   | <span data-ttu-id="03379-122">Int64</span><span class="sxs-lookup"><span data-stu-id="03379-122">Int64</span></span>  | <span data-ttu-id="03379-123">A contagem de ativação no Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="03379-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="03379-124">emiti</span><span class="sxs-lookup"><span data-stu-id="03379-124">ios</span></span>               | <span data-ttu-id="03379-125">Int64</span><span class="sxs-lookup"><span data-stu-id="03379-125">Int64</span></span>  | <span data-ttu-id="03379-126">A contagem de ativação no iOS.</span><span class="sxs-lookup"><span data-stu-id="03379-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="03379-127">Android</span><span class="sxs-lookup"><span data-stu-id="03379-127">android</span></span>           | <span data-ttu-id="03379-128">Int64</span><span class="sxs-lookup"><span data-stu-id="03379-128">Int64</span></span>  | <span data-ttu-id="03379-129">A contagem de ativação em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="03379-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="03379-130">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="03379-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="03379-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="03379-131">Boolean</span></span> | <span data-ttu-id="03379-132">True se o usuário usou o produto em um computador compartilhado antes.</span><span class="sxs-lookup"><span data-stu-id="03379-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="03379-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03379-133">JSON representation</span></span>

<span data-ttu-id="03379-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03379-134">The following is a JSON representation of the resource.</span></span>

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
