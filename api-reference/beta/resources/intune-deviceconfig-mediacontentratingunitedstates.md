---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
ms.openlocfilehash: d62d656c4fbd8744560ab191786d71b732fe6c21
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033309"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="32843-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="32843-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="32843-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="32843-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32843-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="32843-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32843-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="32843-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32843-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="32843-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="32843-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32843-108">Properties</span></span>
|<span data-ttu-id="32843-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32843-109">Property</span></span>|<span data-ttu-id="32843-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="32843-110">Type</span></span>|<span data-ttu-id="32843-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="32843-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32843-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="32843-112">movieRating</span></span>|[<span data-ttu-id="32843-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="32843-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="32843-114">Filmes classificação selecionado para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="32843-114">Movies rating selected for United States.</span></span> <span data-ttu-id="32843-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="32843-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="32843-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="32843-116">tvRating</span></span>|[<span data-ttu-id="32843-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="32843-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="32843-118">Classificação de TV selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="32843-118">TV rating selected for United States.</span></span> <span data-ttu-id="32843-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="32843-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32843-120">Relações</span><span class="sxs-lookup"><span data-stu-id="32843-120">Relationships</span></span>
<span data-ttu-id="32843-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="32843-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="32843-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32843-122">JSON Representation</span></span>
<span data-ttu-id="32843-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32843-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```





