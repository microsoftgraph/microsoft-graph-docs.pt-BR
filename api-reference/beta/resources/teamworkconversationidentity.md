---
title: Tipo de recurso teamworkConversationIdentity
description: Representa uma conversa em Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 84e936368b7cc4589b7611b15cf310f92b055e2a
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211189"
---
# <a name="teamworkconversationidentity-resource-type"></a><span data-ttu-id="a5619-103">Tipo de recurso teamworkConversationIdentity</span><span class="sxs-lookup"><span data-stu-id="a5619-103">teamworkConversationIdentity resource type</span></span>

<span data-ttu-id="a5619-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5619-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5619-105">Representa uma **conversa** (chat, equipe ou canal) no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a5619-105">Represents a **conversation** (chat, team, or channel) in Microsoft Teams.</span></span>

<span data-ttu-id="a5619-106">Herda da [identidade](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="a5619-106">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a5619-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5619-107">Properties</span></span>
|<span data-ttu-id="a5619-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5619-108">Property</span></span>|<span data-ttu-id="a5619-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5619-109">Type</span></span>|<span data-ttu-id="a5619-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5619-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5619-111">conversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="a5619-111">conversationIdentityType</span></span>|<span data-ttu-id="a5619-112">teamworkConversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="a5619-112">teamworkConversationIdentityType</span></span>|<span data-ttu-id="a5619-113">Tipo de conversa.</span><span class="sxs-lookup"><span data-stu-id="a5619-113">Type of conversation.</span></span> <span data-ttu-id="a5619-114">Os valores possíveis são: `team` `channel` , e `chat` .</span><span class="sxs-lookup"><span data-stu-id="a5619-114">Possible values are: `team`, `channel`, and `chat`.</span></span>|
|<span data-ttu-id="a5619-115">displayName</span><span class="sxs-lookup"><span data-stu-id="a5619-115">displayName</span></span>|<span data-ttu-id="a5619-116">String</span><span class="sxs-lookup"><span data-stu-id="a5619-116">String</span></span>|<span data-ttu-id="a5619-117">Herdado da [identidade](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="a5619-117">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="a5619-118">Nome de exibição da conversa.</span><span class="sxs-lookup"><span data-stu-id="a5619-118">Display name of the conversation.</span></span> <span data-ttu-id="a5619-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a5619-119">Optional.</span></span>|
|<span data-ttu-id="a5619-120">id</span><span class="sxs-lookup"><span data-stu-id="a5619-120">id</span></span>|<span data-ttu-id="a5619-121">String</span><span class="sxs-lookup"><span data-stu-id="a5619-121">String</span></span>|<span data-ttu-id="a5619-122">Herdado da [identidade](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="a5619-122">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="a5619-123">ID da conversa.</span><span class="sxs-lookup"><span data-stu-id="a5619-123">ID of the conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5619-124">Relações</span><span class="sxs-lookup"><span data-stu-id="a5619-124">Relationships</span></span>
<span data-ttu-id="a5619-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a5619-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5619-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5619-126">JSON representation</span></span>
<span data-ttu-id="a5619-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a5619-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkConversationIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkConversationIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "conversationIdentityType": "String"
}
```

