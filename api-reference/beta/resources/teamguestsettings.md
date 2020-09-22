---
title: tipo de recurso teamGuestSettings
description: Configurações que definem se os convidados podem criar, atualizar ou excluir canais na equipe.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 49b50293524b35145cb23d27ab630c64caf2ca43
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046648"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="ba05f-103">tipo de recurso teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="ba05f-103">teamGuestSettings resource type</span></span>

<span data-ttu-id="ba05f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba05f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba05f-105">Configurações para configurar se os convidados podem criar, atualizar ou excluir canais na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="ba05f-105">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ba05f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba05f-106">Properties</span></span>
| <span data-ttu-id="ba05f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba05f-107">Property</span></span>     | <span data-ttu-id="ba05f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba05f-108">Type</span></span>   |<span data-ttu-id="ba05f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba05f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba05f-110">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="ba05f-110">allowCreateUpdateChannels</span></span>|<span data-ttu-id="ba05f-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba05f-111">Boolean</span></span>|<span data-ttu-id="ba05f-112">Se definido como true, os convidados podem adicionar e atualizar canais.</span><span class="sxs-lookup"><span data-stu-id="ba05f-112">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="ba05f-113">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="ba05f-113">allowDeleteChannels</span></span>|<span data-ttu-id="ba05f-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba05f-114">Boolean</span></span>|<span data-ttu-id="ba05f-115">Se definido como true, os convidados podem excluir canais.</span><span class="sxs-lookup"><span data-stu-id="ba05f-115">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba05f-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba05f-116">JSON representation</span></span>

<span data-ttu-id="ba05f-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba05f-117">The following is a JSON representation of the resource.</span></span>

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


