---
title: insightIdentity
description: Tipo complexo contendo propriedades de itens compartilhados.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: f4b8bc6b66598753c0755d249ab37283810e8db7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054865"
---
# <a name="insightidentity"></a><span data-ttu-id="caec3-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="caec3-103">insightIdentity</span></span>

<span data-ttu-id="caec3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="caec3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="caec3-105">Tipo complexo contendo propriedades de itens do [sharedInsight](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="caec3-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="caec3-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="caec3-106">JSON representation</span></span>
<span data-ttu-id="caec3-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="caec3-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="caec3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="caec3-108">Properties</span></span>

| <span data-ttu-id="caec3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="caec3-109">Property</span></span>              | <span data-ttu-id="caec3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="caec3-110">Type</span></span>          | <span data-ttu-id="caec3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="caec3-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="caec3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="caec3-112">displayName</span></span>       | <span data-ttu-id="caec3-113">String</span><span class="sxs-lookup"><span data-stu-id="caec3-113">String</span></span>          | <span data-ttu-id="caec3-114">O nome de exibição do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="caec3-114">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="caec3-115">id</span><span class="sxs-lookup"><span data-stu-id="caec3-115">id</span></span>              | <span data-ttu-id="caec3-116">String</span><span class="sxs-lookup"><span data-stu-id="caec3-116">String</span></span>        | <span data-ttu-id="caec3-117">A ID do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="caec3-117">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="caec3-118">address</span><span class="sxs-lookup"><span data-stu-id="caec3-118">address</span></span>             | <span data-ttu-id="caec3-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="caec3-119">String</span></span>      | <span data-ttu-id="caec3-120">O endereço de email do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="caec3-120">The email address of the user who shared the item.</span></span>  |

