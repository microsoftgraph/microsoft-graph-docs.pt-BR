---
title: tipo de recurso de teamGuestSettings
description: Configurações para configurar se os convidados podem criar, atualizar ou excluir canais na equipe de.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 4d76ffcbc5ec675ee670394854183c07721c0af9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522305"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="2a834-103">tipo de recurso de teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="2a834-103">teamGuestSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a834-104">Configurações para configurar se os convidados podem criar, atualizar ou excluir canais em que a [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="2a834-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2a834-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2a834-105">Properties</span></span>
| <span data-ttu-id="2a834-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a834-106">Property</span></span>     | <span data-ttu-id="2a834-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a834-107">Type</span></span>   |<span data-ttu-id="2a834-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a834-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a834-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="2a834-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="2a834-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="2a834-110">Boolean</span></span>|<span data-ttu-id="2a834-111">Se definido como true, convidados pode adicionar e atualizar os canais.</span><span class="sxs-lookup"><span data-stu-id="2a834-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="2a834-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="2a834-112">allowDeleteChannels</span></span>|<span data-ttu-id="2a834-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="2a834-113">Boolean</span></span>|<span data-ttu-id="2a834-114">Se definido como true, convidados pode excluir canais.</span><span class="sxs-lookup"><span data-stu-id="2a834-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a834-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2a834-115">JSON representation</span></span>

<span data-ttu-id="2a834-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2a834-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/teamguestsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
