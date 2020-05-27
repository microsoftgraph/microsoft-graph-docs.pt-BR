---
title: tipo de recurso appRole
description: Representa uma função de aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 8505380b50e32e9c996f960ab2343efa7e372e4a
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383767"
---
# <a name="approle-resource-type"></a><span data-ttu-id="d6181-103">tipo de recurso appRole</span><span class="sxs-lookup"><span data-stu-id="d6181-103">appRole resource type</span></span>

<span data-ttu-id="d6181-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6181-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6181-105">Representa uma função de aplicativo que pode ser solicitada por (e concedida a) um aplicativo cliente ou que pode ser usada para atribuir um aplicativo a usuários ou grupos em uma função especificada.</span><span class="sxs-lookup"><span data-stu-id="d6181-105">Represents an application role that can be requested by (and granted to) a client application, or that can be used to assign an application to users or groups in a specified role.</span></span> 

<span data-ttu-id="d6181-106">A propriedade **appRoles** das entidades [Application](application.md) e [servicePrincipalName](serviceprincipal.md) é uma coleção de **appRole**.</span><span class="sxs-lookup"><span data-stu-id="d6181-106">The **appRoles** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities are a collection of **appRole**.</span></span> 

<span data-ttu-id="d6181-107">Com o [appRoleAssignments](approleassignment.md), as funções de aplicativo podem ser atribuídas a usuários, grupos ou a entidades de serviço de outros aplicativos.</span><span class="sxs-lookup"><span data-stu-id="d6181-107">With [appRoleAssignments](approleassignment.md), app roles can be assigned to users, groups, or other applications' service principals.</span></span>

## <a name="properties"></a><span data-ttu-id="d6181-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6181-108">Properties</span></span>

| <span data-ttu-id="d6181-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6181-109">Property</span></span>   | <span data-ttu-id="d6181-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6181-110">Type</span></span> |<span data-ttu-id="d6181-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6181-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6181-112">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="d6181-112">allowedMemberTypes</span></span>|<span data-ttu-id="d6181-113">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6181-113">String collection</span></span>|<span data-ttu-id="d6181-114">Especifica se esta função de aplicativo pode ser atribuída a usuários e grupos (definindo como `["User"]` ), a outros aplicativos (por configuração `["Application"]` ou ambos (por meio da configuração `["User", "Application"]` ).</span><span class="sxs-lookup"><span data-stu-id="d6181-114">Specifies whether this app role can be assigned to users and groups (by setting to `["User"]`), to other application's (by setting to `["Application"]`, or both (by setting to `["User", "Application"]`).</span></span> <span data-ttu-id="d6181-115">Funções de aplicativo que dão suporte à atribuição de entidades de serviço de outros aplicativos também são conhecidas como [permissões de aplicativo](/graph/auth/auth-concepts#microsoft-graph-permissions).</span><span class="sxs-lookup"><span data-stu-id="d6181-115">App roles supporting assignment of other applications' service principals are also known as [application permissions](/graph/auth/auth-concepts#microsoft-graph-permissions).</span></span>|
|<span data-ttu-id="d6181-116">description</span><span class="sxs-lookup"><span data-stu-id="d6181-116">description</span></span>|<span data-ttu-id="d6181-117">String</span><span class="sxs-lookup"><span data-stu-id="d6181-117">String</span></span>|<span data-ttu-id="d6181-118">A descrição da função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d6181-118">The description for the app role.</span></span> <span data-ttu-id="d6181-119">Isso é exibido quando a função de aplicativo está sendo atribuída e, se a função de aplicativo funciona como uma permissão de aplicativo, durante experiências de consentimento.</span><span class="sxs-lookup"><span data-stu-id="d6181-119">This is displayed when the app role is being assigned and, if the app role functions as an application permission, during  consent experiences.</span></span>|
|<span data-ttu-id="d6181-120">displayName</span><span class="sxs-lookup"><span data-stu-id="d6181-120">displayName</span></span>|<span data-ttu-id="d6181-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6181-121">String</span></span>|<span data-ttu-id="d6181-122">Nome para exibição da permissão que aparece nas experiências de consentimento e atribuição de função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d6181-122">Display name for the permission that appears in the app role assignment and consent experiences.</span></span>|
|<span data-ttu-id="d6181-123">id</span><span class="sxs-lookup"><span data-stu-id="d6181-123">id</span></span>|<span data-ttu-id="d6181-124">Guid</span><span class="sxs-lookup"><span data-stu-id="d6181-124">Guid</span></span>|<span data-ttu-id="d6181-125">Identificador de função exclusivo dentro da coleção **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="d6181-125">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="d6181-126">Ao criar uma nova função de aplicativo, um novo identificador GUID deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="d6181-126">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="d6181-127">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d6181-127">isEnabled</span></span>|<span data-ttu-id="d6181-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6181-128">Boolean</span></span>|<span data-ttu-id="d6181-129">Ao criar ou atualizar uma função de aplicativo, isso deve ser definido como **true** (que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="d6181-129">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="d6181-130">Para excluir uma função, é necessário primeiro defini-la como **false**.</span><span class="sxs-lookup"><span data-stu-id="d6181-130">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="d6181-131">Nesse ponto, em uma chamada subsequente, essa função pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="d6181-131">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="d6181-132">tenham</span><span class="sxs-lookup"><span data-stu-id="d6181-132">origin</span></span>|<span data-ttu-id="d6181-133">String</span><span class="sxs-lookup"><span data-stu-id="d6181-133">String</span></span>| <span data-ttu-id="d6181-134">Especifica se a função de aplicativo é definida no objeto [Application](application.md) ou na entidade [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="d6181-134">Specifies if the app role is defined on the [application](application.md) object or on the [servicePrincipal](serviceprincipal.md) entity.</span></span> <span data-ttu-id="d6181-135">_Não_ deve ser incluído em solicitações POST ou patch.</span><span class="sxs-lookup"><span data-stu-id="d6181-135">Must _not_ be included in any POST or PATCH requests.</span></span> <span data-ttu-id="d6181-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6181-136">Read-only.</span></span> |
|<span data-ttu-id="d6181-137">value</span><span class="sxs-lookup"><span data-stu-id="d6181-137">value</span></span>|<span data-ttu-id="d6181-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6181-138">String</span></span>|<span data-ttu-id="d6181-139">Especifica o valor a ser incluído na `roles` declaração em tokens de ID e tokens de acesso Autenticando um usuário atribuído ou uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="d6181-139">Specifies the value to include in the `roles` claim in ID tokens and access tokens authenticating an assigned user or service principal.</span></span> <span data-ttu-id="d6181-140">Não deve exceder 120 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="d6181-140">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="d6181-141">Os caracteres permitidos são `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` , bem como os caracteres nos intervalos `0-9` `A-Z` e `a-z` .</span><span class="sxs-lookup"><span data-stu-id="d6181-141">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="d6181-142">Qualquer outro caractere, incluindo o caractere de espaço, não é permitido.</span><span class="sxs-lookup"><span data-stu-id="d6181-142">Any other character, including the space character, are not allowed.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="d6181-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6181-143">JSON representation</span></span>

<span data-ttu-id="d6181-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6181-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRole"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
