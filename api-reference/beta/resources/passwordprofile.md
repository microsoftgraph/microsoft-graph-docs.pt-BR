---
title: Tipo de recurso passwordProfile
description: Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade user é um objeto **passwordProfile**.
ms.openlocfilehash: 71a91f0848ba8218d16a59c9e1f867d14e5cad9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040991"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="a6fe3-104">Tipo de recurso passwordProfile</span><span class="sxs-lookup"><span data-stu-id="a6fe3-104">passwordProfile resource type</span></span>

> <span data-ttu-id="a6fe3-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a6fe3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6fe3-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a6fe3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6fe3-p103">Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade [user](user.md) é um objeto **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="a6fe3-p103">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="a6fe3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a6fe3-109">Properties</span></span>
| <span data-ttu-id="a6fe3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6fe3-110">Property</span></span>     | <span data-ttu-id="a6fe3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6fe3-111">Type</span></span>   |<span data-ttu-id="a6fe3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6fe3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6fe3-113">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="a6fe3-113">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="a6fe3-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6fe3-114">Boolean</span></span>| <span data-ttu-id="a6fe3-115">Se **verdadeiro**, na próxima tela de entrada, o usuário deve alterar sua senha.</span><span class="sxs-lookup"><span data-stu-id="a6fe3-115">If **true**, at next sign-in, the user must change their password.</span></span> <span data-ttu-id="a6fe3-116">Após uma alteração de senha, essa propriedade será redefinida automaticamente como \***false**.</span><span class="sxs-lookup"><span data-stu-id="a6fe3-116">After a password change, this property will be automatically reset to \***false**.</span></span> <span data-ttu-id="a6fe3-117">Se não for definido, o padrão é **false**.</span><span class="sxs-lookup"><span data-stu-id="a6fe3-117">If not set, default is **false**.</span></span> |
|<span data-ttu-id="a6fe3-118">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="a6fe3-118">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="a6fe3-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6fe3-119">Boolean</span></span>| <span data-ttu-id="a6fe3-120">Se **verdadeiro**, na próxima tela de entrada, o usuário deve executar uma autenticação multifator (MFA) antes de serem é forçado a alterar sua senha.</span><span class="sxs-lookup"><span data-stu-id="a6fe3-120">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="a6fe3-121">O comportamento é idêntico ao **forceChangePasswordNextSignIn** , exceto pelo fato do usuário é necessário para realizar primeiro uma autenticação multifator antes de alteração de senha.</span><span class="sxs-lookup"><span data-stu-id="a6fe3-121">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="a6fe3-122">Após uma alteração de senha, esta propriedade será redefinida para **false**automaticamente.</span><span class="sxs-lookup"><span data-stu-id="a6fe3-122">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="a6fe3-123">Se não for definido, o padrão é **false**.</span><span class="sxs-lookup"><span data-stu-id="a6fe3-123">If not set, default is **false**.</span></span> |
|<span data-ttu-id="a6fe3-124">password</span><span class="sxs-lookup"><span data-stu-id="a6fe3-124">password</span></span>|<span data-ttu-id="a6fe3-125">String</span><span class="sxs-lookup"><span data-stu-id="a6fe3-125">String</span></span>|<span data-ttu-id="a6fe3-p106">A senha do usuário. Essa propriedade é necessária ao criar um usuário. Pode ser atualizada, mas o usuário precisará alterar a senha no próximo login. A senha deve atender a requisitos mínimos, conforme especificado pelo a propriedade **passwordPolicies** do usuário. Por padrão, é necessária uma senha forte.</span><span class="sxs-lookup"><span data-stu-id="a6fe3-p106">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6fe3-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a6fe3-131">JSON representation</span></span>

<span data-ttu-id="a6fe3-132">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a6fe3-132">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordprofile"
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