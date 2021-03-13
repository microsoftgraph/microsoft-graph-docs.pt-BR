---
title: tipo complexo groupMembers
description: Identifica uma coleção de usuários no locatário que serão permitidos como solicitante, aprovador ou revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0069cd6a8fd738c17a9035b519c4f141c3a5fa55
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761413"
---
# <a name="groupmembers-complex-type"></a><span data-ttu-id="2776e-103">tipo complexo groupMembers</span><span class="sxs-lookup"><span data-stu-id="2776e-103">groupMembers complex type</span></span>

<span data-ttu-id="2776e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2776e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2776e-105">Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2776e-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="2776e-106">O valor " " indica que esse tipo identifica uma coleção de usuários no locatário que serão permitidos como solicitante, aprovador ou `@odata.type` revisor, que são membros de um `#microsoft.graph.groupMembers` grupo específico.</span><span class="sxs-lookup"><span data-stu-id="2776e-106">The `@odata.type` value "`#microsoft.graph.groupMembers`" indicates that this type identifies a collection of users in the tenant who will be allowed as requestor, approver, or reviewer, who are the members of a specific group.</span></span>

## <a name="properties"></a><span data-ttu-id="2776e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2776e-107">Properties</span></span>

| <span data-ttu-id="2776e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2776e-108">Property</span></span>                     | <span data-ttu-id="2776e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2776e-109">Type</span></span>                      | <span data-ttu-id="2776e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2776e-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="2776e-111">id</span><span class="sxs-lookup"><span data-stu-id="2776e-111">id</span></span> |<span data-ttu-id="2776e-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2776e-112">String</span></span> | <span data-ttu-id="2776e-113">A ID do grupo no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2776e-113">The ID of the group in Azure AD.</span></span> |
| <span data-ttu-id="2776e-114">descrição</span><span class="sxs-lookup"><span data-stu-id="2776e-114">description</span></span> |<span data-ttu-id="2776e-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2776e-115">String</span></span> | <span data-ttu-id="2776e-116">O nome do grupo no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2776e-116">The name of the group in Azure AD.</span></span> <span data-ttu-id="2776e-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2776e-117">Read only.</span></span> |
| <span data-ttu-id="2776e-118">isBackup</span><span class="sxs-lookup"><span data-stu-id="2776e-118">isBackup</span></span> | <span data-ttu-id="2776e-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="2776e-119">Boolean</span></span> | <span data-ttu-id="2776e-120">Para **groupMembers** em um estágio de aprovação, essa propriedade indica que os membros do grupo são um aprovador de fallback de backup.</span><span class="sxs-lookup"><span data-stu-id="2776e-120">For **groupMembers** in an approval stage, this property indicates that the group members are a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2776e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2776e-121">JSON representation</span></span>


<span data-ttu-id="2776e-122">A seguir está uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="2776e-122">The following is a JSON representation of the type.</span></span>

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


