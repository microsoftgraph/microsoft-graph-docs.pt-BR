---
title: Tipo de recurso appRole
description: Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente chamando outro aplicativo ou que pode ser usada para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f61eca3971baeb426f4a20697a1e7ffca74e5071
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132472"
---
# <a name="approle-resource-type"></a><span data-ttu-id="a51b3-103">Tipo de recurso appRole</span><span class="sxs-lookup"><span data-stu-id="a51b3-103">appRole resource type</span></span>

<span data-ttu-id="a51b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a51b3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a51b3-105">Representa uma função de aplicativo que pode ser solicitada (e concedida a) um aplicativo cliente ou que pode ser usada para atribuir um aplicativo a usuários ou grupos em uma função especificada.</span><span class="sxs-lookup"><span data-stu-id="a51b3-105">Represents an application role that can be requested by (and granted to) a client application, or that can be used to assign an application to users or groups in a specified role.</span></span> 

<span data-ttu-id="a51b3-106">A **propriedade appRoles** do [aplicativo e](application.md) [entidades servicePrincipal](serviceprincipal.md) são uma coleção de **appRole**.</span><span class="sxs-lookup"><span data-stu-id="a51b3-106">The **appRoles** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities are a collection of **appRole**.</span></span> 

<span data-ttu-id="a51b3-107">Com [appRoleAssignments,](approleassignment.md)as funções de aplicativo podem ser atribuídas a usuários, grupos ou entidades de serviço de outros aplicativos.</span><span class="sxs-lookup"><span data-stu-id="a51b3-107">With [appRoleAssignments](approleassignment.md), app roles can be assigned to users, groups, or other applications' service principals.</span></span>

## <a name="properties"></a><span data-ttu-id="a51b3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a51b3-108">Properties</span></span>

