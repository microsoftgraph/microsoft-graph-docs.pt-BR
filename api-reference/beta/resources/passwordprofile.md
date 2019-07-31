---
title: Tipo de recurso passwordProfile
description: Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade user é um objeto **passwordProfile**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ea3f3daa4807fd56e39930a059d69221e141879c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966224"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="b2499-104">Tipo de recurso passwordProfile</span><span class="sxs-lookup"><span data-stu-id="b2499-104">passwordProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2499-p102">Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade [user](user.md) é um objeto **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="b2499-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="b2499-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2499-107">Properties</span></span>
| <span data-ttu-id="b2499-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2499-108">Property</span></span>     | <span data-ttu-id="b2499-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2499-109">Type</span></span>   |<span data-ttu-id="b2499-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2499-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2499-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="b2499-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="b2499-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2499-112">Boolean</span></span>| <span data-ttu-id="b2499-113">Se **true**, no próximo logon, o usuário deve alterar a senha.</span><span class="sxs-lookup"><span data-stu-id="b2499-113">If **true**, at next sign-in, the user must change their password.</span></span> <span data-ttu-id="b2499-114">Após uma alteração de senha, essa propriedade será automaticamente redefinida como \***false**.</span><span class="sxs-lookup"><span data-stu-id="b2499-114">After a password change, this property will be automatically reset to \***false**.</span></span> <span data-ttu-id="b2499-115">Caso não seja definida, o padrão é **false**.</span><span class="sxs-lookup"><span data-stu-id="b2499-115">If not set, default is **false**.</span></span> |
|<span data-ttu-id="b2499-116">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="b2499-116">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="b2499-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2499-117">Boolean</span></span>| <span data-ttu-id="b2499-118">Se for **true**, na próxima conexão, o usuário deverá executar uma Autenticação Multifator (MFA) antes de ser forçado a alterar sua senha.</span><span class="sxs-lookup"><span data-stu-id="b2499-118">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="b2499-119">O comportamento é idêntico a **forceChangePasswordNextSignIn**, exceto pelo fato de que o usuário deve primeiro executar uma autenticação multifator antes da alteração da senha.</span><span class="sxs-lookup"><span data-stu-id="b2499-119">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="b2499-120">Após uma alteração de senha, esta propriedade será automaticamente redefinida para **false**.</span><span class="sxs-lookup"><span data-stu-id="b2499-120">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="b2499-121">Caso não seja definida, o padrão é **false**.</span><span class="sxs-lookup"><span data-stu-id="b2499-121">If not set, default is **false**.</span></span> |
|<span data-ttu-id="b2499-122">password</span><span class="sxs-lookup"><span data-stu-id="b2499-122">password</span></span>|<span data-ttu-id="b2499-123">String</span><span class="sxs-lookup"><span data-stu-id="b2499-123">String</span></span>|<span data-ttu-id="b2499-p105">A senha do usuário. Essa propriedade é necessária ao criar um usuário. Pode ser atualizada, mas o usuário precisará alterar a senha no próximo login. A senha deve atender a requisitos mínimos, conforme especificado pelo a propriedade **passwordPolicies** do usuário. Por padrão, é necessária uma senha forte.</span><span class="sxs-lookup"><span data-stu-id="b2499-p105">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2499-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2499-129">JSON representation</span></span>

<span data-ttu-id="b2499-130">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b2499-130">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordProfile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
  "forceChangePasswordNextSignInWithMfa": false,
  "password": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
