---
title: Tipo de recurso teamworkBot
description: Um bot no ecossistema do Microsoft Teams.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3413ee882a7ca387d298b148b37266704558031c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158314"
---
# <a name="teamworkbot-resource-type"></a><span data-ttu-id="c8a5c-103">Tipo de recurso teamworkBot</span><span class="sxs-lookup"><span data-stu-id="c8a5c-103">teamworkBot resource type</span></span>

<span data-ttu-id="c8a5c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8a5c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8a5c-105">Representa um bot no ecossistema do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c8a5c-105">Represents a bot in the Microsoft Teams ecosystem.</span></span>

## <a name="methods"></a><span data-ttu-id="c8a5c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c8a5c-106">Methods</span></span>
|<span data-ttu-id="c8a5c-107">Método</span><span class="sxs-lookup"><span data-stu-id="c8a5c-107">Method</span></span>|<span data-ttu-id="c8a5c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c8a5c-108">Return type</span></span>|<span data-ttu-id="c8a5c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8a5c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c8a5c-110">Obter bot</span><span class="sxs-lookup"><span data-stu-id="c8a5c-110">Get bot</span></span>](../api/teamworkbot-get.md)|[<span data-ttu-id="c8a5c-111">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="c8a5c-111">teamworkBot</span></span>](../resources/teamworkbot.md)|<span data-ttu-id="c8a5c-112">Leia as propriedades e os relacionamentos de um objeto [teamworkBot.](../resources/teamworkbot.md)</span><span class="sxs-lookup"><span data-stu-id="c8a5c-112">Read the properties and relationships of a [teamworkBot](../resources/teamworkbot.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c8a5c-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8a5c-113">Properties</span></span>
|<span data-ttu-id="c8a5c-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8a5c-114">Property</span></span>|<span data-ttu-id="c8a5c-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8a5c-115">Type</span></span>|<span data-ttu-id="c8a5c-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8a5c-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8a5c-117">id</span><span class="sxs-lookup"><span data-stu-id="c8a5c-117">id</span></span>|<span data-ttu-id="c8a5c-118">String</span><span class="sxs-lookup"><span data-stu-id="c8a5c-118">String</span></span>|<span data-ttu-id="c8a5c-119">A id do bot associado ao [teamsAppDefinition específico.](../resources/teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c8a5c-119">The id of the bot associated with the specific [teamsAppDefinition](../resources/teamsappdefinition.md).</span></span> <span data-ttu-id="c8a5c-120">Esse valor geralmente é um GUID.</span><span class="sxs-lookup"><span data-stu-id="c8a5c-120">This value is usually a GUID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8a5c-121">Relações</span><span class="sxs-lookup"><span data-stu-id="c8a5c-121">Relationships</span></span>
<span data-ttu-id="c8a5c-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8a5c-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8a5c-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8a5c-123">JSON representation</span></span>
<span data-ttu-id="c8a5c-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8a5c-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkBot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkBot",
  "id": "String (identifier)"
}
```

## <a name="see-also"></a><span data-ttu-id="c8a5c-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="c8a5c-125">See also</span></span>

- <span data-ttu-id="c8a5c-126">Para instalar bots em uma equipe, confira o exemplo 2 em [Listar aplicativos em equipe.](../api/team-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="c8a5c-126">To get bots installed in a team, see example 2 in [List apps in team](../api/team-list-installedapps.md).</span></span>
- <span data-ttu-id="c8a5c-127">Para instalar bots em um chat, confira o exemplo 2 em Aplicativos [de lista no chat.](../api/chat-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="c8a5c-127">To get bots installed in a chat, see example 2 in [List apps in chat](../api/chat-list-installedapps.md).</span></span>
- <span data-ttu-id="c8a5c-128">Para instalar bots no escopo pessoal de um usuário, confira o exemplo 2 em Aplicativos de [lista instalados para o usuário.](../api/userteamwork-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="c8a5c-128">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](../api/userteamwork-list-installedapps.md).</span></span>



