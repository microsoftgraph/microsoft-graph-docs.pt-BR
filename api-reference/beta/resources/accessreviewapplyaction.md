---
title: Tipo de recurso accessReviewApplyAction
description: Representa a ação a ser tomada em usuários revisados após a conclusão de uma instância de revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 09e23095f62c2e09b623e1e0634987f712e56730
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "51469388"
---
# <a name="accessreviewapplyaction-resource-type"></a><span data-ttu-id="e07e2-103">Tipo de recurso accessReviewApplyAction</span><span class="sxs-lookup"><span data-stu-id="e07e2-103">accessReviewApplyAction resource type</span></span>

<span data-ttu-id="e07e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e07e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="e07e2-105">Representa uma classe base para aplicar ações [no accessReviewScheduleSettings](accessreviewschedulesettings.md) de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e07e2-105">Represents a base class for apply actions in the [accessReviewScheduleSettings](accessreviewschedulesettings.md) of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="e07e2-106">Tipos derivados com suporte:</span><span class="sxs-lookup"><span data-stu-id="e07e2-106">Supported derived types:</span></span>

- <span data-ttu-id="e07e2-107">**removeAccessApplyAction** é um tipo derivado de accessReviewApplyAction que indica a remoção do acesso de uma entidade que está sendo revisada após a conclusão da revisão.</span><span class="sxs-lookup"><span data-stu-id="e07e2-107">**removeAccessApplyAction** is a derived type of accessReviewApplyAction that indicates removing access of an entity being reviewed upon completion of the review.</span></span> <span data-ttu-id="e07e2-108">Esse é o tipo padrão para a propriedade applyActions em accessReviewScheduleSettings e não precisa ser especificado.</span><span class="sxs-lookup"><span data-stu-id="e07e2-108">This is the default type for the applyActions property in accessReviewScheduleSettings and does not need to be specified.</span></span>

- <span data-ttu-id="e07e2-109">**disableAndDeleteUserApplyAction** é um tipo derivado de accessReviewApplyAction que indica desabilitar e excluir o usuário que está sendo revisado após a conclusão da revisão.</span><span class="sxs-lookup"><span data-stu-id="e07e2-109">**disableAndDeleteUserApplyAction** is a derived type of accessReviewApplyAction that indicates disabling and deleting the user being reviewed upon completion of the review.</span></span> <span data-ttu-id="e07e2-110">Esse é o tipo não padrão e precisa ser especificado em accessReviewScheduleSettings.</span><span class="sxs-lookup"><span data-stu-id="e07e2-110">This is the non-default type and needs to specified in accessReviewScheduleSettings.</span></span>

## <a name="properties"></a><span data-ttu-id="e07e2-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e07e2-111">Properties</span></span>
<span data-ttu-id="e07e2-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e07e2-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="e07e2-113">Relações</span><span class="sxs-lookup"><span data-stu-id="e07e2-113">Relationships</span></span>
<span data-ttu-id="e07e2-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e07e2-114">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e07e2-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e07e2-115">JSON representation</span></span>
<span data-ttu-id="e07e2-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e07e2-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewApplyAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewApplyAction"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewApplyAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
