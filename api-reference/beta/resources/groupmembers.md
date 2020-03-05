---
title: tipo complexo groupMembers
description: Identifica uma coleção de usuários no locatário que serão permitidos como solicitante, Aprovador ou revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5b4170a3baf186d907340bc1c490c508644ec30a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496933"
---
# <a name="groupmembers-complex-type"></a><span data-ttu-id="80a2d-103">tipo complexo groupMembers</span><span class="sxs-lookup"><span data-stu-id="80a2d-103">groupMembers complex type</span></span>

<span data-ttu-id="80a2d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="80a2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80a2d-105">Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="80a2d-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="80a2d-106">O `@odata.type` valor "`#microsoft.graph.groupMembers`" indica que esse tipo identifica uma coleção de usuários no locatário que será permitido como solicitante, Aprovador ou revisor, que são os membros de um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="80a2d-106">The `@odata.type` value "`#microsoft.graph.groupMembers`" indicates that this type identifies a collection of users in the tenant who will be allowed as requestor, approver, or reviewer, who are the members of a specific group.</span></span>

## <a name="properties"></a><span data-ttu-id="80a2d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80a2d-107">Properties</span></span>

| <span data-ttu-id="80a2d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80a2d-108">Property</span></span>                     | <span data-ttu-id="80a2d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="80a2d-109">Type</span></span>                      | <span data-ttu-id="80a2d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="80a2d-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="80a2d-111">id</span><span class="sxs-lookup"><span data-stu-id="80a2d-111">id</span></span> |<span data-ttu-id="80a2d-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80a2d-112">String</span></span> | <span data-ttu-id="80a2d-113">A ID do grupo no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="80a2d-113">The ID of the group in Azure AD.</span></span> |
| <span data-ttu-id="80a2d-114">description</span><span class="sxs-lookup"><span data-stu-id="80a2d-114">description</span></span> |<span data-ttu-id="80a2d-115">String</span><span class="sxs-lookup"><span data-stu-id="80a2d-115">String</span></span> | <span data-ttu-id="80a2d-116">O nome do grupo no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="80a2d-116">The name of the group in Azure AD.</span></span> <span data-ttu-id="80a2d-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80a2d-117">Read only.</span></span> |
| <span data-ttu-id="80a2d-118">IsBackup</span><span class="sxs-lookup"><span data-stu-id="80a2d-118">isBackup</span></span> | <span data-ttu-id="80a2d-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="80a2d-119">Boolean</span></span> | <span data-ttu-id="80a2d-120">Para o **groupMembers** em um estágio de aprovação, essa propriedade indica que os membros do grupo são aprovadores de fallback de backup.</span><span class="sxs-lookup"><span data-stu-id="80a2d-120">For **groupMembers** in an approval stage, this property indicates that the group members are a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="80a2d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80a2d-121">JSON representation</span></span>


<span data-ttu-id="80a2d-122">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="80a2d-122">The following is a JSON representation of the type.</span></span>

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
