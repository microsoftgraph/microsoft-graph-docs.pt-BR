---
title: tipo de recurso directoryRole
description: Representa uma função do diretório do Azure AD. As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 701920b532e0c7003e624466c2d8d0614f47989f
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118697"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="6b1d7-104">tipo de recurso directoryRole</span><span class="sxs-lookup"><span data-stu-id="6b1d7-104">directoryRole resource type</span></span>

<span data-ttu-id="6b1d7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b1d7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b1d7-106">Representa uma função do diretório do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-106">Represents an Azure AD directory role.</span></span> <span data-ttu-id="6b1d7-107">As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-107">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="6b1d7-108">Para obter mais informações sobre funções de diretório (administrador), confira [Atribuindo funções de administrador no Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="6b1d7-108">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span> <span data-ttu-id="6b1d7-109">Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder a eles as permissões da função de destino.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-109">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="6b1d7-110">Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-110">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="6b1d7-111">Apenas a função de diretório Administradores de Empresa é ativada por padrão.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-111">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="6b1d7-112">Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST com a ID do [directoryRoleTemplate](directoryroletemplate.md) no qual a função de diretório é baseada.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-112">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="6b1d7-113">[Liste modelos de função de diretório](../api/directoryroletemplate-list.md) para ter todas as outras funções de diretório disponíveis.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-113">[List directory role templates](../api/directoryroletemplate-list.md) to get all the other available directory roles.</span></span> <span data-ttu-id="6b1d7-114">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="6b1d7-114">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="6b1d7-115">Por padrão, as funções de diretório têm escopo para serem de todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-115">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="6b1d7-116">No entanto, as funções  de diretório (atualmente apenas o administrador da conta de usuário e o administrador *do helpdesk*) também podem ser escopo para unidades [administrativas](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="6b1d7-116">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="6b1d7-117">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="6b1d7-117">This resource supports:</span></span>

- <span data-ttu-id="6b1d7-118">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryrole-delta.md).</span><span class="sxs-lookup"><span data-stu-id="6b1d7-118">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="6b1d7-119">Métodos</span><span class="sxs-lookup"><span data-stu-id="6b1d7-119">Methods</span></span>

| <span data-ttu-id="6b1d7-120">Método</span><span class="sxs-lookup"><span data-stu-id="6b1d7-120">Method</span></span>       | <span data-ttu-id="6b1d7-121">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6b1d7-121">Return Type</span></span>  |<span data-ttu-id="6b1d7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b1d7-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6b1d7-123">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="6b1d7-123">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="6b1d7-124">directoryRole</span><span class="sxs-lookup"><span data-stu-id="6b1d7-124">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="6b1d7-125">Leia as propriedades e os relacionamentos do objeto directoryRole.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-125">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="6b1d7-126">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="6b1d7-126">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="6b1d7-127">Coleção [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="6b1d7-127">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="6b1d7-128">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-128">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="6b1d7-129">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="6b1d7-129">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="6b1d7-130">directoryObject</span><span class="sxs-lookup"><span data-stu-id="6b1d7-130">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="6b1d7-131">Adicione um usuário à função de diretório postando na propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-131">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="6b1d7-132">Listar membros</span><span class="sxs-lookup"><span data-stu-id="6b1d7-132">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="6b1d7-133">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="6b1d7-133">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="6b1d7-134">Obtenha os usuários que são membros da função directory da propriedade de navegação members.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-134">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="6b1d7-135">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="6b1d7-135">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="6b1d7-136">directoryObject</span><span class="sxs-lookup"><span data-stu-id="6b1d7-136">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="6b1d7-137">Remova um usuário da função de diretório.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-137">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="6b1d7-138">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="6b1d7-138">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="6b1d7-139">directoryRole</span><span class="sxs-lookup"><span data-stu-id="6b1d7-139">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="6b1d7-140">Ative uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-140">Activate a directory role.</span></span>|
|[<span data-ttu-id="6b1d7-141">Listar scopeMembers</span><span class="sxs-lookup"><span data-stu-id="6b1d7-141">List scopeMembers</span></span>](../api/directoryrole-list-scopedmembers.md) |<span data-ttu-id="6b1d7-142">Coleção [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="6b1d7-142">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="6b1d7-143">Listar os membros dessa função de diretório que são escopos para unidades administrativas [,](administrativeunit.md)por meio da coleção de recursos scopedRoleMembership.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-143">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="6b1d7-144">delta</span><span class="sxs-lookup"><span data-stu-id="6b1d7-144">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="6b1d7-145">Coleção directoryRole</span><span class="sxs-lookup"><span data-stu-id="6b1d7-145">directoryRole collection</span></span>| <span data-ttu-id="6b1d7-146">Obtenha alterações incrementais para as funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-146">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="6b1d7-147">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b1d7-147">Properties</span></span>
| <span data-ttu-id="6b1d7-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b1d7-148">Property</span></span>   | <span data-ttu-id="6b1d7-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b1d7-149">Type</span></span> |<span data-ttu-id="6b1d7-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b1d7-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b1d7-151">description</span><span class="sxs-lookup"><span data-stu-id="6b1d7-151">description</span></span>|<span data-ttu-id="6b1d7-152">String</span><span class="sxs-lookup"><span data-stu-id="6b1d7-152">String</span></span>|<span data-ttu-id="6b1d7-p104">A descrição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="6b1d7-155">displayName</span><span class="sxs-lookup"><span data-stu-id="6b1d7-155">displayName</span></span>|<span data-ttu-id="6b1d7-156">String</span><span class="sxs-lookup"><span data-stu-id="6b1d7-156">String</span></span>|<span data-ttu-id="6b1d7-p105">O nome de exibição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="6b1d7-159">id</span><span class="sxs-lookup"><span data-stu-id="6b1d7-159">id</span></span>|<span data-ttu-id="6b1d7-160">String</span><span class="sxs-lookup"><span data-stu-id="6b1d7-160">String</span></span>|<span data-ttu-id="6b1d7-p106">O identificador exclusivo da função de diretório. Herdado de [directoryObject](directoryobject.md). Chave, Não Anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="6b1d7-164">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="6b1d7-164">roleTemplateId</span></span>|<span data-ttu-id="6b1d7-165">String</span><span class="sxs-lookup"><span data-stu-id="6b1d7-165">String</span></span>| <span data-ttu-id="6b1d7-p107">A **id** do [directoryRoleTemplate](directoryroletemplate.md) em que esta função se baseia. A propriedade deve ser especificada ao ativar uma função de diretório em um locatário com uma operação POST. Depois que a função directory tiver sido ativada, a propriedade será somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6b1d7-169">Relações</span><span class="sxs-lookup"><span data-stu-id="6b1d7-169">Relationships</span></span>
| <span data-ttu-id="6b1d7-170">Relação</span><span class="sxs-lookup"><span data-stu-id="6b1d7-170">Relationship</span></span> | <span data-ttu-id="6b1d7-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b1d7-171">Type</span></span> |<span data-ttu-id="6b1d7-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b1d7-172">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b1d7-173">membros</span><span class="sxs-lookup"><span data-stu-id="6b1d7-173">members</span></span>|<span data-ttu-id="6b1d7-174">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="6b1d7-174">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="6b1d7-p108">Usuários que são membros desta função de diretório. Métodos HTTP: GET, POST, DELETE. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6b1d7-179">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="6b1d7-179">scopedMembers</span></span>|<span data-ttu-id="6b1d7-180">Coleção [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="6b1d7-180">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="6b1d7-181">Membros dessa função de diretório com escopo para unidades [administrativas](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="6b1d7-181">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="6b1d7-182">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-182">Read-only.</span></span> <span data-ttu-id="6b1d7-183">Anulável.</span><span class="sxs-lookup"><span data-stu-id="6b1d7-183">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b1d7-184">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b1d7-184">JSON representation</span></span>

<span data-ttu-id="6b1d7-185">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6b1d7-185">Here is a JSON representation of the resource</span></span>

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
