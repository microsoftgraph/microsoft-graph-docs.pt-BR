---
title: Tipo de recurso principalResourceMembershipsScope
description: Permite que os escopos de seleção revisem o acesso das entidades selecionadas aos recursos selecionados.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b22c52c0bf71f1a1169d51e2e6fd3e8ac10e99d9
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579890"
---
# <a name="principalresourcemembershipsscope-resource-type"></a><span data-ttu-id="35de2-103">Tipo de recurso principalResourceMembershipsScope</span><span class="sxs-lookup"><span data-stu-id="35de2-103">principalResourceMembershipsScope resource type</span></span>

<span data-ttu-id="35de2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35de2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="35de2-105">O principalResourceMembershipsScope é um tipo de [accessReviewScope](accessreviewscope.md) que permite selecionar uma coleção de escopos principais e uma coleção de escopos de recursos e revisar o acesso de entidades selecionadas aos recursos selecionados.</span><span class="sxs-lookup"><span data-stu-id="35de2-105">The principalResourceMembershipsScope is a type of [accessReviewScope](accessreviewscope.md) which allows you to select a collection of principal scopes and a collection of resource scopes and review access of selected principals to selected resources.</span></span> <span data-ttu-id="35de2-106">Ele é usado para configurar a propriedade **scope** de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="35de2-106">It is used to configure the **scope** property of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span>

<span data-ttu-id="35de2-107">Herda de [accessReviewScope](../resources/accessreviewscope.md).</span><span class="sxs-lookup"><span data-stu-id="35de2-107">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="35de2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35de2-108">Properties</span></span>
|<span data-ttu-id="35de2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35de2-109">Property</span></span>|<span data-ttu-id="35de2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="35de2-110">Type</span></span>|<span data-ttu-id="35de2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="35de2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35de2-112">principalScopes</span><span class="sxs-lookup"><span data-stu-id="35de2-112">principalScopes</span></span>|<span data-ttu-id="35de2-113">[Coleção accessReviewScope](../resources/accessreviewscope.md)</span><span class="sxs-lookup"><span data-stu-id="35de2-113">[accessReviewScope](../resources/accessreviewscope.md) collection</span></span>|<span data-ttu-id="35de2-114">Define os escopos das entidades a serem incluídas em uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="35de2-114">Defines the scopes of the principals to be included in an access review.</span></span>|
|<span data-ttu-id="35de2-115">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="35de2-115">resourceScopes</span></span>|<span data-ttu-id="35de2-116">[Coleção accessReviewScope](../resources/accessreviewscope.md)</span><span class="sxs-lookup"><span data-stu-id="35de2-116">[accessReviewScope](../resources/accessreviewscope.md) collection</span></span>|<span data-ttu-id="35de2-117">Define os escopos dos recursos para os quais o acesso será revisado.</span><span class="sxs-lookup"><span data-stu-id="35de2-117">Defines the scopes of the resources for which access will be reviewed.</span></span>|

<span data-ttu-id="35de2-118">Você também deve especificar a **propriedade @odata.type com** o valor `#microsoft.graph.principalResourceMembershipsScope` .</span><span class="sxs-lookup"><span data-stu-id="35de2-118">You must also specify the **@odata.type** type property with the value `#microsoft.graph.principalResourceMembershipsScope`.</span></span> <span data-ttu-id="35de2-119">Para obter mais  informações sobre opções de configuração para escopo usando **o principalResourceMembershipsScope,** consulte Configure the scope of your [access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span><span class="sxs-lookup"><span data-stu-id="35de2-119">For more about configuration options for **scope** using **principalResourceMembershipsScope**, see [Configure the scope of your access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span></span>

## <a name="relationships"></a><span data-ttu-id="35de2-120">Relações</span><span class="sxs-lookup"><span data-stu-id="35de2-120">Relationships</span></span>
<span data-ttu-id="35de2-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35de2-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="35de2-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35de2-122">JSON representation</span></span>
<span data-ttu-id="35de2-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35de2-123">The following is a JSON representation of the resource.</span></span>
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
