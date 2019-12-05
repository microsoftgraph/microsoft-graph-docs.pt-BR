---
title: insightIdentity
description: Tipo complexo contendo propriedades de itens compartilhados.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 1dc952ba931e1a0cb4302dac881f2d5ec015c591
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844336"
---
# <a name="insightidentity"></a><span data-ttu-id="04602-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="04602-103">insightIdentity</span></span>

<span data-ttu-id="04602-104">Tipo complexo contendo propriedades de itens do [sharedInsight](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="04602-104">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="04602-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04602-105">JSON representation</span></span>
<span data-ttu-id="04602-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="04602-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="04602-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04602-107">Properties</span></span>

| <span data-ttu-id="04602-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04602-108">Property</span></span>              | <span data-ttu-id="04602-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="04602-109">Type</span></span>          | <span data-ttu-id="04602-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="04602-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="04602-111">displayName</span><span class="sxs-lookup"><span data-stu-id="04602-111">displayName</span></span>       | <span data-ttu-id="04602-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04602-112">String</span></span>          | <span data-ttu-id="04602-113">O nome de exibição do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="04602-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="04602-114">id</span><span class="sxs-lookup"><span data-stu-id="04602-114">id</span></span>              | <span data-ttu-id="04602-115">String</span><span class="sxs-lookup"><span data-stu-id="04602-115">String</span></span>        | <span data-ttu-id="04602-116">A ID do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="04602-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="04602-117">address</span><span class="sxs-lookup"><span data-stu-id="04602-117">address</span></span>             | <span data-ttu-id="04602-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04602-118">String</span></span>      | <span data-ttu-id="04602-119">O endereço de email do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="04602-119">The email address of the user who shared the item.</span></span>  |
