---
title: tipo de recurso directoryRole
description: Representa uma função do diretório do Azure AD. As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*. Para obter mais informações sobre funções de diretório (administrador), confira Atribuindo funções de administrador no Azure AD. Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder a eles as permissões da função de destino. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função de diretório Administradores de Empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST com a ID do directoryRoleTemplate no qual a função directory se baseia. Herda de directoryObject.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 30b22313da70c33bffc0b759f9b474f4deac2ac1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521247"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="0b56f-110">tipo de recurso directoryRole</span><span class="sxs-lookup"><span data-stu-id="0b56f-110">directoryRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b56f-p102">Representa uma função do diretório do Azure AD. As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*. Para obter mais informações sobre funções de diretório (administrador), confira [Atribuindo funções de administrador no Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder a eles as permissões da função de destino. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função de diretório Administradores de Empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST com a ID do [directoryRoleTemplate](directoryroletemplate.md) no qual a função directory se baseia. Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="0b56f-p102">Represents an Azure AD directory role. Azure AD directory roles are also known as *administrator roles*. For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based. Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="0b56f-119">Por padrão, as funções de diretório limitam-se para ser todo o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0b56f-119">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="0b56f-120">No entanto, funções de diretório (atualmente somente o *administrador da conta de usuário* e *Administração de assistência técnica*) podem também ser escopo [unidades administrativas](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="0b56f-120">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="0b56f-121">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="0b56f-121">This resource supports:</span></span>

- <span data-ttu-id="0b56f-122">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryrole-delta.md).</span><span class="sxs-lookup"><span data-stu-id="0b56f-122">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="0b56f-123">Métodos</span><span class="sxs-lookup"><span data-stu-id="0b56f-123">Methods</span></span>

| <span data-ttu-id="0b56f-124">Método</span><span class="sxs-lookup"><span data-stu-id="0b56f-124">Method</span></span>       | <span data-ttu-id="0b56f-125">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0b56f-125">Return Type</span></span>  |<span data-ttu-id="0b56f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b56f-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0b56f-127">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="0b56f-127">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="0b56f-128">directoryRole</span><span class="sxs-lookup"><span data-stu-id="0b56f-128">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="0b56f-129">Leia as propriedades e os relacionamentos do objeto directoryRole.</span><span class="sxs-lookup"><span data-stu-id="0b56f-129">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="0b56f-130">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="0b56f-130">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="0b56f-131">Coleção [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="0b56f-131">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="0b56f-132">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="0b56f-132">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="0b56f-133">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="0b56f-133">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="0b56f-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="0b56f-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="0b56f-135">Adicione um usuário à função de diretório postando na propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="0b56f-135">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="0b56f-136">Listar membros</span><span class="sxs-lookup"><span data-stu-id="0b56f-136">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="0b56f-137">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="0b56f-137">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="0b56f-138">Obtenha os usuários que são membros da função directory da propriedade de navegação members.</span><span class="sxs-lookup"><span data-stu-id="0b56f-138">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="0b56f-139">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="0b56f-139">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="0b56f-140">directoryObject</span><span class="sxs-lookup"><span data-stu-id="0b56f-140">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="0b56f-141">Remova um usuário da função de diretório.</span><span class="sxs-lookup"><span data-stu-id="0b56f-141">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="0b56f-142">Membros da função com escopo de lista</span><span class="sxs-lookup"><span data-stu-id="0b56f-142">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="0b56f-143">coleção [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="0b56f-143">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="0b56f-144">Lista os membros dessa função directory que têm como escopo para [unidades administrativas](administrativeunit.md), toda a coleção de recursos scopedRoleMembership.</span><span class="sxs-lookup"><span data-stu-id="0b56f-144">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="0b56f-145">delta</span><span class="sxs-lookup"><span data-stu-id="0b56f-145">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="0b56f-146">Coleção directoryRole</span><span class="sxs-lookup"><span data-stu-id="0b56f-146">directoryRole collection</span></span>| <span data-ttu-id="0b56f-147">Obtenha as alterações incrementais para funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="0b56f-147">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="0b56f-148">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b56f-148">Properties</span></span>
| <span data-ttu-id="0b56f-149">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b56f-149">Property</span></span>   | <span data-ttu-id="0b56f-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b56f-150">Type</span></span> |<span data-ttu-id="0b56f-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b56f-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b56f-152">description</span><span class="sxs-lookup"><span data-stu-id="0b56f-152">description</span></span>|<span data-ttu-id="0b56f-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b56f-153">String</span></span>|<span data-ttu-id="0b56f-p104">A descrição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b56f-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="0b56f-156">displayName</span><span class="sxs-lookup"><span data-stu-id="0b56f-156">displayName</span></span>|<span data-ttu-id="0b56f-157">String</span><span class="sxs-lookup"><span data-stu-id="0b56f-157">String</span></span>|<span data-ttu-id="0b56f-p105">O nome de exibição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b56f-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="0b56f-160">id</span><span class="sxs-lookup"><span data-stu-id="0b56f-160">id</span></span>|<span data-ttu-id="0b56f-161">String</span><span class="sxs-lookup"><span data-stu-id="0b56f-161">String</span></span>|<span data-ttu-id="0b56f-p106">O identificador exclusivo da função de diretório. Herdado de [directoryObject](directoryobject.md). Chave, Não Anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="0b56f-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="0b56f-165">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="0b56f-165">roleTemplateId</span></span>|<span data-ttu-id="0b56f-166">String</span><span class="sxs-lookup"><span data-stu-id="0b56f-166">String</span></span>| <span data-ttu-id="0b56f-p107">A **id** do [directoryRoleTemplate](directoryroletemplate.md) em que esta função se baseia. A propriedade deve ser especificada ao ativar uma função de diretório em um locatário com uma operação POST. Depois que a função directory tiver sido ativada, a propriedade será somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b56f-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0b56f-170">Relações</span><span class="sxs-lookup"><span data-stu-id="0b56f-170">Relationships</span></span>
| <span data-ttu-id="0b56f-171">Relação</span><span class="sxs-lookup"><span data-stu-id="0b56f-171">Relationship</span></span> | <span data-ttu-id="0b56f-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b56f-172">Type</span></span> |<span data-ttu-id="0b56f-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b56f-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b56f-174">membros</span><span class="sxs-lookup"><span data-stu-id="0b56f-174">members</span></span>|<span data-ttu-id="0b56f-175">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="0b56f-175">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="0b56f-p108">Usuários que são membros desta função de diretório. Métodos HTTP: GET, POST, DELETE. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0b56f-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="0b56f-180">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="0b56f-180">scopedMembers</span></span>|<span data-ttu-id="0b56f-181">coleção [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="0b56f-181">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="0b56f-182">Membros da função diretório que têm o escopo para [unidades administrativas](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="0b56f-182">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="0b56f-183">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b56f-183">Read-only.</span></span> <span data-ttu-id="0b56f-184">Anulável.</span><span class="sxs-lookup"><span data-stu-id="0b56f-184">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b56f-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b56f-185">JSON representation</span></span>

<span data-ttu-id="0b56f-186">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0b56f-186">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole"
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
