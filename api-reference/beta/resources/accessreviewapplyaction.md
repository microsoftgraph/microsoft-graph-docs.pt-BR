---
title: tipo de recurso accessReviewApplyAction
description: Representa a ação a ser tomada nos usuários revisados após a conclusão de uma instância de revisão do Access.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 33aa0f7a9d7fbfeab9b957f4c94b87d6f6e50d44
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000768"
---
# <a name="accessreviewapplyaction-resource-type"></a><span data-ttu-id="48a5b-103">tipo de recurso accessReviewApplyAction</span><span class="sxs-lookup"><span data-stu-id="48a5b-103">accessReviewApplyAction resource type</span></span>

<span data-ttu-id="48a5b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48a5b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48a5b-105">Representa uma classe base para aplicar ações no [accessReviewScheduleSettings](accessreviewschedulesettings.md) de um [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="48a5b-105">Represents a base class for apply actions in the [accessReviewScheduleSettings](accessreviewschedulesettings.md) of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="48a5b-106">Tipos derivados suportados:</span><span class="sxs-lookup"><span data-stu-id="48a5b-106">Supported derived types:</span></span>

- <span data-ttu-id="48a5b-107">**removeAccessApplyAction** é um tipo derivado de accessReviewApplyAction que indica remover o acesso de uma entidade que está sendo revisada após a conclusão da revisão.</span><span class="sxs-lookup"><span data-stu-id="48a5b-107">**removeAccessApplyAction** is a derived type of accessReviewApplyAction that indicates removing access of an entity being reviewed upon completion of the review.</span></span> <span data-ttu-id="48a5b-108">Este é o tipo padrão para a propriedade applyActions em accessReviewScheduleSettings e não precisa ser especificado.</span><span class="sxs-lookup"><span data-stu-id="48a5b-108">This is the default type for the applyActions property in accessReviewScheduleSettings and does not need to be specified.</span></span>

- <span data-ttu-id="48a5b-109">**disableAndDeleteUserApplyAction** é um tipo derivado de accessReviewApplyAction que indica desabilitar e excluir o usuário que está sendo revisado após a conclusão da revisão.</span><span class="sxs-lookup"><span data-stu-id="48a5b-109">**disableAndDeleteUserApplyAction** is a derived type of accessReviewApplyAction that indicates disabling and deleting the user being reviewed upon completion of the review.</span></span> <span data-ttu-id="48a5b-110">Este é o tipo não padrão e precisa ser especificado em accessReviewScheduleSettings.</span><span class="sxs-lookup"><span data-stu-id="48a5b-110">This is the non-default type and needs to specified in accessReviewScheduleSettings.</span></span>

## <a name="properties"></a><span data-ttu-id="48a5b-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48a5b-111">Properties</span></span>
<span data-ttu-id="48a5b-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="48a5b-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="48a5b-113">Relações</span><span class="sxs-lookup"><span data-stu-id="48a5b-113">Relationships</span></span>
<span data-ttu-id="48a5b-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="48a5b-114">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="48a5b-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48a5b-115">JSON representation</span></span>
<span data-ttu-id="48a5b-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48a5b-116">The following is a JSON representation of the resource.</span></span>
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
