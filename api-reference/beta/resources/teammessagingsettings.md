---
title: tipo de recurso de teamMessagingSettings
description: Configurações para configurar mensagens e menções na equipe de.
ms.openlocfilehash: 51a0fb53079e8fd79f469f022efb2f293e9a6cba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035202"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="66992-103">tipo de recurso de teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="66992-103">teamMessagingSettings resource type</span></span>

> <span data-ttu-id="66992-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="66992-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66992-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="66992-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66992-106">Configurações para configurar mensagens e menções na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="66992-106">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="66992-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66992-107">Properties</span></span>
| <span data-ttu-id="66992-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66992-108">Property</span></span>     | <span data-ttu-id="66992-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="66992-109">Type</span></span>   |<span data-ttu-id="66992-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="66992-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66992-111">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="66992-111">allowUserEditMessages</span></span>|<span data-ttu-id="66992-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="66992-112">Boolean</span></span>|<span data-ttu-id="66992-113">Se definido como true, os usuários pode editar suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="66992-113">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="66992-114">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="66992-114">allowUserDeleteMessages</span></span>|<span data-ttu-id="66992-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="66992-115">Boolean</span></span>|<span data-ttu-id="66992-116">Se definido como true, os usuários pode excluir suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="66992-116">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="66992-117">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="66992-117">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="66992-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="66992-118">Boolean</span></span>|<span data-ttu-id="66992-119">Se definido como true, proprietários pode excluir qualquer mensagem.</span><span class="sxs-lookup"><span data-stu-id="66992-119">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="66992-120">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="66992-120">allowTeamMentions</span></span>|<span data-ttu-id="66992-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="66992-121">Boolean</span></span>|<span data-ttu-id="66992-122">Se definido como true, @team menções são permitidas.</span><span class="sxs-lookup"><span data-stu-id="66992-122">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="66992-123">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="66992-123">allowChannelMentions</span></span>|<span data-ttu-id="66992-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="66992-124">Boolean</span></span>|<span data-ttu-id="66992-125">Se definido como true, @channel menções são permitidas.</span><span class="sxs-lookup"><span data-stu-id="66992-125">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66992-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66992-126">JSON representation</span></span>

<span data-ttu-id="66992-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66992-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
