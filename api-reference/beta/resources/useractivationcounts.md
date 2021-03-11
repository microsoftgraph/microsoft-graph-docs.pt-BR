---
title: Tipo de recurso userActivationCounts
description: Veja a seguir uma representação JSON do recurso.
author: jpettere
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 719a73739a64dca2bd7a052cc9cdd51007173eff
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719896"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="56997-103">Tipo de recurso userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="56997-103">userActivationCounts resource type</span></span>

<span data-ttu-id="56997-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56997-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="56997-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56997-105">Properties</span></span>

| <span data-ttu-id="56997-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56997-106">Property</span></span>          | <span data-ttu-id="56997-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="56997-107">Type</span></span>   | <span data-ttu-id="56997-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="56997-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="56997-109">productType</span><span class="sxs-lookup"><span data-stu-id="56997-109">productType</span></span>       | <span data-ttu-id="56997-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56997-110">String</span></span> | <span data-ttu-id="56997-111">O tipo de produto, como "Microsoft 365 ProPlus" ou "Project Client".</span><span class="sxs-lookup"><span data-stu-id="56997-111">The product type, such as "Microsoft 365 ProPlus"or "Project Client".</span></span> |
| <span data-ttu-id="56997-112">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="56997-112">lastActivatedDate</span></span> | <span data-ttu-id="56997-113">Data</span><span class="sxs-lookup"><span data-stu-id="56997-113">Date</span></span>   | <span data-ttu-id="56997-114">A data da ativação mais recente.</span><span class="sxs-lookup"><span data-stu-id="56997-114">The date of the latest activation.</span></span>       |
| <span data-ttu-id="56997-115">windows</span><span class="sxs-lookup"><span data-stu-id="56997-115">windows</span></span>           | <span data-ttu-id="56997-116">Int64</span><span class="sxs-lookup"><span data-stu-id="56997-116">Int64</span></span>  | <span data-ttu-id="56997-117">A contagem de ativação no Windows.</span><span class="sxs-lookup"><span data-stu-id="56997-117">The activation count on Windows.</span></span> <span data-ttu-id="56997-118">Esse número inclui todas as ativações em qualquer computador Windows.</span><span class="sxs-lookup"><span data-stu-id="56997-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="56997-119">mac</span><span class="sxs-lookup"><span data-stu-id="56997-119">mac</span></span>               | <span data-ttu-id="56997-120">Int64</span><span class="sxs-lookup"><span data-stu-id="56997-120">Int64</span></span>  | <span data-ttu-id="56997-121">A contagem de ativação no Mac OS.</span><span class="sxs-lookup"><span data-stu-id="56997-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="56997-122">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="56997-122">windows10Mobile</span></span>   | <span data-ttu-id="56997-123">Int64</span><span class="sxs-lookup"><span data-stu-id="56997-123">Int64</span></span>  | <span data-ttu-id="56997-124">A contagem de ativação no Windows 10 mobile.</span><span class="sxs-lookup"><span data-stu-id="56997-124">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="56997-125">ios</span><span class="sxs-lookup"><span data-stu-id="56997-125">ios</span></span>               | <span data-ttu-id="56997-126">Int64</span><span class="sxs-lookup"><span data-stu-id="56997-126">Int64</span></span>  | <span data-ttu-id="56997-127">A contagem de ativação no iOS.</span><span class="sxs-lookup"><span data-stu-id="56997-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="56997-128">android</span><span class="sxs-lookup"><span data-stu-id="56997-128">android</span></span>           | <span data-ttu-id="56997-129">Int64</span><span class="sxs-lookup"><span data-stu-id="56997-129">Int64</span></span>  | <span data-ttu-id="56997-130">A contagem de ativação em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="56997-130">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="56997-131">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="56997-131">activatedOnSharedComputer</span></span>   | <span data-ttu-id="56997-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="56997-132">Boolean</span></span> | <span data-ttu-id="56997-133">True se o usuário usou o produto em um computador compartilhado antes.</span><span class="sxs-lookup"><span data-stu-id="56997-133">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="56997-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56997-134">JSON representation</span></span>

<span data-ttu-id="56997-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="56997-135">The following is a JSON representation of the resource.</span></span>

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


