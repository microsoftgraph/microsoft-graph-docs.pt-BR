---
title: tipo de recurso de userActivationCounts
description: Veja a seguir uma representação JSON do recurso.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: cae194545f13d312ee78b572659017752e43a6a6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845287"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="2ecc1-103">tipo de recurso de userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="2ecc1-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2ecc1-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ecc1-104">Properties</span></span>

| <span data-ttu-id="2ecc1-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ecc1-105">Property</span></span>          | <span data-ttu-id="2ecc1-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ecc1-106">Type</span></span>   | <span data-ttu-id="2ecc1-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ecc1-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="2ecc1-108">productType</span><span class="sxs-lookup"><span data-stu-id="2ecc1-108">productType</span></span>       | <span data-ttu-id="2ecc1-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ecc1-109">String</span></span> | <span data-ttu-id="2ecc1-110">O tipo de produto, como "Office 365 ProPlus", "Cliente do projeto," ou "Visio Pro para Office 365".</span><span class="sxs-lookup"><span data-stu-id="2ecc1-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="2ecc1-111">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="2ecc1-111">lastActivatedDate</span></span> | <span data-ttu-id="2ecc1-112">Data</span><span class="sxs-lookup"><span data-stu-id="2ecc1-112">Date</span></span>   | <span data-ttu-id="2ecc1-113">A data da ativação mais recente.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="2ecc1-114">Windows</span><span class="sxs-lookup"><span data-stu-id="2ecc1-114">windows</span></span>           | <span data-ttu-id="2ecc1-115">Int64</span><span class="sxs-lookup"><span data-stu-id="2ecc1-115">Int64</span></span>  | <span data-ttu-id="2ecc1-116">A contagem de ativação do Windows.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-116">The activation count on Windows.</span></span> <span data-ttu-id="2ecc1-117">Esse número inclui cada ativação em qualquer computador do Windows.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="2ecc1-118">mac</span><span class="sxs-lookup"><span data-stu-id="2ecc1-118">mac</span></span>               | <span data-ttu-id="2ecc1-119">Int64</span><span class="sxs-lookup"><span data-stu-id="2ecc1-119">Int64</span></span>  | <span data-ttu-id="2ecc1-120">A contagem de ativação no Mac OS.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="2ecc1-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="2ecc1-121">windows10Mobile</span></span>   | <span data-ttu-id="2ecc1-122">Int64</span><span class="sxs-lookup"><span data-stu-id="2ecc1-122">Int64</span></span>  | <span data-ttu-id="2ecc1-123">A ativação contar com 10 do Windows mobile.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="2ecc1-124">IOS</span><span class="sxs-lookup"><span data-stu-id="2ecc1-124">ios</span></span>               | <span data-ttu-id="2ecc1-125">Int64</span><span class="sxs-lookup"><span data-stu-id="2ecc1-125">Int64</span></span>  | <span data-ttu-id="2ecc1-126">A contagem de ativação no iOS.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="2ecc1-127">Android</span><span class="sxs-lookup"><span data-stu-id="2ecc1-127">android</span></span>           | <span data-ttu-id="2ecc1-128">Int64</span><span class="sxs-lookup"><span data-stu-id="2ecc1-128">Int64</span></span>  | <span data-ttu-id="2ecc1-129">A contagem de ativação em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="2ecc1-130">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="2ecc1-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="2ecc1-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ecc1-131">Boolean</span></span> | <span data-ttu-id="2ecc1-132">True se o usuário utilizou o produto em um computador compartilhado antes.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2ecc1-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ecc1-133">JSON representation</span></span>

<span data-ttu-id="2ecc1-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ecc1-134">The following is a JSON representation of the resource.</span></span>

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
