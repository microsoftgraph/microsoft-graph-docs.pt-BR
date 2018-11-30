---
title: tipo de recurso de teamFunSettings
description: Configurações para configurar o uso de Giphy, memes e adesivos na equipe de.
ms.openlocfilehash: e8cf62b88a3afa3e5caf6b9425312d7a26af4d20
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033552"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="ee317-103">tipo de recurso de teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="ee317-103">teamFunSettings resource type</span></span>

> <span data-ttu-id="ee317-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ee317-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee317-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ee317-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ee317-106">Configurações para configurar o uso de Giphy, adesivos e memes em [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="ee317-106">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ee317-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee317-107">Properties</span></span>
| <span data-ttu-id="ee317-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee317-108">Property</span></span>     | <span data-ttu-id="ee317-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee317-109">Type</span></span>   |<span data-ttu-id="ee317-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee317-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee317-111">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="ee317-111">allowGiphy</span></span>|<span data-ttu-id="ee317-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="ee317-112">Boolean</span></span>|<span data-ttu-id="ee317-113">Se definido como true, permite que o uso de Giphy.</span><span class="sxs-lookup"><span data-stu-id="ee317-113">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="ee317-114">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="ee317-114">giphyContentRating</span></span>|<span data-ttu-id="ee317-115">Cadeia de caracteres (enum)</span><span class="sxs-lookup"><span data-stu-id="ee317-115">String (enum)</span></span>|<span data-ttu-id="ee317-116">Classificação de conteúdo Giphy.</span><span class="sxs-lookup"><span data-stu-id="ee317-116">Giphy content rating.</span></span> <span data-ttu-id="ee317-117">Os valores possíveis são: `moderate` e `strict`.</span><span class="sxs-lookup"><span data-stu-id="ee317-117">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="ee317-118">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="ee317-118">allowStickersAndMemes</span></span>|<span data-ttu-id="ee317-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="ee317-119">Boolean</span></span>|<span data-ttu-id="ee317-120">Se definido como true, permite que os usuários incluem adesivos e memes.</span><span class="sxs-lookup"><span data-stu-id="ee317-120">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="ee317-121">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="ee317-121">allowCustomMemes</span></span>|<span data-ttu-id="ee317-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="ee317-122">Boolean</span></span>|<span data-ttu-id="ee317-123">Se definido como true, permite que os usuários incluem memes personalizado.</span><span class="sxs-lookup"><span data-stu-id="ee317-123">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee317-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee317-124">JSON representation</span></span>

<span data-ttu-id="ee317-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee317-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
