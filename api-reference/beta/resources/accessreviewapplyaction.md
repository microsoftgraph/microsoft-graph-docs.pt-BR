---
title: Tipo de recurso accessReviewApplyAction
description: Representa a ação a ser tomada em usuários revisados após a conclusão de uma instância de revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c7f1425bb7155762f973f65fd766db8da55b8d77
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579638"
---
# <a name="accessreviewapplyaction-resource-type"></a><span data-ttu-id="e3ddf-103">Tipo de recurso accessReviewApplyAction</span><span class="sxs-lookup"><span data-stu-id="e3ddf-103">accessReviewApplyAction resource type</span></span>

<span data-ttu-id="e3ddf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3ddf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="e3ddf-105">Representa uma classe base para aplicar ações [no accessReviewScheduleSettings](accessreviewschedulesettings.md) de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e3ddf-105">Represents a base class for apply actions in the [accessReviewScheduleSettings](accessreviewschedulesettings.md) of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="e3ddf-106">Tipos derivados com suporte:</span><span class="sxs-lookup"><span data-stu-id="e3ddf-106">Supported derived types:</span></span>

- <span data-ttu-id="e3ddf-107">[removeAccessApplyAction](removeaccessapplyaction.md) é um tipo derivado de accessReviewApplyAction que indica a remoção do acesso de uma entidade que está sendo revisada após a conclusão da revisão.</span><span class="sxs-lookup"><span data-stu-id="e3ddf-107">[removeAccessApplyAction](removeaccessapplyaction.md) is a derived type of accessReviewApplyAction that indicates removing access of an entity being reviewed upon completion of the review.</span></span> <span data-ttu-id="e3ddf-108">Esse é o tipo padrão para a propriedade applyActions em accessReviewScheduleSettings e não precisa ser especificado.</span><span class="sxs-lookup"><span data-stu-id="e3ddf-108">This is the default type for the applyActions property in accessReviewScheduleSettings and does not need to be specified.</span></span>

- <span data-ttu-id="e3ddf-109">[disableAndDeleteUserApplyAction](disableanddeleteuserapplyaction.md) é um tipo derivado de accessReviewApplyAction que indica desabilitar e excluir o usuário que está sendo revisado após a conclusão da revisão.</span><span class="sxs-lookup"><span data-stu-id="e3ddf-109">[disableAndDeleteUserApplyAction](disableanddeleteuserapplyaction.md) is a derived type of accessReviewApplyAction that indicates disabling and deleting the user being reviewed upon completion of the review.</span></span> <span data-ttu-id="e3ddf-110">Esse é o tipo não padrão e precisa ser especificado em accessReviewScheduleSettings.</span><span class="sxs-lookup"><span data-stu-id="e3ddf-110">This is the non-default type and needs to specified in accessReviewScheduleSettings.</span></span>

## <a name="properties"></a><span data-ttu-id="e3ddf-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3ddf-111">Properties</span></span>
<span data-ttu-id="e3ddf-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e3ddf-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="e3ddf-113">Relações</span><span class="sxs-lookup"><span data-stu-id="e3ddf-113">Relationships</span></span>
<span data-ttu-id="e3ddf-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3ddf-114">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e3ddf-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3ddf-115">JSON representation</span></span>
<span data-ttu-id="e3ddf-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3ddf-116">The following is a JSON representation of the resource.</span></span>
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
