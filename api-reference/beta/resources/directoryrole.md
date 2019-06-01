---
title: tipo de recurso directoryRole
description: Representa uma função do diretório do Azure AD. As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*. Para obter mais informações sobre funções de diretório (administrador), confira Atribuindo funções de administrador no Azure AD. Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder a eles as permissões da função de destino. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função de diretório Administradores de Empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, envie uma solicitação POST com a ID do directoryRoleTemplate na qual a função de diretório se baseia. Herda de directoryObject.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ac9b08e2e39bce6a20703089d6bfe69c8b25f55f
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657900"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="de8f1-110">tipo de recurso directoryRole</span><span class="sxs-lookup"><span data-stu-id="de8f1-110">directoryRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de8f1-111">Representa uma função do diretório do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="de8f1-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="de8f1-112">As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*.</span><span class="sxs-lookup"><span data-stu-id="de8f1-112">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="de8f1-113">Para obter mais informações sobre funções de diretório (administrador), confira [Atribuindo funções de administrador no Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="de8f1-113">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="de8f1-114">Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder a eles as permissões da função de destino.</span><span class="sxs-lookup"><span data-stu-id="de8f1-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="de8f1-115">Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário.</span><span class="sxs-lookup"><span data-stu-id="de8f1-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="de8f1-116">Apenas a função de diretório Administradores de Empresa é ativada por padrão.</span><span class="sxs-lookup"><span data-stu-id="de8f1-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="de8f1-117">Para ativar outras funções de diretório disponíveis, envie uma solicitação POST com a ID do [directoryRoleTemplate](directoryroletemplate.md) na qual a função de diretório se baseia.</span><span class="sxs-lookup"><span data-stu-id="de8f1-117">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="de8f1-118">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="de8f1-118">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="de8f1-119">Por padrão, as funções de diretório têm o escopo para todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="de8f1-119">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="de8f1-120">No entanto, as funções de diretório (atualmente, somente o administrador da *conta de usuário* e o *administrador de helpdesk*) também podem ter escopo para [unidades administrativas](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="de8f1-120">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="de8f1-121">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="de8f1-121">This resource supports:</span></span>

- <span data-ttu-id="de8f1-122">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryrole-delta.md).</span><span class="sxs-lookup"><span data-stu-id="de8f1-122">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="de8f1-123">Métodos</span><span class="sxs-lookup"><span data-stu-id="de8f1-123">Methods</span></span>

