---
title: Tipo complexo userSet
description: O tipo base abstrato para tipos usados nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição de pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a36ca6012c86486ae2eba0a2f73cce401d5609d9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136127"
---
# <a name="userset-complex-type"></a><span data-ttu-id="3ec49-103">Tipo complexo userSet</span><span class="sxs-lookup"><span data-stu-id="3ec49-103">userSet complex type</span></span>

<span data-ttu-id="3ec49-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ec49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ec49-105">Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3ec49-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="3ec49-106">O tipo de base abstrata para [o singleUser](singleuser.md),[groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md)e [externalSponsors](externalsponsors.md) tipos.</span><span class="sxs-lookup"><span data-stu-id="3ec49-106">The abstract base type for the [singleUser](singleuser.md),[groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md), and [externalSponsors](externalsponsors.md) types.</span></span>

## <a name="properties"></a><span data-ttu-id="3ec49-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ec49-107">Properties</span></span>

| <span data-ttu-id="3ec49-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ec49-108">Property</span></span>                     | <span data-ttu-id="3ec49-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ec49-109">Type</span></span>                      | <span data-ttu-id="3ec49-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ec49-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="3ec49-111">isBackup</span><span class="sxs-lookup"><span data-stu-id="3ec49-111">isBackup</span></span> | <span data-ttu-id="3ec49-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ec49-112">Boolean</span></span> | <span data-ttu-id="3ec49-113">Para um usuário em um estágio de aprovação, essa propriedade indica se o usuário é um aprovador de fallback de backup.</span><span class="sxs-lookup"><span data-stu-id="3ec49-113">For a user in an approval stage, this property indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3ec49-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ec49-114">JSON representation</span></span>

<span data-ttu-id="3ec49-115">A seguir está uma representação JSON de userSet.</span><span class="sxs-lookup"><span data-stu-id="3ec49-115">The following is a JSON representation of userSet.</span></span>  <span data-ttu-id="3ec49-116">Observe que um userSet é uma classe base abstrata e, portanto, não seria enviado ou recebido.</span><span class="sxs-lookup"><span data-stu-id="3ec49-116">Note that a userSet is an abstract base class, and so would not be sent or received.</span></span>  <span data-ttu-id="3ec49-117">Em vez disso, um dos `@odata.type` " `#microsoft.graph.singleUser` ", " `#microsoft.graph.groupMembers` ", " `#microsoft.graph.connectedOrganizationMembers` " `#microsoft.graph.requestorManager` ", " " ou " `#microsoft.graph.internalSponsors` seria `#microsoft.graph.externalSponsors` usado.</span><span class="sxs-lookup"><span data-stu-id="3ec49-117">Instead, one of the `@odata.type` of "`#microsoft.graph.singleUser`", "`#microsoft.graph.groupMembers`", "`#microsoft.graph.connectedOrganizationMembers`", "`#microsoft.graph.requestorManager`", "`#microsoft.graph.internalSponsors`" or "`#microsoft.graph.externalSponsors`" would be used.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSet"
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


