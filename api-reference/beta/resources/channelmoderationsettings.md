---
title: Tipo de recurso channelModerationSettings
description: Usado para controlar quem pode iniciar novas postagens e responder a postagens em um canal.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b67d55eb57d1a4b554b027270f700cbd590d4416
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796581"
---
# <a name="channelmoderationsettings-resource-type"></a><span data-ttu-id="c94fa-103">Tipo de recurso channelModerationSettings</span><span class="sxs-lookup"><span data-stu-id="c94fa-103">channelModerationSettings resource type</span></span>

<span data-ttu-id="c94fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c94fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c94fa-105">No Microsoft Teams, os proprietários de equipe podem ativar a moderação para um canal para controlar quem pode iniciar novas postagens e responder a postagens nesse canal.</span><span class="sxs-lookup"><span data-stu-id="c94fa-105">In Microsoft Teams, team owners can turn on moderation for a channel to control who can start new posts and reply to posts in that channel.</span></span> <span data-ttu-id="c94fa-106">Por exemplo, os proprietários podem querer fazer o seguinte:</span><span class="sxs-lookup"><span data-stu-id="c94fa-106">For example, owners might want to do the following:</span></span>

- <span data-ttu-id="c94fa-107">Use um canal somente para comunicados.</span><span class="sxs-lookup"><span data-stu-id="c94fa-107">Use a channel for announcements only.</span></span>
- <span data-ttu-id="c94fa-108">Use um canal para discussões em uma equipe de classe onde somente o professor pode iniciar novas discussões.</span><span class="sxs-lookup"><span data-stu-id="c94fa-108">Use a channel for discussions in a class team where only the teacher can start new discussions.</span></span>
- <span data-ttu-id="c94fa-109">Use um canal para problemas em que novas postagens podem ser iniciadas por conectores.</span><span class="sxs-lookup"><span data-stu-id="c94fa-109">Use a channel for livesite issues where new posts can be started by connectors.</span></span>

<span data-ttu-id="c94fa-110">Por padrão, a moderação é, o que significa que as configurações usuais de canal se aplicam aos proprietários da equipe e membros da equipe, com controle adicional para permitir que apenas membros da equipe ou todos, incluindo convidados, iniciem uma nova postagem de `OFF` canal.</span><span class="sxs-lookup"><span data-stu-id="c94fa-110">By default, moderation is `OFF`, which means that the usual channel settings apply to team owners and team members, with additional control to allow only team members or everyone including guests to start a new channel post.</span></span> <span data-ttu-id="c94fa-111">Configurar a moderação do canal `ON` para permitir que apenas moderadores iniciem novas postagens, com controle adicional para membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="c94fa-111">Setting channel moderation to `ON` allows only moderators to start new posts, with additional control for team members.</span></span>

<span data-ttu-id="c94fa-112">Para dar suporte às configurações de moderação de canal por meio das APIs do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="c94fa-112">To support channel moderation settings via Microsoft Graph APIs:</span></span>

- <span data-ttu-id="c94fa-113">Os membros da equipe devem ser capazes de consultar as configurações de moderação do canal.</span><span class="sxs-lookup"><span data-stu-id="c94fa-113">Team members should be able to query channel moderation settings.</span></span>
- <span data-ttu-id="c94fa-114">Os proprietários de equipe devem ser capazes de definir configurações de moderação de canal.</span><span class="sxs-lookup"><span data-stu-id="c94fa-114">Team owners should be able to set channel moderation settings.</span></span>

## <a name="properties"></a><span data-ttu-id="c94fa-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c94fa-115">Properties</span></span>
|<span data-ttu-id="c94fa-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c94fa-116">Property</span></span>|<span data-ttu-id="c94fa-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="c94fa-117">Type</span></span>|<span data-ttu-id="c94fa-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="c94fa-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c94fa-119">allowNewMessageFromBots</span><span class="sxs-lookup"><span data-stu-id="c94fa-119">allowNewMessageFromBots</span></span>|<span data-ttu-id="c94fa-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="c94fa-120">Boolean</span></span>|<span data-ttu-id="c94fa-121">Indica se os bots têm permissão para postar mensagens.</span><span class="sxs-lookup"><span data-stu-id="c94fa-121">Indicates whether bots are allowed to post messages.</span></span>|
|<span data-ttu-id="c94fa-122">allowNewMessageFromConnectors</span><span class="sxs-lookup"><span data-stu-id="c94fa-122">allowNewMessageFromConnectors</span></span>|<span data-ttu-id="c94fa-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="c94fa-123">Boolean</span></span>|<span data-ttu-id="c94fa-124">Indica se os conectores têm permissão para postar mensagens.</span><span class="sxs-lookup"><span data-stu-id="c94fa-124">Indicates whether connectors are allowed to post messages.</span></span>|
|<span data-ttu-id="c94fa-125">replyRestriction</span><span class="sxs-lookup"><span data-stu-id="c94fa-125">replyRestriction</span></span>|<span data-ttu-id="c94fa-126">replyRestriction</span><span class="sxs-lookup"><span data-stu-id="c94fa-126">replyRestriction</span></span>|<span data-ttu-id="c94fa-127">Indica quem tem permissão para responder ao canal de equipes.</span><span class="sxs-lookup"><span data-stu-id="c94fa-127">Indicates who is allowed to reply to the teams channel.</span></span> <span data-ttu-id="c94fa-128">Os valores possíveis são: `everyone`, `authorAndModerators`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c94fa-128">Possible values are: `everyone`, `authorAndModerators`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c94fa-129">userNewMessageRestriction</span><span class="sxs-lookup"><span data-stu-id="c94fa-129">userNewMessageRestriction</span></span>|<span data-ttu-id="c94fa-130">userNewMessageRestriction</span><span class="sxs-lookup"><span data-stu-id="c94fa-130">userNewMessageRestriction</span></span>|<span data-ttu-id="c94fa-131">Indica quem tem permissão para postar mensagens no canal de equipes.</span><span class="sxs-lookup"><span data-stu-id="c94fa-131">Indicates who is allowed to post messages to teams channel.</span></span> <span data-ttu-id="c94fa-132">Os valores possíveis são: `everyone`, `everyoneExceptGuests`, `moderators`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c94fa-132">Possible values are: `everyone`, `everyoneExceptGuests`, `moderators`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c94fa-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c94fa-133">JSON representation</span></span>
<span data-ttu-id="c94fa-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c94fa-134">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelModerationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelModerationSettings",
  "userNewMessageRestriction": "String",
  "replyRestriction": "String",
  "allowNewMessageFromBots": "Boolean",
  "allowNewMessageFromConnectors": "Boolean"
}
```

## <a name="see-also"></a><span data-ttu-id="c94fa-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="c94fa-135">See also</span></span>

- <span data-ttu-id="c94fa-136">Para modificar as configurações de moderação de um canal, consulte o exemplo 2 no [canal de atualização.](../api/channel-patch.md)</span><span class="sxs-lookup"><span data-stu-id="c94fa-136">To modify moderation settings of a channel, see example 2 in [Update channel](../api/channel-patch.md).</span></span>
