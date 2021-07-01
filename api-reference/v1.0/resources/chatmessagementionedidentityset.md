---
title: Tipo de recurso chatMessageMentionedIdentitySet
description: Representa o recurso @mentioned em uma mensagem em um chat ou em um canal.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 42369cd75b030ee7c46a6f270fcee548f42338a4
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211061"
---
# <a name="chatmessagementionedidentityset-resource-type"></a><span data-ttu-id="a583d-103">Tipo de recurso chatMessageMentionedIdentitySet</span><span class="sxs-lookup"><span data-stu-id="a583d-103">chatMessageMentionedIdentitySet resource type</span></span>

<span data-ttu-id="a583d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a583d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a583d-105">Representa o recurso (usuário, aplicativo ou conversa) @mentioned em uma [mensagem](../resources/chatmessage.md) em um chat ou em um canal.</span><span class="sxs-lookup"><span data-stu-id="a583d-105">Represents the resource (user, application, or conversation) @mentioned in a [message](../resources/chatmessage.md) in a chat or a channel.</span></span>


<span data-ttu-id="a583d-106">Herda de [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="a583d-106">Inherits from [identitySet](../resources/identityset.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a583d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a583d-107">Properties</span></span>
|<span data-ttu-id="a583d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a583d-108">Property</span></span>|<span data-ttu-id="a583d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a583d-109">Type</span></span>|<span data-ttu-id="a583d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a583d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a583d-111">aplicativo</span><span class="sxs-lookup"><span data-stu-id="a583d-111">application</span></span>|[<span data-ttu-id="a583d-112">identity</span><span class="sxs-lookup"><span data-stu-id="a583d-112">identity</span></span>](../resources/identity.md)|<span data-ttu-id="a583d-113">Herdado [de identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="a583d-113">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="a583d-114">Se presente, representa um aplicativo (por exemplo, bot) @mentioned em uma [mensagem](../resources/chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="a583d-114">If present, represents an application (for example, bot) @mentioned in a [message](../resources/chatmessage.md).</span></span>|
|<span data-ttu-id="a583d-115">conversa</span><span class="sxs-lookup"><span data-stu-id="a583d-115">conversation</span></span>|[<span data-ttu-id="a583d-116">teamworkConversationIdentity</span><span class="sxs-lookup"><span data-stu-id="a583d-116">teamworkConversationIdentity</span></span>](../resources/teamworkconversationidentity.md)|<span data-ttu-id="a583d-117">Se presente, representa uma conversa (por exemplo, equipe ou canal) @mentioned em uma [mensagem](../resources/chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="a583d-117">If present, represents a conversation (for example, team or channel) @mentioned in a [message](../resources/chatmessage.md).</span></span>|
|<span data-ttu-id="a583d-118">device</span><span class="sxs-lookup"><span data-stu-id="a583d-118">device</span></span>|[<span data-ttu-id="a583d-119">identity</span><span class="sxs-lookup"><span data-stu-id="a583d-119">identity</span></span>](../resources/identity.md)|<span data-ttu-id="a583d-120">Herdado [de identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="a583d-120">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="a583d-121">Não é usado porque não tem suporte para @mention dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a583d-121">Not used because it's not supported to @mention devices.</span></span>|
|<span data-ttu-id="a583d-122">user</span><span class="sxs-lookup"><span data-stu-id="a583d-122">user</span></span>|[<span data-ttu-id="a583d-123">identity</span><span class="sxs-lookup"><span data-stu-id="a583d-123">identity</span></span>](../resources/identity.md)|<span data-ttu-id="a583d-124">Herdado [de identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="a583d-124">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="a583d-125">Se presente, representa um usuário @mentioned em uma [mensagem](../resources/chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="a583d-125">If present, represents a user @mentioned in a [message](../resources/chatmessage.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="a583d-126">Relações</span><span class="sxs-lookup"><span data-stu-id="a583d-126">Relationships</span></span>
<span data-ttu-id="a583d-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a583d-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a583d-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a583d-128">JSON representation</span></span>
<span data-ttu-id="a583d-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a583d-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageMentionedIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageMentionedIdentitySet",
  "user": {
    "@odata.type": "microsoft.graph.identity"
  },
  "application": {
    "@odata.type": "microsoft.graph.identity"
  },
  "device": {
    "@odata.type": "microsoft.graph.identity"
  },
  "conversation": {
    "@odata.type": "microsoft.graph.teamworkConversationIdentity"
  }
}
```