---
title: Tipo de recurso accessReviewInstanceDecisionItemServicePrincipalTarget
description: Representa o destino de uma revisão como um destino de entidade de serviço.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7d8032282d7ddaf41779b73f707b0749e3c82dd0
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "51469220"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a><span data-ttu-id="9c04d-103">Tipo de recurso accessReviewInstanceDecisionItemServicePrincipalTarget</span><span class="sxs-lookup"><span data-stu-id="9c04d-103">accessReviewInstanceDecisionItemServicePrincipalTarget resource type</span></span>

<span data-ttu-id="9c04d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c04d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="9c04d-105">Representa uma entidade de serviço em revisão em [um accessReviewInstance](accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="9c04d-105">Represents a service principal under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="9c04d-106">Herda [de accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="9c04d-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9c04d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c04d-107">Properties</span></span>
| <span data-ttu-id="9c04d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c04d-108">Property</span></span> | <span data-ttu-id="9c04d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c04d-109">Type</span></span> | <span data-ttu-id="9c04d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c04d-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="9c04d-111">servicePrincipalID</span><span class="sxs-lookup"><span data-stu-id="9c04d-111">servicePrincipalID</span></span> | <span data-ttu-id="9c04d-112">String</span><span class="sxs-lookup"><span data-stu-id="9c04d-112">String</span></span> | <span data-ttu-id="9c04d-113">O identificador da entidade de serviço cujo acesso está sendo revisado.</span><span class="sxs-lookup"><span data-stu-id="9c04d-113">The identifier of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="9c04d-114">servicePrincipalDisplayName</span><span class="sxs-lookup"><span data-stu-id="9c04d-114">servicePrincipalDisplayName</span></span> | <span data-ttu-id="9c04d-115">String</span><span class="sxs-lookup"><span data-stu-id="9c04d-115">String</span></span> | <span data-ttu-id="9c04d-116">O nome de exibição da entidade de serviço cujo acesso está sendo revisado.</span><span class="sxs-lookup"><span data-stu-id="9c04d-116">The display name of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="9c04d-117">appId</span><span class="sxs-lookup"><span data-stu-id="9c04d-117">appId</span></span> | <span data-ttu-id="9c04d-118">String</span><span class="sxs-lookup"><span data-stu-id="9c04d-118">String</span></span> | <span data-ttu-id="9c04d-119">O appId da entidade principal do serviço que está sendo revisada.</span><span class="sxs-lookup"><span data-stu-id="9c04d-119">The appId for the service principal entity being reviewed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9c04d-120">Relações</span><span class="sxs-lookup"><span data-stu-id="9c04d-120">Relationships</span></span>
<span data-ttu-id="9c04d-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c04d-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c04d-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c04d-122">JSON representation</span></span>
<span data-ttu-id="9c04d-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c04d-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemServicePrincipalTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemServicePrincipalTarget",
  "servicePrincipalId": "String",
  "servicePrincipalDisplayName": "String",
  "appId": "String"
}
```
