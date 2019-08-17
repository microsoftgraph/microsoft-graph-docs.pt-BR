---
title: tipo de recurso directoryRole
description: Representa uma função do diretório do Azure AD. As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f09a6f248e7a677cb5e19bcc00085933b90b24a4
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450498"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="7cdb4-104">tipo de recurso directoryRole</span><span class="sxs-lookup"><span data-stu-id="7cdb4-104">directoryRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cdb4-105">Representa uma função do diretório do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-105">Represents an Azure AD directory role.</span></span> <span data-ttu-id="7cdb4-106">As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-106">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="7cdb4-107">Para obter mais informações sobre funções de diretório (administrador), confira [Atribuindo funções de administrador no Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="7cdb4-107">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="7cdb4-108">Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder a eles as permissões da função de destino.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-108">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="7cdb4-109">Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-109">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="7cdb4-110">Apenas a função de diretório Administradores de Empresa é ativada por padrão.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-110">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="7cdb4-111">Para ativar outras funções de diretório disponíveis, envie uma solicitação POST com a ID do [directoryRoleTemplate](directoryroletemplate.md) na qual a função de diretório se baseia.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-111">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="7cdb4-112">[Listar modelos de função de diretório](../api/directoryroletemplate-list.md) para obter todas as outras funções de diretório disponíveis.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-112">[List directory role templates](../api/directoryroletemplate-list.md) to get all the other available directory roles.</span></span> <span data-ttu-id="7cdb4-113">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="7cdb4-113">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="7cdb4-114">Por padrão, as funções de diretório têm o escopo para todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-114">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="7cdb4-115">No entanto, as funções de diretório (atualmente, somente o administrador da *conta de usuário* e o *administrador de helpdesk*) também podem ter escopo para [unidades administrativas](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="7cdb4-115">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="7cdb4-116">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="7cdb4-116">This resource supports:</span></span>

- <span data-ttu-id="7cdb4-117">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryrole-delta.md).</span><span class="sxs-lookup"><span data-stu-id="7cdb4-117">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="7cdb4-118">Métodos</span><span class="sxs-lookup"><span data-stu-id="7cdb4-118">Methods</span></span>

| <span data-ttu-id="7cdb4-119">Método</span><span class="sxs-lookup"><span data-stu-id="7cdb4-119">Method</span></span>       | <span data-ttu-id="7cdb4-120">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7cdb4-120">Return Type</span></span>  |<span data-ttu-id="7cdb4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cdb4-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7cdb4-122">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="7cdb4-122">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="7cdb4-123">directoryRole</span><span class="sxs-lookup"><span data-stu-id="7cdb4-123">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="7cdb4-124">Leia as propriedades e os relacionamentos do objeto directoryRole.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-124">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="7cdb4-125">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="7cdb4-125">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="7cdb4-126">Coleção [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="7cdb4-126">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="7cdb4-127">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-127">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="7cdb4-128">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="7cdb4-128">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="7cdb4-129">directoryObject</span><span class="sxs-lookup"><span data-stu-id="7cdb4-129">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="7cdb4-130">Adicione um usuário à função de diretório postando na propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-130">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="7cdb4-131">Listar membros</span><span class="sxs-lookup"><span data-stu-id="7cdb4-131">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="7cdb4-132">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="7cdb4-132">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="7cdb4-133">Obtenha os usuários que são membros da função directory da propriedade de navegação members.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-133">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="7cdb4-134">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="7cdb4-134">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="7cdb4-135">directoryObject</span><span class="sxs-lookup"><span data-stu-id="7cdb4-135">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="7cdb4-136">Remova um usuário da função de diretório.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-136">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="7cdb4-137">Listar membros de função com escopo</span><span class="sxs-lookup"><span data-stu-id="7cdb4-137">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="7cdb4-138">Coleção [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="7cdb4-138">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="7cdb4-139">Listar os membros dessa função de diretório que estão no escopo de [unidades administrativas](administrativeunit.md), por meio da coleção de recursos scopedRoleMembership.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-139">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="7cdb4-140">delta</span><span class="sxs-lookup"><span data-stu-id="7cdb4-140">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="7cdb4-141">Coleção directoryRole</span><span class="sxs-lookup"><span data-stu-id="7cdb4-141">directoryRole collection</span></span>| <span data-ttu-id="7cdb4-142">Obtenha alterações incrementais para as funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-142">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="7cdb4-143">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7cdb4-143">Properties</span></span>
| <span data-ttu-id="7cdb4-144">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7cdb4-144">Property</span></span>   | <span data-ttu-id="7cdb4-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="7cdb4-145">Type</span></span> |<span data-ttu-id="7cdb4-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cdb4-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7cdb4-147">description</span><span class="sxs-lookup"><span data-stu-id="7cdb4-147">description</span></span>|<span data-ttu-id="7cdb4-148">String</span><span class="sxs-lookup"><span data-stu-id="7cdb4-148">String</span></span>|<span data-ttu-id="7cdb4-p104">A descrição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="7cdb4-151">displayName</span><span class="sxs-lookup"><span data-stu-id="7cdb4-151">displayName</span></span>|<span data-ttu-id="7cdb4-152">String</span><span class="sxs-lookup"><span data-stu-id="7cdb4-152">String</span></span>|<span data-ttu-id="7cdb4-p105">O nome de exibição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="7cdb4-155">id</span><span class="sxs-lookup"><span data-stu-id="7cdb4-155">id</span></span>|<span data-ttu-id="7cdb4-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7cdb4-156">String</span></span>|<span data-ttu-id="7cdb4-p106">O identificador exclusivo da função de diretório. Herdado de [directoryObject](directoryobject.md). Chave, Não Anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="7cdb4-160">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="7cdb4-160">roleTemplateId</span></span>|<span data-ttu-id="7cdb4-161">String</span><span class="sxs-lookup"><span data-stu-id="7cdb4-161">String</span></span>| <span data-ttu-id="7cdb4-p107">A **id** do [directoryRoleTemplate](directoryroletemplate.md) em que esta função se baseia. A propriedade deve ser especificada ao ativar uma função de diretório em um locatário com uma operação POST. Depois que a função directory tiver sido ativada, a propriedade será somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7cdb4-165">Relações</span><span class="sxs-lookup"><span data-stu-id="7cdb4-165">Relationships</span></span>
| <span data-ttu-id="7cdb4-166">Relação</span><span class="sxs-lookup"><span data-stu-id="7cdb4-166">Relationship</span></span> | <span data-ttu-id="7cdb4-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="7cdb4-167">Type</span></span> |<span data-ttu-id="7cdb4-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cdb4-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7cdb4-169">membros</span><span class="sxs-lookup"><span data-stu-id="7cdb4-169">members</span></span>|<span data-ttu-id="7cdb4-170">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="7cdb4-170">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="7cdb4-p108">Usuários que são membros desta função de diretório. Métodos HTTP: GET, POST, DELETE. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="7cdb4-175">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="7cdb4-175">scopedMembers</span></span>|<span data-ttu-id="7cdb4-176">Coleção [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="7cdb4-176">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="7cdb4-177">Membros desta função de diretório com escopo para [unidades administrativas](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="7cdb4-177">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="7cdb4-178">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-178">Read-only.</span></span> <span data-ttu-id="7cdb4-179">Anulável.</span><span class="sxs-lookup"><span data-stu-id="7cdb4-179">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7cdb4-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7cdb4-180">JSON representation</span></span>

<span data-ttu-id="7cdb4-181">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7cdb4-181">Here is a JSON representation of the resource</span></span>

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
