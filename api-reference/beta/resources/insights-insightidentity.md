---
title: insightIdentity
description: Tipo complexo contendo propriedades de itens compartilhados.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 8718ab248dada75f04d92d6a8717dd4f43ee8106
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333593"
---
# <a name="insightidentity"></a><span data-ttu-id="1540f-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="1540f-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1540f-104">Tipo complexo contendo propriedades de itens [compartilhados](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="1540f-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="1540f-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1540f-105">JSON representation</span></span>
<span data-ttu-id="1540f-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1540f-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="1540f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1540f-107">Properties</span></span>

| <span data-ttu-id="1540f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1540f-108">Property</span></span>              | <span data-ttu-id="1540f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1540f-109">Type</span></span>          | <span data-ttu-id="1540f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1540f-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="1540f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1540f-111">displayName</span></span>       | <span data-ttu-id="1540f-112">String</span><span class="sxs-lookup"><span data-stu-id="1540f-112">String</span></span>          | <span data-ttu-id="1540f-113">O nome de exibição do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="1540f-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="1540f-114">id</span><span class="sxs-lookup"><span data-stu-id="1540f-114">id</span></span>              | <span data-ttu-id="1540f-115">String</span><span class="sxs-lookup"><span data-stu-id="1540f-115">String</span></span>        | <span data-ttu-id="1540f-116">A ID do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="1540f-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="1540f-117">address</span><span class="sxs-lookup"><span data-stu-id="1540f-117">address</span></span>             | <span data-ttu-id="1540f-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1540f-118">String</span></span>      | <span data-ttu-id="1540f-119">O endereço de email do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="1540f-119">The email address of the user who shared the item.</span></span>  |
