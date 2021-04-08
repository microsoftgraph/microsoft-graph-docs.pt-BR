---
title: Tipo de recurso appRole
description: Representa uma função de aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 06a5f97048be74388b49a79c8661b49043ddf727
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638834"
---
# <a name="approle-resource-type"></a><span data-ttu-id="1a118-103">Tipo de recurso appRole</span><span class="sxs-lookup"><span data-stu-id="1a118-103">appRole resource type</span></span>

<span data-ttu-id="1a118-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a118-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a118-105">Representa uma função de aplicativo que pode ser solicitada por (e concedida a) um aplicativo cliente ou que pode ser usada para atribuir um aplicativo a usuários ou grupos em uma função especificada.</span><span class="sxs-lookup"><span data-stu-id="1a118-105">Represents an application role that can be requested by (and granted to) a client application, or that can be used to assign an application to users or groups in a specified role.</span></span> 

<span data-ttu-id="1a118-106">Para adicionar, atualizar ou remover funções de aplicativo para um aplicativo, [atualize o aplicativo](../api/application-update.md) para o aplicativo ou serviço.</span><span class="sxs-lookup"><span data-stu-id="1a118-106">To add, update, or remove app roles for an application, [update the application](../api/application-update.md) for the app or service.</span></span> <span data-ttu-id="1a118-107">As funções do aplicativo na entidade de aplicativo estarão disponíveis em todos os locatários onde o aplicativo é usado.</span><span class="sxs-lookup"><span data-stu-id="1a118-107">App roles on the application entity will be available in all tenants where the application is used.</span></span> <span data-ttu-id="1a118-108">Para definir funções de aplicativo que só são aplicáveis em seu locatário (por exemplo, funções [](../api/serviceprincipal-update.md) de aplicativo que representam funções personalizadas em sua instância de um aplicativo de vários locatários), você também pode atualizar a entidade de serviço do aplicativo, para adicionar ou atualizar funções de aplicativo à coleção **appRoles.**</span><span class="sxs-lookup"><span data-stu-id="1a118-108">To define app roles that are only applicable in your tenant (for example, app roles representing custom roles in your instance of a multi-tenant application), you can also [update the service principal](../api/serviceprincipal-update.md) for the app, to add or update app roles to the **appRoles** collection.</span></span>

<span data-ttu-id="1a118-109">Com [appRoleAssignments,](approleassignment.md)as funções do aplicativo podem ser atribuídas a usuários, grupos ou entidades de serviço de outros aplicativos.</span><span class="sxs-lookup"><span data-stu-id="1a118-109">With [appRoleAssignments](approleassignment.md), app roles can be assigned to users, groups, or other applications' service principals.</span></span>

## <a name="properties"></a><span data-ttu-id="1a118-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a118-110">Properties</span></span>

