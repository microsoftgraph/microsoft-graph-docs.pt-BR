---
title: tipo de recurso appRole
description: Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente que esteja chamando outro aplicativo ou que possa ser usada para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificada. A propriedade **appRoles** da entidade servicePrincipalName e da entidade Application é uma coleção de **appRole**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 35c26e52c5d7eb9529474d08a43b68fceddfc954
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013315"
---
# <a name="approle-resource-type"></a><span data-ttu-id="644a1-104">tipo de recurso appRole</span><span class="sxs-lookup"><span data-stu-id="644a1-104">appRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="644a1-105">Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente que esteja chamando outro aplicativo ou que possa ser usada para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificada.</span><span class="sxs-lookup"><span data-stu-id="644a1-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="644a1-106">A propriedade **appRoles** da entidade [servicePrincipalName](serviceprincipal.md) e da entidade [Application](application.md) é uma coleção de **appRole**.</span><span class="sxs-lookup"><span data-stu-id="644a1-106">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="644a1-107">Importante: essa funcionalidade está desabilitada na versão atual.</span><span class="sxs-lookup"><span data-stu-id="644a1-107">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="644a1-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="644a1-108">JSON representation</span></span>

<span data-ttu-id="644a1-109">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="644a1-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="644a1-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="644a1-110">Properties</span></span>
| <span data-ttu-id="644a1-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="644a1-111">Property</span></span>     | <span data-ttu-id="644a1-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="644a1-112">Type</span></span>   |<span data-ttu-id="644a1-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="644a1-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="644a1-114">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="644a1-114">allowedMemberTypes</span></span>|<span data-ttu-id="644a1-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="644a1-115">String collection</span></span>|<span data-ttu-id="644a1-116">Especifica se essa definição de função de aplicativo pode ser atribuída a usuários e grupos por meio da configuração de "usuário" ou a outros aplicativos (que estão acessando esse aplicativo em cenários de serviço de daemon) definindo como "aplicativo" ou ambos.</span><span class="sxs-lookup"><span data-stu-id="644a1-116">Specifies whether this app role definition can be assigned to users and groups by setting to "User", or to other applications (that are accessing this application in daemon service scenarios) by setting to "Application", or to both.</span></span>|
|<span data-ttu-id="644a1-117">descrição</span><span class="sxs-lookup"><span data-stu-id="644a1-117">description</span></span>|<span data-ttu-id="644a1-118">String</span><span class="sxs-lookup"><span data-stu-id="644a1-118">String</span></span>|<span data-ttu-id="644a1-119">Texto de ajuda de permissão que aparece nas experiências de consentimento e atribuição de aplicativo de administração.</span><span class="sxs-lookup"><span data-stu-id="644a1-119">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="644a1-120">displayName</span><span class="sxs-lookup"><span data-stu-id="644a1-120">displayName</span></span>|<span data-ttu-id="644a1-121">String</span><span class="sxs-lookup"><span data-stu-id="644a1-121">String</span></span>|<span data-ttu-id="644a1-122">Nome para exibição da permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.</span><span class="sxs-lookup"><span data-stu-id="644a1-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="644a1-123">id</span><span class="sxs-lookup"><span data-stu-id="644a1-123">id</span></span>|<span data-ttu-id="644a1-124">Guid</span><span class="sxs-lookup"><span data-stu-id="644a1-124">Guid</span></span>|<span data-ttu-id="644a1-125">Identificador de função exclusivo dentro da coleção **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="644a1-125">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="644a1-126">Ao criar uma nova função de aplicativo, um novo identificador GUID deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="644a1-126">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="644a1-127">isEnabled</span><span class="sxs-lookup"><span data-stu-id="644a1-127">isEnabled</span></span>|<span data-ttu-id="644a1-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="644a1-128">Boolean</span></span>|<span data-ttu-id="644a1-129">Ao criar ou atualizar uma função de aplicativo, isso deve ser definido como **true** (que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="644a1-129">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="644a1-130">Para excluir uma função, é necessário primeiro defini-la como **false**.</span><span class="sxs-lookup"><span data-stu-id="644a1-130">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="644a1-131">Nesse ponto, em uma chamada subsequente, essa função pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="644a1-131">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="644a1-132">tenham</span><span class="sxs-lookup"><span data-stu-id="644a1-132">origin</span></span>|<span data-ttu-id="644a1-133">String</span><span class="sxs-lookup"><span data-stu-id="644a1-133">String</span></span>| <span data-ttu-id="644a1-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="644a1-134">Read-only.</span></span> <span data-ttu-id="644a1-135">Especifica se a função de aplicativo é definida no objeto Application ou no objeto servicePrincipalName.</span><span class="sxs-lookup"><span data-stu-id="644a1-135">Specifies if the app role is defined on the Application object or on the ServicePrincipal object.</span></span> <span data-ttu-id="644a1-136">_Não_ deve ser incluído em solicitações POST ou patch.</span><span class="sxs-lookup"><span data-stu-id="644a1-136">Must _not_ be included in any POST or PATCH requests.</span></span> |
|<span data-ttu-id="644a1-137">value</span><span class="sxs-lookup"><span data-stu-id="644a1-137">value</span></span>|<span data-ttu-id="644a1-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="644a1-138">String</span></span>|<span data-ttu-id="644a1-139">Especifica o valor que será incluído na `roles` declaração em tokens de autenticação e de acesso.</span><span class="sxs-lookup"><span data-stu-id="644a1-139">Specifies the value which will be included in the `roles` claim in authentication and access tokens.</span></span> <span data-ttu-id="644a1-140">Não deve exceder 120 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="644a1-140">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="644a1-141">Caracteres `:` `!` `#` `$` permitidos são `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `A-Z` como os caracteres nos intervalos `a-z`e. `0-9` `^` `@` `[` `]` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`</span><span class="sxs-lookup"><span data-stu-id="644a1-141">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="644a1-142">Qualquer outro caractere, incluindo o caractere de espaço, não é permitido.</span><span class="sxs-lookup"><span data-stu-id="644a1-142">Any other character, including the space character, are not allowed.</span></span>  |


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
