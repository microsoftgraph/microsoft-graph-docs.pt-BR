---
title: insightIdentity
description: Tipo complexo contendo propriedades de itens compartilhados.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 418b991ff24613fa46c3adc6e7a98474ffa4e2b1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021886"
---
# <a name="insightidentity"></a><span data-ttu-id="f7a8c-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="f7a8c-103">insightIdentity</span></span>

<span data-ttu-id="f7a8c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7a8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7a8c-105">Tipo complexo contendo propriedades de itens do [sharedInsight](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="f7a8c-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="f7a8c-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7a8c-106">JSON representation</span></span>
<span data-ttu-id="f7a8c-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f7a8c-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.insightIdentity"
}-->
```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="f7a8c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7a8c-108">Properties</span></span>

| <span data-ttu-id="f7a8c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7a8c-109">Property</span></span>              | <span data-ttu-id="f7a8c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7a8c-110">Type</span></span>          | <span data-ttu-id="f7a8c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7a8c-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="f7a8c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f7a8c-112">displayName</span></span>       | <span data-ttu-id="f7a8c-113">String</span><span class="sxs-lookup"><span data-stu-id="f7a8c-113">String</span></span>          | <span data-ttu-id="f7a8c-114">O nome de exibição do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="f7a8c-114">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="f7a8c-115">id</span><span class="sxs-lookup"><span data-stu-id="f7a8c-115">id</span></span>              | <span data-ttu-id="f7a8c-116">String</span><span class="sxs-lookup"><span data-stu-id="f7a8c-116">String</span></span>        | <span data-ttu-id="f7a8c-117">A ID do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="f7a8c-117">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="f7a8c-118">address</span><span class="sxs-lookup"><span data-stu-id="f7a8c-118">address</span></span>             | <span data-ttu-id="f7a8c-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7a8c-119">String</span></span>      | <span data-ttu-id="f7a8c-120">O endereço de email do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="f7a8c-120">The email address of the user who shared the item.</span></span>  |


