---
title: tipo de recurso de teamGuestSettings
description: Configurações para configurar se os convidados podem criar, atualizar ou excluir canais na equipe de.
localization_priority: Normal
ms.openlocfilehash: f0947101fc8de83d1a56ffa922d9b1e2d79d520f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844869"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="b00bf-103">tipo de recurso de teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="b00bf-103">teamGuestSettings resource type</span></span>



<span data-ttu-id="b00bf-104">Configurações para configurar se os convidados podem criar, atualizar ou excluir canais em que a [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="b00bf-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b00bf-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b00bf-105">Properties</span></span>
| <span data-ttu-id="b00bf-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b00bf-106">Property</span></span>     | <span data-ttu-id="b00bf-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b00bf-107">Type</span></span>   |<span data-ttu-id="b00bf-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b00bf-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b00bf-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="b00bf-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="b00bf-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="b00bf-110">Boolean</span></span>|<span data-ttu-id="b00bf-111">Se definido como true, convidados pode adicionar e atualizar os canais.</span><span class="sxs-lookup"><span data-stu-id="b00bf-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="b00bf-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="b00bf-112">allowDeleteChannels</span></span>|<span data-ttu-id="b00bf-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="b00bf-113">Boolean</span></span>|<span data-ttu-id="b00bf-114">Se definido como true, convidados pode excluir canais.</span><span class="sxs-lookup"><span data-stu-id="b00bf-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b00bf-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b00bf-115">JSON representation</span></span>

<span data-ttu-id="b00bf-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b00bf-116">The following is a JSON representation of the resource.</span></span>

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
