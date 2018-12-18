---
title: Tipo de recurso mediaContentRatingJapan
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 98af9a6678b26c2cef15950cae769f3057009479
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337426"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="d5578-103">Tipo de recurso mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="d5578-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="d5578-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d5578-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5578-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d5578-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5578-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d5578-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5578-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d5578-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="d5578-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5578-108">Properties</span></span>
|<span data-ttu-id="d5578-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5578-109">Property</span></span>|<span data-ttu-id="d5578-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5578-110">Type</span></span>|<span data-ttu-id="d5578-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5578-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5578-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="d5578-112">movieRating</span></span>|[<span data-ttu-id="d5578-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="d5578-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="d5578-114">Filmes classificação selecionado para japonês.</span><span class="sxs-lookup"><span data-stu-id="d5578-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="d5578-115">Os possíveis valores são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="d5578-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="d5578-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="d5578-116">tvRating</span></span>|[<span data-ttu-id="d5578-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d5578-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="d5578-118">Classificação de TV selecionada para japonês.</span><span class="sxs-lookup"><span data-stu-id="d5578-118">TV rating selected for Japan.</span></span> <span data-ttu-id="d5578-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="d5578-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5578-120">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="d5578-120">Relationships</span></span>
<span data-ttu-id="d5578-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5578-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d5578-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5578-122">JSON Representation</span></span>
<span data-ttu-id="d5578-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5578-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```