| <span data-ttu-id="1a118-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a118-111">Property</span></span>   | <span data-ttu-id="1a118-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a118-112">Type</span></span> |<span data-ttu-id="1a118-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a118-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a118-114">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="1a118-114">allowedMemberTypes</span></span>|<span data-ttu-id="1a118-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a118-115">String collection</span></span>|<span data-ttu-id="1a118-116">Especifica se essa função de aplicativo pode ser atribuída a usuários e grupos (definindo como ), para outro aplicativo (definindo como , ou `["User"]` `["Application"]` ambos (definindo como `["User", "Application"]` ).</span><span class="sxs-lookup"><span data-stu-id="1a118-116">Specifies whether this app role can be assigned to users and groups (by setting to `["User"]`), to other application's (by setting to `["Application"]`, or both (by setting to `["User", "Application"]`).</span></span> <span data-ttu-id="1a118-117">Funções de aplicativo que suportam a atribuição a entidades de serviço de outros aplicativos também são conhecidas como [permissões de aplicativo.](/graph/auth/auth-concepts#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="1a118-117">App roles supporting assignment to other applications' service principals are also known as [application permissions](/graph/auth/auth-concepts#microsoft-graph-permissions).</span></span> <span data-ttu-id="1a118-118">O valor "Application" só é suportado para funções de aplicativo definidas em **entidades de** aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1a118-118">The "Application" value is only supported for app roles defined on **application** entities.</span></span> |
|<span data-ttu-id="1a118-119">description</span><span class="sxs-lookup"><span data-stu-id="1a118-119">description</span></span>|<span data-ttu-id="1a118-120">String</span><span class="sxs-lookup"><span data-stu-id="1a118-120">String</span></span>|<span data-ttu-id="1a118-121">A descrição da função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1a118-121">The description for the app role.</span></span> <span data-ttu-id="1a118-122">Isso é exibido quando a função do aplicativo está sendo atribuída e, se a função do aplicativo funcionar como uma permissão de aplicativo, durante experiências de consentimento.</span><span class="sxs-lookup"><span data-stu-id="1a118-122">This is displayed when the app role is being assigned and, if the app role functions as an application permission, during  consent experiences.</span></span>|
|<span data-ttu-id="1a118-123">displayName</span><span class="sxs-lookup"><span data-stu-id="1a118-123">displayName</span></span>|<span data-ttu-id="1a118-124">String</span><span class="sxs-lookup"><span data-stu-id="1a118-124">String</span></span>|<span data-ttu-id="1a118-125">Nome de exibição para a permissão que aparece na atribuição de função de aplicativo e experiências de consentimento.</span><span class="sxs-lookup"><span data-stu-id="1a118-125">Display name for the permission that appears in the app role assignment and consent experiences.</span></span>|
|<span data-ttu-id="1a118-126">id</span><span class="sxs-lookup"><span data-stu-id="1a118-126">id</span></span>|<span data-ttu-id="1a118-127">Guid</span><span class="sxs-lookup"><span data-stu-id="1a118-127">Guid</span></span>|<span data-ttu-id="1a118-128">Identificador de função exclusivo dentro da **coleção appRoles.**</span><span class="sxs-lookup"><span data-stu-id="1a118-128">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="1a118-129">Ao criar uma nova função de aplicativo, um novo identificador guid deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="1a118-129">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="1a118-130">isEnabled</span><span class="sxs-lookup"><span data-stu-id="1a118-130">isEnabled</span></span>|<span data-ttu-id="1a118-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a118-131">Boolean</span></span>|<span data-ttu-id="1a118-132">Ao criar ou atualizar uma função de aplicativo, isso deve ser definido como **true** (que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="1a118-132">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="1a118-133">Para excluir uma função, isso deve ser definido primeiro como **false**.</span><span class="sxs-lookup"><span data-stu-id="1a118-133">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="1a118-134">Nesse ponto, em uma chamada subsequente, essa função pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="1a118-134">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="1a118-135">origin</span><span class="sxs-lookup"><span data-stu-id="1a118-135">origin</span></span>|<span data-ttu-id="1a118-136">String</span><span class="sxs-lookup"><span data-stu-id="1a118-136">String</span></span>| <span data-ttu-id="1a118-137">Especifica se a função de aplicativo é definida no objeto [application](application.md) ou na [entidade servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="1a118-137">Specifies if the app role is defined on the [application](application.md) object or on the [servicePrincipal](serviceprincipal.md) entity.</span></span> <span data-ttu-id="1a118-138">Não _deve_ ser incluído em nenhuma solicitação POST ou PATCH.</span><span class="sxs-lookup"><span data-stu-id="1a118-138">Must _not_ be included in any POST or PATCH requests.</span></span> <span data-ttu-id="1a118-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a118-139">Read-only.</span></span> |
|<span data-ttu-id="1a118-140">value</span><span class="sxs-lookup"><span data-stu-id="1a118-140">value</span></span>|<span data-ttu-id="1a118-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a118-141">String</span></span>|<span data-ttu-id="1a118-142">Especifica o valor a ser incluído na declaração em tokens de ID e tokens de acesso autenticando um usuário ou entidade `roles` de serviço atribuído.</span><span class="sxs-lookup"><span data-stu-id="1a118-142">Specifies the value to include in the `roles` claim in ID tokens and access tokens authenticating an assigned user or service principal.</span></span> <span data-ttu-id="1a118-143">Não deve exceder 120 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="1a118-143">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="1a118-144">Os caracteres `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` permitidos são , bem como caracteres nos intervalos `0-9` `A-Z` e `a-z` .</span><span class="sxs-lookup"><span data-stu-id="1a118-144">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="1a118-145">Qualquer outro caractere, incluindo o caractere de espaço, não é permitido.</span><span class="sxs-lookup"><span data-stu-id="1a118-145">Any other character, including the space character, are not allowed.</span></span> <span data-ttu-id="1a118-146">Pode não começar com `.` .</span><span class="sxs-lookup"><span data-stu-id="1a118-146">May not begin with `.`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1a118-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a118-147">JSON representation</span></span>

<span data-ttu-id="1a118-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a118-148">The following is a JSON representation of the resource.</span></span>

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


