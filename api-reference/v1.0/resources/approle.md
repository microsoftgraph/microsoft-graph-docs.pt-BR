---
title: tipo de recurso appRole
description: Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente que esteja chamando outro aplicativo ou que possa ser usada para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: d094a91ca7e8b923322853fbdabcf63e65e2082d
ms.sourcegitcommit: 7370fb65d11d1347123a3f6d320d2c6d36f34224
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2020
ms.locfileid: "48338162"
---
# <a name="approle-resource-type"></a><span data-ttu-id="68ece-103">tipo de recurso appRole</span><span class="sxs-lookup"><span data-stu-id="68ece-103">appRole resource type</span></span>

<span data-ttu-id="68ece-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68ece-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68ece-105">Representa uma função de aplicativo que pode ser solicitada por (e concedida a) um aplicativo cliente ou que pode ser usada para atribuir um aplicativo a usuários ou grupos em uma função especificada.</span><span class="sxs-lookup"><span data-stu-id="68ece-105">Represents an application role that can be requested by (and granted to) a client application, or that can be used to assign an application to users or groups in a specified role.</span></span> 

<span data-ttu-id="68ece-106">A propriedade **appRoles** das entidades [Application](application.md) e [servicePrincipalName](serviceprincipal.md) é uma coleção de **appRole**.</span><span class="sxs-lookup"><span data-stu-id="68ece-106">The **appRoles** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities are a collection of **appRole**.</span></span> 

<span data-ttu-id="68ece-107">Com o [appRoleAssignments](approleassignment.md), as funções de aplicativo podem ser atribuídas a usuários, grupos ou a entidades de serviço de outros aplicativos.</span><span class="sxs-lookup"><span data-stu-id="68ece-107">With [appRoleAssignments](approleassignment.md), app roles can be assigned to users, groups, or other applications' service principals.</span></span>

## <a name="properties"></a><span data-ttu-id="68ece-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68ece-108">Properties</span></span>

