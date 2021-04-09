---
title: Tipo de recurso permissionScope
description: Representa a definição de uma permissão delegada, às vezes conhecida como uma permissão OAuth 2.0 ou um escopo OAuth 2.0. Depois de definida, a permissão delegada poderá ser solicitada por um aplicativo cliente
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: f98e91da1ff46ef944b2de49add36f174673fad8
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638890"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="9d139-104">Tipo de recurso permissionScope</span><span class="sxs-lookup"><span data-stu-id="9d139-104">permissionScope resource type</span></span>

<span data-ttu-id="9d139-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d139-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d139-106">Representa a definição de uma [permissão delegada](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="9d139-106">Represents the definition of a [delegated permission](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span>

<span data-ttu-id="9d139-107">As permissões delegadas podem ser solicitadas por aplicativos cliente que precisam de um token de acesso à API que definiu as permissões.</span><span class="sxs-lookup"><span data-stu-id="9d139-107">Delegated permissions can be requested by client applications needing an access token to the API which defined the permissions.</span></span> <span data-ttu-id="9d139-108">As permissões delegadas podem ser solicitadas [dinamicamente](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent), usando o parâmetro em uma solicitação de autorização para a plataforma de identidade da Microsoft ou estaticamente, por meio da coleção `scopes` **requiredResourceAccess** no objeto [application.](application.md) [](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope)</span><span class="sxs-lookup"><span data-stu-id="9d139-108">Delegated permissions can be requested [dynamically](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent), using the `scopes` parameter in an authorization request to the Microsoft identity platform, or [statically](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope), through the **requiredResourceAccess** collection on the [application](application.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="9d139-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d139-109">Properties</span></span>

| <span data-ttu-id="9d139-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d139-110">Property</span></span> | <span data-ttu-id="9d139-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d139-111">Type</span></span> | <span data-ttu-id="9d139-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d139-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9d139-113">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="9d139-113">adminConsentDescription</span></span>|<span data-ttu-id="9d139-114">String</span><span class="sxs-lookup"><span data-stu-id="9d139-114">String</span></span>|<span data-ttu-id="9d139-115">Uma descrição das permissões delegadas, destinadas a ser lidas por um administrador concedendo a permissão em nome de todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="9d139-115">A description of the delegated permissions, intended to be read by an administrator granting the permission on behalf of all users.</span></span> <span data-ttu-id="9d139-116">Este texto aparece em experiências de consentimento de administrador em todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d139-116">This text appears in tenant-wide admin consent experiences.</span></span>|
|<span data-ttu-id="9d139-117">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="9d139-117">adminConsentDisplayName</span></span>|<span data-ttu-id="9d139-118">String</span><span class="sxs-lookup"><span data-stu-id="9d139-118">String</span></span>|<span data-ttu-id="9d139-119">O título da permissão, destinado a ser lido por um administrador concedendo a permissão em nome de todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="9d139-119">The permission's title, intended to be read by an administrator granting the permission on behalf of all users.</span></span>|
|<span data-ttu-id="9d139-120">id</span><span class="sxs-lookup"><span data-stu-id="9d139-120">id</span></span>|<span data-ttu-id="9d139-121">Guid</span><span class="sxs-lookup"><span data-stu-id="9d139-121">Guid</span></span>|<span data-ttu-id="9d139-122">Identificador de permissão delegado exclusivo dentro da coleção de permissões delegadas definidas para um aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="9d139-122">Unique delegated permission identifier inside the collection of delegated permissions defined for a resource application.</span></span>|
|<span data-ttu-id="9d139-123">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9d139-123">isEnabled</span></span>|<span data-ttu-id="9d139-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="9d139-124">Boolean</span></span>|<span data-ttu-id="9d139-125">Ao criar ou atualizar uma permissão, essa propriedade deve ser definida como **true** (que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="9d139-125">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="9d139-126">Para excluir uma permissão, essa propriedade deve primeiro ser definida como **false**.</span><span class="sxs-lookup"><span data-stu-id="9d139-126">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="9d139-127">Nesse ponto, em uma chamada subsequente, a permissão pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="9d139-127">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="9d139-128">tipo</span><span class="sxs-lookup"><span data-stu-id="9d139-128">type</span></span>|<span data-ttu-id="9d139-129">String</span><span class="sxs-lookup"><span data-stu-id="9d139-129">String</span></span>|<span data-ttu-id="9d139-130">Especifica se essa permissão delegada deve ser considerada segura para usuários que não sejam administradores consentirem em nome de si mesmos ou se um administrador deve ser necessário para consentir as permissões.</span><span class="sxs-lookup"><span data-stu-id="9d139-130">Specifies whether this delegated permission should be considered safe for non-admin users to consent to on behalf of themselves, or whether an administrator should be required for consent to the permissions.</span></span> <span data-ttu-id="9d139-131">Esse será o comportamento padrão, mas cada cliente pode optar por personalizar o comportamento em sua organização (permitindo, restringindo ou limitando o consentimento do usuário para essa permissão delegada.)</span><span class="sxs-lookup"><span data-stu-id="9d139-131">This will be the default behavior, but each customer can choose to customize the behavior in their organization (by allowing, restricting or limiting user consent to this delegated permission.)</span></span>|
|<span data-ttu-id="9d139-132">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="9d139-132">userConsentDescription</span></span>|<span data-ttu-id="9d139-133">String</span><span class="sxs-lookup"><span data-stu-id="9d139-133">String</span></span>|<span data-ttu-id="9d139-134">Uma descrição das permissões delegadas, destinadas a ser lidas por um usuário concedendo a permissão em seu próprio nome.</span><span class="sxs-lookup"><span data-stu-id="9d139-134">A description of the delegated permissions, intended to be read by a user granting the permission on their own behalf.</span></span> <span data-ttu-id="9d139-135">Este texto aparece em experiências de consentimento em que o usuário está consentindo apenas em nome de si mesmo.</span><span class="sxs-lookup"><span data-stu-id="9d139-135">This text appears in consent experiences where the user is consenting only on behalf of themselves.</span></span>|
|<span data-ttu-id="9d139-136">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="9d139-136">userConsentDisplayName</span></span>|<span data-ttu-id="9d139-137">String</span><span class="sxs-lookup"><span data-stu-id="9d139-137">String</span></span>|<span data-ttu-id="9d139-138">Um título para a permissão, destinado a ser lido por um usuário concedendo a permissão em seu próprio nome.</span><span class="sxs-lookup"><span data-stu-id="9d139-138">A title for the permission, intended to be read by a user granting the permission on their own behalf.</span></span> <span data-ttu-id="9d139-139">Este texto aparece em experiências de consentimento em que o usuário está consentindo apenas em nome de si mesmo.</span><span class="sxs-lookup"><span data-stu-id="9d139-139">This text appears in consent experiences where the user is consenting only on behalf of themselves.</span></span>|
|<span data-ttu-id="9d139-140">value</span><span class="sxs-lookup"><span data-stu-id="9d139-140">value</span></span>|<span data-ttu-id="9d139-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d139-141">String</span></span>|<span data-ttu-id="9d139-142">Especifica o valor a ser incluído na declaração `scp` (escopo) em tokens de acesso.</span><span class="sxs-lookup"><span data-stu-id="9d139-142">Specifies the value to include in the `scp` (scope) claim in access tokens.</span></span> <span data-ttu-id="9d139-143">Não deve exceder 120 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="9d139-143">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="9d139-144">Os caracteres `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` permitidos são , bem como caracteres nos intervalos `0-9` `A-Z` e `a-z` .</span><span class="sxs-lookup"><span data-stu-id="9d139-144">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="9d139-145">Qualquer outro caractere, incluindo o caractere de espaço, não é permitido.</span><span class="sxs-lookup"><span data-stu-id="9d139-145">Any other character, including the space character, are not allowed.</span></span> <span data-ttu-id="9d139-146">Pode não começar com `.` .</span><span class="sxs-lookup"><span data-stu-id="9d139-146">May not begin with `.`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d139-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d139-147">JSON representation</span></span>

<span data-ttu-id="9d139-148">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9d139-148">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "id": "guid",
  "adminConsentDisplayName": "string",
  "adminConsentDescription": "string",
  "userConsentDisplayName": "string",
  "userConsentDescription": "string",
  "value": "string",
  "type": "string",
  "isEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
