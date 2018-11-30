---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
ms.openlocfilehash: e44af4a72aee8c97a12b3d8dcad767bba08ad005
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033488"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="faa0c-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="faa0c-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="faa0c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="faa0c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="faa0c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="faa0c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="faa0c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="faa0c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="faa0c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="faa0c-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="faa0c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="faa0c-108">Properties</span></span>
|<span data-ttu-id="faa0c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="faa0c-109">Property</span></span>|<span data-ttu-id="faa0c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="faa0c-110">Type</span></span>|<span data-ttu-id="faa0c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="faa0c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faa0c-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="faa0c-112">movieRating</span></span>|[<span data-ttu-id="faa0c-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="faa0c-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="faa0c-114">Filmes classificação selecionado no Canadá.</span><span class="sxs-lookup"><span data-stu-id="faa0c-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="faa0c-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="faa0c-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="faa0c-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="faa0c-116">tvRating</span></span>|[<span data-ttu-id="faa0c-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="faa0c-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="faa0c-118">Classificação de TV selecionada para Canadá.</span><span class="sxs-lookup"><span data-stu-id="faa0c-118">TV rating selected for Canada.</span></span> <span data-ttu-id="faa0c-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="faa0c-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="faa0c-120">Relações</span><span class="sxs-lookup"><span data-stu-id="faa0c-120">Relationships</span></span>
<span data-ttu-id="faa0c-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="faa0c-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="faa0c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="faa0c-122">JSON Representation</span></span>
<span data-ttu-id="faa0c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="faa0c-123">Here is a JSON representation of the resource.</span></span>
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





