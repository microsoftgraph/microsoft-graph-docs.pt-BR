---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 99b67a5d2f65b9ccf29ba3ce1a8c5a214f92535c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825610"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="1a9b7-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="1a9b7-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="1a9b7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1a9b7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a9b7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1a9b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a9b7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1a9b7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a9b7-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1a9b7-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="1a9b7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a9b7-108">Properties</span></span>
|<span data-ttu-id="1a9b7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a9b7-109">Property</span></span>|<span data-ttu-id="1a9b7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a9b7-110">Type</span></span>|<span data-ttu-id="1a9b7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a9b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a9b7-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="1a9b7-112">movieRating</span></span>|[<span data-ttu-id="1a9b7-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="1a9b7-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="1a9b7-114">Filmes classificação selecionado para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="1a9b7-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="1a9b7-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="1a9b7-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="1a9b7-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="1a9b7-116">tvRating</span></span>|[<span data-ttu-id="1a9b7-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1a9b7-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="1a9b7-118">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="1a9b7-118">TV rating selected for Germany.</span></span> <span data-ttu-id="1a9b7-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="1a9b7-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a9b7-120">Relações</span><span class="sxs-lookup"><span data-stu-id="1a9b7-120">Relationships</span></span>
<span data-ttu-id="1a9b7-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a9b7-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1a9b7-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a9b7-122">JSON Representation</span></span>
<span data-ttu-id="1a9b7-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a9b7-123">Here is a JSON representation of the resource.</span></span>
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





