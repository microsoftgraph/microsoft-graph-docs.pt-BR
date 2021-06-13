---
title: Tipo de recurso passwordProfile
description: Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade user é um objeto **passwordProfile**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: eketo-msft
ms.openlocfilehash: 47c55261316f2d85d27a4c993b358676578e74fd
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911330"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="e1d8f-104">Tipo de recurso passwordProfile</span><span class="sxs-lookup"><span data-stu-id="e1d8f-104">passwordProfile resource type</span></span>

<span data-ttu-id="e1d8f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1d8f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1d8f-p102">Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade [user](user.md) é um objeto **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="e1d8f-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="e1d8f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1d8f-108">Properties</span></span>
| <span data-ttu-id="e1d8f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1d8f-109">Property</span></span>     | <span data-ttu-id="e1d8f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1d8f-110">Type</span></span>   |<span data-ttu-id="e1d8f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1d8f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1d8f-112">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="e1d8f-112">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="e1d8f-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="e1d8f-113">Boolean</span></span>| <span data-ttu-id="e1d8f-114">Se `true` , no próximo login, o usuário deve alterar sua senha.</span><span class="sxs-lookup"><span data-stu-id="e1d8f-114">If `true`, at next sign-in, the user must change their password.</span></span> <span data-ttu-id="e1d8f-115">Após uma alteração de senha, essa propriedade será redefinida automaticamente para \* `false` .</span><span class="sxs-lookup"><span data-stu-id="e1d8f-115">After a password change, this property will be automatically reset to \*`false`.</span></span> <span data-ttu-id="e1d8f-116">Se não estiver definido, o padrão será `false` .</span><span class="sxs-lookup"><span data-stu-id="e1d8f-116">If not set, default is `false`.</span></span> |
|<span data-ttu-id="e1d8f-117">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="e1d8f-117">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="e1d8f-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="e1d8f-118">Boolean</span></span>| <span data-ttu-id="e1d8f-119">Se , na próxima entrada, o usuário deve executar uma `true` autenticação multifafação (MFA) antes de ser forçado a alterar sua senha.</span><span class="sxs-lookup"><span data-stu-id="e1d8f-119">If `true`, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="e1d8f-120">O comportamento é idêntico a **forceChangePasswordNextSignIn**, exceto pelo fato de que o usuário deve primeiro executar uma autenticação multifator antes da alteração da senha.</span><span class="sxs-lookup"><span data-stu-id="e1d8f-120">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="e1d8f-121">Após uma alteração de senha, essa propriedade será redefinida automaticamente para `false` .</span><span class="sxs-lookup"><span data-stu-id="e1d8f-121">After a password change, this property will be automatically reset to `false`.</span></span> <span data-ttu-id="e1d8f-122">Se não estiver definido, o padrão será `false` .</span><span class="sxs-lookup"><span data-stu-id="e1d8f-122">If not set, default is `false`.</span></span> |
|<span data-ttu-id="e1d8f-123">password</span><span class="sxs-lookup"><span data-stu-id="e1d8f-123">password</span></span>|<span data-ttu-id="e1d8f-124">String</span><span class="sxs-lookup"><span data-stu-id="e1d8f-124">String</span></span>|<span data-ttu-id="e1d8f-p105">A senha do usuário. Essa propriedade é necessária ao criar um usuário. Pode ser atualizada, mas o usuário precisará alterar a senha no próximo login. A senha deve atender a requisitos mínimos, conforme especificado pelo a propriedade **passwordPolicies** do usuário. Por padrão, é necessária uma senha forte.</span><span class="sxs-lookup"><span data-stu-id="e1d8f-p105">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1d8f-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1d8f-130">JSON representation</span></span>

<span data-ttu-id="e1d8f-131">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e1d8f-131">Here is a JSON representation of the resource</span></span>

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


