---
title: Tipo de recurso mediaContentRatingUnitedKingdom
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7d21ac4650072c4523f9e120d5d73ad393686635
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408072"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="6685e-103">Tipo de recurso mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="6685e-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="6685e-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="6685e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6685e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6685e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6685e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="6685e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6685e-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6685e-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6685e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6685e-108">Properties</span></span>
|<span data-ttu-id="6685e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6685e-109">Property</span></span>|<span data-ttu-id="6685e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6685e-110">Type</span></span>|<span data-ttu-id="6685e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6685e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6685e-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="6685e-112">movieRating</span></span>|[<span data-ttu-id="6685e-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="6685e-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="6685e-114">Filmes classificação selecionado para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="6685e-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="6685e-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="6685e-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="6685e-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="6685e-116">tvRating</span></span>|[<span data-ttu-id="6685e-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6685e-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="6685e-118">Classificação de TV selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="6685e-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="6685e-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="6685e-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6685e-120">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="6685e-120">Relationships</span></span>
<span data-ttu-id="6685e-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6685e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6685e-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6685e-122">JSON Representation</span></span>
<span data-ttu-id="6685e-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6685e-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```




