---
title: tipo de recurso directoryRole
description: Representa uma função do diretório do Azure AD. As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*.
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d9b500e3f5a3768dd345d1e7e8df41c63b1aa54b
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450673"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="9bd4f-104">tipo de recurso directoryRole</span><span class="sxs-lookup"><span data-stu-id="9bd4f-104">directoryRole resource type</span></span>

<span data-ttu-id="9bd4f-105">Representa uma função do diretório do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-105">Represents an Azure AD directory role.</span></span> <span data-ttu-id="9bd4f-106">As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-106">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="9bd4f-107">Para obter mais informações sobre funções de diretório (administrador), confira [Atribuindo funções de administrador no Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="9bd4f-107">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="9bd4f-108">Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder a eles as permissões da função de destino.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-108">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="9bd4f-109">Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-109">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="9bd4f-110">Apenas a função de diretório Administradores de Empresa é ativada por padrão.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-110">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="9bd4f-111">Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST com a ID do [directoryRoleTemplate](directoryroletemplate.md) no qual a função directory se baseia.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-111">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="9bd4f-112">[Liste modelos de função de diretório](../api/directoryroletemplate-list.md) para ter todas as outras funções de diretório disponíveis.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-112">[List directory role templates](../api/directoryroletemplate-list.md) to get all the other available directory roles.</span></span> <span data-ttu-id="9bd4f-113">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="9bd4f-113">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="9bd4f-114">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="9bd4f-114">This resource supports:</span></span>

- <span data-ttu-id="9bd4f-115">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryrole-delta.md).</span><span class="sxs-lookup"><span data-stu-id="9bd4f-115">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="9bd4f-116">Métodos</span><span class="sxs-lookup"><span data-stu-id="9bd4f-116">Methods</span></span>

| <span data-ttu-id="9bd4f-117">Método</span><span class="sxs-lookup"><span data-stu-id="9bd4f-117">Method</span></span>       | <span data-ttu-id="9bd4f-118">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9bd4f-118">Return Type</span></span>  |<span data-ttu-id="9bd4f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bd4f-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9bd4f-120">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="9bd4f-120">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="9bd4f-121">directoryRole</span><span class="sxs-lookup"><span data-stu-id="9bd4f-121">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="9bd4f-122">Leia as propriedades e os relacionamentos do objeto directoryRole.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-122">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="9bd4f-123">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="9bd4f-123">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="9bd4f-124">Coleção [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="9bd4f-124">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="9bd4f-125">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-125">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="9bd4f-126">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="9bd4f-126">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="9bd4f-127">directoryObject</span><span class="sxs-lookup"><span data-stu-id="9bd4f-127">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="9bd4f-128">Adicione um usuário à função de diretório postando na propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-128">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="9bd4f-129">Listar membros</span><span class="sxs-lookup"><span data-stu-id="9bd4f-129">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="9bd4f-130">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="9bd4f-130">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="9bd4f-131">Obtenha os usuários que são membros da função directory da propriedade de navegação members.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-131">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="9bd4f-132">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="9bd4f-132">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="9bd4f-133">directoryObject</span><span class="sxs-lookup"><span data-stu-id="9bd4f-133">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="9bd4f-134">Remova um usuário da função de diretório.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-134">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="9bd4f-135">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="9bd4f-135">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="9bd4f-136">directoryRole</span><span class="sxs-lookup"><span data-stu-id="9bd4f-136">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="9bd4f-137">Ative uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-137">Activate a directory role.</span></span>|
|[<span data-ttu-id="9bd4f-138">delta</span><span class="sxs-lookup"><span data-stu-id="9bd4f-138">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="9bd4f-139">Coleção directoryRole</span><span class="sxs-lookup"><span data-stu-id="9bd4f-139">directoryRole collection</span></span>| <span data-ttu-id="9bd4f-140">Obtenha alterações incrementais para as funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-140">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="9bd4f-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9bd4f-141">Properties</span></span>
| <span data-ttu-id="9bd4f-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bd4f-142">Property</span></span>   | <span data-ttu-id="9bd4f-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bd4f-143">Type</span></span> | <span data-ttu-id="9bd4f-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bd4f-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9bd4f-145">description</span><span class="sxs-lookup"><span data-stu-id="9bd4f-145">description</span></span>|<span data-ttu-id="9bd4f-146">String</span><span class="sxs-lookup"><span data-stu-id="9bd4f-146">String</span></span>|<span data-ttu-id="9bd4f-p103">A descrição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-p103">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="9bd4f-149">displayName</span><span class="sxs-lookup"><span data-stu-id="9bd4f-149">displayName</span></span>|<span data-ttu-id="9bd4f-150">String</span><span class="sxs-lookup"><span data-stu-id="9bd4f-150">String</span></span>|<span data-ttu-id="9bd4f-p104">O nome de exibição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-p104">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="9bd4f-153">id</span><span class="sxs-lookup"><span data-stu-id="9bd4f-153">id</span></span>|<span data-ttu-id="9bd4f-154">String</span><span class="sxs-lookup"><span data-stu-id="9bd4f-154">String</span></span>|<span data-ttu-id="9bd4f-p105">O identificador exclusivo da função de diretório. Herdado de [directoryObject](directoryobject.md). Chave, Não Anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-p105">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="9bd4f-158">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="9bd4f-158">roleTemplateId</span></span>|<span data-ttu-id="9bd4f-159">String</span><span class="sxs-lookup"><span data-stu-id="9bd4f-159">String</span></span>| <span data-ttu-id="9bd4f-p106">A **id** do [directoryRoleTemplate](directoryroletemplate.md) em que esta função se baseia. A propriedade deve ser especificada ao ativar uma função de diretório em um locatário com uma operação POST. Depois que a função directory tiver sido ativada, a propriedade será somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-p106">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9bd4f-163">Relações</span><span class="sxs-lookup"><span data-stu-id="9bd4f-163">Relationships</span></span>
| <span data-ttu-id="9bd4f-164">Relação</span><span class="sxs-lookup"><span data-stu-id="9bd4f-164">Relationship</span></span> | <span data-ttu-id="9bd4f-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bd4f-165">Type</span></span> |<span data-ttu-id="9bd4f-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bd4f-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bd4f-167">membros</span><span class="sxs-lookup"><span data-stu-id="9bd4f-167">members</span></span>|<span data-ttu-id="9bd4f-168">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="9bd4f-168">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="9bd4f-p107">Usuários que são membros desta função de diretório. Métodos HTTP: GET, POST, DELETE. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="9bd4f-p107">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9bd4f-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9bd4f-173">JSON representation</span></span>

<span data-ttu-id="9bd4f-174">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9bd4f-174">Here is a JSON representation of the resource</span></span>

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
