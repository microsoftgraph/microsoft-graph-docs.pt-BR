---
title: tipo de recurso userActivationCounts
description: Veja a seguir uma representação JSON do recurso.
author: krbain
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d81e8078d785761c09aa1070120924b2318415a9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057882"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="accce-103">tipo de recurso userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="accce-103">userActivationCounts resource type</span></span>

<span data-ttu-id="accce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="accce-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="accce-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="accce-105">Properties</span></span>

| <span data-ttu-id="accce-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="accce-106">Property</span></span>          | <span data-ttu-id="accce-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="accce-107">Type</span></span>   | <span data-ttu-id="accce-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="accce-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="accce-109">ProductType</span><span class="sxs-lookup"><span data-stu-id="accce-109">productType</span></span>       | <span data-ttu-id="accce-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="accce-110">String</span></span> | <span data-ttu-id="accce-111">O tipo de produto, como "Microsoft 365 ProPlus" ou "Project Client".</span><span class="sxs-lookup"><span data-stu-id="accce-111">The product type, such as "Microsoft 365 ProPlus"or "Project Client".</span></span> |
| <span data-ttu-id="accce-112">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="accce-112">lastActivatedDate</span></span> | <span data-ttu-id="accce-113">Data</span><span class="sxs-lookup"><span data-stu-id="accce-113">Date</span></span>   | <span data-ttu-id="accce-114">A data da ativação mais recente.</span><span class="sxs-lookup"><span data-stu-id="accce-114">The date of the latest activation.</span></span>       |
| <span data-ttu-id="accce-115">Windows</span><span class="sxs-lookup"><span data-stu-id="accce-115">windows</span></span>           | <span data-ttu-id="accce-116">Int64</span><span class="sxs-lookup"><span data-stu-id="accce-116">Int64</span></span>  | <span data-ttu-id="accce-117">A contagem de ativação no Windows.</span><span class="sxs-lookup"><span data-stu-id="accce-117">The activation count on Windows.</span></span> <span data-ttu-id="accce-118">Esse número inclui todas as ativações em qualquer computador Windows.</span><span class="sxs-lookup"><span data-stu-id="accce-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="accce-119">mac</span><span class="sxs-lookup"><span data-stu-id="accce-119">mac</span></span>               | <span data-ttu-id="accce-120">Int64</span><span class="sxs-lookup"><span data-stu-id="accce-120">Int64</span></span>  | <span data-ttu-id="accce-121">A contagem de ativação no Mac OS.</span><span class="sxs-lookup"><span data-stu-id="accce-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="accce-122">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="accce-122">windows10Mobile</span></span>   | <span data-ttu-id="accce-123">Int64</span><span class="sxs-lookup"><span data-stu-id="accce-123">Int64</span></span>  | <span data-ttu-id="accce-124">A contagem de ativação no Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="accce-124">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="accce-125">emiti</span><span class="sxs-lookup"><span data-stu-id="accce-125">ios</span></span>               | <span data-ttu-id="accce-126">Int64</span><span class="sxs-lookup"><span data-stu-id="accce-126">Int64</span></span>  | <span data-ttu-id="accce-127">A contagem de ativação no iOS.</span><span class="sxs-lookup"><span data-stu-id="accce-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="accce-128">Android</span><span class="sxs-lookup"><span data-stu-id="accce-128">android</span></span>           | <span data-ttu-id="accce-129">Int64</span><span class="sxs-lookup"><span data-stu-id="accce-129">Int64</span></span>  | <span data-ttu-id="accce-130">A contagem de ativação em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="accce-130">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="accce-131">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="accce-131">activatedOnSharedComputer</span></span>   | <span data-ttu-id="accce-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="accce-132">Boolean</span></span> | <span data-ttu-id="accce-133">True se o usuário usou o produto em um computador compartilhado antes.</span><span class="sxs-lookup"><span data-stu-id="accce-133">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="accce-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="accce-134">JSON representation</span></span>

<span data-ttu-id="accce-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="accce-135">The following is a JSON representation of the resource.</span></span>

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


