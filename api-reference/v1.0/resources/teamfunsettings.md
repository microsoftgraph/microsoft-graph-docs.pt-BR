---
title: tipo de recurso teamFunSettings
description: Configurações que definem o uso de Giphy, memes e figurinhas na equipe.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: c701ffe76c82a6cb4b3586272926290f634a02d9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548513"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="269e8-103">tipo de recurso teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="269e8-103">teamFunSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="269e8-104">Configurações para configurar o uso de Giphy, memes e selos na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="269e8-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="269e8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="269e8-105">Properties</span></span>
| <span data-ttu-id="269e8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="269e8-106">Property</span></span>     | <span data-ttu-id="269e8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="269e8-107">Type</span></span>   |<span data-ttu-id="269e8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="269e8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="269e8-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="269e8-109">allowGiphy</span></span>|<span data-ttu-id="269e8-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="269e8-110">Boolean</span></span>|<span data-ttu-id="269e8-111">Se definido como true, habilita o uso do Giphy.</span><span class="sxs-lookup"><span data-stu-id="269e8-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="269e8-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="269e8-112">giphyContentRating</span></span>|<span data-ttu-id="269e8-113">Cadeia de caracteres (enum)</span><span class="sxs-lookup"><span data-stu-id="269e8-113">String (enum)</span></span>|<span data-ttu-id="269e8-114">Classificação de conteúdo do Giphy.</span><span class="sxs-lookup"><span data-stu-id="269e8-114">Giphy content rating.</span></span> <span data-ttu-id="269e8-115">Os valores possíveis são: `moderate` e `strict`.</span><span class="sxs-lookup"><span data-stu-id="269e8-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="269e8-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="269e8-116">allowStickersAndMemes</span></span>|<span data-ttu-id="269e8-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="269e8-117">Boolean</span></span>|<span data-ttu-id="269e8-118">Se definido como true, permite que os usuários incluam adesivos e memes.</span><span class="sxs-lookup"><span data-stu-id="269e8-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="269e8-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="269e8-119">allowCustomMemes</span></span>|<span data-ttu-id="269e8-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="269e8-120">Boolean</span></span>|<span data-ttu-id="269e8-121">Se definido como true, permite que os usuários incluam memes personalizados.</span><span class="sxs-lookup"><span data-stu-id="269e8-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="269e8-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="269e8-122">JSON representation</span></span>

<span data-ttu-id="269e8-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="269e8-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamfunsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
