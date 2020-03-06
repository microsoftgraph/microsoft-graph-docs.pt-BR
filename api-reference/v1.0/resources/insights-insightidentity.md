---
title: insightIdentity
description: Tipo complexo contendo propriedades de itens compartilhados.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3a23344a18979c7d1aa69b8e841007812797b238
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531298"
---
# <a name="insightidentity"></a><span data-ttu-id="96098-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="96098-103">insightIdentity</span></span>

<span data-ttu-id="96098-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96098-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="96098-105">Tipo complexo contendo propriedades de itens do [sharedInsight](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="96098-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="96098-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96098-106">JSON representation</span></span>
<span data-ttu-id="96098-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="96098-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="96098-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96098-108">Properties</span></span>

| <span data-ttu-id="96098-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96098-109">Property</span></span>              | <span data-ttu-id="96098-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="96098-110">Type</span></span>          | <span data-ttu-id="96098-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="96098-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="96098-112">displayName</span><span class="sxs-lookup"><span data-stu-id="96098-112">displayName</span></span>       | <span data-ttu-id="96098-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96098-113">String</span></span>          | <span data-ttu-id="96098-114">O nome de exibição do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="96098-114">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="96098-115">id</span><span class="sxs-lookup"><span data-stu-id="96098-115">id</span></span>              | <span data-ttu-id="96098-116">String</span><span class="sxs-lookup"><span data-stu-id="96098-116">String</span></span>        | <span data-ttu-id="96098-117">A ID do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="96098-117">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="96098-118">address</span><span class="sxs-lookup"><span data-stu-id="96098-118">address</span></span>             | <span data-ttu-id="96098-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96098-119">String</span></span>      | <span data-ttu-id="96098-120">O endereço de email do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="96098-120">The email address of the user who shared the item.</span></span>  |
