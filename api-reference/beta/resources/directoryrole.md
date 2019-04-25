---
title: tipo de recurso directoryRole
description: Representa uma função do diretório do Azure AD. As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*. Para obter mais informações sobre funções de diretório (administrador), confira Atribuindo funções de administrador no Azure AD. Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder a eles as permissões da função de destino. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função de diretório Administradores de Empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, envie uma solicitação POST com a ID do directoryRoleTemplate na qual a função de diretório se baseia. Herda de directoryObject.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 30b22313da70c33bffc0b759f9b474f4deac2ac1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535263"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="1a925-110">tipo de recurso directoryRole</span><span class="sxs-lookup"><span data-stu-id="1a925-110">directoryRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a925-111">Representa uma função do diretório do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1a925-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="1a925-112">As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*.</span><span class="sxs-lookup"><span data-stu-id="1a925-112">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="1a925-113">Para obter mais informações sobre funções de diretório (administrador), confira [Atribuindo funções de administrador no Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="1a925-113">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="1a925-114">Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder a eles as permissões da função de destino.</span><span class="sxs-lookup"><span data-stu-id="1a925-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="1a925-115">Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário.</span><span class="sxs-lookup"><span data-stu-id="1a925-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="1a925-116">Apenas a função de diretório Administradores de Empresa é ativada por padrão.</span><span class="sxs-lookup"><span data-stu-id="1a925-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="1a925-117">Para ativar outras funções de diretório disponíveis, envie uma solicitação POST com a ID do [directoryRoleTemplate](directoryroletemplate.md) na qual a função de diretório se baseia.</span><span class="sxs-lookup"><span data-stu-id="1a925-117">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="1a925-118">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="1a925-118">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="1a925-119">Por padrão, as funções de diretório têm o escopo para todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a925-119">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="1a925-120">No enTanto, as funções de diretório (atualmente, somente o administrador da *conta de usuário* e o *administrador de helpdesk*) também podem ter escopo para [unidades administrativas](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="1a925-120">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="1a925-121">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="1a925-121">This resource supports:</span></span>

- <span data-ttu-id="1a925-122">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryrole-delta.md).</span><span class="sxs-lookup"><span data-stu-id="1a925-122">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="1a925-123">Métodos</span><span class="sxs-lookup"><span data-stu-id="1a925-123">Methods</span></span>

| <span data-ttu-id="1a925-124">Método</span><span class="sxs-lookup"><span data-stu-id="1a925-124">Method</span></span>       | <span data-ttu-id="1a925-125">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1a925-125">Return Type</span></span>  |<span data-ttu-id="1a925-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a925-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1a925-127">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="1a925-127">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="1a925-128">directoryRole</span><span class="sxs-lookup"><span data-stu-id="1a925-128">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="1a925-129">Leia as propriedades e os relacionamentos do objeto directoryRole.</span><span class="sxs-lookup"><span data-stu-id="1a925-129">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="1a925-130">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="1a925-130">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="1a925-131">Coleção [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="1a925-131">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="1a925-132">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="1a925-132">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="1a925-133">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="1a925-133">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="1a925-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="1a925-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="1a925-135">Adicione um usuário à função de diretório postando na propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="1a925-135">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="1a925-136">Listar membros</span><span class="sxs-lookup"><span data-stu-id="1a925-136">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="1a925-137">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="1a925-137">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1a925-138">Obtenha os usuários que são membros da função directory da propriedade de navegação members.</span><span class="sxs-lookup"><span data-stu-id="1a925-138">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="1a925-139">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="1a925-139">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="1a925-140">directoryObject</span><span class="sxs-lookup"><span data-stu-id="1a925-140">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="1a925-141">Remover um usuário da função de diretório.</span><span class="sxs-lookup"><span data-stu-id="1a925-141">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="1a925-142">Listar membros de função com escopo</span><span class="sxs-lookup"><span data-stu-id="1a925-142">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="1a925-143">Coleção [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="1a925-143">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="1a925-144">Listar os membros dessa função de diretório que estão no escopo de [unidades administrativas](administrativeunit.md), por meio da coleção de recursos scopedRoleMembership.</span><span class="sxs-lookup"><span data-stu-id="1a925-144">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="1a925-145">delta</span><span class="sxs-lookup"><span data-stu-id="1a925-145">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="1a925-146">Coleção directoryRole</span><span class="sxs-lookup"><span data-stu-id="1a925-146">directoryRole collection</span></span>| <span data-ttu-id="1a925-147">Obter alterações incrementais para funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="1a925-147">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="1a925-148">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a925-148">Properties</span></span>
| <span data-ttu-id="1a925-149">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a925-149">Property</span></span>   | <span data-ttu-id="1a925-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a925-150">Type</span></span> |<span data-ttu-id="1a925-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a925-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a925-152">description</span><span class="sxs-lookup"><span data-stu-id="1a925-152">description</span></span>|<span data-ttu-id="1a925-153">String</span><span class="sxs-lookup"><span data-stu-id="1a925-153">String</span></span>|<span data-ttu-id="1a925-p104">A descrição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a925-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="1a925-156">displayName</span><span class="sxs-lookup"><span data-stu-id="1a925-156">displayName</span></span>|<span data-ttu-id="1a925-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a925-157">String</span></span>|<span data-ttu-id="1a925-p105">O nome de exibição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a925-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="1a925-160">id</span><span class="sxs-lookup"><span data-stu-id="1a925-160">id</span></span>|<span data-ttu-id="1a925-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a925-161">String</span></span>|<span data-ttu-id="1a925-p106">O identificador exclusivo da função de diretório. Herdado de [directoryObject](directoryobject.md). Chave, Não Anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="1a925-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="1a925-165">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="1a925-165">roleTemplateId</span></span>|<span data-ttu-id="1a925-166">String</span><span class="sxs-lookup"><span data-stu-id="1a925-166">String</span></span>| <span data-ttu-id="1a925-p107">A **id** do [directoryRoleTemplate](directoryroletemplate.md) em que esta função se baseia. A propriedade deve ser especificada ao ativar uma função de diretório em um locatário com uma operação POST. Depois que a função directory tiver sido ativada, a propriedade será somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a925-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1a925-170">Relações</span><span class="sxs-lookup"><span data-stu-id="1a925-170">Relationships</span></span>
| <span data-ttu-id="1a925-171">Relação</span><span class="sxs-lookup"><span data-stu-id="1a925-171">Relationship</span></span> | <span data-ttu-id="1a925-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a925-172">Type</span></span> |<span data-ttu-id="1a925-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a925-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a925-174">members</span><span class="sxs-lookup"><span data-stu-id="1a925-174">members</span></span>|<span data-ttu-id="1a925-175">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="1a925-175">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="1a925-p108">Usuários que são membros desta função de diretório. Métodos HTTP: GET, POST, DELETE. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="1a925-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="1a925-180">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="1a925-180">scopedMembers</span></span>|<span data-ttu-id="1a925-181">Coleção [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="1a925-181">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="1a925-182">Membros desta função de diretório com escopo para [unidades administrativas](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="1a925-182">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="1a925-183">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a925-183">Read-only.</span></span> <span data-ttu-id="1a925-184">Anulável.</span><span class="sxs-lookup"><span data-stu-id="1a925-184">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a925-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a925-185">JSON representation</span></span>

<span data-ttu-id="1a925-186">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1a925-186">Here is a JSON representation of the resource</span></span>

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
