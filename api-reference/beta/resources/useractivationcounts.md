---
title: Tipo de recurso userActivationCounts
description: Veja a seguir uma representação JSON do recurso.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 48adb73bac65ddced88aea3edb18deae7653f5b3
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761790"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="f3c8f-103">Tipo de recurso userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="f3c8f-103">userActivationCounts resource type</span></span>

<span data-ttu-id="f3c8f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3c8f-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f3c8f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3c8f-105">Properties</span></span>

| <span data-ttu-id="f3c8f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3c8f-106">Property</span></span>          | <span data-ttu-id="f3c8f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3c8f-107">Type</span></span>   | <span data-ttu-id="f3c8f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3c8f-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="f3c8f-109">productType</span><span class="sxs-lookup"><span data-stu-id="f3c8f-109">productType</span></span>       | <span data-ttu-id="f3c8f-110">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f3c8f-110">String</span></span> | <span data-ttu-id="f3c8f-111">O tipo de produto, como "Microsoft 365 ProPlus" ou "Project Client".</span><span class="sxs-lookup"><span data-stu-id="f3c8f-111">The product type, such as "Microsoft 365 ProPlus"or "Project Client".</span></span> |
| <span data-ttu-id="f3c8f-112">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="f3c8f-112">lastActivatedDate</span></span> | <span data-ttu-id="f3c8f-113">Data</span><span class="sxs-lookup"><span data-stu-id="f3c8f-113">Date</span></span>   | <span data-ttu-id="f3c8f-114">A data da ativação mais recente.</span><span class="sxs-lookup"><span data-stu-id="f3c8f-114">The date of the latest activation.</span></span>       |
| <span data-ttu-id="f3c8f-115">windows</span><span class="sxs-lookup"><span data-stu-id="f3c8f-115">windows</span></span>           | <span data-ttu-id="f3c8f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f3c8f-116">Int64</span></span>  | <span data-ttu-id="f3c8f-117">A contagem de ativação no Windows.</span><span class="sxs-lookup"><span data-stu-id="f3c8f-117">The activation count on Windows.</span></span> <span data-ttu-id="f3c8f-118">Esse número inclui todas as ativações em qualquer computador Windows.</span><span class="sxs-lookup"><span data-stu-id="f3c8f-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="f3c8f-119">mac</span><span class="sxs-lookup"><span data-stu-id="f3c8f-119">mac</span></span>               | <span data-ttu-id="f3c8f-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f3c8f-120">Int64</span></span>  | <span data-ttu-id="f3c8f-121">A contagem de ativação no Mac OS.</span><span class="sxs-lookup"><span data-stu-id="f3c8f-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="f3c8f-122">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="f3c8f-122">windows10Mobile</span></span>   | <span data-ttu-id="f3c8f-123">Int64</span><span class="sxs-lookup"><span data-stu-id="f3c8f-123">Int64</span></span>  | <span data-ttu-id="f3c8f-124">A contagem de ativação no Windows 10 mobile.</span><span class="sxs-lookup"><span data-stu-id="f3c8f-124">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="f3c8f-125">ios</span><span class="sxs-lookup"><span data-stu-id="f3c8f-125">ios</span></span>               | <span data-ttu-id="f3c8f-126">Int64</span><span class="sxs-lookup"><span data-stu-id="f3c8f-126">Int64</span></span>  | <span data-ttu-id="f3c8f-127">A contagem de ativação no iOS.</span><span class="sxs-lookup"><span data-stu-id="f3c8f-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="f3c8f-128">android</span><span class="sxs-lookup"><span data-stu-id="f3c8f-128">android</span></span>           | <span data-ttu-id="f3c8f-129">Int64</span><span class="sxs-lookup"><span data-stu-id="f3c8f-129">Int64</span></span>  | <span data-ttu-id="f3c8f-130">A contagem de ativação em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="f3c8f-130">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="f3c8f-131">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="f3c8f-131">activatedOnSharedComputer</span></span>   | <span data-ttu-id="f3c8f-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3c8f-132">Boolean</span></span> | <span data-ttu-id="f3c8f-133">True se o usuário usou o produto em um computador compartilhado antes.</span><span class="sxs-lookup"><span data-stu-id="f3c8f-133">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f3c8f-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3c8f-134">JSON representation</span></span>

<span data-ttu-id="f3c8f-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3c8f-135">The following is a JSON representation of the resource.</span></span>

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


