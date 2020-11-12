---
title: tipo de recurso accessReviewInstanceDecisionItemUserTarget
description: Representa o destino de uma revisão como um usuário.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aa2117895599ba1d2c4b9829b7cad22b581f2055
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000777"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a><span data-ttu-id="3d0fc-103">tipo de recurso accessReviewInstanceDecisionItemUserTarget</span><span class="sxs-lookup"><span data-stu-id="3d0fc-103">accessReviewInstanceDecisionItemUserTarget resource type</span></span>

<span data-ttu-id="3d0fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d0fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3d0fc-105">Representa uma identidade de usuário em revisão em um [accessReviewInstance](accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="3d0fc-105">Represents a user identity under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="3d0fc-106">Herda de [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="3d0fc-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3d0fc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d0fc-107">Properties</span></span>
|<span data-ttu-id="3d0fc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d0fc-108">Property</span></span>|<span data-ttu-id="3d0fc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d0fc-109">Type</span></span>|<span data-ttu-id="3d0fc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d0fc-110">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="3d0fc-111">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3d0fc-111">userDisplayName</span></span> | <span data-ttu-id="3d0fc-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d0fc-112">String</span></span> | <span data-ttu-id="3d0fc-113">O nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="3d0fc-113">The name of user.</span></span> |
| <span data-ttu-id="3d0fc-114">userId</span><span class="sxs-lookup"><span data-stu-id="3d0fc-114">userId</span></span> | <span data-ttu-id="3d0fc-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d0fc-115">String</span></span> | <span data-ttu-id="3d0fc-116">O identificador do usuário.</span><span class="sxs-lookup"><span data-stu-id="3d0fc-116">The identifier of user.</span></span> |
| <span data-ttu-id="3d0fc-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3d0fc-117">userPrincipalName</span></span> | <span data-ttu-id="3d0fc-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d0fc-118">String</span></span> | <span data-ttu-id="3d0fc-119">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="3d0fc-119">The user principal name.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3d0fc-120">Relações</span><span class="sxs-lookup"><span data-stu-id="3d0fc-120">Relationships</span></span>
<span data-ttu-id="3d0fc-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d0fc-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d0fc-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d0fc-122">JSON representation</span></span>
<span data-ttu-id="3d0fc-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d0fc-123">The following is a JSON representation of the resource.</span></span>
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
