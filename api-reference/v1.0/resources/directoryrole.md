---
title: tipo de recurso directoryRole
description: Representa uma função do diretório do Azure AD. As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*. Para obter mais informações sobre funções de diretório (administrador), confira Atribuindo funções de administrador no Azure AD. Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder a eles as permissões da função de destino. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função de diretório Administradores de Empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST com a ID do directoryRoleTemplate no qual a função directory se baseia. Herda de directoryObject.
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 863eab2d015c81a61fbfc71c3a39cf75ff6840cf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032750"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="08d7e-110">tipo de recurso directoryRole</span><span class="sxs-lookup"><span data-stu-id="08d7e-110">directoryRole resource type</span></span>

<span data-ttu-id="08d7e-111">Representa uma função do diretório do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="08d7e-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="08d7e-112">As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*.</span><span class="sxs-lookup"><span data-stu-id="08d7e-112">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="08d7e-113">Para obter mais informações sobre funções de diretório (administrador), confira [Atribuindo funções de administrador no Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="08d7e-113">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="08d7e-114">Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder a eles as permissões da função de destino.</span><span class="sxs-lookup"><span data-stu-id="08d7e-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="08d7e-115">Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário.</span><span class="sxs-lookup"><span data-stu-id="08d7e-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="08d7e-116">Apenas a função de diretório Administradores de Empresa é ativada por padrão.</span><span class="sxs-lookup"><span data-stu-id="08d7e-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="08d7e-117">Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST com a ID do [directoryRoleTemplate](directoryroletemplate.md) no qual a função directory se baseia.</span><span class="sxs-lookup"><span data-stu-id="08d7e-117">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="08d7e-118">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="08d7e-118">Inherits from [directoryObject](directoryobject.md).</span></span>
<span data-ttu-id="08d7e-119">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="08d7e-119">This resource supports:</span></span>

- <span data-ttu-id="08d7e-120">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryrole-delta.md).</span><span class="sxs-lookup"><span data-stu-id="08d7e-120">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="08d7e-121">Métodos</span><span class="sxs-lookup"><span data-stu-id="08d7e-121">Methods</span></span>

| <span data-ttu-id="08d7e-122">Método</span><span class="sxs-lookup"><span data-stu-id="08d7e-122">Method</span></span>       | <span data-ttu-id="08d7e-123">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="08d7e-123">Return Type</span></span>  |<span data-ttu-id="08d7e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="08d7e-124">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="08d7e-125">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="08d7e-125">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="08d7e-126">directoryRole</span><span class="sxs-lookup"><span data-stu-id="08d7e-126">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="08d7e-127">Leia as propriedades e os relacionamentos do objeto directoryRole.</span><span class="sxs-lookup"><span data-stu-id="08d7e-127">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="08d7e-128">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="08d7e-128">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="08d7e-129">Coleção [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="08d7e-129">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="08d7e-130">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="08d7e-130">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="08d7e-131">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="08d7e-131">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="08d7e-132">directoryObject</span><span class="sxs-lookup"><span data-stu-id="08d7e-132">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="08d7e-133">Adicione um usuário à função de diretório postando na propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="08d7e-133">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="08d7e-134">Listar membros</span><span class="sxs-lookup"><span data-stu-id="08d7e-134">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="08d7e-135">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="08d7e-135">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="08d7e-136">Obtenha os usuários que são membros da função directory da propriedade de navegação members.</span><span class="sxs-lookup"><span data-stu-id="08d7e-136">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="08d7e-137">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="08d7e-137">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="08d7e-138">directoryObject</span><span class="sxs-lookup"><span data-stu-id="08d7e-138">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="08d7e-139">Remova um usuário da função de diretório.</span><span class="sxs-lookup"><span data-stu-id="08d7e-139">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="08d7e-140">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="08d7e-140">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="08d7e-141">directoryRole</span><span class="sxs-lookup"><span data-stu-id="08d7e-141">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="08d7e-142">Ative uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="08d7e-142">Activate a directory role.</span></span>|
|[<span data-ttu-id="08d7e-143">delta</span><span class="sxs-lookup"><span data-stu-id="08d7e-143">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="08d7e-144">Coleção directoryRole</span><span class="sxs-lookup"><span data-stu-id="08d7e-144">directoryRole collection</span></span>| <span data-ttu-id="08d7e-145">Obtenha alterações incrementais para as funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="08d7e-145">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="08d7e-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08d7e-146">Properties</span></span>
| <span data-ttu-id="08d7e-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08d7e-147">Property</span></span>   | <span data-ttu-id="08d7e-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="08d7e-148">Type</span></span> | <span data-ttu-id="08d7e-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="08d7e-149">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="08d7e-150">description</span><span class="sxs-lookup"><span data-stu-id="08d7e-150">description</span></span>|<span data-ttu-id="08d7e-151">String</span><span class="sxs-lookup"><span data-stu-id="08d7e-151">String</span></span>|<span data-ttu-id="08d7e-p103">A descrição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="08d7e-p103">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="08d7e-154">displayName</span><span class="sxs-lookup"><span data-stu-id="08d7e-154">displayName</span></span>|<span data-ttu-id="08d7e-155">String</span><span class="sxs-lookup"><span data-stu-id="08d7e-155">String</span></span>|<span data-ttu-id="08d7e-p104">O nome de exibição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="08d7e-p104">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="08d7e-158">id</span><span class="sxs-lookup"><span data-stu-id="08d7e-158">id</span></span>|<span data-ttu-id="08d7e-159">String</span><span class="sxs-lookup"><span data-stu-id="08d7e-159">String</span></span>|<span data-ttu-id="08d7e-p105">O identificador exclusivo da função de diretório. Herdado de [directoryObject](directoryobject.md). Chave, Não Anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="08d7e-p105">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="08d7e-163">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="08d7e-163">roleTemplateId</span></span>|<span data-ttu-id="08d7e-164">String</span><span class="sxs-lookup"><span data-stu-id="08d7e-164">String</span></span>| <span data-ttu-id="08d7e-p106">A **id** do [directoryRoleTemplate](directoryroletemplate.md) em que esta função se baseia. A propriedade deve ser especificada ao ativar uma função de diretório em um locatário com uma operação POST. Depois que a função directory tiver sido ativada, a propriedade será somente leitura.</span><span class="sxs-lookup"><span data-stu-id="08d7e-p106">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="08d7e-168">Relações</span><span class="sxs-lookup"><span data-stu-id="08d7e-168">Relationships</span></span>
| <span data-ttu-id="08d7e-169">Relação</span><span class="sxs-lookup"><span data-stu-id="08d7e-169">Relationship</span></span> | <span data-ttu-id="08d7e-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="08d7e-170">Type</span></span> |<span data-ttu-id="08d7e-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="08d7e-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08d7e-172">membros</span><span class="sxs-lookup"><span data-stu-id="08d7e-172">members</span></span>|<span data-ttu-id="08d7e-173">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="08d7e-173">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="08d7e-p107">Usuários que são membros desta função de diretório. Métodos HTTP: GET, POST, DELETE. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="08d7e-p107">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08d7e-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08d7e-178">JSON representation</span></span>

<span data-ttu-id="08d7e-179">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="08d7e-179">Here is a JSON representation of the resource</span></span>

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
