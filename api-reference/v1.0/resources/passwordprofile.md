---
title: Tipo de recurso passwordProfile
description: Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade user é um objeto **passwordProfile**.
localization_priority: Priority
author: eketo-msft
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 0b74a273d4ccab75814c32bc8b185f15de02e6a3
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208194"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="e8d05-104">Tipo de recurso passwordProfile</span><span class="sxs-lookup"><span data-stu-id="e8d05-104">passwordProfile resource type</span></span>

<span data-ttu-id="e8d05-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8d05-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e8d05-p102">Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade [user](user.md) é um objeto **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="e8d05-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="e8d05-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8d05-108">Properties</span></span>
| <span data-ttu-id="e8d05-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8d05-109">Property</span></span>     | <span data-ttu-id="e8d05-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8d05-110">Type</span></span>   |<span data-ttu-id="e8d05-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8d05-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8d05-112">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="e8d05-112">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="e8d05-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="e8d05-113">Boolean</span></span>| <span data-ttu-id="e8d05-114">`true` se o usuário precisar alterar sua senha no próximo logon; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="e8d05-114">`true` if the user must change her password on the next login; otherwise `false`.</span></span> <span data-ttu-id="e8d05-115">Se não for definido, o padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="e8d05-115">If not set, default is `false`.</span></span> <span data-ttu-id="e8d05-116">**OBSERVAÇÃO:**  Para locatários do Azure B2C, defina `false` e use políticas personalizadas e fluxos de usuário para forçar a redefinição de senha na primeira entrada.</span><span class="sxs-lookup"><span data-stu-id="e8d05-116">**NOTE:**  For Azure B2C tenants, set to `false` and instead use custom policies and user flows to force password reset at first sign in.</span></span> <span data-ttu-id="e8d05-117">Confira [Forçar redefinição de senha no primeiro logon](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon).</span><span class="sxs-lookup"><span data-stu-id="e8d05-117">See [Force password reset at first logon](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon).</span></span>|
|<span data-ttu-id="e8d05-118">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="e8d05-118">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="e8d05-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="e8d05-119">Boolean</span></span>| <span data-ttu-id="e8d05-120">Se `true`, na próxima conexão, o usuário deverá executar uma autenticação multifator (MFA) antes de ser forçado a alterar sua senha.</span><span class="sxs-lookup"><span data-stu-id="e8d05-120">If `true`, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="e8d05-121">O comportamento é idêntico a **forceChangePasswordNextSignIn**, exceto pelo fato de que o usuário deve primeiro executar uma autenticação multifator antes da alteração da senha.</span><span class="sxs-lookup"><span data-stu-id="e8d05-121">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="e8d05-122">Após a alteração da senha, esta propriedade será redefinida automaticamente para `false`.</span><span class="sxs-lookup"><span data-stu-id="e8d05-122">After a password change, this property will be automatically reset to `false`.</span></span> <span data-ttu-id="e8d05-123">Se não estiver definido, o padrão será `false`.</span><span class="sxs-lookup"><span data-stu-id="e8d05-123">If not set, default is `false`.</span></span> |
|<span data-ttu-id="e8d05-124">password</span><span class="sxs-lookup"><span data-stu-id="e8d05-124">password</span></span>|<span data-ttu-id="e8d05-125">String</span><span class="sxs-lookup"><span data-stu-id="e8d05-125">String</span></span>|<span data-ttu-id="e8d05-p105">A senha do usuário. Essa propriedade é necessária ao criar um usuário. Pode ser atualizada, mas o usuário precisará alterar a senha no próximo login. A senha deve atender a requisitos mínimos, conforme especificado pelo a propriedade **passwordPolicies** do usuário. Por padrão, é necessária uma senha forte.</span><span class="sxs-lookup"><span data-stu-id="e8d05-p105">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8d05-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8d05-131">JSON representation</span></span>

<span data-ttu-id="e8d05-132">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e8d05-132">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="e8d05-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="e8d05-133">See also</span></span>

[<span data-ttu-id="e8d05-134">Atualizar o passwordProfile de um usuário</span><span class="sxs-lookup"><span data-stu-id="e8d05-134">Update the passwordProfile of a user</span></span>](../api/user-update.md#example-3-update-the-passwordprofile-of-a-user-to-reset-their-password)
