---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60208f2bace4826f06ff5a81f02bc087211d52a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542281"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="2c943-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="2c943-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="2c943-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2c943-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c943-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c943-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c943-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2c943-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2c943-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c943-107">Properties</span></span>
|<span data-ttu-id="2c943-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c943-108">Property</span></span>|<span data-ttu-id="2c943-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c943-109">Type</span></span>|<span data-ttu-id="2c943-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c943-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c943-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="2c943-111">movieRating</span></span>|[<span data-ttu-id="2c943-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="2c943-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="2c943-113">Classificação de filmes selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="2c943-113">Movies rating selected for United States.</span></span> <span data-ttu-id="2c943-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="2c943-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="2c943-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="2c943-115">tvRating</span></span>|[<span data-ttu-id="2c943-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="2c943-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="2c943-117">Classificação de TV selecionada para Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="2c943-117">TV rating selected for United States.</span></span> <span data-ttu-id="2c943-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="2c943-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c943-119">Relações</span><span class="sxs-lookup"><span data-stu-id="2c943-119">Relationships</span></span>
<span data-ttu-id="2c943-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c943-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c943-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c943-121">JSON Representation</span></span>
<span data-ttu-id="2c943-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c943-122">Here is a JSON representation of the resource.</span></span>
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





