---
title: Tipo de recurso principalResourceMembershipsScope
description: Permite que a seleção do escopo de revisão de acesso revise o acesso das entidades selecionadas aos recursos selecionados.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: dc6c81092ce08ba49e4adde28b0376a17d6ccf0d
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030968"
---
# <a name="principalresourcemembershipsscope-resource-type"></a><span data-ttu-id="fc363-103">Tipo de recurso principalResourceMembershipsScope</span><span class="sxs-lookup"><span data-stu-id="fc363-103">principalResourceMembershipsScope resource type</span></span>

<span data-ttu-id="fc363-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc363-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc363-105">O principalResourceMembershipsScope é um tipo de [accessReviewScope](accessreviewscope.md) que permite selecionar uma coleção de escopos principais e uma coleção de escopos de recursos e revisar o acesso de entidades selecionadas aos recursos selecionados.</span><span class="sxs-lookup"><span data-stu-id="fc363-105">The principalResourceMembershipsScope is a type of [accessReviewScope](accessreviewscope.md) which allows you to select a collection of principal scopes and a collection of resource scopes and review access of selected principals to selected resources.</span></span> <span data-ttu-id="fc363-106">Ele é usado para configurar a propriedade **scope** de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="fc363-106">It is used to configure the **scope** property of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span>

<span data-ttu-id="fc363-107">Herda de [accessReviewScope](../resources/accessreviewscope.md).</span><span class="sxs-lookup"><span data-stu-id="fc363-107">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fc363-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc363-108">Properties</span></span>
|<span data-ttu-id="fc363-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc363-109">Property</span></span>|<span data-ttu-id="fc363-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc363-110">Type</span></span>|<span data-ttu-id="fc363-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc363-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc363-112">principalScopes</span><span class="sxs-lookup"><span data-stu-id="fc363-112">principalScopes</span></span>|<span data-ttu-id="fc363-113">[Coleção accessReviewScope](../resources/accessreviewscope.md)</span><span class="sxs-lookup"><span data-stu-id="fc363-113">[accessReviewScope](../resources/accessreviewscope.md) collection</span></span>|<span data-ttu-id="fc363-114">Define os escopos das entidades cujo acesso aos recursos é revisado na revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="fc363-114">Defines the scopes of the principals whose access to resources are reviewed in the access review.</span></span>|
|<span data-ttu-id="fc363-115">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="fc363-115">resourceScopes</span></span>|<span data-ttu-id="fc363-116">[Coleção accessReviewScope](../resources/accessreviewscope.md)</span><span class="sxs-lookup"><span data-stu-id="fc363-116">[accessReviewScope](../resources/accessreviewscope.md) collection</span></span>|<span data-ttu-id="fc363-117">Define os escopos dos recursos para os quais o acesso é revisado.</span><span class="sxs-lookup"><span data-stu-id="fc363-117">Defines the scopes of the resources for which access is reviewed.</span></span>|

<span data-ttu-id="fc363-118">Você também deve especificar a **propriedade @odata.type com** o valor `#microsoft.graph.principalResourceMembershipsScope` .</span><span class="sxs-lookup"><span data-stu-id="fc363-118">You must also specify the **@odata.type** type property with the value `#microsoft.graph.principalResourceMembershipsScope`.</span></span> <span data-ttu-id="fc363-119">Para obter mais  informações sobre opções de configuração para escopo usando **o principalResourceMembershipsScope,** consulte Configure the scope of your [access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span><span class="sxs-lookup"><span data-stu-id="fc363-119">For more about configuration options for **scope** using **principalResourceMembershipsScope**, see [Configure the scope of your access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span></span>

## <a name="relationships"></a><span data-ttu-id="fc363-120">Relações</span><span class="sxs-lookup"><span data-stu-id="fc363-120">Relationships</span></span>
<span data-ttu-id="fc363-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc363-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc363-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc363-122">JSON representation</span></span>
<span data-ttu-id="fc363-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc363-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.principalResourceMembershipsScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
  "principalScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ],
  "resourceScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ]
}
```
