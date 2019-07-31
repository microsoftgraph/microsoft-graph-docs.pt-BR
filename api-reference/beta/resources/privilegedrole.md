---
title: tipo de recurso privilegedRole
description: Representa uma função de administrador do Azure AD, como um **administrador global, administrador de cobrança, administrador de serviço, administrador de usuário, administrador de senha**, etc.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 98e5cd2c53b398339e8db65bec520a16f72d8f39
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965744"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="2d342-103">tipo de recurso privilegedRole</span><span class="sxs-lookup"><span data-stu-id="2d342-103">privilegedRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d342-104">Representa uma função de administrador do Azure AD, como um **administrador global, administrador de cobrança, administrador de serviço, administrador de usuário, administrador de senha**, etc.</span><span class="sxs-lookup"><span data-stu-id="2d342-104">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="2d342-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="2d342-105">Methods</span></span>

| <span data-ttu-id="2d342-106">Método</span><span class="sxs-lookup"><span data-stu-id="2d342-106">Method</span></span>           | <span data-ttu-id="2d342-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2d342-107">Return Type</span></span>    |<span data-ttu-id="2d342-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d342-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2d342-109">Listar objetos privilegedRole</span><span class="sxs-lookup"><span data-stu-id="2d342-109">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="2d342-110">[privilegedRole](privilegedrole.md) collection</span><span class="sxs-lookup"><span data-stu-id="2d342-110">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="2d342-111">Obtenha a coleção de privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="2d342-111">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="2d342-112">Get privilegedRole</span><span class="sxs-lookup"><span data-stu-id="2d342-112">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="2d342-113">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="2d342-113">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="2d342-114">Leia as propriedades e os relacionamentos do objeto privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="2d342-114">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="2d342-115">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="2d342-115">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="2d342-116">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="2d342-116">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="2d342-117">Obtenha uma coleção de objetos Assignment para essa função.</span><span class="sxs-lookup"><span data-stu-id="2d342-117">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="2d342-118">selfActivate</span><span class="sxs-lookup"><span data-stu-id="2d342-118">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="2d342-119">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="2d342-119">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="2d342-120">Ative a função atribuída.</span><span class="sxs-lookup"><span data-stu-id="2d342-120">Activate the assigned role.</span></span>|
|[<span data-ttu-id="2d342-121">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="2d342-121">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="2d342-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="2d342-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="2d342-123">Desative a função atribuída.</span><span class="sxs-lookup"><span data-stu-id="2d342-123">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="2d342-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d342-124">Properties</span></span>
| <span data-ttu-id="2d342-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d342-125">Property</span></span>     | <span data-ttu-id="2d342-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d342-126">Type</span></span>   |<span data-ttu-id="2d342-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d342-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d342-128">id</span><span class="sxs-lookup"><span data-stu-id="2d342-128">id</span></span>|<span data-ttu-id="2d342-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d342-129">string</span></span>|<span data-ttu-id="2d342-130">O identificador exclusivo para a função de administrador.</span><span class="sxs-lookup"><span data-stu-id="2d342-130">The unique identifier for administrator role.</span></span> <span data-ttu-id="2d342-131">É uma cadeia de caracteres GUID e tem o mesmo valor que a ID de modelo de função do Azure AD para a função determinada.</span><span class="sxs-lookup"><span data-stu-id="2d342-131">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="2d342-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2d342-132">Read-only.</span></span>|
|<span data-ttu-id="2d342-133">name</span><span class="sxs-lookup"><span data-stu-id="2d342-133">name</span></span>|<span data-ttu-id="2d342-134">string</span><span class="sxs-lookup"><span data-stu-id="2d342-134">string</span></span>|<span data-ttu-id="2d342-135">Nome da função.</span><span class="sxs-lookup"><span data-stu-id="2d342-135">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d342-136">Relações</span><span class="sxs-lookup"><span data-stu-id="2d342-136">Relationships</span></span>
| <span data-ttu-id="2d342-137">Relação</span><span class="sxs-lookup"><span data-stu-id="2d342-137">Relationship</span></span> | <span data-ttu-id="2d342-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d342-138">Type</span></span>   |<span data-ttu-id="2d342-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d342-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d342-140">assignments</span><span class="sxs-lookup"><span data-stu-id="2d342-140">assignments</span></span>|<span data-ttu-id="2d342-141">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="2d342-141">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="2d342-142">As atribuições para essa função.</span><span class="sxs-lookup"><span data-stu-id="2d342-142">The assignments for this role.</span></span> <span data-ttu-id="2d342-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2d342-143">Read-only.</span></span> <span data-ttu-id="2d342-144">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2d342-144">Nullable.</span></span>|
|<span data-ttu-id="2d342-145">settings</span><span class="sxs-lookup"><span data-stu-id="2d342-145">settings</span></span>|[<span data-ttu-id="2d342-146">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="2d342-146">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="2d342-147">As configurações dessa função.</span><span class="sxs-lookup"><span data-stu-id="2d342-147">The settings for this role.</span></span> <span data-ttu-id="2d342-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2d342-148">Read-only.</span></span> <span data-ttu-id="2d342-149">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2d342-149">Nullable.</span></span>|
|<span data-ttu-id="2d342-150">summary</span><span class="sxs-lookup"><span data-stu-id="2d342-150">summary</span></span>|[<span data-ttu-id="2d342-151">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="2d342-151">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="2d342-152">As informações resumidas para essa função.</span><span class="sxs-lookup"><span data-stu-id="2d342-152">The summary information for this role.</span></span> <span data-ttu-id="2d342-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2d342-153">Read-only.</span></span> <span data-ttu-id="2d342-154">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2d342-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d342-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d342-155">JSON representation</span></span>

<span data-ttu-id="2d342-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d342-156">Here is a JSON representation of the resource.</span></span>

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
