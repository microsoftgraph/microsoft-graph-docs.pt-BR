---
title: insightIdentity
description: Tipo complexo contendo propriedades de itens compartilhados.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 6b5a4b3c6e43f0314860935af810d20d91663c96
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005748"
---
# <a name="insightidentity"></a><span data-ttu-id="d7abb-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="d7abb-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7abb-104">Tipo complexo contendo propriedades de itens [compartilhados](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="d7abb-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="d7abb-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7abb-105">JSON representation</span></span>
<span data-ttu-id="d7abb-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d7abb-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="d7abb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7abb-107">Properties</span></span>

| <span data-ttu-id="d7abb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7abb-108">Property</span></span>              | <span data-ttu-id="d7abb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7abb-109">Type</span></span>          | <span data-ttu-id="d7abb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7abb-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="d7abb-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d7abb-111">displayName</span></span>       | <span data-ttu-id="d7abb-112">String</span><span class="sxs-lookup"><span data-stu-id="d7abb-112">String</span></span>          | <span data-ttu-id="d7abb-113">O nome de exibição do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="d7abb-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="d7abb-114">id</span><span class="sxs-lookup"><span data-stu-id="d7abb-114">id</span></span>              | <span data-ttu-id="d7abb-115">String</span><span class="sxs-lookup"><span data-stu-id="d7abb-115">String</span></span>        | <span data-ttu-id="d7abb-116">A ID do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="d7abb-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="d7abb-117">address</span><span class="sxs-lookup"><span data-stu-id="d7abb-117">address</span></span>             | <span data-ttu-id="d7abb-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7abb-118">String</span></span>      | <span data-ttu-id="d7abb-119">O endereço de email do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="d7abb-119">The email address of the user who shared the item.</span></span>  |
