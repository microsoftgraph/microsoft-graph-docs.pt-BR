---
title: tipo de recurso de office365ActivationCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 30386b3833b8140d4c602e27cb3a78f3a68670dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824987"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="07089-103">tipo de recurso de office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="07089-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="07089-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07089-104">Properties</span></span>

| <span data-ttu-id="07089-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07089-105">Property</span></span>          | <span data-ttu-id="07089-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="07089-106">Type</span></span>   | <span data-ttu-id="07089-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="07089-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="07089-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="07089-108">reportRefreshDate</span></span> | <span data-ttu-id="07089-109">Data</span><span class="sxs-lookup"><span data-stu-id="07089-109">Date</span></span>   | <span data-ttu-id="07089-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="07089-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="07089-111">productType</span><span class="sxs-lookup"><span data-stu-id="07089-111">productType</span></span>       | <span data-ttu-id="07089-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07089-112">String</span></span> | <span data-ttu-id="07089-113">O tipo de produto, como "Office 365 ProPlus", "Cliente do projeto," ou "Visio Pro para Office 365".</span><span class="sxs-lookup"><span data-stu-id="07089-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="07089-114">Windows</span><span class="sxs-lookup"><span data-stu-id="07089-114">windows</span></span>           | <span data-ttu-id="07089-115">Int64</span><span class="sxs-lookup"><span data-stu-id="07089-115">Int64</span></span>  | <span data-ttu-id="07089-116">A contagem de ativação do Windows.</span><span class="sxs-lookup"><span data-stu-id="07089-116">The activation count on Windows.</span></span> <span data-ttu-id="07089-117">Esse número inclui cada ativação em qualquer computador do Windows.</span><span class="sxs-lookup"><span data-stu-id="07089-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="07089-118">mac</span><span class="sxs-lookup"><span data-stu-id="07089-118">mac</span></span>               | <span data-ttu-id="07089-119">Int64</span><span class="sxs-lookup"><span data-stu-id="07089-119">Int64</span></span>  | <span data-ttu-id="07089-120">A contagem de ativação no Mac OS.</span><span class="sxs-lookup"><span data-stu-id="07089-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="07089-121">Android</span><span class="sxs-lookup"><span data-stu-id="07089-121">android</span></span>           | <span data-ttu-id="07089-122">Int64</span><span class="sxs-lookup"><span data-stu-id="07089-122">Int64</span></span>  | <span data-ttu-id="07089-123">A contagem de ativação em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="07089-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="07089-124">IOS</span><span class="sxs-lookup"><span data-stu-id="07089-124">ios</span></span>               | <span data-ttu-id="07089-125">Int64</span><span class="sxs-lookup"><span data-stu-id="07089-125">Int64</span></span>  | <span data-ttu-id="07089-126">A contagem de ativação no iOS.</span><span class="sxs-lookup"><span data-stu-id="07089-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="07089-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="07089-127">windows10Mobile</span></span>   | <span data-ttu-id="07089-128">Int64</span><span class="sxs-lookup"><span data-stu-id="07089-128">Int64</span></span>  | <span data-ttu-id="07089-129">A ativação contar com 10 do Windows mobile.</span><span class="sxs-lookup"><span data-stu-id="07089-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="07089-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07089-130">JSON representation</span></span>

<span data-ttu-id="07089-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07089-131">The following is a JSON representation of the resource.</span></span>

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
