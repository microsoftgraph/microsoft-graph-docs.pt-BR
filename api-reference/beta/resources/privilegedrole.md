---
title: tipo de recurso privilegedRole
description: Representa uma função de administrador do Azure AD, como um **administrador global, administrador de cobrança, administrador de serviço, administrador de usuário, administrador de senha**, etc.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 51114eea797d27886f48c664d06d0b88d4a35a2d
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217908"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="2f117-103">tipo de recurso privilegedRole</span><span class="sxs-lookup"><span data-stu-id="2f117-103">privilegedRole resource type</span></span>

<span data-ttu-id="2f117-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f117-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f117-105">Representa uma função de administrador do Azure AD, como um **administrador global, administrador de cobrança, administrador de serviço, administrador de usuário, administrador de senha**, etc.</span><span class="sxs-lookup"><span data-stu-id="2f117-105">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="2f117-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2f117-106">Methods</span></span>

| <span data-ttu-id="2f117-107">Método</span><span class="sxs-lookup"><span data-stu-id="2f117-107">Method</span></span>           | <span data-ttu-id="2f117-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2f117-108">Return Type</span></span>    |<span data-ttu-id="2f117-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f117-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2f117-110">Listar objetos privilegedRole</span><span class="sxs-lookup"><span data-stu-id="2f117-110">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="2f117-111">[privilegedRole](privilegedrole.md) collection</span><span class="sxs-lookup"><span data-stu-id="2f117-111">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="2f117-112">Obtenha a coleção de privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="2f117-112">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="2f117-113">Get privilegedRole</span><span class="sxs-lookup"><span data-stu-id="2f117-113">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="2f117-114">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="2f117-114">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="2f117-115">Leia as propriedades e os relacionamentos do objeto privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="2f117-115">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="2f117-116">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="2f117-116">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="2f117-117">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="2f117-117">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="2f117-118">Obtenha uma coleção de objetos Assignment para essa função.</span><span class="sxs-lookup"><span data-stu-id="2f117-118">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="2f117-119">selfActivate</span><span class="sxs-lookup"><span data-stu-id="2f117-119">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="2f117-120">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="2f117-120">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="2f117-121">Ative a função atribuída.</span><span class="sxs-lookup"><span data-stu-id="2f117-121">Activate the assigned role.</span></span>|
|[<span data-ttu-id="2f117-122">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="2f117-122">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="2f117-123">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="2f117-123">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="2f117-124">Desative a função atribuída.</span><span class="sxs-lookup"><span data-stu-id="2f117-124">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="2f117-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2f117-125">Properties</span></span>
| <span data-ttu-id="2f117-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f117-126">Property</span></span>     | <span data-ttu-id="2f117-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f117-127">Type</span></span>   |<span data-ttu-id="2f117-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f117-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f117-129">id</span><span class="sxs-lookup"><span data-stu-id="2f117-129">id</span></span>|<span data-ttu-id="2f117-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f117-130">string</span></span>|<span data-ttu-id="2f117-131">O identificador exclusivo para a função de administrador.</span><span class="sxs-lookup"><span data-stu-id="2f117-131">The unique identifier for administrator role.</span></span> <span data-ttu-id="2f117-132">É uma cadeia de caracteres GUID e tem o mesmo valor que a ID de modelo de função do Azure AD para a função determinada.</span><span class="sxs-lookup"><span data-stu-id="2f117-132">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="2f117-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f117-133">Read-only.</span></span>|
|<span data-ttu-id="2f117-134">name</span><span class="sxs-lookup"><span data-stu-id="2f117-134">name</span></span>|<span data-ttu-id="2f117-135">string</span><span class="sxs-lookup"><span data-stu-id="2f117-135">string</span></span>|<span data-ttu-id="2f117-136">Nome da função.</span><span class="sxs-lookup"><span data-stu-id="2f117-136">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f117-137">Relações</span><span class="sxs-lookup"><span data-stu-id="2f117-137">Relationships</span></span>
| <span data-ttu-id="2f117-138">Relação</span><span class="sxs-lookup"><span data-stu-id="2f117-138">Relationship</span></span> | <span data-ttu-id="2f117-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f117-139">Type</span></span>   |<span data-ttu-id="2f117-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f117-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f117-141">assignments</span><span class="sxs-lookup"><span data-stu-id="2f117-141">assignments</span></span>|<span data-ttu-id="2f117-142">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="2f117-142">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="2f117-143">As atribuições para essa função.</span><span class="sxs-lookup"><span data-stu-id="2f117-143">The assignments for this role.</span></span> <span data-ttu-id="2f117-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f117-144">Read-only.</span></span> <span data-ttu-id="2f117-145">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f117-145">Nullable.</span></span>|
|<span data-ttu-id="2f117-146">settings</span><span class="sxs-lookup"><span data-stu-id="2f117-146">settings</span></span>|[<span data-ttu-id="2f117-147">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="2f117-147">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="2f117-148">As configurações dessa função.</span><span class="sxs-lookup"><span data-stu-id="2f117-148">The settings for this role.</span></span> <span data-ttu-id="2f117-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f117-149">Read-only.</span></span> <span data-ttu-id="2f117-150">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f117-150">Nullable.</span></span>|
|<span data-ttu-id="2f117-151">summary</span><span class="sxs-lookup"><span data-stu-id="2f117-151">summary</span></span>|[<span data-ttu-id="2f117-152">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="2f117-152">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="2f117-153">As informações resumidas para essa função.</span><span class="sxs-lookup"><span data-stu-id="2f117-153">The summary information for this role.</span></span> <span data-ttu-id="2f117-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f117-154">Read-only.</span></span> <span data-ttu-id="2f117-155">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f117-155">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f117-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2f117-156">JSON representation</span></span>

<span data-ttu-id="2f117-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2f117-157">Here is a JSON representation of the resource.</span></span>

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
