---
title: Tipo de recurso do teamworkBot
description: Um bot no ecossistema do Microsoft Teams.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 99bdde9a4ff26945dd5aa040f2741fdf50c1273b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50476402"
---
# <a name="teamworkbot-resource-type"></a><span data-ttu-id="7f421-103">Tipo de recurso do teamworkBot</span><span class="sxs-lookup"><span data-stu-id="7f421-103">teamworkBot resource type</span></span>

<span data-ttu-id="7f421-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f421-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7f421-105">Representa um bot no ecossistema do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7f421-105">Represents a bot in the Microsoft Teams ecosystem.</span></span>

## <a name="methods"></a><span data-ttu-id="7f421-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="7f421-106">Methods</span></span>
|<span data-ttu-id="7f421-107">Método</span><span class="sxs-lookup"><span data-stu-id="7f421-107">Method</span></span>|<span data-ttu-id="7f421-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7f421-108">Return type</span></span>|<span data-ttu-id="7f421-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f421-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7f421-110">Obter bot</span><span class="sxs-lookup"><span data-stu-id="7f421-110">Get bot</span></span>](../api/teamworkbot-get.md)|[<span data-ttu-id="7f421-111">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="7f421-111">teamworkBot</span></span>](../resources/teamworkbot.md)|<span data-ttu-id="7f421-112">Leia as propriedades e as relações de um objeto [teamworkBot.](../resources/teamworkbot.md)</span><span class="sxs-lookup"><span data-stu-id="7f421-112">Read the properties and relationships of a [teamworkBot](../resources/teamworkbot.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7f421-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f421-113">Properties</span></span>
|<span data-ttu-id="7f421-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f421-114">Property</span></span>|<span data-ttu-id="7f421-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f421-115">Type</span></span>|<span data-ttu-id="7f421-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f421-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f421-117">id</span><span class="sxs-lookup"><span data-stu-id="7f421-117">id</span></span>|<span data-ttu-id="7f421-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f421-118">String</span></span>|<span data-ttu-id="7f421-119">A ID do bot associado ao [teamsAppDefinition específico.](../resources/teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7f421-119">The ID of the bot associated with the specific [teamsAppDefinition](../resources/teamsappdefinition.md).</span></span> <span data-ttu-id="7f421-120">Esse valor geralmente é um GUID.</span><span class="sxs-lookup"><span data-stu-id="7f421-120">This value is usually a GUID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f421-121">Relações</span><span class="sxs-lookup"><span data-stu-id="7f421-121">Relationships</span></span>
<span data-ttu-id="7f421-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7f421-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f421-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f421-123">JSON representation</span></span>
<span data-ttu-id="7f421-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f421-124">The following is a JSON representation of the resource.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="7f421-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="7f421-125">See also</span></span>

- <span data-ttu-id="7f421-126">Para instalar bots em uma equipe, consulte o exemplo 2 em [Listar aplicativos em equipe](../api/team-list-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="7f421-126">To get bots installed in a team, see example 2 in [List apps in team](../api/team-list-installedapps.md).</span></span> <!-- - To get bots installed in a chat, see example 2 in [List apps in chat](../api/chat-list-installedapps.md). -->
- <span data-ttu-id="7f421-127">Para instalar bots no escopo pessoal de um usuário, consulte o exemplo 2 em Aplicativos de [lista instalados para usuário](../api/userteamwork-list-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="7f421-127">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](../api/userteamwork-list-installedapps.md).</span></span>



