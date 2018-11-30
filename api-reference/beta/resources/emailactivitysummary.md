---
title: tipo de recurso de emailActivitySummary
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 039592a33cd004b9a5dc7800c0dbd4ece91bd48c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038548"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="a347e-103">tipo de recurso de emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="a347e-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a347e-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a347e-104">Properties</span></span>

| <span data-ttu-id="a347e-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a347e-105">Property</span></span>          | <span data-ttu-id="a347e-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="a347e-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="a347e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a347e-107">reportRefreshDate</span></span> | <span data-ttu-id="a347e-108">Data</span><span class="sxs-lookup"><span data-stu-id="a347e-108">Date</span></span>   |
| <span data-ttu-id="a347e-109">enviar</span><span class="sxs-lookup"><span data-stu-id="a347e-109">send</span></span>              | <span data-ttu-id="a347e-110">Int64</span><span class="sxs-lookup"><span data-stu-id="a347e-110">Int64</span></span>  |
| <span data-ttu-id="a347e-111">receber</span><span class="sxs-lookup"><span data-stu-id="a347e-111">receive</span></span>           | <span data-ttu-id="a347e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="a347e-112">Int64</span></span>  |
| <span data-ttu-id="a347e-113">leitura</span><span class="sxs-lookup"><span data-stu-id="a347e-113">read</span></span>              | <span data-ttu-id="a347e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="a347e-114">Int64</span></span>  |
| <span data-ttu-id="a347e-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="a347e-115">reportDate</span></span>        | <span data-ttu-id="a347e-116">Data</span><span class="sxs-lookup"><span data-stu-id="a347e-116">Date</span></span>   |
| <span data-ttu-id="a347e-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a347e-117">reportPeriod</span></span>      | <span data-ttu-id="a347e-118">String</span><span class="sxs-lookup"><span data-stu-id="a347e-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a347e-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a347e-119">JSON representation</span></span>

<span data-ttu-id="a347e-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a347e-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
