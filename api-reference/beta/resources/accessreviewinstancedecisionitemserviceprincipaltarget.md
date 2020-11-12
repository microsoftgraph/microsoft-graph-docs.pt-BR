---
title: tipo de recurso accessReviewInstanceDecisionItemServicePrincipalTarget
description: Representa o destino de uma revisão como um destino principal de serviço.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e9943a287dd28a44f3b36eae1a92d1b2c385496c
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000778"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a><span data-ttu-id="c619c-103">tipo de recurso accessReviewInstanceDecisionItemServicePrincipalTarget</span><span class="sxs-lookup"><span data-stu-id="c619c-103">accessReviewInstanceDecisionItemServicePrincipalTarget resource type</span></span>

<span data-ttu-id="c619c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c619c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c619c-105">Representa uma entidade de serviço em revisão em um [accessReviewInstance](accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="c619c-105">Represents a service principal under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="c619c-106">Herda de [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="c619c-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c619c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c619c-107">Properties</span></span>
| <span data-ttu-id="c619c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c619c-108">Property</span></span> | <span data-ttu-id="c619c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c619c-109">Type</span></span> | <span data-ttu-id="c619c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c619c-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="c619c-111">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="c619c-111">servicePrincipalID</span></span> | <span data-ttu-id="c619c-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c619c-112">String</span></span> | <span data-ttu-id="c619c-113">O identificador da entidade de serviço cujo acesso está sendo revisado.</span><span class="sxs-lookup"><span data-stu-id="c619c-113">The identifier of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="c619c-114">servicePrincipalDisplayName</span><span class="sxs-lookup"><span data-stu-id="c619c-114">servicePrincipalDisplayName</span></span> | <span data-ttu-id="c619c-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c619c-115">String</span></span> | <span data-ttu-id="c619c-116">O nome de exibição da entidade de serviço cujo acesso está sendo revisado.</span><span class="sxs-lookup"><span data-stu-id="c619c-116">The display name of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="c619c-117">appId</span><span class="sxs-lookup"><span data-stu-id="c619c-117">appId</span></span> | <span data-ttu-id="c619c-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c619c-118">String</span></span> | <span data-ttu-id="c619c-119">A appId da entidade de segurança de serviço que está sendo revisada.</span><span class="sxs-lookup"><span data-stu-id="c619c-119">The appId for the service principal entity being reviewed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c619c-120">Relações</span><span class="sxs-lookup"><span data-stu-id="c619c-120">Relationships</span></span>
<span data-ttu-id="c619c-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c619c-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c619c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c619c-122">JSON representation</span></span>
<span data-ttu-id="c619c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c619c-123">The following is a JSON representation of the resource.</span></span>
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
