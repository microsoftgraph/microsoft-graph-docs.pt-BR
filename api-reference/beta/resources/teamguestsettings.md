---
title: tipo de recurso teamGuestSettings
description: Configurações que definem se os convidados podem criar, atualizar ou excluir canais na equipe.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 4d76ffcbc5ec675ee670394854183c07721c0af9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554006"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="cf5b4-103">tipo de recurso teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="cf5b4-103">teamGuestSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf5b4-104">Configurações para configurar se os convidados podem criar, atualizar ou excluir canais na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="cf5b4-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cf5b4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf5b4-105">Properties</span></span>
| <span data-ttu-id="cf5b4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf5b4-106">Property</span></span>     | <span data-ttu-id="cf5b4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf5b4-107">Type</span></span>   |<span data-ttu-id="cf5b4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf5b4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf5b4-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="cf5b4-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="cf5b4-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="cf5b4-110">Boolean</span></span>|<span data-ttu-id="cf5b4-111">Se definido como true, os convidados podem adicionar e atualizar canais.</span><span class="sxs-lookup"><span data-stu-id="cf5b4-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="cf5b4-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="cf5b4-112">allowDeleteChannels</span></span>|<span data-ttu-id="cf5b4-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="cf5b4-113">Boolean</span></span>|<span data-ttu-id="cf5b4-114">Se definido como true, os convidados podem excluir canais.</span><span class="sxs-lookup"><span data-stu-id="cf5b4-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf5b4-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf5b4-115">JSON representation</span></span>

<span data-ttu-id="cf5b4-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf5b4-116">The following is a JSON representation of the resource.</span></span>

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
