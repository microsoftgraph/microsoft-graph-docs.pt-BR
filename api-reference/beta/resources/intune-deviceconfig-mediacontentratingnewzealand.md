---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a1866a6bf0c8d1849eb2fbf478b4f5d14fa3e5c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916933"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="b7b4e-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="b7b4e-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="b7b4e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b7b4e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7b4e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b7b4e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7b4e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b7b4e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7b4e-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b7b4e-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b7b4e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7b4e-108">Properties</span></span>
|<span data-ttu-id="b7b4e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7b4e-109">Property</span></span>|<span data-ttu-id="b7b4e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7b4e-110">Type</span></span>|<span data-ttu-id="b7b4e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7b4e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7b4e-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="b7b4e-112">movieRating</span></span>|[<span data-ttu-id="b7b4e-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="b7b4e-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="b7b4e-114">Filmes selecionado para a Nova Zelândia de classificação.</span><span class="sxs-lookup"><span data-stu-id="b7b4e-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="b7b4e-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="b7b4e-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="b7b4e-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="b7b4e-116">tvRating</span></span>|[<span data-ttu-id="b7b4e-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b7b4e-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="b7b4e-118">Classificação de TV selecionada para a Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="b7b4e-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="b7b4e-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="b7b4e-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7b4e-120">Relações</span><span class="sxs-lookup"><span data-stu-id="b7b4e-120">Relationships</span></span>
<span data-ttu-id="b7b4e-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b7b4e-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b7b4e-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7b4e-122">JSON Representation</span></span>
<span data-ttu-id="b7b4e-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b7b4e-123">Here is a JSON representation of the resource.</span></span>
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





