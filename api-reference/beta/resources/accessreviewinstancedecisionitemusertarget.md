---
title: Tipo de recurso accessReviewInstanceDecisionItemUserTarget
description: Representa o destino de uma revisão como um usuário.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 73fba5b7329a6dd13ddc455b9ba327467dde9016
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133466"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a><span data-ttu-id="3167f-103">Tipo de recurso accessReviewInstanceDecisionItemUserTarget</span><span class="sxs-lookup"><span data-stu-id="3167f-103">accessReviewInstanceDecisionItemUserTarget resource type</span></span>

<span data-ttu-id="3167f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3167f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3167f-105">Representa uma identidade de usuário sob revisão em [um accessReviewInstance](accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="3167f-105">Represents a user identity under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="3167f-106">Herda de [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="3167f-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3167f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3167f-107">Properties</span></span>
|<span data-ttu-id="3167f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3167f-108">Property</span></span>|<span data-ttu-id="3167f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3167f-109">Type</span></span>|<span data-ttu-id="3167f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3167f-110">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="3167f-111">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3167f-111">userDisplayName</span></span> | <span data-ttu-id="3167f-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3167f-112">String</span></span> | <span data-ttu-id="3167f-113">O nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="3167f-113">The name of user.</span></span> |
| <span data-ttu-id="3167f-114">userId</span><span class="sxs-lookup"><span data-stu-id="3167f-114">userId</span></span> | <span data-ttu-id="3167f-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3167f-115">String</span></span> | <span data-ttu-id="3167f-116">O identificador do usuário.</span><span class="sxs-lookup"><span data-stu-id="3167f-116">The identifier of user.</span></span> |
| <span data-ttu-id="3167f-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3167f-117">userPrincipalName</span></span> | <span data-ttu-id="3167f-118">String</span><span class="sxs-lookup"><span data-stu-id="3167f-118">String</span></span> | <span data-ttu-id="3167f-119">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="3167f-119">The user principal name.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3167f-120">Relações</span><span class="sxs-lookup"><span data-stu-id="3167f-120">Relationships</span></span>
<span data-ttu-id="3167f-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3167f-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3167f-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3167f-122">JSON representation</span></span>
<span data-ttu-id="3167f-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3167f-123">The following is a JSON representation of the resource.</span></span>
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
