---
title: tipo de recurso appRole
description: Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente que esteja ligando para outro aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: f98cb4d1c32256dccf5e2748116cdd7fc1869f68
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937389"
---
# <a name="approle-resource-type"></a><span data-ttu-id="eee41-103">tipo de recurso appRole</span><span class="sxs-lookup"><span data-stu-id="eee41-103">appRole resource type</span></span>

<span data-ttu-id="eee41-104">Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente que esteja chamando outro aplicativo ou que possa ser usada para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificada.</span><span class="sxs-lookup"><span data-stu-id="eee41-104">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="eee41-105">A propriedade **appRoles**</span><span class="sxs-lookup"><span data-stu-id="eee41-105">The **appRoles** property</span></span> <!-- of the [servicePrincipal](serviceprincipal.md) entity and --> <span data-ttu-id="eee41-106">a entidade do [aplicativo](application.md) é uma coleção de **appRole**.</span><span class="sxs-lookup"><span data-stu-id="eee41-106">of the [application](application.md) entity is a collection of **appRole**.</span></span>

## <a name="properties"></a><span data-ttu-id="eee41-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eee41-107">Properties</span></span>
| <span data-ttu-id="eee41-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eee41-108">Property</span></span>     | <span data-ttu-id="eee41-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="eee41-109">Type</span></span>   |<span data-ttu-id="eee41-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="eee41-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eee41-111">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="eee41-111">allowedMemberTypes</span></span>|<span data-ttu-id="eee41-112">String collection</span><span class="sxs-lookup"><span data-stu-id="eee41-112">String collection</span></span>|<span data-ttu-id="eee41-113">Especifica se essa definição de função de aplicativo pode ser atribuída a usuários e grupos por meio da configuração de "usuário" ou a outros aplicativos (que estão acessando esse aplicativo em cenários de serviço de daemon) definindo como "aplicativo" ou ambos.</span><span class="sxs-lookup"><span data-stu-id="eee41-113">Specifies whether this app role definition can be assigned to users and groups by setting to "User", or to other applications (that are accessing this application in daemon service scenarios) by setting to "Application", or to both.</span></span>|
|<span data-ttu-id="eee41-114">description</span><span class="sxs-lookup"><span data-stu-id="eee41-114">description</span></span>|<span data-ttu-id="eee41-115">String</span><span class="sxs-lookup"><span data-stu-id="eee41-115">String</span></span>|<span data-ttu-id="eee41-116">Texto de ajuda de permissão que aparece nas experiências de consentimento e atribuição de aplicativo de administração.</span><span class="sxs-lookup"><span data-stu-id="eee41-116">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="eee41-117">displayName</span><span class="sxs-lookup"><span data-stu-id="eee41-117">displayName</span></span>|<span data-ttu-id="eee41-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eee41-118">String</span></span>|<span data-ttu-id="eee41-119">Nome para exibição da permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.</span><span class="sxs-lookup"><span data-stu-id="eee41-119">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="eee41-120">id</span><span class="sxs-lookup"><span data-stu-id="eee41-120">id</span></span>|<span data-ttu-id="eee41-121">Guid</span><span class="sxs-lookup"><span data-stu-id="eee41-121">Guid</span></span>|<span data-ttu-id="eee41-122">Identificador de função exclusivo dentro da coleção **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="eee41-122">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="eee41-123">Ao criar uma nova função de aplicativo, um novo identificador GUID deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="eee41-123">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="eee41-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="eee41-124">isEnabled</span></span>|<span data-ttu-id="eee41-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="eee41-125">Boolean</span></span>|<span data-ttu-id="eee41-126">Ao criar ou atualizar uma função de aplicativo, isso deve ser definido como **true** (que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="eee41-126">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="eee41-127">Para excluir uma função, é necessário primeiro defini-la como **false**.</span><span class="sxs-lookup"><span data-stu-id="eee41-127">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="eee41-128">Nesse ponto, em uma chamada subsequente, essa função pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="eee41-128">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="eee41-129">tenham</span><span class="sxs-lookup"><span data-stu-id="eee41-129">origin</span></span>|<span data-ttu-id="eee41-130">String</span><span class="sxs-lookup"><span data-stu-id="eee41-130">String</span></span>| <span data-ttu-id="eee41-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eee41-131">Read-only.</span></span> <span data-ttu-id="eee41-132">Especifica se a função de aplicativo é definida no objeto Application</span><span class="sxs-lookup"><span data-stu-id="eee41-132">Specifies if the app role is defined on the Application object</span></span> <!-- or on the ServicePrincipal object --><span data-ttu-id="eee41-133">.</span><span class="sxs-lookup"><span data-stu-id="eee41-133"></span></span> <span data-ttu-id="eee41-134">_Não_ deve ser incluído em solicitações POST ou patch.</span><span class="sxs-lookup"><span data-stu-id="eee41-134">Must _not_ be included in any POST or PATCH requests.</span></span> |
|<span data-ttu-id="eee41-135">value</span><span class="sxs-lookup"><span data-stu-id="eee41-135">value</span></span>|<span data-ttu-id="eee41-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eee41-136">String</span></span>|<span data-ttu-id="eee41-137">Especifica o valor que será incluído na `roles` declaração em tokens de autenticação e de acesso.</span><span class="sxs-lookup"><span data-stu-id="eee41-137">Specifies the value which will be included in the `roles` claim in authentication and access tokens.</span></span> <span data-ttu-id="eee41-138">Não deve exceder 120 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="eee41-138">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="eee41-139">Caracteres `:` `!` `#` `$` permitidos são `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `A-Z` como os caracteres nos intervalos `a-z`e. `0-9` `^` `@` `[` `]` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`</span><span class="sxs-lookup"><span data-stu-id="eee41-139">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="eee41-140">Qualquer outro caractere, incluindo o caractere de espaço, não é permitido.</span><span class="sxs-lookup"><span data-stu-id="eee41-140">Any other character, including the space character, are not allowed.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="eee41-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eee41-141">JSON representation</span></span>

<span data-ttu-id="eee41-142">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="eee41-142">Here is a JSON representation of the resource</span></span>

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
