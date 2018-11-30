---
title: Tipo de recurso mediaContentRatingFrance
description: Ainda não documentado
ms.openlocfilehash: dabadb4d03181d3cd66db582005c4ec58f28aa9d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035063"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="d6237-103">Tipo de recurso mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="d6237-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="d6237-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d6237-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6237-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d6237-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6237-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d6237-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6237-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6237-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="d6237-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6237-108">Properties</span></span>
|<span data-ttu-id="d6237-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6237-109">Property</span></span>|<span data-ttu-id="d6237-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6237-110">Type</span></span>|<span data-ttu-id="d6237-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6237-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6237-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="d6237-112">movieRating</span></span>|[<span data-ttu-id="d6237-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="d6237-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="d6237-114">Filmes selecionado de classificação da França.</span><span class="sxs-lookup"><span data-stu-id="d6237-114">Movies rating selected for France.</span></span> <span data-ttu-id="d6237-115">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="d6237-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="d6237-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="d6237-116">tvRating</span></span>|[<span data-ttu-id="d6237-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d6237-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="d6237-118">Classificação de TV selecionada para França.</span><span class="sxs-lookup"><span data-stu-id="d6237-118">TV rating selected for France.</span></span> <span data-ttu-id="d6237-119">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="d6237-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6237-120">Relações</span><span class="sxs-lookup"><span data-stu-id="d6237-120">Relationships</span></span>
<span data-ttu-id="d6237-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6237-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6237-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6237-122">JSON Representation</span></span>
<span data-ttu-id="d6237-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6237-123">Here is a JSON representation of the resource.</span></span>
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





