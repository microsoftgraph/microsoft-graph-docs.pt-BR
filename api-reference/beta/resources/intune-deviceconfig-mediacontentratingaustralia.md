---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 259860387e005f7fe5bfd2d402be5c03ef21149f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396634"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="e2f23-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="e2f23-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="e2f23-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e2f23-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e2f23-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e2f23-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2f23-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e2f23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2f23-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e2f23-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e2f23-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2f23-108">Properties</span></span>
|<span data-ttu-id="e2f23-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2f23-109">Property</span></span>|<span data-ttu-id="e2f23-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2f23-110">Type</span></span>|<span data-ttu-id="e2f23-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2f23-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2f23-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="e2f23-112">movieRating</span></span>|[<span data-ttu-id="e2f23-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="e2f23-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="e2f23-114">Filmes selecionado para Austrália de classificação.</span><span class="sxs-lookup"><span data-stu-id="e2f23-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="e2f23-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="e2f23-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="e2f23-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="e2f23-116">tvRating</span></span>|[<span data-ttu-id="e2f23-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e2f23-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="e2f23-118">Classificação de TV selecionada para Austrália.</span><span class="sxs-lookup"><span data-stu-id="e2f23-118">TV rating selected for Australia.</span></span> <span data-ttu-id="e2f23-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="e2f23-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2f23-120">Relações</span><span class="sxs-lookup"><span data-stu-id="e2f23-120">Relationships</span></span>
<span data-ttu-id="e2f23-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2f23-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2f23-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2f23-122">JSON Representation</span></span>
<span data-ttu-id="e2f23-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2f23-123">Here is a JSON representation of the resource.</span></span>
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




