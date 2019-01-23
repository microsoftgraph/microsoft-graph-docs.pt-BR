---
title: Tipo de recurso mediaContentRatingFrance
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bb199abfc350a8b88913e353d377745714368c95
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412363"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="4415b-103">Tipo de recurso mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="4415b-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="4415b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="4415b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4415b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4415b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4415b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="4415b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4415b-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4415b-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="4415b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4415b-108">Properties</span></span>
|<span data-ttu-id="4415b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4415b-109">Property</span></span>|<span data-ttu-id="4415b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4415b-110">Type</span></span>|<span data-ttu-id="4415b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4415b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4415b-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="4415b-112">movieRating</span></span>|[<span data-ttu-id="4415b-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="4415b-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="4415b-114">Filmes selecionado de classificação da França.</span><span class="sxs-lookup"><span data-stu-id="4415b-114">Movies rating selected for France.</span></span> <span data-ttu-id="4415b-115">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="4415b-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="4415b-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="4415b-116">tvRating</span></span>|[<span data-ttu-id="4415b-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="4415b-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="4415b-118">Classificação de TV selecionada para França.</span><span class="sxs-lookup"><span data-stu-id="4415b-118">TV rating selected for France.</span></span> <span data-ttu-id="4415b-119">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="4415b-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4415b-120">Relações</span><span class="sxs-lookup"><span data-stu-id="4415b-120">Relationships</span></span>
<span data-ttu-id="4415b-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4415b-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4415b-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4415b-122">JSON Representation</span></span>
<span data-ttu-id="4415b-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4415b-123">Here is a JSON representation of the resource.</span></span>
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




