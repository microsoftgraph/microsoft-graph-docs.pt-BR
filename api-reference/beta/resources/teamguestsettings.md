---
title: tipo de recurso teamGuestSettings
description: Configurações que definem se os convidados podem criar, atualizar ou excluir canais na equipe.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: be38d577d52e0086059f9a5627c670fb537941ce
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519943"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="771d0-103">tipo de recurso teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="771d0-103">teamGuestSettings resource type</span></span>

<span data-ttu-id="771d0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="771d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="771d0-105">Configurações para configurar se os convidados podem criar, atualizar ou excluir canais na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="771d0-105">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="771d0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="771d0-106">Properties</span></span>
| <span data-ttu-id="771d0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="771d0-107">Property</span></span>     | <span data-ttu-id="771d0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="771d0-108">Type</span></span>   |<span data-ttu-id="771d0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="771d0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="771d0-110">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="771d0-110">allowCreateUpdateChannels</span></span>|<span data-ttu-id="771d0-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="771d0-111">Boolean</span></span>|<span data-ttu-id="771d0-112">Se definido como true, os convidados podem adicionar e atualizar canais.</span><span class="sxs-lookup"><span data-stu-id="771d0-112">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="771d0-113">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="771d0-113">allowDeleteChannels</span></span>|<span data-ttu-id="771d0-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="771d0-114">Boolean</span></span>|<span data-ttu-id="771d0-115">Se definido como true, os convidados podem excluir canais.</span><span class="sxs-lookup"><span data-stu-id="771d0-115">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="771d0-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="771d0-116">JSON representation</span></span>

<span data-ttu-id="771d0-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="771d0-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
