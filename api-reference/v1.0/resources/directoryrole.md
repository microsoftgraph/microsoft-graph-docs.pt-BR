---
title: tipo de recurso directoryRole
description: Representa uma função do diretório do Azure AD. As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*.
localization_priority: Priority
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ffff28d87464289db6280aa1a7e3822736db02b8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439895"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="95906-104">tipo de recurso directoryRole</span><span class="sxs-lookup"><span data-stu-id="95906-104">directoryRole resource type</span></span>

<span data-ttu-id="95906-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95906-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95906-106">Representa uma função do diretório do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="95906-106">Represents an Azure AD directory role.</span></span> <span data-ttu-id="95906-107">As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*.</span><span class="sxs-lookup"><span data-stu-id="95906-107">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="95906-108">Para obter mais informações sobre funções de diretório (administrador), confira [Atribuindo funções de administrador no Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="95906-108">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span> <span data-ttu-id="95906-109">Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder a eles as permissões da função de destino.</span><span class="sxs-lookup"><span data-stu-id="95906-109">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="95906-110">Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário.</span><span class="sxs-lookup"><span data-stu-id="95906-110">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="95906-111">Apenas a função de diretório Administradores de Empresa é ativada por padrão.</span><span class="sxs-lookup"><span data-stu-id="95906-111">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="95906-112">Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST com a ID do [directoryRoleTemplate](directoryroletemplate.md) no qual a função directory se baseia.</span><span class="sxs-lookup"><span data-stu-id="95906-112">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="95906-113">[Liste modelos de função de diretório](../api/directoryroletemplate-list.md) para ter todas as outras funções de diretório disponíveis.</span><span class="sxs-lookup"><span data-stu-id="95906-113">[List directory role templates](../api/directoryroletemplate-list.md) to get all the other available directory roles.</span></span> <span data-ttu-id="95906-114">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="95906-114">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="95906-115">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="95906-115">This resource supports:</span></span>

- <span data-ttu-id="95906-116">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryrole-delta.md).</span><span class="sxs-lookup"><span data-stu-id="95906-116">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="95906-117">Métodos</span><span class="sxs-lookup"><span data-stu-id="95906-117">Methods</span></span>

| <span data-ttu-id="95906-118">Método</span><span class="sxs-lookup"><span data-stu-id="95906-118">Method</span></span>       | <span data-ttu-id="95906-119">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="95906-119">Return Type</span></span>  |<span data-ttu-id="95906-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="95906-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="95906-121">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="95906-121">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="95906-122">directoryRole</span><span class="sxs-lookup"><span data-stu-id="95906-122">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="95906-123">Leia as propriedades e os relacionamentos do objeto directoryRole.</span><span class="sxs-lookup"><span data-stu-id="95906-123">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="95906-124">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="95906-124">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="95906-125">Coleção [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="95906-125">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="95906-126">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="95906-126">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="95906-127">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="95906-127">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="95906-128">directoryObject</span><span class="sxs-lookup"><span data-stu-id="95906-128">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="95906-129">Adicione um usuário à função de diretório postando na propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="95906-129">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="95906-130">Listar membros</span><span class="sxs-lookup"><span data-stu-id="95906-130">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="95906-131">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="95906-131">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="95906-132">Obtenha os usuários que são membros da função directory da propriedade de navegação members.</span><span class="sxs-lookup"><span data-stu-id="95906-132">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="95906-133">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="95906-133">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="95906-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="95906-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="95906-135">Remova um usuário da função de diretório.</span><span class="sxs-lookup"><span data-stu-id="95906-135">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="95906-136">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="95906-136">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="95906-137">directoryRole</span><span class="sxs-lookup"><span data-stu-id="95906-137">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="95906-138">Ative uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="95906-138">Activate a directory role.</span></span>|
|[<span data-ttu-id="95906-139">delta</span><span class="sxs-lookup"><span data-stu-id="95906-139">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="95906-140">Coleção directoryRole</span><span class="sxs-lookup"><span data-stu-id="95906-140">directoryRole collection</span></span>| <span data-ttu-id="95906-141">Obtenha alterações incrementais para as funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="95906-141">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="95906-142">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95906-142">Properties</span></span>
| <span data-ttu-id="95906-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95906-143">Property</span></span>   | <span data-ttu-id="95906-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="95906-144">Type</span></span> | <span data-ttu-id="95906-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="95906-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="95906-146">description</span><span class="sxs-lookup"><span data-stu-id="95906-146">description</span></span>|<span data-ttu-id="95906-147">String</span><span class="sxs-lookup"><span data-stu-id="95906-147">String</span></span>|<span data-ttu-id="95906-p103">A descrição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="95906-p103">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="95906-150">displayName</span><span class="sxs-lookup"><span data-stu-id="95906-150">displayName</span></span>|<span data-ttu-id="95906-151">String</span><span class="sxs-lookup"><span data-stu-id="95906-151">String</span></span>|<span data-ttu-id="95906-p104">O nome de exibição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="95906-p104">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="95906-154">id</span><span class="sxs-lookup"><span data-stu-id="95906-154">id</span></span>|<span data-ttu-id="95906-155">String</span><span class="sxs-lookup"><span data-stu-id="95906-155">String</span></span>|<span data-ttu-id="95906-p105">O identificador exclusivo da função de diretório. Herdado de [directoryObject](directoryobject.md). Chave, Não Anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="95906-p105">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="95906-159">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="95906-159">roleTemplateId</span></span>|<span data-ttu-id="95906-160">String</span><span class="sxs-lookup"><span data-stu-id="95906-160">String</span></span>| <span data-ttu-id="95906-p106">A **id** do [directoryRoleTemplate](directoryroletemplate.md) em que esta função se baseia. A propriedade deve ser especificada ao ativar uma função de diretório em um locatário com uma operação POST. Depois que a função directory tiver sido ativada, a propriedade será somente leitura.</span><span class="sxs-lookup"><span data-stu-id="95906-p106">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="95906-164">Relações</span><span class="sxs-lookup"><span data-stu-id="95906-164">Relationships</span></span>
| <span data-ttu-id="95906-165">Relação</span><span class="sxs-lookup"><span data-stu-id="95906-165">Relationship</span></span> | <span data-ttu-id="95906-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="95906-166">Type</span></span> |<span data-ttu-id="95906-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="95906-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95906-168">membros</span><span class="sxs-lookup"><span data-stu-id="95906-168">members</span></span>|<span data-ttu-id="95906-169">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="95906-169">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="95906-p107">Usuários que são membros desta função de diretório. Métodos HTTP: GET, POST, DELETE. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="95906-p107">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95906-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95906-174">JSON representation</span></span>

<span data-ttu-id="95906-175">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="95906-175">Here is a JSON representation of the resource</span></span>

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
