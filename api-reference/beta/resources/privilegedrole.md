---
title: Tipo de recurso privilegedRole
description: 'Representa uma função de administrador do Azure AD, como: **Administrador Global,** Administrador de Cobrança, Administrador de Serviço, Administrador de Usuário, Administrador de Senha etc.'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 4eca2f1a3d9de4fa7f625cd6b559b5a0c9c03916
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444011"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="c43a6-103">Tipo de recurso privilegedRole</span><span class="sxs-lookup"><span data-stu-id="c43a6-103">privilegedRole resource type</span></span>

<span data-ttu-id="c43a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c43a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c43a6-105">Representa uma função de administrador do Azure AD, como: **Administrador Global,** Administrador de Cobrança, Administrador de Serviço, Administrador de Usuário, Administrador de Senha etc.</span><span class="sxs-lookup"><span data-stu-id="c43a6-105">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="c43a6-106">Methods</span><span class="sxs-lookup"><span data-stu-id="c43a6-106">Methods</span></span>

| <span data-ttu-id="c43a6-107">Método</span><span class="sxs-lookup"><span data-stu-id="c43a6-107">Method</span></span>           | <span data-ttu-id="c43a6-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c43a6-108">Return Type</span></span>    |<span data-ttu-id="c43a6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c43a6-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c43a6-110">Listar objetos privilegedRole</span><span class="sxs-lookup"><span data-stu-id="c43a6-110">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="c43a6-111">[privilegedRole](privilegedrole.md) collection</span><span class="sxs-lookup"><span data-stu-id="c43a6-111">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="c43a6-112">Obter a coleção privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="c43a6-112">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="c43a6-113">Get privilegedRole</span><span class="sxs-lookup"><span data-stu-id="c43a6-113">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="c43a6-114">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="c43a6-114">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="c43a6-115">Ler propriedades e relações do objeto privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="c43a6-115">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="c43a6-116">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="c43a6-116">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="c43a6-117">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="c43a6-117">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="c43a6-118">Obter uma coleção de objetos de atribuição para essa função.</span><span class="sxs-lookup"><span data-stu-id="c43a6-118">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="c43a6-119">selfActivate</span><span class="sxs-lookup"><span data-stu-id="c43a6-119">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="c43a6-120">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c43a6-120">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="c43a6-121">Ative a função atribuída.</span><span class="sxs-lookup"><span data-stu-id="c43a6-121">Activate the assigned role.</span></span>|
|[<span data-ttu-id="c43a6-122">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="c43a6-122">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="c43a6-123">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c43a6-123">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="c43a6-124">Desative a função atribuída.</span><span class="sxs-lookup"><span data-stu-id="c43a6-124">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="c43a6-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c43a6-125">Properties</span></span>
| <span data-ttu-id="c43a6-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c43a6-126">Property</span></span>     | <span data-ttu-id="c43a6-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="c43a6-127">Type</span></span>   |<span data-ttu-id="c43a6-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="c43a6-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c43a6-129">id</span><span class="sxs-lookup"><span data-stu-id="c43a6-129">id</span></span>|<span data-ttu-id="c43a6-130">string</span><span class="sxs-lookup"><span data-stu-id="c43a6-130">string</span></span>|<span data-ttu-id="c43a6-131">O identificador exclusivo da função de administrador.</span><span class="sxs-lookup"><span data-stu-id="c43a6-131">The unique identifier for administrator role.</span></span> <span data-ttu-id="c43a6-132">É uma cadeia de caracteres GUID e tem o mesmo valor que a id do modelo de função do Azure AD para a função determinada.</span><span class="sxs-lookup"><span data-stu-id="c43a6-132">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="c43a6-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c43a6-133">Read-only.</span></span>|
|<span data-ttu-id="c43a6-134">name</span><span class="sxs-lookup"><span data-stu-id="c43a6-134">name</span></span>|<span data-ttu-id="c43a6-135">string</span><span class="sxs-lookup"><span data-stu-id="c43a6-135">string</span></span>|<span data-ttu-id="c43a6-136">Nome da função.</span><span class="sxs-lookup"><span data-stu-id="c43a6-136">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c43a6-137">Relações</span><span class="sxs-lookup"><span data-stu-id="c43a6-137">Relationships</span></span>
| <span data-ttu-id="c43a6-138">Relação</span><span class="sxs-lookup"><span data-stu-id="c43a6-138">Relationship</span></span> | <span data-ttu-id="c43a6-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="c43a6-139">Type</span></span>   |<span data-ttu-id="c43a6-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="c43a6-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c43a6-141">assignments</span><span class="sxs-lookup"><span data-stu-id="c43a6-141">assignments</span></span>|<span data-ttu-id="c43a6-142">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="c43a6-142">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="c43a6-143">As atribuições dessa função.</span><span class="sxs-lookup"><span data-stu-id="c43a6-143">The assignments for this role.</span></span> <span data-ttu-id="c43a6-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c43a6-144">Read-only.</span></span> <span data-ttu-id="c43a6-145">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c43a6-145">Nullable.</span></span>|
|<span data-ttu-id="c43a6-146">settings</span><span class="sxs-lookup"><span data-stu-id="c43a6-146">settings</span></span>|[<span data-ttu-id="c43a6-147">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="c43a6-147">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="c43a6-148">As configurações dessa função.</span><span class="sxs-lookup"><span data-stu-id="c43a6-148">The settings for this role.</span></span> <span data-ttu-id="c43a6-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c43a6-149">Read-only.</span></span> <span data-ttu-id="c43a6-150">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c43a6-150">Nullable.</span></span>|
|<span data-ttu-id="c43a6-151">summary</span><span class="sxs-lookup"><span data-stu-id="c43a6-151">summary</span></span>|[<span data-ttu-id="c43a6-152">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="c43a6-152">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="c43a6-153">As informações resumidas para essa função.</span><span class="sxs-lookup"><span data-stu-id="c43a6-153">The summary information for this role.</span></span> <span data-ttu-id="c43a6-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c43a6-154">Read-only.</span></span> <span data-ttu-id="c43a6-155">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c43a6-155">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c43a6-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c43a6-156">JSON representation</span></span>

<span data-ttu-id="c43a6-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c43a6-157">Here is a JSON representation of the resource.</span></span>

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


