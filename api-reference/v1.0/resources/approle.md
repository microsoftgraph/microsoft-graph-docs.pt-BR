---
title: tipo de recurso appRole
description: Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente que esteja ligando para outro aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: e94b1bce8f7888cf2bca4f316dfa8d6a6a96c244
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451654"
---
# <a name="approle-resource-type"></a><span data-ttu-id="9a708-103">tipo de recurso appRole</span><span class="sxs-lookup"><span data-stu-id="9a708-103">appRole resource type</span></span>

<span data-ttu-id="9a708-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a708-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9a708-105">Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente que esteja chamando outro aplicativo ou que possa ser usada para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificada.</span><span class="sxs-lookup"><span data-stu-id="9a708-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="9a708-106">A propriedade **appRoles**</span><span class="sxs-lookup"><span data-stu-id="9a708-106">The **appRoles** property</span></span> <!-- of the [servicePrincipal](serviceprincipal.md) entity and --> <span data-ttu-id="9a708-107">a entidade do [aplicativo](application.md) é uma coleção de **appRole**.</span><span class="sxs-lookup"><span data-stu-id="9a708-107">of the [application](application.md) entity is a collection of **appRole**.</span></span>

## <a name="properties"></a><span data-ttu-id="9a708-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a708-108">Properties</span></span>
| <span data-ttu-id="9a708-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a708-109">Property</span></span>     | <span data-ttu-id="9a708-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a708-110">Type</span></span>   |<span data-ttu-id="9a708-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a708-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a708-112">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="9a708-112">allowedMemberTypes</span></span>|<span data-ttu-id="9a708-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a708-113">String collection</span></span>|<span data-ttu-id="9a708-114">Especifica se essa definição de função de aplicativo pode ser atribuída a usuários e grupos por meio da configuração de "usuário" ou a outros aplicativos (que estão acessando esse aplicativo em cenários de serviço de daemon) definindo como "aplicativo" ou ambos.</span><span class="sxs-lookup"><span data-stu-id="9a708-114">Specifies whether this app role definition can be assigned to users and groups by setting to "User", or to other applications (that are accessing this application in daemon service scenarios) by setting to "Application", or to both.</span></span>|
|<span data-ttu-id="9a708-115">description</span><span class="sxs-lookup"><span data-stu-id="9a708-115">description</span></span>|<span data-ttu-id="9a708-116">String</span><span class="sxs-lookup"><span data-stu-id="9a708-116">String</span></span>|<span data-ttu-id="9a708-117">Texto de ajuda de permissão que aparece nas experiências de consentimento e atribuição de aplicativo de administração.</span><span class="sxs-lookup"><span data-stu-id="9a708-117">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="9a708-118">displayName</span><span class="sxs-lookup"><span data-stu-id="9a708-118">displayName</span></span>|<span data-ttu-id="9a708-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a708-119">String</span></span>|<span data-ttu-id="9a708-120">Nome para exibição da permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.</span><span class="sxs-lookup"><span data-stu-id="9a708-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="9a708-121">id</span><span class="sxs-lookup"><span data-stu-id="9a708-121">id</span></span>|<span data-ttu-id="9a708-122">Guid</span><span class="sxs-lookup"><span data-stu-id="9a708-122">Guid</span></span>|<span data-ttu-id="9a708-123">Identificador de função exclusivo dentro da coleção **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="9a708-123">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="9a708-124">Ao criar uma nova função de aplicativo, um novo identificador GUID deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="9a708-124">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="9a708-125">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9a708-125">isEnabled</span></span>|<span data-ttu-id="9a708-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a708-126">Boolean</span></span>|<span data-ttu-id="9a708-127">Ao criar ou atualizar uma função de aplicativo, isso deve ser definido como **true** (que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="9a708-127">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="9a708-128">Para excluir uma função, é necessário primeiro defini-la como **false**.</span><span class="sxs-lookup"><span data-stu-id="9a708-128">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="9a708-129">Nesse ponto, em uma chamada subsequente, essa função pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="9a708-129">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="9a708-130">tenham</span><span class="sxs-lookup"><span data-stu-id="9a708-130">origin</span></span>|<span data-ttu-id="9a708-131">String</span><span class="sxs-lookup"><span data-stu-id="9a708-131">String</span></span>| <span data-ttu-id="9a708-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a708-132">Read-only.</span></span> <span data-ttu-id="9a708-133">Especifica se a função de aplicativo é definida no objeto Application</span><span class="sxs-lookup"><span data-stu-id="9a708-133">Specifies if the app role is defined on the Application object</span></span> <!-- or on the ServicePrincipal object --><span data-ttu-id="9a708-134">.</span><span class="sxs-lookup"><span data-stu-id="9a708-134">.</span></span> <span data-ttu-id="9a708-135">_Não_ deve ser incluído em solicitações POST ou patch.</span><span class="sxs-lookup"><span data-stu-id="9a708-135">Must _not_ be included in any POST or PATCH requests.</span></span> |
|<span data-ttu-id="9a708-136">value</span><span class="sxs-lookup"><span data-stu-id="9a708-136">value</span></span>|<span data-ttu-id="9a708-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a708-137">String</span></span>|<span data-ttu-id="9a708-138">Especifica o valor que será incluído na `roles` declaração em tokens de autenticação e de acesso.</span><span class="sxs-lookup"><span data-stu-id="9a708-138">Specifies the value which will be included in the `roles` claim in authentication and access tokens.</span></span> <span data-ttu-id="9a708-139">Não deve exceder 120 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="9a708-139">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="9a708-140">Os caracteres permitidos `:` `!` `#` `$` `%` são `&` `'` `(` `)` `0-9` `a-z`, bem como os `A-Z` caracteres nos intervalos e. `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`</span><span class="sxs-lookup"><span data-stu-id="9a708-140">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="9a708-141">Qualquer outro caractere, incluindo o caractere de espaço, não é permitido.</span><span class="sxs-lookup"><span data-stu-id="9a708-141">Any other character, including the space character, are not allowed.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="9a708-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a708-142">JSON representation</span></span>

<span data-ttu-id="9a708-143">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9a708-143">Here is a JSON representation of the resource</span></span>

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
