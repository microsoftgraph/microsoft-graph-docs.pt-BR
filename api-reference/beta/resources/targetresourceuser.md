---
title: tipo de recurso de targetResourceUser
description: Indica o objeto de usuário que foi adicionado, atualizado ou excluído por administradores como parte da atividade de auditoria. Derivado do recurso targetResource.
ms.openlocfilehash: 632d0551b3aba434c3309c8c874947708eb9a9f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036427"
---
# <a name="targetresourceuser-resource-type"></a><span data-ttu-id="656a2-104">tipo de recurso de targetResourceUser</span><span class="sxs-lookup"><span data-stu-id="656a2-104">targetResourceUser resource type</span></span>
<span data-ttu-id="656a2-105">Indica o objeto de usuário que foi adicionado, atualizado ou excluído por administradores como parte da atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="656a2-105">Indicates the user object that was added, updated or deleted by admins as part of audit activity.</span></span> <span data-ttu-id="656a2-106">Derivado do recurso [targetResource](targetresource.md) .</span><span class="sxs-lookup"><span data-stu-id="656a2-106">Derived from the [targetResource](targetresource.md) resource.</span></span>


## <a name="properties"></a><span data-ttu-id="656a2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="656a2-107">Properties</span></span>
| <span data-ttu-id="656a2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="656a2-108">Property</span></span>     | <span data-ttu-id="656a2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="656a2-109">Type</span></span>   |<span data-ttu-id="656a2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="656a2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="656a2-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="656a2-111">userPrincipalName</span></span>|<span data-ttu-id="656a2-112">String</span><span class="sxs-lookup"><span data-stu-id="656a2-112">String</span></span>|<span data-ttu-id="656a2-113">Indica a Id exclusiva do usuário.</span><span class="sxs-lookup"><span data-stu-id="656a2-113">Indicates the Unique Id of the User.</span></span> <span data-ttu-id="656a2-114">Se refere à Id de usuário para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="656a2-114">Refers to User Id for a specific user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="656a2-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="656a2-115">JSON representation</span></span>

<span data-ttu-id="656a2-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="656a2-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceUser"
}-->

```json
{
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->