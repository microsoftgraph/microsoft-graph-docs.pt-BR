---
title: tipo de recurso appRole
description: Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente que esteja chamando outro aplicativo ou que possa ser usada para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificada. A propriedade **appRoles** da entidade servicePrincipalName e da entidade Application é uma coleção de **appRole**.
localization_priority: Normal
ms.openlocfilehash: 0ff9c2195b8a1abe52ff505c1a01c86244e332c7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328491"
---
# <a name="approle-resource-type"></a><span data-ttu-id="9f3d6-104">tipo de recurso appRole</span><span class="sxs-lookup"><span data-stu-id="9f3d6-104">appRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f3d6-105">Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente que esteja chamando outro aplicativo ou que possa ser usada para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificada.</span><span class="sxs-lookup"><span data-stu-id="9f3d6-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="9f3d6-106">A propriedade **appRoles** da entidade [servicePrincipalName](serviceprincipal.md) e da entidade [Application](application.md) é uma coleção de **appRole**.</span><span class="sxs-lookup"><span data-stu-id="9f3d6-106">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="9f3d6-107">Importante: essa funcionalidade está desabilitada na versão atual.</span><span class="sxs-lookup"><span data-stu-id="9f3d6-107">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f3d6-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f3d6-108">JSON representation</span></span>

<span data-ttu-id="9f3d6-109">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9f3d6-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="9f3d6-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f3d6-110">Properties</span></span>
| <span data-ttu-id="9f3d6-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f3d6-111">Property</span></span>     | <span data-ttu-id="9f3d6-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f3d6-112">Type</span></span>   |<span data-ttu-id="9f3d6-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f3d6-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f3d6-114">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="9f3d6-114">allowedMemberTypes</span></span>|<span data-ttu-id="9f3d6-115">Coleção String</span><span class="sxs-lookup"><span data-stu-id="9f3d6-115">String collection</span></span>|<span data-ttu-id="9f3d6-116">Especifica se essa definição de função de aplicativo pode ser atribuída a usuários e grupos por meio da configuração de "usuário" ou a outros aplicativos (que estão acessando esse aplicativo em cenários de serviço de daemon) definindo como "aplicativo" ou ambos.</span><span class="sxs-lookup"><span data-stu-id="9f3d6-116">Specifies whether this app role definition can be assigned to users and groups by setting to “User”, or to other applications (that are accessing this application in daemon service scenarios) by setting to “Application”, or to both.</span></span>|
|<span data-ttu-id="9f3d6-117">description</span><span class="sxs-lookup"><span data-stu-id="9f3d6-117">description</span></span>|<span data-ttu-id="9f3d6-118">String</span><span class="sxs-lookup"><span data-stu-id="9f3d6-118">String</span></span>|<span data-ttu-id="9f3d6-119">Texto de ajuda de permissão que aparece nas experiências de consentimento e atribuição de aplicativo de administração.</span><span class="sxs-lookup"><span data-stu-id="9f3d6-119">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="9f3d6-120">displayName</span><span class="sxs-lookup"><span data-stu-id="9f3d6-120">displayName</span></span>|<span data-ttu-id="9f3d6-121">String</span><span class="sxs-lookup"><span data-stu-id="9f3d6-121">String</span></span>|<span data-ttu-id="9f3d6-122">Nome para exibição da permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.</span><span class="sxs-lookup"><span data-stu-id="9f3d6-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="9f3d6-123">id</span><span class="sxs-lookup"><span data-stu-id="9f3d6-123">id</span></span>|<span data-ttu-id="9f3d6-124">Guid</span><span class="sxs-lookup"><span data-stu-id="9f3d6-124">Guid</span></span>|<span data-ttu-id="9f3d6-125">Identificador de função exclusivo dentro da coleção **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="9f3d6-125">Unique role identifier inside the **appRoles** collection.</span></span>|
|<span data-ttu-id="9f3d6-126">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9f3d6-126">isEnabled</span></span>|<span data-ttu-id="9f3d6-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f3d6-127">Boolean</span></span>|<span data-ttu-id="9f3d6-128">Ao criar ou atualizar uma definição de função, isso deve ser definido como **true** (que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="9f3d6-128">When creating or updating a role definition, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="9f3d6-129">Para excluir uma função, é necessário primeiro defini-la como **false**.</span><span class="sxs-lookup"><span data-stu-id="9f3d6-129">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="9f3d6-130">Nesse ponto, em uma chamada subsequente, essa função pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="9f3d6-130">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="9f3d6-131">value</span><span class="sxs-lookup"><span data-stu-id="9f3d6-131">value</span></span>|<span data-ttu-id="9f3d6-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f3d6-132">String</span></span>|<span data-ttu-id="9f3d6-133">Especifica o valor da declaração de funções que o aplicativo deve esperar nos tokens de autenticação e acesso.</span><span class="sxs-lookup"><span data-stu-id="9f3d6-133">Specifies the value of the roles claim that the application should expect in the authentication and access tokens.</span></span>|

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
