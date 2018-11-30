---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
ms.openlocfilehash: 821a648f839e531c2efaa3da4b4b1aead65c9673
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036597"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="60f77-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="60f77-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="60f77-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="60f77-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60f77-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="60f77-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60f77-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="60f77-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60f77-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="60f77-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="60f77-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60f77-108">Properties</span></span>
|<span data-ttu-id="60f77-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60f77-109">Property</span></span>|<span data-ttu-id="60f77-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="60f77-110">Type</span></span>|<span data-ttu-id="60f77-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="60f77-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60f77-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="60f77-112">movieRating</span></span>|[<span data-ttu-id="60f77-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="60f77-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="60f77-114">Filmes classificação selecionado para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="60f77-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="60f77-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="60f77-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="60f77-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="60f77-116">tvRating</span></span>|[<span data-ttu-id="60f77-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="60f77-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="60f77-118">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="60f77-118">TV rating selected for Germany.</span></span> <span data-ttu-id="60f77-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="60f77-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60f77-120">Relações</span><span class="sxs-lookup"><span data-stu-id="60f77-120">Relationships</span></span>
<span data-ttu-id="60f77-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="60f77-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="60f77-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60f77-122">JSON Representation</span></span>
<span data-ttu-id="60f77-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60f77-123">Here is a JSON representation of the resource.</span></span>
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





