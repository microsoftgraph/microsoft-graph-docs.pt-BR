---
title: tipo de recurso privilegedRole
description: Representa uma função de administrador do Azure AD, como um **administrador global, administrador de cobrança, administrador de serviço, administrador de usuário, administrador de senha**, etc.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 3d0b24022696fbb0df861ce0c2a78e0c9bbbd6e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070517"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="f3ffa-103">tipo de recurso privilegedRole</span><span class="sxs-lookup"><span data-stu-id="f3ffa-103">privilegedRole resource type</span></span>

<span data-ttu-id="f3ffa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3ffa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3ffa-105">Representa uma função de administrador do Azure AD, como um **administrador global, administrador de cobrança, administrador de serviço, administrador de usuário, administrador de senha**, etc.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-105">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="f3ffa-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f3ffa-106">Methods</span></span>

| <span data-ttu-id="f3ffa-107">Método</span><span class="sxs-lookup"><span data-stu-id="f3ffa-107">Method</span></span>           | <span data-ttu-id="f3ffa-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f3ffa-108">Return Type</span></span>    |<span data-ttu-id="f3ffa-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3ffa-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f3ffa-110">Listar objetos privilegedRole</span><span class="sxs-lookup"><span data-stu-id="f3ffa-110">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="f3ffa-111">[privilegedRole](privilegedrole.md) collection</span><span class="sxs-lookup"><span data-stu-id="f3ffa-111">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="f3ffa-112">Obtenha a coleção de privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-112">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="f3ffa-113">Get privilegedRole</span><span class="sxs-lookup"><span data-stu-id="f3ffa-113">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="f3ffa-114">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="f3ffa-114">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="f3ffa-115">Leia as propriedades e os relacionamentos do objeto privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-115">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="f3ffa-116">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="f3ffa-116">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="f3ffa-117">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="f3ffa-117">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="f3ffa-118">Obtenha uma coleção de objetos Assignment para essa função.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-118">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="f3ffa-119">selfActivate</span><span class="sxs-lookup"><span data-stu-id="f3ffa-119">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="f3ffa-120">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f3ffa-120">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="f3ffa-121">Ative a função atribuída.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-121">Activate the assigned role.</span></span>|
|[<span data-ttu-id="f3ffa-122">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="f3ffa-122">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="f3ffa-123">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f3ffa-123">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="f3ffa-124">Desative a função atribuída.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-124">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="f3ffa-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3ffa-125">Properties</span></span>
| <span data-ttu-id="f3ffa-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3ffa-126">Property</span></span>     | <span data-ttu-id="f3ffa-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3ffa-127">Type</span></span>   |<span data-ttu-id="f3ffa-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3ffa-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3ffa-129">id</span><span class="sxs-lookup"><span data-stu-id="f3ffa-129">id</span></span>|<span data-ttu-id="f3ffa-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3ffa-130">string</span></span>|<span data-ttu-id="f3ffa-131">O identificador exclusivo para a função de administrador.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-131">The unique identifier for administrator role.</span></span> <span data-ttu-id="f3ffa-132">É uma cadeia de caracteres GUID e tem o mesmo valor que a ID de modelo de função do Azure AD para a função determinada.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-132">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="f3ffa-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-133">Read-only.</span></span>|
|<span data-ttu-id="f3ffa-134">name</span><span class="sxs-lookup"><span data-stu-id="f3ffa-134">name</span></span>|<span data-ttu-id="f3ffa-135">string</span><span class="sxs-lookup"><span data-stu-id="f3ffa-135">string</span></span>|<span data-ttu-id="f3ffa-136">Nome da função.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-136">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3ffa-137">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="f3ffa-137">Relationships</span></span>
| <span data-ttu-id="f3ffa-138">Relação</span><span class="sxs-lookup"><span data-stu-id="f3ffa-138">Relationship</span></span> | <span data-ttu-id="f3ffa-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3ffa-139">Type</span></span>   |<span data-ttu-id="f3ffa-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3ffa-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3ffa-141">assignments</span><span class="sxs-lookup"><span data-stu-id="f3ffa-141">assignments</span></span>|<span data-ttu-id="f3ffa-142">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="f3ffa-142">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="f3ffa-143">As atribuições para essa função.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-143">The assignments for this role.</span></span> <span data-ttu-id="f3ffa-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-144">Read-only.</span></span> <span data-ttu-id="f3ffa-145">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-145">Nullable.</span></span>|
|<span data-ttu-id="f3ffa-146">settings</span><span class="sxs-lookup"><span data-stu-id="f3ffa-146">settings</span></span>|[<span data-ttu-id="f3ffa-147">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="f3ffa-147">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="f3ffa-148">As configurações dessa função.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-148">The settings for this role.</span></span> <span data-ttu-id="f3ffa-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-149">Read-only.</span></span> <span data-ttu-id="f3ffa-150">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-150">Nullable.</span></span>|
|<span data-ttu-id="f3ffa-151">summary</span><span class="sxs-lookup"><span data-stu-id="f3ffa-151">summary</span></span>|[<span data-ttu-id="f3ffa-152">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="f3ffa-152">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="f3ffa-153">As informações resumidas para essa função.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-153">The summary information for this role.</span></span> <span data-ttu-id="f3ffa-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-154">Read-only.</span></span> <span data-ttu-id="f3ffa-155">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-155">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f3ffa-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3ffa-156">JSON representation</span></span>

<span data-ttu-id="f3ffa-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3ffa-157">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedRole"
}-->

```json
{
  "id": "string (identifier)",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


