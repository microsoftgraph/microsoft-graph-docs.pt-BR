---
title: Tipo de recurso mediaContentRatingFrance
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e149077493280145b2681cc2ad0111ec45534a0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862311"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="ee8cc-103">Tipo de recurso mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="ee8cc-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="ee8cc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ee8cc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee8cc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ee8cc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee8cc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ee8cc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee8cc-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ee8cc-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ee8cc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee8cc-108">Properties</span></span>
|<span data-ttu-id="ee8cc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee8cc-109">Property</span></span>|<span data-ttu-id="ee8cc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee8cc-110">Type</span></span>|<span data-ttu-id="ee8cc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee8cc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee8cc-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="ee8cc-112">movieRating</span></span>|[<span data-ttu-id="ee8cc-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="ee8cc-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="ee8cc-114">Filmes selecionado de classificação da França.</span><span class="sxs-lookup"><span data-stu-id="ee8cc-114">Movies rating selected for France.</span></span> <span data-ttu-id="ee8cc-115">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="ee8cc-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="ee8cc-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="ee8cc-116">tvRating</span></span>|[<span data-ttu-id="ee8cc-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="ee8cc-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="ee8cc-118">Classificação de TV selecionada para França.</span><span class="sxs-lookup"><span data-stu-id="ee8cc-118">TV rating selected for France.</span></span> <span data-ttu-id="ee8cc-119">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="ee8cc-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee8cc-120">Relações</span><span class="sxs-lookup"><span data-stu-id="ee8cc-120">Relationships</span></span>
<span data-ttu-id="ee8cc-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee8cc-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ee8cc-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee8cc-122">JSON Representation</span></span>
<span data-ttu-id="ee8cc-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee8cc-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```