| <span data-ttu-id="a51b3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a51b3-109">Property</span></span>   | <span data-ttu-id="a51b3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a51b3-110">Type</span></span> |<span data-ttu-id="a51b3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a51b3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a51b3-112">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="a51b3-112">allowedMemberTypes</span></span>|<span data-ttu-id="a51b3-113">String collection</span><span class="sxs-lookup"><span data-stu-id="a51b3-113">String collection</span></span>|<span data-ttu-id="a51b3-114">Especifica se essa função de aplicativo pode ser atribuída a usuários e grupos (configurando como ), para outro aplicativo (configurando para , ou `["User"]` `["Application"]` ambos (definindo como `["User", "Application"]` ).</span><span class="sxs-lookup"><span data-stu-id="a51b3-114">Specifies whether this app role can be assigned to users and groups (by setting to `["User"]`), to other application's (by setting to `["Application"]`, or both (by setting to `["User", "Application"]`).</span></span> <span data-ttu-id="a51b3-115">Funções de aplicativo que suportam a atribuição a entidades de serviço de outros aplicativos também são conhecidas como [permissões de aplicativo.](/graph/auth/auth-concepts#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="a51b3-115">App roles supporting assignment to other applications' service principals are also known as [application permissions](/graph/auth/auth-concepts#microsoft-graph-permissions).</span></span> <span data-ttu-id="a51b3-116">O valor "Aplicativo" só tem suporte para funções de aplicativo definidas em **entidades** de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a51b3-116">The "Application" value is only supported for app roles defined on **application** entities.</span></span>|
|<span data-ttu-id="a51b3-117">description</span><span class="sxs-lookup"><span data-stu-id="a51b3-117">description</span></span>|<span data-ttu-id="a51b3-118">String</span><span class="sxs-lookup"><span data-stu-id="a51b3-118">String</span></span>|<span data-ttu-id="a51b3-119">A descrição da função do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a51b3-119">The description for the app role.</span></span> <span data-ttu-id="a51b3-120">Isso é exibido quando a função de aplicativo está sendo atribuída e, se a função de aplicativo funciona como uma permissão de aplicativo, durante experiências de consentimento.</span><span class="sxs-lookup"><span data-stu-id="a51b3-120">This is displayed when the app role is being assigned and, if the app role functions as an application permission, during  consent experiences.</span></span>|
|<span data-ttu-id="a51b3-121">displayName</span><span class="sxs-lookup"><span data-stu-id="a51b3-121">displayName</span></span>|<span data-ttu-id="a51b3-122">String</span><span class="sxs-lookup"><span data-stu-id="a51b3-122">String</span></span>|<span data-ttu-id="a51b3-123">Nome de exibição da permissão que aparece na atribuição de função de aplicativo e experiências de consentimento.</span><span class="sxs-lookup"><span data-stu-id="a51b3-123">Display name for the permission that appears in the app role assignment and consent experiences.</span></span>|
|<span data-ttu-id="a51b3-124">id</span><span class="sxs-lookup"><span data-stu-id="a51b3-124">id</span></span>|<span data-ttu-id="a51b3-125">Guid</span><span class="sxs-lookup"><span data-stu-id="a51b3-125">Guid</span></span>|<span data-ttu-id="a51b3-126">Identificador de função exclusivo dentro da **coleção appRoles.**</span><span class="sxs-lookup"><span data-stu-id="a51b3-126">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="a51b3-127">Ao criar uma nova função de aplicativo, um novo identificador Guid deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="a51b3-127">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="a51b3-128">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a51b3-128">isEnabled</span></span>|<span data-ttu-id="a51b3-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="a51b3-129">Boolean</span></span>|<span data-ttu-id="a51b3-130">Ao criar ou atualizar uma função de aplicativo, isso deve ser definido como **verdadeiro** (que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="a51b3-130">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="a51b3-131">Para excluir uma função, primeiro deve ser definido como **false**.</span><span class="sxs-lookup"><span data-stu-id="a51b3-131">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="a51b3-132">Nesse ponto, em uma chamada subsequente, essa função pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="a51b3-132">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="a51b3-133">origin</span><span class="sxs-lookup"><span data-stu-id="a51b3-133">origin</span></span>|<span data-ttu-id="a51b3-134">String</span><span class="sxs-lookup"><span data-stu-id="a51b3-134">String</span></span>| <span data-ttu-id="a51b3-135">Especifica se a função de aplicativo é definida no [objeto de](application.md) aplicativo ou na [entidade servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="a51b3-135">Specifies if the app role is defined on the [application](application.md) object or on the [servicePrincipal](serviceprincipal.md) entity.</span></span> <span data-ttu-id="a51b3-136">Não _deve ser_ incluído em solicitações POST ou PATCH.</span><span class="sxs-lookup"><span data-stu-id="a51b3-136">Must _not_ be included in any POST or PATCH requests.</span></span> <span data-ttu-id="a51b3-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a51b3-137">Read-only.</span></span> |
|<span data-ttu-id="a51b3-138">value</span><span class="sxs-lookup"><span data-stu-id="a51b3-138">value</span></span>|<span data-ttu-id="a51b3-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a51b3-139">String</span></span>|<span data-ttu-id="a51b3-140">Especifica o valor a ser incluído na declaração em tokens de ID e tokens de acesso autenticando um usuário atribuído ou entidade `roles` de serviço.</span><span class="sxs-lookup"><span data-stu-id="a51b3-140">Specifies the value to include in the `roles` claim in ID tokens and access tokens authenticating an assigned user or service principal.</span></span> <span data-ttu-id="a51b3-141">Não deve exceder 120 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="a51b3-141">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="a51b3-142">Os caracteres `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` permitidos são , bem como caracteres nos intervalos `0-9` e `A-Z` `a-z` .</span><span class="sxs-lookup"><span data-stu-id="a51b3-142">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="a51b3-143">Qualquer outro caractere, incluindo o caractere de espaço, não é permitido.</span><span class="sxs-lookup"><span data-stu-id="a51b3-143">Any other character, including the space character, are not allowed.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a51b3-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a51b3-144">JSON representation</span></span>

<span data-ttu-id="a51b3-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a51b3-145">The following is a JSON representation of the resource.</span></span>

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

