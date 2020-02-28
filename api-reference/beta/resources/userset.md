---
title: tipo complexo userset
description: O tipo base abstrato para tipos usados nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f23953b30918dec40f37f7809c7c024167c34132
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331363"
---
# <a name="userset-complex-type"></a><span data-ttu-id="35281-103">tipo complexo userset</span><span class="sxs-lookup"><span data-stu-id="35281-103">userSet complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35281-104">Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="35281-104">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="35281-105">O tipo de base abstrato para os tipos [únicousuário](singleuser.md),[groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md)e [externalSponsors](externalsponsors.md) .</span><span class="sxs-lookup"><span data-stu-id="35281-105">The abstract base type for the [singleUser](singleuser.md),[groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md), and [externalSponsors](externalsponsors.md) types.</span></span>

## <a name="properties"></a><span data-ttu-id="35281-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35281-106">Properties</span></span>

| <span data-ttu-id="35281-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35281-107">Property</span></span>                     | <span data-ttu-id="35281-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="35281-108">Type</span></span>                      | <span data-ttu-id="35281-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="35281-109">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="35281-110">IsBackup</span><span class="sxs-lookup"><span data-stu-id="35281-110">isBackup</span></span> | <span data-ttu-id="35281-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="35281-111">Boolean</span></span> | <span data-ttu-id="35281-112">Para um usuário em uma fase de aprovação, essa propriedade indica se o usuário é um Aprovador de fallback de backup.</span><span class="sxs-lookup"><span data-stu-id="35281-112">For a user in an approval stage, this property indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35281-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35281-113">JSON representation</span></span>

<span data-ttu-id="35281-114">Veja a seguir uma representação JSON de userset.</span><span class="sxs-lookup"><span data-stu-id="35281-114">The following is a JSON representation of userSet.</span></span>  <span data-ttu-id="35281-115">Observe que um userset é uma classe base abstrata e, portanto, não seria enviado ou recebido.</span><span class="sxs-lookup"><span data-stu-id="35281-115">Note that a userSet is an abstract base class, and so would not be sent or received.</span></span>  <span data-ttu-id="35281-116">Em vez disso, um `@odata.type` de "`#microsoft.graph.singleUser`", "`#microsoft.graph.groupMembers`", "`#microsoft.graph.connectedOrganizationMembers`", "`#microsoft.graph.requestorManager`", "`#microsoft.graph.internalSponsors`" ou "`#microsoft.graph.externalSponsors`" seria usado.</span><span class="sxs-lookup"><span data-stu-id="35281-116">Instead, one of the `@odata.type` of "`#microsoft.graph.singleUser`", "`#microsoft.graph.groupMembers`", "`#microsoft.graph.connectedOrganizationMembers`", "`#microsoft.graph.requestorManager`", "`#microsoft.graph.internalSponsors`" or "`#microsoft.graph.externalSponsors`" would be used.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSet",
  "baseType": ""
}-->

```json
{
       "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSet complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
