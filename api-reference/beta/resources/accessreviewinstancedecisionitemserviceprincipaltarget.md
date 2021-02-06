---
title: Tipo de recurso accessReviewInstanceDecisionItemServicePrincipalTarget
description: Representa o destino de uma revisão como um destino de entidade de serviço.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ef944fdd1b8dbe989b1ad92e3d49b1b057fdef74
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133494"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a><span data-ttu-id="6c8ab-103">Tipo de recurso accessReviewInstanceDecisionItemServicePrincipalTarget</span><span class="sxs-lookup"><span data-stu-id="6c8ab-103">accessReviewInstanceDecisionItemServicePrincipalTarget resource type</span></span>

<span data-ttu-id="6c8ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c8ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c8ab-105">Representa uma entidade de serviço em revisão em [um accessReviewInstance](accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="6c8ab-105">Represents a service principal under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="6c8ab-106">Herda de [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="6c8ab-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6c8ab-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c8ab-107">Properties</span></span>
| <span data-ttu-id="6c8ab-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c8ab-108">Property</span></span> | <span data-ttu-id="6c8ab-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c8ab-109">Type</span></span> | <span data-ttu-id="6c8ab-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c8ab-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="6c8ab-111">servicePrincipalID</span><span class="sxs-lookup"><span data-stu-id="6c8ab-111">servicePrincipalID</span></span> | <span data-ttu-id="6c8ab-112">String</span><span class="sxs-lookup"><span data-stu-id="6c8ab-112">String</span></span> | <span data-ttu-id="6c8ab-113">O identificador da entidade de serviço cujo acesso está sendo revisado.</span><span class="sxs-lookup"><span data-stu-id="6c8ab-113">The identifier of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="6c8ab-114">servicePrincipalDisplayName</span><span class="sxs-lookup"><span data-stu-id="6c8ab-114">servicePrincipalDisplayName</span></span> | <span data-ttu-id="6c8ab-115">String</span><span class="sxs-lookup"><span data-stu-id="6c8ab-115">String</span></span> | <span data-ttu-id="6c8ab-116">O nome de exibição da entidade de serviço cujo acesso está sendo revisado.</span><span class="sxs-lookup"><span data-stu-id="6c8ab-116">The display name of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="6c8ab-117">appId</span><span class="sxs-lookup"><span data-stu-id="6c8ab-117">appId</span></span> | <span data-ttu-id="6c8ab-118">String</span><span class="sxs-lookup"><span data-stu-id="6c8ab-118">String</span></span> | <span data-ttu-id="6c8ab-119">A appId da entidade de entidade de serviço que está sendo revisada.</span><span class="sxs-lookup"><span data-stu-id="6c8ab-119">The appId for the service principal entity being reviewed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6c8ab-120">Relações</span><span class="sxs-lookup"><span data-stu-id="6c8ab-120">Relationships</span></span>
<span data-ttu-id="6c8ab-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c8ab-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c8ab-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c8ab-122">JSON representation</span></span>
<span data-ttu-id="6c8ab-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c8ab-123">The following is a JSON representation of the resource.</span></span>
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
