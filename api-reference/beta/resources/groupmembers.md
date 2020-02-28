---
title: tipo complexo groupMembers
description: Identifica uma coleção de usuários no locatário que serão permitidos como solicitante, Aprovador ou revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7ca1b7b0a2ae4021dc2def637e0326044ab8749e
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331344"
---
# <a name="groupmembers-complex-type"></a><span data-ttu-id="58976-103">tipo complexo groupMembers</span><span class="sxs-lookup"><span data-stu-id="58976-103">groupMembers complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58976-104">Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="58976-104">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="58976-105">O `@odata.type` valor "`#microsoft.graph.groupMembers`" indica que esse tipo identifica uma coleção de usuários no locatário que será permitido como solicitante, Aprovador ou revisor, que são os membros de um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="58976-105">The `@odata.type` value "`#microsoft.graph.groupMembers`" indicates that this type identifies a collection of users in the tenant who will be allowed as requestor, approver, or reviewer, who are the members of a specific group.</span></span>

## <a name="properties"></a><span data-ttu-id="58976-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58976-106">Properties</span></span>

| <span data-ttu-id="58976-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58976-107">Property</span></span>                     | <span data-ttu-id="58976-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="58976-108">Type</span></span>                      | <span data-ttu-id="58976-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="58976-109">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="58976-110">id</span><span class="sxs-lookup"><span data-stu-id="58976-110">id</span></span> |<span data-ttu-id="58976-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58976-111">String</span></span> | <span data-ttu-id="58976-112">A ID do grupo no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="58976-112">The ID of the group in Azure AD.</span></span> |
| <span data-ttu-id="58976-113">descrição</span><span class="sxs-lookup"><span data-stu-id="58976-113">description</span></span> |<span data-ttu-id="58976-114">String</span><span class="sxs-lookup"><span data-stu-id="58976-114">String</span></span> | <span data-ttu-id="58976-115">O nome do grupo no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="58976-115">The name of the group in Azure AD.</span></span> <span data-ttu-id="58976-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="58976-116">Read only.</span></span> |
| <span data-ttu-id="58976-117">IsBackup</span><span class="sxs-lookup"><span data-stu-id="58976-117">isBackup</span></span> | <span data-ttu-id="58976-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="58976-118">Boolean</span></span> | <span data-ttu-id="58976-119">Para o **groupMembers** em um estágio de aprovação, essa propriedade indica que os membros do grupo são aprovadores de fallback de backup.</span><span class="sxs-lookup"><span data-stu-id="58976-119">For **groupMembers** in an approval stage, this property indicates that the group members are a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="58976-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58976-120">JSON representation</span></span>


<span data-ttu-id="58976-121">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="58976-121">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupMembers",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "id": "string (identifier)",
  "description": "string",
  "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupMembers complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
