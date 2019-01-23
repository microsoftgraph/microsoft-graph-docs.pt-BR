---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a5a1b61069aa3568c8cb017c6c28bb3e992c38b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394513"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="7229d-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="7229d-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="7229d-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7229d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7229d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7229d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7229d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7229d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7229d-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7229d-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7229d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7229d-108">Properties</span></span>
|<span data-ttu-id="7229d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7229d-109">Property</span></span>|<span data-ttu-id="7229d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7229d-110">Type</span></span>|<span data-ttu-id="7229d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7229d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7229d-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="7229d-112">movieRating</span></span>|[<span data-ttu-id="7229d-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="7229d-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="7229d-114">Filmes classificação selecionado para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="7229d-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="7229d-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="7229d-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="7229d-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="7229d-116">tvRating</span></span>|[<span data-ttu-id="7229d-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="7229d-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="7229d-118">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="7229d-118">TV rating selected for Germany.</span></span> <span data-ttu-id="7229d-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="7229d-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7229d-120">Relações</span><span class="sxs-lookup"><span data-stu-id="7229d-120">Relationships</span></span>
<span data-ttu-id="7229d-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7229d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7229d-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7229d-122">JSON Representation</span></span>
<span data-ttu-id="7229d-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7229d-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```




