---
title: tipo de recurso permissionScope
description: Representa a definição de uma permissão delegada, às vezes referida como uma permissão OAuth 2,0 ou um escopo de 2,0 OAuth. Uma vez definido, a permissão delegada pode ser solicitada por um aplicativo cliente
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 9a7c69e13fecf4e446f43fb6b2554c1cfd5bdee2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984240"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="347b8-104">tipo de recurso permissionScope</span><span class="sxs-lookup"><span data-stu-id="347b8-104">permissionScope resource type</span></span>

<span data-ttu-id="347b8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="347b8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="347b8-106">Representa a definição de uma [permissão delegada](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="347b8-106">Represents the definition of a [delegated permission](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span>

<span data-ttu-id="347b8-107">As permissões delegadas podem ser solicitadas por aplicativos cliente que precisam de um token de acesso para a API que definiu as permissões.</span><span class="sxs-lookup"><span data-stu-id="347b8-107">Delegated permissions can be requested by client applications needing an access token to the API which defined the permissions.</span></span> <span data-ttu-id="347b8-108">As permissões delegadas podem ser solicitadas [dinamicamente](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent), usando o `scopes` parâmetro em uma solicitação de autorização para a plataforma de identidade da Microsoft, ou [estaticamente](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope), através da coleção **requiredResourceAccess** no objeto [Application](application.md) .</span><span class="sxs-lookup"><span data-stu-id="347b8-108">Delegated permissions can be requested [dynamically](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent), using the `scopes` parameter in an authorization request to the Microsoft identity platform, or [statically](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope), through the **requiredResourceAccess** collection on the [application](application.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="347b8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="347b8-109">Properties</span></span>

| <span data-ttu-id="347b8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="347b8-110">Property</span></span> | <span data-ttu-id="347b8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="347b8-111">Type</span></span> | <span data-ttu-id="347b8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="347b8-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="347b8-113">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="347b8-113">adminConsentDescription</span></span>|<span data-ttu-id="347b8-114">String</span><span class="sxs-lookup"><span data-stu-id="347b8-114">String</span></span>|<span data-ttu-id="347b8-115">Uma descrição das permissões delegadas, que devem ser lidas por um administrador que concede a permissão em nome de todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="347b8-115">A description of the delegated permissions, intended to be read by an administrator granting the permission on behalf of all users.</span></span> <span data-ttu-id="347b8-116">Esse texto aparece em experiências de consentimento de administrador em todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="347b8-116">This text appears in tenant-wide admin consent experiences.</span></span>|
|<span data-ttu-id="347b8-117">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="347b8-117">adminConsentDisplayName</span></span>|<span data-ttu-id="347b8-118">String</span><span class="sxs-lookup"><span data-stu-id="347b8-118">String</span></span>|<span data-ttu-id="347b8-119">O título da permissão, destinado a ser lido por um administrador que concede a permissão em nome de todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="347b8-119">The permission's title, intended to be read by an administrator granting the permission on behalf of all users.</span></span>|
|<span data-ttu-id="347b8-120">id</span><span class="sxs-lookup"><span data-stu-id="347b8-120">id</span></span>|<span data-ttu-id="347b8-121">Guid</span><span class="sxs-lookup"><span data-stu-id="347b8-121">Guid</span></span>|<span data-ttu-id="347b8-122">Identificador de permissão delegada exclusiva dentro da coleção de permissões delegadas definido para um aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="347b8-122">Unique delegated permission identifier inside the collection of delegated permissions defined for a resource application.</span></span>|
|<span data-ttu-id="347b8-123">isEnabled</span><span class="sxs-lookup"><span data-stu-id="347b8-123">isEnabled</span></span>|<span data-ttu-id="347b8-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="347b8-124">Boolean</span></span>|<span data-ttu-id="347b8-125">Ao criar ou atualizar uma permissão, essa propriedade deve ser definida como **true** (que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="347b8-125">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="347b8-126">Para excluir uma permissão, essa propriedade deve ser definida primeiro como **false**.</span><span class="sxs-lookup"><span data-stu-id="347b8-126">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="347b8-127">Nesse ponto, em uma chamada subsequente, a permissão pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="347b8-127">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="347b8-128">tipo</span><span class="sxs-lookup"><span data-stu-id="347b8-128">type</span></span>|<span data-ttu-id="347b8-129">String</span><span class="sxs-lookup"><span data-stu-id="347b8-129">String</span></span>|<span data-ttu-id="347b8-130">Especifica se essa permissão delegada deve ser considerada segura para que usuários que não são administradores consentissem em nome de si mesmas ou se um administrador deve ser necessário para o consentimento das permissões.</span><span class="sxs-lookup"><span data-stu-id="347b8-130">Specifies whether this delegated permission should be considered safe for non-admin users to consent to on behalf of themselves, or whether an administrator should be required for consent to the permissions.</span></span> <span data-ttu-id="347b8-131">Esse será o comportamento padrão, mas cada cliente poderá optar por personalizar o comportamento em sua organização (permitindo, restringindo ou limitando o consentimento do usuário a essa permissão delegada).</span><span class="sxs-lookup"><span data-stu-id="347b8-131">This will be the default behavior, but each customer can choose to customize the behavior in their organization (by allowing, restricting or limiting user consent to this delegated permission.)</span></span>|
|<span data-ttu-id="347b8-132">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="347b8-132">userConsentDescription</span></span>|<span data-ttu-id="347b8-133">String</span><span class="sxs-lookup"><span data-stu-id="347b8-133">String</span></span>|<span data-ttu-id="347b8-134">Uma descrição das permissões delegadas, que devem ser lidas por um usuário que concede a permissão em seu próprio nome.</span><span class="sxs-lookup"><span data-stu-id="347b8-134">A description of the delegated permissions, intended to be read by a user granting the permission on their own behalf.</span></span> <span data-ttu-id="347b8-135">Esse texto aparece em experiências de consentimento onde o usuário está concordando somente em nome de si mesmo.</span><span class="sxs-lookup"><span data-stu-id="347b8-135">This text appears in consent experiences where the user is consenting only on behalf of themselves.</span></span>|
|<span data-ttu-id="347b8-136">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="347b8-136">userConsentDisplayName</span></span>|<span data-ttu-id="347b8-137">String</span><span class="sxs-lookup"><span data-stu-id="347b8-137">String</span></span>|<span data-ttu-id="347b8-138">Um título para a permissão, que deve ser lido por um usuário que conceda a permissão em seu próprio nome.</span><span class="sxs-lookup"><span data-stu-id="347b8-138">A title for the permission, intended to be read by a user granting the permission on their own behalf.</span></span> <span data-ttu-id="347b8-139">Esse texto aparece em experiências de consentimento onde o usuário está concordando somente em nome de si mesmo.</span><span class="sxs-lookup"><span data-stu-id="347b8-139">This text appears in consent experiences where the user is consenting only on behalf of themselves.</span></span>|
|<span data-ttu-id="347b8-140">value</span><span class="sxs-lookup"><span data-stu-id="347b8-140">value</span></span>|<span data-ttu-id="347b8-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="347b8-141">String</span></span>|<span data-ttu-id="347b8-142">Especifica o valor a ser incluído na `scp` declaração (escopo) em tokens de acesso.</span><span class="sxs-lookup"><span data-stu-id="347b8-142">Specifies the value to include in the `scp` (scope) claim in access tokens.</span></span> <span data-ttu-id="347b8-143">Não deve exceder 120 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="347b8-143">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="347b8-144">Os caracteres permitidos são `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` , bem como os caracteres nos intervalos `0-9` `A-Z` e `a-z` .</span><span class="sxs-lookup"><span data-stu-id="347b8-144">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="347b8-145">Qualquer outro caractere, incluindo o caractere de espaço, não é permitido.</span><span class="sxs-lookup"><span data-stu-id="347b8-145">Any other character, including the space character, are not allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="347b8-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="347b8-146">JSON representation</span></span>

<span data-ttu-id="347b8-147">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="347b8-147">Here is a JSON representation of the resource</span></span>

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

