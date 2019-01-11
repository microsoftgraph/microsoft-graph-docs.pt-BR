---
title: tipo de recurso directoryRole
description: Representa uma função de diretório do Windows Azure AD. Funções de diretório do Windows Azure AD também são conhecidos como *funções de administrador*. Para obter mais informações sobre as funções de diretório (administrador), consulte a atribuição de funções de administrador no Azure AD. Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder as permissões da função de destino. Para ler uma função de diretório ou atualizar seus membros, ele deve primeiro ser ativado no inquilino. Por padrão, apenas a função do diretório de administradores de empresa é ativada. Para ativar a outras funções de diretório disponíveis que você enviar uma solicitação POST com a ID do directoryRoleTemplate na qual a função de diretório se baseia. Herda de directoryObject.
localization_priority: Priority
ms.openlocfilehash: 05d897d6426b2feab7c08adaa125788590675f66
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820864"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="264d6-110">tipo de recurso directoryRole</span><span class="sxs-lookup"><span data-stu-id="264d6-110">directoryRole resource type</span></span>

<span data-ttu-id="264d6-111">Representa uma função de diretório do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="264d6-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="264d6-112">Funções de diretório do Windows Azure AD também são conhecidos como *funções de administrador*.</span><span class="sxs-lookup"><span data-stu-id="264d6-112">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="264d6-113">Para obter mais informações sobre as funções de diretório (administrador), consulte [Atribuindo funções de administrador no Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="264d6-113">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="264d6-114">Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder as permissões da função de destino.</span><span class="sxs-lookup"><span data-stu-id="264d6-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="264d6-115">Para ler uma função de diretório ou atualizar seus membros, ele deve primeiro ser ativado no inquilino.</span><span class="sxs-lookup"><span data-stu-id="264d6-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="264d6-116">Por padrão, apenas a função do diretório de administradores de empresa é ativada.</span><span class="sxs-lookup"><span data-stu-id="264d6-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="264d6-117">Para ativar a outras funções de diretório disponíveis que você enviar uma solicitação POST com a ID de [directoryRoleTemplate](directoryroletemplate.md) na qual a função de diretório se baseia.</span><span class="sxs-lookup"><span data-stu-id="264d6-117">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="264d6-118">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="264d6-118">Inherits from [directoryObject](directoryobject.md).</span></span>
<span data-ttu-id="264d6-119">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="264d6-119">This resource supports:</span></span>

- <span data-ttu-id="264d6-120">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryrole-delta.md).</span><span class="sxs-lookup"><span data-stu-id="264d6-120">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="264d6-121">Métodos</span><span class="sxs-lookup"><span data-stu-id="264d6-121">Methods</span></span>

| <span data-ttu-id="264d6-122">Método</span><span class="sxs-lookup"><span data-stu-id="264d6-122">Method</span></span>       | <span data-ttu-id="264d6-123">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="264d6-123">Return Type</span></span>  |<span data-ttu-id="264d6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="264d6-124">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="264d6-125">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="264d6-125">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="264d6-126">directoryRole</span><span class="sxs-lookup"><span data-stu-id="264d6-126">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="264d6-127">Leia as propriedades e os relacionamentos do objeto directoryRole.</span><span class="sxs-lookup"><span data-stu-id="264d6-127">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="264d6-128">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="264d6-128">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="264d6-129">Coleção [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="264d6-129">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="264d6-130">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="264d6-130">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="264d6-131">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="264d6-131">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="264d6-132">directoryObject</span><span class="sxs-lookup"><span data-stu-id="264d6-132">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="264d6-133">Adicione um usuário à função de diretório postando na propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="264d6-133">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="264d6-134">Listar membros</span><span class="sxs-lookup"><span data-stu-id="264d6-134">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="264d6-135">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="264d6-135">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="264d6-136">Obtenha os usuários que são membros da função directory da propriedade de navegação members.</span><span class="sxs-lookup"><span data-stu-id="264d6-136">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="264d6-137">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="264d6-137">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="264d6-138">directoryObject</span><span class="sxs-lookup"><span data-stu-id="264d6-138">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="264d6-139">Remova um usuário da função de diretório.</span><span class="sxs-lookup"><span data-stu-id="264d6-139">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="264d6-140">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="264d6-140">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="264d6-141">directoryRole</span><span class="sxs-lookup"><span data-stu-id="264d6-141">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="264d6-142">Ative uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="264d6-142">Activate a directory role.</span></span>|
|[<span data-ttu-id="264d6-143">delta</span><span class="sxs-lookup"><span data-stu-id="264d6-143">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="264d6-144">Coleção directoryRole</span><span class="sxs-lookup"><span data-stu-id="264d6-144">directoryRole collection</span></span>| <span data-ttu-id="264d6-145">Obtenha as alterações incrementais para funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="264d6-145">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="264d6-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="264d6-146">Properties</span></span>
| <span data-ttu-id="264d6-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="264d6-147">Property</span></span>   | <span data-ttu-id="264d6-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="264d6-148">Type</span></span> | <span data-ttu-id="264d6-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="264d6-149">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="264d6-150">description</span><span class="sxs-lookup"><span data-stu-id="264d6-150">description</span></span>|<span data-ttu-id="264d6-151">String</span><span class="sxs-lookup"><span data-stu-id="264d6-151">String</span></span>|<span data-ttu-id="264d6-p103">A descrição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="264d6-p103">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="264d6-154">displayName</span><span class="sxs-lookup"><span data-stu-id="264d6-154">displayName</span></span>|<span data-ttu-id="264d6-155">String</span><span class="sxs-lookup"><span data-stu-id="264d6-155">String</span></span>|<span data-ttu-id="264d6-p104">O nome de exibição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="264d6-p104">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="264d6-158">id</span><span class="sxs-lookup"><span data-stu-id="264d6-158">id</span></span>|<span data-ttu-id="264d6-159">String</span><span class="sxs-lookup"><span data-stu-id="264d6-159">String</span></span>|<span data-ttu-id="264d6-p105">O identificador exclusivo da função de diretório. Herdado de [directoryObject](directoryobject.md). Chave, Não Anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="264d6-p105">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="264d6-163">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="264d6-163">roleTemplateId</span></span>|<span data-ttu-id="264d6-164">String</span><span class="sxs-lookup"><span data-stu-id="264d6-164">String</span></span>| <span data-ttu-id="264d6-p106">A **id** do [directoryRoleTemplate](directoryroletemplate.md) em que esta função se baseia. A propriedade deve ser especificada ao ativar uma função de diretório em um locatário com uma operação POST. Depois que a função directory tiver sido ativada, a propriedade será somente leitura.</span><span class="sxs-lookup"><span data-stu-id="264d6-p106">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="264d6-168">Relações</span><span class="sxs-lookup"><span data-stu-id="264d6-168">Relationships</span></span>
| <span data-ttu-id="264d6-169">Relação</span><span class="sxs-lookup"><span data-stu-id="264d6-169">Relationship</span></span> | <span data-ttu-id="264d6-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="264d6-170">Type</span></span> |<span data-ttu-id="264d6-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="264d6-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="264d6-172">membros</span><span class="sxs-lookup"><span data-stu-id="264d6-172">members</span></span>|<span data-ttu-id="264d6-173">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="264d6-173">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="264d6-p107">Usuários que são membros desta função de diretório. Métodos HTTP: GET, POST, DELETE. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="264d6-p107">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="264d6-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="264d6-178">JSON representation</span></span>

<span data-ttu-id="264d6-179">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="264d6-179">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRole",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