| <span data-ttu-id="68ece-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68ece-109">Property</span></span>   | <span data-ttu-id="68ece-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="68ece-110">Type</span></span> |<span data-ttu-id="68ece-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="68ece-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68ece-112">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="68ece-112">allowedMemberTypes</span></span>|<span data-ttu-id="68ece-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="68ece-113">String collection</span></span>|<span data-ttu-id="68ece-114">Especifica se esta função de aplicativo pode ser atribuída a usuários e grupos (definindo como `["User"]` ), a outros aplicativos (por configuração `["Application"]` ou ambos (por meio da configuração `["User", "Application"]` ).</span><span class="sxs-lookup"><span data-stu-id="68ece-114">Specifies whether this app role can be assigned to users and groups (by setting to `["User"]`), to other application's (by setting to `["Application"]`, or both (by setting to `["User", "Application"]`).</span></span> <span data-ttu-id="68ece-115">As funções de aplicativo que dão suporte à atribuição à entidade de serviço de outros aplicativos são também conhecidas como [permissões de aplicativo](/graph/auth/auth-concepts#microsoft-graph-permissions).</span><span class="sxs-lookup"><span data-stu-id="68ece-115">App roles supporting assignment to other applications' service principals are also known as [application permissions](/graph/auth/auth-concepts#microsoft-graph-permissions).</span></span> <span data-ttu-id="68ece-116">O valor "Application" só tem suporte para funções de aplicativo definidas em entidades de **aplicativo** .</span><span class="sxs-lookup"><span data-stu-id="68ece-116">The "Application" value is only supported for app roles defined on **application** entities.</span></span>|
|<span data-ttu-id="68ece-117">description</span><span class="sxs-lookup"><span data-stu-id="68ece-117">description</span></span>|<span data-ttu-id="68ece-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68ece-118">String</span></span>|<span data-ttu-id="68ece-119">A descrição da função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="68ece-119">The description for the app role.</span></span> <span data-ttu-id="68ece-120">Isso é exibido quando a função de aplicativo está sendo atribuída e, se a função de aplicativo funciona como uma permissão de aplicativo, durante experiências de consentimento.</span><span class="sxs-lookup"><span data-stu-id="68ece-120">This is displayed when the app role is being assigned and, if the app role functions as an application permission, during  consent experiences.</span></span>|
|<span data-ttu-id="68ece-121">displayName</span><span class="sxs-lookup"><span data-stu-id="68ece-121">displayName</span></span>|<span data-ttu-id="68ece-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68ece-122">String</span></span>|<span data-ttu-id="68ece-123">Nome para exibição da permissão que aparece nas experiências de consentimento e atribuição de função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="68ece-123">Display name for the permission that appears in the app role assignment and consent experiences.</span></span>|
|<span data-ttu-id="68ece-124">id</span><span class="sxs-lookup"><span data-stu-id="68ece-124">id</span></span>|<span data-ttu-id="68ece-125">Guid</span><span class="sxs-lookup"><span data-stu-id="68ece-125">Guid</span></span>|<span data-ttu-id="68ece-126">Identificador de função exclusivo dentro da coleção **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="68ece-126">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="68ece-127">Ao criar uma nova função de aplicativo, um novo identificador GUID deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="68ece-127">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="68ece-128">isEnabled</span><span class="sxs-lookup"><span data-stu-id="68ece-128">isEnabled</span></span>|<span data-ttu-id="68ece-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="68ece-129">Boolean</span></span>|<span data-ttu-id="68ece-130">Ao criar ou atualizar uma função de aplicativo, isso deve ser definido como **true** (que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="68ece-130">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="68ece-131">Para excluir uma função, é necessário primeiro defini-la como **false**.</span><span class="sxs-lookup"><span data-stu-id="68ece-131">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="68ece-132">Nesse ponto, em uma chamada subsequente, essa função pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="68ece-132">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="68ece-133">tenham</span><span class="sxs-lookup"><span data-stu-id="68ece-133">origin</span></span>|<span data-ttu-id="68ece-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68ece-134">String</span></span>| <span data-ttu-id="68ece-135">Especifica se a função de aplicativo é definida no objeto [Application](application.md) ou na entidade [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="68ece-135">Specifies if the app role is defined on the [application](application.md) object or on the [servicePrincipal](serviceprincipal.md) entity.</span></span> <span data-ttu-id="68ece-136">_Não_ deve ser incluído em solicitações POST ou patch.</span><span class="sxs-lookup"><span data-stu-id="68ece-136">Must _not_ be included in any POST or PATCH requests.</span></span> <span data-ttu-id="68ece-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="68ece-137">Read-only.</span></span> |
|<span data-ttu-id="68ece-138">value</span><span class="sxs-lookup"><span data-stu-id="68ece-138">value</span></span>|<span data-ttu-id="68ece-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68ece-139">String</span></span>|<span data-ttu-id="68ece-140">Especifica o valor a ser incluído na `roles` declaração em tokens de ID e tokens de acesso Autenticando um usuário atribuído ou uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="68ece-140">Specifies the value to include in the `roles` claim in ID tokens and access tokens authenticating an assigned user or service principal.</span></span> <span data-ttu-id="68ece-141">Não deve exceder 120 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="68ece-141">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="68ece-142">Os caracteres permitidos são `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` , bem como os caracteres nos intervalos `0-9` `A-Z` e `a-z` .</span><span class="sxs-lookup"><span data-stu-id="68ece-142">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="68ece-143">Qualquer outro caractere, incluindo o caractere de espaço, não é permitido.</span><span class="sxs-lookup"><span data-stu-id="68ece-143">Any other character, including the space character, are not allowed.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="68ece-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68ece-144">JSON representation</span></span>

<span data-ttu-id="68ece-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68ece-145">The following is a JSON representation of the resource.</span></span>

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

