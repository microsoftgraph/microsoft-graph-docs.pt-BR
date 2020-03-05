---
title: tipo complexo userset
description: O tipo base abstrato para tipos usados nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 77f0f990587531c10914644366e066a0fd659f37
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519502"
---
# <a name="userset-complex-type"></a><span data-ttu-id="a00cf-103">tipo complexo userset</span><span class="sxs-lookup"><span data-stu-id="a00cf-103">userSet complex type</span></span>

<span data-ttu-id="a00cf-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a00cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a00cf-105">Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a00cf-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="a00cf-106">O tipo de base abstrato para os tipos [únicousuário](singleuser.md),[groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md)e [externalSponsors](externalsponsors.md) .</span><span class="sxs-lookup"><span data-stu-id="a00cf-106">The abstract base type for the [singleUser](singleuser.md),[groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md), and [externalSponsors](externalsponsors.md) types.</span></span>

## <a name="properties"></a><span data-ttu-id="a00cf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a00cf-107">Properties</span></span>

| <span data-ttu-id="a00cf-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a00cf-108">Property</span></span>                     | <span data-ttu-id="a00cf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a00cf-109">Type</span></span>                      | <span data-ttu-id="a00cf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a00cf-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="a00cf-111">IsBackup</span><span class="sxs-lookup"><span data-stu-id="a00cf-111">isBackup</span></span> | <span data-ttu-id="a00cf-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="a00cf-112">Boolean</span></span> | <span data-ttu-id="a00cf-113">Para um usuário em uma fase de aprovação, essa propriedade indica se o usuário é um Aprovador de fallback de backup.</span><span class="sxs-lookup"><span data-stu-id="a00cf-113">For a user in an approval stage, this property indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a00cf-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a00cf-114">JSON representation</span></span>

<span data-ttu-id="a00cf-115">Veja a seguir uma representação JSON de userset.</span><span class="sxs-lookup"><span data-stu-id="a00cf-115">The following is a JSON representation of userSet.</span></span>  <span data-ttu-id="a00cf-116">Observe que um userset é uma classe base abstrata e, portanto, não seria enviado ou recebido.</span><span class="sxs-lookup"><span data-stu-id="a00cf-116">Note that a userSet is an abstract base class, and so would not be sent or received.</span></span>  <span data-ttu-id="a00cf-117">Em vez disso, um `@odata.type` de "`#microsoft.graph.singleUser`", "`#microsoft.graph.groupMembers`", "`#microsoft.graph.connectedOrganizationMembers`", "`#microsoft.graph.requestorManager`", "`#microsoft.graph.internalSponsors`" ou "`#microsoft.graph.externalSponsors`" seria usado.</span><span class="sxs-lookup"><span data-stu-id="a00cf-117">Instead, one of the `@odata.type` of "`#microsoft.graph.singleUser`", "`#microsoft.graph.groupMembers`", "`#microsoft.graph.connectedOrganizationMembers`", "`#microsoft.graph.requestorManager`", "`#microsoft.graph.internalSponsors`" or "`#microsoft.graph.externalSponsors`" would be used.</span></span>

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