| <span data-ttu-id="de8f1-124">Método</span><span class="sxs-lookup"><span data-stu-id="de8f1-124">Method</span></span>       | <span data-ttu-id="de8f1-125">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="de8f1-125">Return Type</span></span>  |<span data-ttu-id="de8f1-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="de8f1-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="de8f1-127">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="de8f1-127">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="de8f1-128">directoryRole</span><span class="sxs-lookup"><span data-stu-id="de8f1-128">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="de8f1-129">Leia as propriedades e os relacionamentos do objeto directoryRole.</span><span class="sxs-lookup"><span data-stu-id="de8f1-129">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="de8f1-130">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="de8f1-130">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="de8f1-131">Coleção [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="de8f1-131">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="de8f1-132">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="de8f1-132">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="de8f1-133">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="de8f1-133">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="de8f1-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="de8f1-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="de8f1-135">Adicione um usuário à função de diretório postando na propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="de8f1-135">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="de8f1-136">Listar membros</span><span class="sxs-lookup"><span data-stu-id="de8f1-136">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="de8f1-137">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="de8f1-137">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="de8f1-138">Obtenha os usuários que são membros da função directory da propriedade de navegação members.</span><span class="sxs-lookup"><span data-stu-id="de8f1-138">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="de8f1-139">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="de8f1-139">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="de8f1-140">directoryObject</span><span class="sxs-lookup"><span data-stu-id="de8f1-140">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="de8f1-141">Remova um usuário da função de diretório.</span><span class="sxs-lookup"><span data-stu-id="de8f1-141">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="de8f1-142">Listar membros de função com escopo</span><span class="sxs-lookup"><span data-stu-id="de8f1-142">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="de8f1-143">Coleção [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="de8f1-143">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="de8f1-144">Listar os membros dessa função de diretório que estão no escopo de [unidades administrativas](administrativeunit.md), por meio da coleção de recursos scopedRoleMembership.</span><span class="sxs-lookup"><span data-stu-id="de8f1-144">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="de8f1-145">delta</span><span class="sxs-lookup"><span data-stu-id="de8f1-145">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="de8f1-146">Coleção directoryRole</span><span class="sxs-lookup"><span data-stu-id="de8f1-146">directoryRole collection</span></span>| <span data-ttu-id="de8f1-147">Obtenha alterações incrementais para as funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="de8f1-147">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="de8f1-148">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de8f1-148">Properties</span></span>
| <span data-ttu-id="de8f1-149">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de8f1-149">Property</span></span>   | <span data-ttu-id="de8f1-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="de8f1-150">Type</span></span> |<span data-ttu-id="de8f1-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="de8f1-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de8f1-152">description</span><span class="sxs-lookup"><span data-stu-id="de8f1-152">description</span></span>|<span data-ttu-id="de8f1-153">String</span><span class="sxs-lookup"><span data-stu-id="de8f1-153">String</span></span>|<span data-ttu-id="de8f1-p104">A descrição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de8f1-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="de8f1-156">displayName</span><span class="sxs-lookup"><span data-stu-id="de8f1-156">displayName</span></span>|<span data-ttu-id="de8f1-157">String</span><span class="sxs-lookup"><span data-stu-id="de8f1-157">String</span></span>|<span data-ttu-id="de8f1-p105">O nome de exibição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de8f1-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="de8f1-160">id</span><span class="sxs-lookup"><span data-stu-id="de8f1-160">id</span></span>|<span data-ttu-id="de8f1-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de8f1-161">String</span></span>|<span data-ttu-id="de8f1-p106">O identificador exclusivo da função de diretório. Herdado de [directoryObject](directoryobject.md). Chave, Não Anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="de8f1-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="de8f1-165">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="de8f1-165">roleTemplateId</span></span>|<span data-ttu-id="de8f1-166">String</span><span class="sxs-lookup"><span data-stu-id="de8f1-166">String</span></span>| <span data-ttu-id="de8f1-p107">A **id** do [directoryRoleTemplate](directoryroletemplate.md) em que esta função se baseia. A propriedade deve ser especificada ao ativar uma função de diretório em um locatário com uma operação POST. Depois que a função directory tiver sido ativada, a propriedade será somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de8f1-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="de8f1-170">Relações</span><span class="sxs-lookup"><span data-stu-id="de8f1-170">Relationships</span></span>
| <span data-ttu-id="de8f1-171">Relação</span><span class="sxs-lookup"><span data-stu-id="de8f1-171">Relationship</span></span> | <span data-ttu-id="de8f1-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="de8f1-172">Type</span></span> |<span data-ttu-id="de8f1-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="de8f1-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de8f1-174">membros</span><span class="sxs-lookup"><span data-stu-id="de8f1-174">members</span></span>|<span data-ttu-id="de8f1-175">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="de8f1-175">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="de8f1-p108">Usuários que são membros desta função de diretório. Métodos HTTP: GET, POST, DELETE. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="de8f1-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="de8f1-180">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="de8f1-180">scopedMembers</span></span>|<span data-ttu-id="de8f1-181">Coleção [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="de8f1-181">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="de8f1-182">Membros desta função de diretório com escopo para [unidades administrativas](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="de8f1-182">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="de8f1-183">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de8f1-183">Read-only.</span></span> <span data-ttu-id="de8f1-184">Anulável.</span><span class="sxs-lookup"><span data-stu-id="de8f1-184">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de8f1-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de8f1-185">JSON representation</span></span>

<span data-ttu-id="de8f1-186">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="de8f1-186">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->
