---
title: tipo de recurso de teamGuestSettings
description: Configurações para configurar se os convidados podem criar, atualizar ou excluir canais na equipe de.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: cb6e83093945a96784bfb91a76bc343a8c13d0ac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924367"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="70926-103">tipo de recurso de teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="70926-103">teamGuestSettings resource type</span></span>



<span data-ttu-id="70926-104">Configurações para configurar se os convidados podem criar, atualizar ou excluir canais em que a [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="70926-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="70926-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70926-105">Properties</span></span>
| <span data-ttu-id="70926-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70926-106">Property</span></span>     | <span data-ttu-id="70926-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="70926-107">Type</span></span>   |<span data-ttu-id="70926-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="70926-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70926-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="70926-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="70926-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="70926-110">Boolean</span></span>|<span data-ttu-id="70926-111">Se definido como true, convidados pode adicionar e atualizar os canais.</span><span class="sxs-lookup"><span data-stu-id="70926-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="70926-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="70926-112">allowDeleteChannels</span></span>|<span data-ttu-id="70926-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="70926-113">Boolean</span></span>|<span data-ttu-id="70926-114">Se definido como true, convidados pode excluir canais.</span><span class="sxs-lookup"><span data-stu-id="70926-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70926-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70926-115">JSON representation</span></span>

<span data-ttu-id="70926-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70926-116">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
