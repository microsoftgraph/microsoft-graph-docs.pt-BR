---
title: tipo de recurso de office365ActivationsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: f57393a538631664be8845fdaeda9f35d07c986f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849305"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="4de6f-103">tipo de recurso de office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="4de6f-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4de6f-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4de6f-104">Properties</span></span>

| <span data-ttu-id="4de6f-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4de6f-105">Property</span></span>                 | <span data-ttu-id="4de6f-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="4de6f-106">Type</span></span>   | <span data-ttu-id="4de6f-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="4de6f-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="4de6f-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4de6f-108">reportRefreshDate</span></span>        | <span data-ttu-id="4de6f-109">Data</span><span class="sxs-lookup"><span data-stu-id="4de6f-109">Date</span></span>   | <span data-ttu-id="4de6f-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4de6f-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="4de6f-111">productType</span><span class="sxs-lookup"><span data-stu-id="4de6f-111">productType</span></span>              | <span data-ttu-id="4de6f-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4de6f-112">String</span></span> | <span data-ttu-id="4de6f-113">O tipo de produto, como "Office 365 ProPlus", "Cliente do projeto," ou "Visio Pro para Office 365".</span><span class="sxs-lookup"><span data-stu-id="4de6f-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="4de6f-114">atribuído</span><span class="sxs-lookup"><span data-stu-id="4de6f-114">assigned</span></span>                 | <span data-ttu-id="4de6f-115">Int64</span><span class="sxs-lookup"><span data-stu-id="4de6f-115">Int64</span></span>  | <span data-ttu-id="4de6f-116">O número de usuários foram atribuído para a licença do produto.</span><span class="sxs-lookup"><span data-stu-id="4de6f-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="4de6f-117">ativado</span><span class="sxs-lookup"><span data-stu-id="4de6f-117">activated</span></span>                | <span data-ttu-id="4de6f-118">Int64</span><span class="sxs-lookup"><span data-stu-id="4de6f-118">Int64</span></span>  | <span data-ttu-id="4de6f-119">O número de usuários que ativou o produto.</span><span class="sxs-lookup"><span data-stu-id="4de6f-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="4de6f-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="4de6f-120">sharedComputerActivation</span></span> | <span data-ttu-id="4de6f-121">Int64</span><span class="sxs-lookup"><span data-stu-id="4de6f-121">Int64</span></span>  | <span data-ttu-id="4de6f-122">O número de usuários que usaram o produto em um computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="4de6f-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4de6f-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4de6f-123">JSON representation</span></span>

<span data-ttu-id="4de6f-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4de6f-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "assigned": 1024, 
  "activated": 1024,
  "sharedComputerActivation": 1024
}
```
