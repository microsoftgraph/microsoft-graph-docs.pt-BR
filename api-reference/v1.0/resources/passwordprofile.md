---
title: Tipo de recurso passwordProfile
description: Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade user é um objeto **passwordProfile**.
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ae916f3723ed59bc317e3a59507da81841d0c563
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035592"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="2210b-104">Tipo de recurso passwordProfile</span><span class="sxs-lookup"><span data-stu-id="2210b-104">passwordProfile resource type</span></span>

<span data-ttu-id="2210b-p102">Contém o perfil de senha associado a um usuário. A propriedade **passwordProfile** da entidade [user](user.md) é um objeto **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="2210b-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="2210b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2210b-107">Properties</span></span>
| <span data-ttu-id="2210b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2210b-108">Property</span></span>     | <span data-ttu-id="2210b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2210b-109">Type</span></span>   |<span data-ttu-id="2210b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2210b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2210b-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="2210b-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="2210b-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="2210b-112">Boolean</span></span>| <span data-ttu-id="2210b-113">**true** se o usuário precisa alterar sua senha no próximo login; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="2210b-113">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="2210b-114">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="2210b-114">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="2210b-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="2210b-115">Boolean</span></span>| <span data-ttu-id="2210b-116">Se for **true**, na próxima conexão, o usuário deverá executar uma Autenticação Multifator (MFA) antes de ser forçado a alterar sua senha.</span><span class="sxs-lookup"><span data-stu-id="2210b-116">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="2210b-117">O comportamento é idêntico a **forceChangePasswordNextSignIn**, exceto pelo fato de que o usuário deve primeiro executar uma autenticação multifator antes da alteração da senha.</span><span class="sxs-lookup"><span data-stu-id="2210b-117">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="2210b-118">Após uma alteração de senha, esta propriedade será automaticamente redefinida para **false**.</span><span class="sxs-lookup"><span data-stu-id="2210b-118">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="2210b-119">Caso não seja definida, o padrão é **false**.</span><span class="sxs-lookup"><span data-stu-id="2210b-119">If not set, default is **false**.</span></span> |
|<span data-ttu-id="2210b-120">password</span><span class="sxs-lookup"><span data-stu-id="2210b-120">password</span></span>|<span data-ttu-id="2210b-121">String</span><span class="sxs-lookup"><span data-stu-id="2210b-121">String</span></span>|<span data-ttu-id="2210b-p104">A senha do usuário. Essa propriedade é necessária ao criar um usuário. Pode ser atualizada, mas o usuário precisará alterar a senha no próximo login. A senha deve atender a requisitos mínimos, conforme especificado pelo a propriedade **passwordPolicies** do usuário. Por padrão, é necessária uma senha forte.</span><span class="sxs-lookup"><span data-stu-id="2210b-p104">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2210b-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2210b-127">JSON representation</span></span>

<span data-ttu-id="2210b-128">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2210b-128">Here is a JSON representation of the resource</span></span>

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
