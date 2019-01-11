---
title: Tipo de recurso passwordProfile
description: Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade user é um objeto **passwordProfile**.
localization_priority: Priority
ms.openlocfilehash: 80d774906fb4897f57b943af827cfbc32e90511f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819660"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="a2f3a-104">Tipo de recurso passwordProfile</span><span class="sxs-lookup"><span data-stu-id="a2f3a-104">passwordProfile resource type</span></span>

<span data-ttu-id="a2f3a-p102">Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade [user](user.md) é um objeto **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="a2f3a-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="a2f3a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2f3a-107">Properties</span></span>
| <span data-ttu-id="a2f3a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2f3a-108">Property</span></span>     | <span data-ttu-id="a2f3a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2f3a-109">Type</span></span>   |<span data-ttu-id="a2f3a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2f3a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2f3a-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="a2f3a-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="a2f3a-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="a2f3a-112">Boolean</span></span>| <span data-ttu-id="a2f3a-113">**true** se o usuário precisa alterar sua senha no próximo login; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="a2f3a-113">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="a2f3a-114">password</span><span class="sxs-lookup"><span data-stu-id="a2f3a-114">password</span></span>|<span data-ttu-id="a2f3a-115">String</span><span class="sxs-lookup"><span data-stu-id="a2f3a-115">String</span></span>|<span data-ttu-id="a2f3a-p103">A senha do usuário. Essa propriedade é necessária ao criar um usuário. Pode ser atualizada, mas o usuário precisará alterar a senha no próximo login. A senha deve atender a requisitos mínimos, conforme especificado pelo a propriedade **passwordPolicies** do usuário. Por padrão, é necessária uma senha forte.</span><span class="sxs-lookup"><span data-stu-id="a2f3a-p103">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2f3a-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2f3a-121">JSON representation</span></span>

<span data-ttu-id="a2f3a-122">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a2f3a-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordProfile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
  "password": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
