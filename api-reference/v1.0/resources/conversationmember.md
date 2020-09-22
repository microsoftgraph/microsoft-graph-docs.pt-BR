---
title: tipo de recurso conversationMember
description: Representa o usuário em uma conversa.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e2c888ea55b331762761857c14b4710bf582be3f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056916"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="0f08d-103">tipo de recurso conversationMember</span><span class="sxs-lookup"><span data-stu-id="0f08d-103">conversationMember resource type</span></span>

<span data-ttu-id="0f08d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f08d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f08d-105">Representa um usuário em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="0f08d-105">Represents a user in a [team](team.md).</span></span>
<span data-ttu-id="0f08d-106">Confira também [aadUserConversationMember](aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="0f08d-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0f08d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f08d-107">Properties</span></span>

| <span data-ttu-id="0f08d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f08d-108">Property</span></span>   | <span data-ttu-id="0f08d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f08d-109">Type</span></span> |<span data-ttu-id="0f08d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f08d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f08d-111">id</span><span class="sxs-lookup"><span data-stu-id="0f08d-111">id</span></span>|<span data-ttu-id="0f08d-112">String</span><span class="sxs-lookup"><span data-stu-id="0f08d-112">String</span></span>| <span data-ttu-id="0f08d-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0f08d-113">Read-only.</span></span> <span data-ttu-id="0f08d-114">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f08d-114">Unique ID of the user.</span></span>|
|<span data-ttu-id="0f08d-115">displayName</span><span class="sxs-lookup"><span data-stu-id="0f08d-115">displayName</span></span>| <span data-ttu-id="0f08d-116">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f08d-116">string</span></span> | <span data-ttu-id="0f08d-117">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f08d-117">The display name of the user.</span></span> |
|<span data-ttu-id="0f08d-118">funções</span><span class="sxs-lookup"><span data-stu-id="0f08d-118">roles</span></span>| <span data-ttu-id="0f08d-119">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f08d-119">string collection</span></span> | <span data-ttu-id="0f08d-120">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="0f08d-120">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0f08d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f08d-121">JSON representation</span></span>

<span data-ttu-id="0f08d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f08d-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "roles": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

