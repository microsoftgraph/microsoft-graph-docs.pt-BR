---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
ms.openlocfilehash: e7650d7155c06ff30b541d873830865bed1d92ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040438"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="bdcd9-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="bdcd9-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="bdcd9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bdcd9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdcd9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bdcd9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bdcd9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bdcd9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdcd9-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bdcd9-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="bdcd9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bdcd9-108">Properties</span></span>
|<span data-ttu-id="bdcd9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdcd9-109">Property</span></span>|<span data-ttu-id="bdcd9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdcd9-110">Type</span></span>|<span data-ttu-id="bdcd9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdcd9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdcd9-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="bdcd9-112">movieRating</span></span>|[<span data-ttu-id="bdcd9-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="bdcd9-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="bdcd9-114">Filmes selecionado para a Nova Zelândia de classificação.</span><span class="sxs-lookup"><span data-stu-id="bdcd9-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="bdcd9-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="bdcd9-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="bdcd9-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="bdcd9-116">tvRating</span></span>|[<span data-ttu-id="bdcd9-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="bdcd9-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="bdcd9-118">Classificação de TV selecionada para a Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="bdcd9-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="bdcd9-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="bdcd9-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdcd9-120">Relações</span><span class="sxs-lookup"><span data-stu-id="bdcd9-120">Relationships</span></span>
<span data-ttu-id="bdcd9-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bdcd9-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bdcd9-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bdcd9-122">JSON Representation</span></span>
<span data-ttu-id="bdcd9-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bdcd9-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```





