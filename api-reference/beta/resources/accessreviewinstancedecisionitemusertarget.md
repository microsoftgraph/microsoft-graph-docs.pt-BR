---
title: Tipo de recurso accessReviewInstanceDecisionItemUserTarget
description: Representa o destino de uma revisão como usuário.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f10796937aa99e5808cb51bdb4069bd99d645db2
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "51469210"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a><span data-ttu-id="6707c-103">Tipo de recurso accessReviewInstanceDecisionItemUserTarget</span><span class="sxs-lookup"><span data-stu-id="6707c-103">accessReviewInstanceDecisionItemUserTarget resource type</span></span>

<span data-ttu-id="6707c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6707c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="6707c-105">Representa uma identidade de usuário em revisão em [um accessReviewInstance](accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="6707c-105">Represents a user identity under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="6707c-106">Herda [de accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="6707c-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6707c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6707c-107">Properties</span></span>
|<span data-ttu-id="6707c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6707c-108">Property</span></span>|<span data-ttu-id="6707c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6707c-109">Type</span></span>|<span data-ttu-id="6707c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6707c-110">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="6707c-111">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="6707c-111">userDisplayName</span></span> | <span data-ttu-id="6707c-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6707c-112">String</span></span> | <span data-ttu-id="6707c-113">O nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="6707c-113">The name of user.</span></span> |
| <span data-ttu-id="6707c-114">userId</span><span class="sxs-lookup"><span data-stu-id="6707c-114">userId</span></span> | <span data-ttu-id="6707c-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6707c-115">String</span></span> | <span data-ttu-id="6707c-116">O identificador do usuário.</span><span class="sxs-lookup"><span data-stu-id="6707c-116">The identifier of user.</span></span> |
| <span data-ttu-id="6707c-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6707c-117">userPrincipalName</span></span> | <span data-ttu-id="6707c-118">String</span><span class="sxs-lookup"><span data-stu-id="6707c-118">String</span></span> | <span data-ttu-id="6707c-119">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="6707c-119">The user principal name.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6707c-120">Relações</span><span class="sxs-lookup"><span data-stu-id="6707c-120">Relationships</span></span>
<span data-ttu-id="6707c-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6707c-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6707c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6707c-122">JSON representation</span></span>
<span data-ttu-id="6707c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6707c-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemUserTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```
