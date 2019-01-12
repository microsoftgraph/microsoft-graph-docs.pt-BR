---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5147cc307c39187b2daab4cd4031bf449f7cc4e5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962986"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="cd15d-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="cd15d-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="cd15d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cd15d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd15d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cd15d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cd15d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cd15d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd15d-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cd15d-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="cd15d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd15d-108">Properties</span></span>
|<span data-ttu-id="cd15d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd15d-109">Property</span></span>|<span data-ttu-id="cd15d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd15d-110">Type</span></span>|<span data-ttu-id="cd15d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd15d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd15d-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="cd15d-112">movieRating</span></span>|[<span data-ttu-id="cd15d-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="cd15d-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="cd15d-114">Filmes selecionado para Austrália de classificação.</span><span class="sxs-lookup"><span data-stu-id="cd15d-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="cd15d-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="cd15d-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="cd15d-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="cd15d-116">tvRating</span></span>|[<span data-ttu-id="cd15d-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="cd15d-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="cd15d-118">Classificação de TV selecionada para Austrália.</span><span class="sxs-lookup"><span data-stu-id="cd15d-118">TV rating selected for Australia.</span></span> <span data-ttu-id="cd15d-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="cd15d-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd15d-120">Relações</span><span class="sxs-lookup"><span data-stu-id="cd15d-120">Relationships</span></span>
<span data-ttu-id="cd15d-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd15d-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cd15d-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd15d-122">JSON Representation</span></span>
<span data-ttu-id="cd15d-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd15d-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```





