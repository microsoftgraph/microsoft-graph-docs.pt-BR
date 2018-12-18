---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: b7e02226ccea817a609d6e7f3059bff8e6bdb9ce
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318358"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="3719e-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="3719e-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="3719e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3719e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3719e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3719e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3719e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3719e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3719e-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3719e-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3719e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3719e-108">Properties</span></span>
|<span data-ttu-id="3719e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3719e-109">Property</span></span>|<span data-ttu-id="3719e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3719e-110">Type</span></span>|<span data-ttu-id="3719e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3719e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3719e-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="3719e-112">movieRating</span></span>|[<span data-ttu-id="3719e-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="3719e-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="3719e-114">Filmes classificação selecionado para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="3719e-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="3719e-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="3719e-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="3719e-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="3719e-116">tvRating</span></span>|[<span data-ttu-id="3719e-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="3719e-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="3719e-118">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="3719e-118">TV rating selected for Germany.</span></span> <span data-ttu-id="3719e-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="3719e-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3719e-120">Relações</span><span class="sxs-lookup"><span data-stu-id="3719e-120">Relationships</span></span>
<span data-ttu-id="3719e-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3719e-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3719e-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3719e-122">JSON Representation</span></span>
<span data-ttu-id="3719e-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3719e-123">Here is a JSON representation of the resource.</span></span>
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





