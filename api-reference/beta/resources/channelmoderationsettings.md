---
title: tipo de recurso channelModerationSettings
description: Usado para controlar quem pode iniciar novas postagens e responder a postagens em um canal.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c2de1c16ed998a0b793d14c6a4d791613e0bef62
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706213"
---
# <a name="channelmoderationsettings-resource-type"></a><span data-ttu-id="32e89-103">tipo de recurso channelModerationSettings</span><span class="sxs-lookup"><span data-stu-id="32e89-103">channelModerationSettings resource type</span></span>

<span data-ttu-id="32e89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32e89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32e89-105">No Microsoft Teams, os proprietários de equipe podem ativar a moderação de um canal para controlar quem pode iniciar novas postagens e responder a postagens nesse canal.</span><span class="sxs-lookup"><span data-stu-id="32e89-105">In Microsoft Teams, team owners can turn on moderation for a channel to control who can start new posts and reply to posts in that channel.</span></span> <span data-ttu-id="32e89-106">Por exemplo, os proprietários podem querer fazer o seguinte:</span><span class="sxs-lookup"><span data-stu-id="32e89-106">For example, owners might want to do the following:</span></span>

- <span data-ttu-id="32e89-107">Usar um canal somente para comunicados.</span><span class="sxs-lookup"><span data-stu-id="32e89-107">Use a channel for announcements only.</span></span>
- <span data-ttu-id="32e89-108">Use um canal para discussões em uma equipe de aula onde apenas o professor pode iniciar novas discussões.</span><span class="sxs-lookup"><span data-stu-id="32e89-108">Use a channel for discussions in a class team where only the teacher can start new discussions.</span></span>
- <span data-ttu-id="32e89-109">Use um canal para problemas de Livesite onde novas postagens podem ser iniciadas por conectores.</span><span class="sxs-lookup"><span data-stu-id="32e89-109">Use a channel for livesite issues where new posts can be started by connectors.</span></span>

<span data-ttu-id="32e89-110">Por padrão, a moderação é `OFF` , o que significa que as configurações de canal usuais se aplicam aos proprietários da equipe e aos membros da equipe, com controle adicional para permitir que somente membros da equipe ou todos, incluindo convidados, iniciem uma nova postagem de canal.</span><span class="sxs-lookup"><span data-stu-id="32e89-110">By default, moderation is `OFF`, which means that the usual channel settings apply to team owners and team members, with additional control to allow only team members or everyone including guests to start a new channel post.</span></span> <span data-ttu-id="32e89-111">Configurar a moderação do canal para `ON` permitir que apenas moderadores iniciem novas postagens, com controle adicional para membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="32e89-111">Setting channel moderation to `ON` allows only moderators to start new posts, with additonal control for team members.</span></span>

<span data-ttu-id="32e89-112">Para dar suporte às configurações de moderação de canal através das APIs do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="32e89-112">To support channel moderation settings via Microsoft Graph APIs:</span></span>

- <span data-ttu-id="32e89-113">Os membros da equipe devem ser capazes de consultar as configurações de moderação do canal.</span><span class="sxs-lookup"><span data-stu-id="32e89-113">Team members should be able to query channel moderation settings.</span></span>
- <span data-ttu-id="32e89-114">Os proprietários de equipe devem ser capazes de definir as configurações de moderação do canal.</span><span class="sxs-lookup"><span data-stu-id="32e89-114">Team owners should be able to set channel moderation settings.</span></span>

## <a name="properties"></a><span data-ttu-id="32e89-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32e89-115">Properties</span></span>
|<span data-ttu-id="32e89-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32e89-116">Property</span></span>|<span data-ttu-id="32e89-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="32e89-117">Type</span></span>|<span data-ttu-id="32e89-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="32e89-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32e89-119">allowNewMessageFromBots</span><span class="sxs-lookup"><span data-stu-id="32e89-119">allowNewMessageFromBots</span></span>|<span data-ttu-id="32e89-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="32e89-120">Boolean</span></span>|<span data-ttu-id="32e89-121">Indica se os bots podem postar mensagens.</span><span class="sxs-lookup"><span data-stu-id="32e89-121">Indicates whether bots are allowed to post messages.</span></span>|
|<span data-ttu-id="32e89-122">allowNewMessageFromConnectors</span><span class="sxs-lookup"><span data-stu-id="32e89-122">allowNewMessageFromConnectors</span></span>|<span data-ttu-id="32e89-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="32e89-123">Boolean</span></span>|<span data-ttu-id="32e89-124">Indica se os conectores têm permissão para postar mensagens.</span><span class="sxs-lookup"><span data-stu-id="32e89-124">Indicates whether connectors are allowed to post messages.</span></span>|
|<span data-ttu-id="32e89-125">replyRestriction</span><span class="sxs-lookup"><span data-stu-id="32e89-125">replyRestriction</span></span>|<span data-ttu-id="32e89-126">replyRestriction</span><span class="sxs-lookup"><span data-stu-id="32e89-126">replyRestriction</span></span>|<span data-ttu-id="32e89-127">Indica quem tem permissão para responder ao canal Teams.</span><span class="sxs-lookup"><span data-stu-id="32e89-127">Indicates who is allowed to reply to the teams channel.</span></span> <span data-ttu-id="32e89-128">Os valores possíveis são: `everyone`, `authorAndModerators`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="32e89-128">Possible values are: `everyone`, `authorAndModerators`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="32e89-129">userNewMessageRestriction</span><span class="sxs-lookup"><span data-stu-id="32e89-129">userNewMessageRestriction</span></span>|<span data-ttu-id="32e89-130">userNewMessageRestriction</span><span class="sxs-lookup"><span data-stu-id="32e89-130">userNewMessageRestriction</span></span>|<span data-ttu-id="32e89-131">Indica quem tem permissão para postar mensagens no canal do teams.</span><span class="sxs-lookup"><span data-stu-id="32e89-131">Indicates who is allowed to post messages to teams channel.</span></span> <span data-ttu-id="32e89-132">Os valores possíveis são: `everyone`, `everyoneExceptGuests`, `moderators`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="32e89-132">Possible values are: `everyone`, `everyoneExceptGuests`, `moderators`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32e89-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32e89-133">JSON representation</span></span>
<span data-ttu-id="32e89-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32e89-134">The following is a JSON representation of the resource.</span></span>
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
