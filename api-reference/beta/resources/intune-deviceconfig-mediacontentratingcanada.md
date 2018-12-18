---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: efdc88934e46c849f48c0eb24ddd49535b824044
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331952"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="93bfc-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="93bfc-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="93bfc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="93bfc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93bfc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="93bfc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="93bfc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="93bfc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93bfc-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="93bfc-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="93bfc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93bfc-108">Properties</span></span>
|<span data-ttu-id="93bfc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93bfc-109">Property</span></span>|<span data-ttu-id="93bfc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="93bfc-110">Type</span></span>|<span data-ttu-id="93bfc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="93bfc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93bfc-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="93bfc-112">movieRating</span></span>|[<span data-ttu-id="93bfc-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="93bfc-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="93bfc-114">Filmes classificação selecionado no Canadá.</span><span class="sxs-lookup"><span data-stu-id="93bfc-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="93bfc-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="93bfc-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="93bfc-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="93bfc-116">tvRating</span></span>|[<span data-ttu-id="93bfc-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="93bfc-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="93bfc-118">Classificação de TV selecionada para Canadá.</span><span class="sxs-lookup"><span data-stu-id="93bfc-118">TV rating selected for Canada.</span></span> <span data-ttu-id="93bfc-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="93bfc-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93bfc-120">Relações</span><span class="sxs-lookup"><span data-stu-id="93bfc-120">Relationships</span></span>
<span data-ttu-id="93bfc-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93bfc-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="93bfc-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93bfc-122">JSON Representation</span></span>
<span data-ttu-id="93bfc-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93bfc-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```





