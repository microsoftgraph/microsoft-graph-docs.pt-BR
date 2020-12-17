---
title: tipo de recurso teamworkBot
description: Um bot no ecossistema do Microsoft Teams.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 383c646fdb30d082daa73e37fd227238db195b6b
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706255"
---
# <a name="teamworkbot-resource-type"></a><span data-ttu-id="18722-103">tipo de recurso teamworkBot</span><span class="sxs-lookup"><span data-stu-id="18722-103">teamworkBot resource type</span></span>

<span data-ttu-id="18722-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18722-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18722-105">Representa um bot no ecossistema do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="18722-105">Represents a bot in the Microsoft Teams ecosystem.</span></span>

## <a name="methods"></a><span data-ttu-id="18722-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="18722-106">Methods</span></span>
|<span data-ttu-id="18722-107">Método</span><span class="sxs-lookup"><span data-stu-id="18722-107">Method</span></span>|<span data-ttu-id="18722-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="18722-108">Return type</span></span>|<span data-ttu-id="18722-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="18722-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="18722-110">Obter bot</span><span class="sxs-lookup"><span data-stu-id="18722-110">Get bot</span></span>](../api/teamworkbot-get.md)|[<span data-ttu-id="18722-111">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="18722-111">teamworkBot</span></span>](../resources/teamworkbot.md)|<span data-ttu-id="18722-112">Leia as propriedades e os relacionamentos de um objeto [teamworkBot](../resources/teamworkbot.md) .</span><span class="sxs-lookup"><span data-stu-id="18722-112">Read the properties and relationships of a [teamworkBot](../resources/teamworkbot.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="18722-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18722-113">Properties</span></span>
|<span data-ttu-id="18722-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18722-114">Property</span></span>|<span data-ttu-id="18722-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="18722-115">Type</span></span>|<span data-ttu-id="18722-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="18722-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18722-117">id</span><span class="sxs-lookup"><span data-stu-id="18722-117">id</span></span>|<span data-ttu-id="18722-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18722-118">String</span></span>|<span data-ttu-id="18722-119">A ID do bot associada ao [teamsAppDefinition](../resources/teamsappdefinition.md)específico.</span><span class="sxs-lookup"><span data-stu-id="18722-119">The id of the bot associated with the specific [teamsAppDefinition](../resources/teamsappdefinition.md).</span></span> <span data-ttu-id="18722-120">Esse valor geralmente é um GUID.</span><span class="sxs-lookup"><span data-stu-id="18722-120">This value is usually a GUID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18722-121">Relações</span><span class="sxs-lookup"><span data-stu-id="18722-121">Relationships</span></span>
<span data-ttu-id="18722-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18722-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="18722-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18722-123">JSON representation</span></span>
<span data-ttu-id="18722-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18722-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkBot",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkBot",
  "id": "String (identifier)"
}
```

## <a name="see-also"></a><span data-ttu-id="18722-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="18722-125">See also</span></span>

- <span data-ttu-id="18722-126">Para obter bots instalados em uma equipe, confira o exemplo 2 em [list apps in Team](../api/team-list-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="18722-126">To get bots installed in a team, see example 2 in [List apps in team](../api/team-list-installedapps.md).</span></span>
- <span data-ttu-id="18722-127">Para obter bots instalados em um chat, confira o exemplo 2 em [listar aplicativos no chat](../api/chat-list-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="18722-127">To get bots installed in a chat, see example 2 in [List apps in chat](../api/chat-list-installedapps.md).</span></span>
- <span data-ttu-id="18722-128">Para obter bots instalados no escopo pessoal de um usuário, confira o exemplo 2 em [listar aplicativos instalados para o usuário](../api/userteamwork-list-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="18722-128">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](../api/userteamwork-list-installedapps.md).</span></span>



