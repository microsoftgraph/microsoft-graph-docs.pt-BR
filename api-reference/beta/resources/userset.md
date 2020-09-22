---
title: tipo complexo userset
description: O tipo base abstrato para tipos usados nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aabd0716990f67d0b73b4bb300b6953caa0bfe07
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057805"
---
# <a name="userset-complex-type"></a><span data-ttu-id="ea4e7-103">tipo complexo userset</span><span class="sxs-lookup"><span data-stu-id="ea4e7-103">userSet complex type</span></span>

<span data-ttu-id="ea4e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea4e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea4e7-105">Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ea4e7-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="ea4e7-106">O tipo de base abstrato para os tipos [únicousuário](singleuser.md),[groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md)e [externalSponsors](externalsponsors.md) .</span><span class="sxs-lookup"><span data-stu-id="ea4e7-106">The abstract base type for the [singleUser](singleuser.md),[groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md), and [externalSponsors](externalsponsors.md) types.</span></span>

## <a name="properties"></a><span data-ttu-id="ea4e7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea4e7-107">Properties</span></span>

| <span data-ttu-id="ea4e7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea4e7-108">Property</span></span>                     | <span data-ttu-id="ea4e7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea4e7-109">Type</span></span>                      | <span data-ttu-id="ea4e7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea4e7-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="ea4e7-111">IsBackup</span><span class="sxs-lookup"><span data-stu-id="ea4e7-111">isBackup</span></span> | <span data-ttu-id="ea4e7-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="ea4e7-112">Boolean</span></span> | <span data-ttu-id="ea4e7-113">Para um usuário em uma fase de aprovação, essa propriedade indica se o usuário é um Aprovador de fallback de backup.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-113">For a user in an approval stage, this property indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ea4e7-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea4e7-114">JSON representation</span></span>

<span data-ttu-id="ea4e7-115">Veja a seguir uma representação JSON de userset.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-115">The following is a JSON representation of userSet.</span></span>  <span data-ttu-id="ea4e7-116">Observe que um userset é uma classe base abstrata e, portanto, não seria enviado ou recebido.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-116">Note that a userSet is an abstract base class, and so would not be sent or received.</span></span>  <span data-ttu-id="ea4e7-117">Em vez disso, um de `@odata.type` " `#microsoft.graph.singleUser` ", " `#microsoft.graph.groupMembers` ", " `#microsoft.graph.connectedOrganizationMembers` ", " `#microsoft.graph.requestorManager` ", " `#microsoft.graph.internalSponsors` " ou " `#microsoft.graph.externalSponsors` " seria usado.</span><span class="sxs-lookup"><span data-stu-id="ea4e7-117">Instead, one of the `@odata.type` of "`#microsoft.graph.singleUser`", "`#microsoft.graph.groupMembers`", "`#microsoft.graph.connectedOrganizationMembers`", "`#microsoft.graph.requestorManager`", "`#microsoft.graph.internalSponsors`" or "`#microsoft.graph.externalSponsors`" would be used.</span></span>

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


