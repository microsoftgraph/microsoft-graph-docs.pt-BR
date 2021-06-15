---
title: Tipo de recurso passwordProfile
description: Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade user é um objeto **passwordProfile**.
localization_priority: Priority
author: eketo-msft
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 4a61c570974edcfc1431af211e131c24cfec6589
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911645"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="cf46a-104">Tipo de recurso passwordProfile</span><span class="sxs-lookup"><span data-stu-id="cf46a-104">passwordProfile resource type</span></span>

<span data-ttu-id="cf46a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf46a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cf46a-p102">Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade [user](user.md) é um objeto **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="cf46a-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="cf46a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf46a-108">Properties</span></span>
| <span data-ttu-id="cf46a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf46a-109">Property</span></span>     | <span data-ttu-id="cf46a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf46a-110">Type</span></span>   |<span data-ttu-id="cf46a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf46a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf46a-112">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="cf46a-112">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="cf46a-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="cf46a-113">Boolean</span></span>| <span data-ttu-id="cf46a-114">`true` se o usuário precisar alterar sua senha no próximo logon; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="cf46a-114">`true` if the user must change her password on the next login; otherwise `false`.</span></span> |
|<span data-ttu-id="cf46a-115">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="cf46a-115">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="cf46a-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="cf46a-116">Boolean</span></span>| <span data-ttu-id="cf46a-117">Se `true`, na próxima conexão, o usuário deverá executar uma autenticação multifator (MFA) antes de ser forçado a alterar sua senha.</span><span class="sxs-lookup"><span data-stu-id="cf46a-117">If `true`, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="cf46a-118">O comportamento é idêntico a **forceChangePasswordNextSignIn**, exceto pelo fato de que o usuário deve primeiro executar uma autenticação multifator antes da alteração da senha.</span><span class="sxs-lookup"><span data-stu-id="cf46a-118">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="cf46a-119">Após a alteração da senha, esta propriedade será redefinida automaticamente para `false`.</span><span class="sxs-lookup"><span data-stu-id="cf46a-119">After a password change, this property will be automatically reset to `false`.</span></span> <span data-ttu-id="cf46a-120">Se não estiver definido, o padrão será `false`.</span><span class="sxs-lookup"><span data-stu-id="cf46a-120">If not set, default is `false`.</span></span> |
|<span data-ttu-id="cf46a-121">password</span><span class="sxs-lookup"><span data-stu-id="cf46a-121">password</span></span>|<span data-ttu-id="cf46a-122">String</span><span class="sxs-lookup"><span data-stu-id="cf46a-122">String</span></span>|<span data-ttu-id="cf46a-p104">A senha do usuário. Essa propriedade é necessária ao criar um usuário. Pode ser atualizada, mas o usuário precisará alterar a senha no próximo login. A senha deve atender a requisitos mínimos, conforme especificado pelo a propriedade **passwordPolicies** do usuário. Por padrão, é necessária uma senha forte.</span><span class="sxs-lookup"><span data-stu-id="cf46a-p104">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf46a-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf46a-128">JSON representation</span></span>

<span data-ttu-id="cf46a-129">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="cf46a-129">Here is a JSON representation of the resource</span></span>

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

