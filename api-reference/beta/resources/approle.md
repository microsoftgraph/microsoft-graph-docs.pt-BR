---
title: tipo de recurso appRole
description: Representa uma função de aplicativo que podem ser solicitados por um aplicativo cliente chamar outro aplicativo ou que podem ser usadas para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificado. A propriedade **appRoles** da entidade servicePrincipal e da entidade do aplicativo é uma coleção de **appRole**.
ms.openlocfilehash: f87ef6f40fbeb18ec4b3a2373fb2a19e14da84a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034587"
---
# <a name="approle-resource-type"></a><span data-ttu-id="bb406-104">tipo de recurso appRole</span><span class="sxs-lookup"><span data-stu-id="bb406-104">appRole resource type</span></span>

> <span data-ttu-id="bb406-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bb406-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb406-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bb406-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb406-107">Representa uma função de aplicativo que podem ser solicitados por um aplicativo cliente chamar outro aplicativo ou que podem ser usadas para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificado.</span><span class="sxs-lookup"><span data-stu-id="bb406-107">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="bb406-108">A propriedade **appRoles** da entidade [servicePrincipal](serviceprincipal.md) e da entidade do [aplicativo](application.md) é uma coleção de **appRole**.</span><span class="sxs-lookup"><span data-stu-id="bb406-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="bb406-109">Importante: Essa funcionalidade está desabilitada na versão atual.</span><span class="sxs-lookup"><span data-stu-id="bb406-109">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb406-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb406-110">JSON representation</span></span>

<span data-ttu-id="bb406-111">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bb406-111">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approle"
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
## <a name="properties"></a><span data-ttu-id="bb406-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb406-112">Properties</span></span>
| <span data-ttu-id="bb406-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb406-113">Property</span></span>     | <span data-ttu-id="bb406-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb406-114">Type</span></span>   |<span data-ttu-id="bb406-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb406-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb406-116">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="bb406-116">allowedMemberTypes</span></span>|<span data-ttu-id="bb406-117">String collection</span><span class="sxs-lookup"><span data-stu-id="bb406-117">String collection</span></span>|<span data-ttu-id="bb406-118">Especifica se esta definição de aplicativo de função pode ser atribuída aos usuários e grupos pela configuração para "User", ou para outros aplicativos (que estão acessando este aplicativo em cenários de serviço daemon) por configuração para "Aplicativo", ou ambos.</span><span class="sxs-lookup"><span data-stu-id="bb406-118">Specifies whether this app role definition can be assigned to users and groups by setting to “User”, or to other applications (that are accessing this application in daemon service scenarios) by setting to “Application”, or to both.</span></span>|
|<span data-ttu-id="bb406-119">description</span><span class="sxs-lookup"><span data-stu-id="bb406-119">description</span></span>|<span data-ttu-id="bb406-120">String</span><span class="sxs-lookup"><span data-stu-id="bb406-120">String</span></span>|<span data-ttu-id="bb406-121">Permissão ajudam o texto que aparece na atribuição app admin e experiências de consentimento.</span><span class="sxs-lookup"><span data-stu-id="bb406-121">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="bb406-122">displayName</span><span class="sxs-lookup"><span data-stu-id="bb406-122">displayName</span></span>|<span data-ttu-id="bb406-123">String</span><span class="sxs-lookup"><span data-stu-id="bb406-123">String</span></span>|<span data-ttu-id="bb406-124">Nome para exibição da permissão que aparece nas experiências de atribuição de consentimento e app admin.</span><span class="sxs-lookup"><span data-stu-id="bb406-124">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="bb406-125">id</span><span class="sxs-lookup"><span data-stu-id="bb406-125">id</span></span>|<span data-ttu-id="bb406-126">Guid</span><span class="sxs-lookup"><span data-stu-id="bb406-126">Guid</span></span>|<span data-ttu-id="bb406-127">Identificador exclusivo de função dentro da coleção **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="bb406-127">Unique role identifier inside the **appRoles** collection.</span></span>|
|<span data-ttu-id="bb406-128">isEnabled</span><span class="sxs-lookup"><span data-stu-id="bb406-128">isEnabled</span></span>|<span data-ttu-id="bb406-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb406-129">Boolean</span></span>|<span data-ttu-id="bb406-130">Ao criar ou atualizar uma definição de função, isso deve ser definido como **true** (o que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="bb406-130">When creating or updating a role definition, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="bb406-131">Para excluir uma função, isso deve primeiro ser definido como **false**.</span><span class="sxs-lookup"><span data-stu-id="bb406-131">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="bb406-132">Nesse momento, em uma chamada subsequente, essa função pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="bb406-132">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="bb406-133">valor</span><span class="sxs-lookup"><span data-stu-id="bb406-133">value</span></span>|<span data-ttu-id="bb406-134">String</span><span class="sxs-lookup"><span data-stu-id="bb406-134">String</span></span>|<span data-ttu-id="bb406-135">Especifica o valor da declaração funções que o aplicativo deve esperar em tokens de acesso e autenticação.</span><span class="sxs-lookup"><span data-stu-id="bb406-135">Specifies the value of the roles claim that the application should expect in the authentication and access tokens.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->