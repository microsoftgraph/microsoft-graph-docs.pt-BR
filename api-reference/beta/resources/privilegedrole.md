---
title: tipo de recurso de privilegedRole
description: 'Representa uma função de administrador do Azure AD, tais como: **Administrador Global, administrador de faturamento, administrador de serviço, administrador do usuário, senha de administrador**, etc.'
ms.openlocfilehash: 0c04ab9de13732e4ac9eecb943a10945bec59d02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034077"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="360a5-103">tipo de recurso de privilegedRole</span><span class="sxs-lookup"><span data-stu-id="360a5-103">privilegedRole resource type</span></span>

> <span data-ttu-id="360a5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="360a5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="360a5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="360a5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="360a5-106">Representa uma função de administrador do Azure AD, tais como: **Administrador Global, administrador de faturamento, administrador de serviço, administrador do usuário, senha de administrador**, etc.</span><span class="sxs-lookup"><span data-stu-id="360a5-106">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="360a5-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="360a5-107">Methods</span></span>

| <span data-ttu-id="360a5-108">Método</span><span class="sxs-lookup"><span data-stu-id="360a5-108">Method</span></span>           | <span data-ttu-id="360a5-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="360a5-109">Return Type</span></span>    |<span data-ttu-id="360a5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="360a5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="360a5-111">Objetos de privilegedRole List</span><span class="sxs-lookup"><span data-stu-id="360a5-111">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="360a5-112">coleção [privilegedRole](privilegedrole.md)</span><span class="sxs-lookup"><span data-stu-id="360a5-112">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="360a5-113">Obtenha a coleção de privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="360a5-113">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="360a5-114">Obter privilegedRole</span><span class="sxs-lookup"><span data-stu-id="360a5-114">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="360a5-115">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="360a5-115">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="360a5-116">Leia as propriedades e os relacionamentos do objeto privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="360a5-116">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="360a5-117">Lista de atribuições</span><span class="sxs-lookup"><span data-stu-id="360a5-117">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="360a5-118">coleção [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="360a5-118">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="360a5-119">Obtenha uma coleção de objetos de atribuição para essa função.</span><span class="sxs-lookup"><span data-stu-id="360a5-119">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="360a5-120">selfActivate</span><span class="sxs-lookup"><span data-stu-id="360a5-120">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="360a5-121">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="360a5-121">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="360a5-122">Ative a função atribuída.</span><span class="sxs-lookup"><span data-stu-id="360a5-122">Activate the assigned role.</span></span>|
|[<span data-ttu-id="360a5-123">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="360a5-123">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="360a5-124">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="360a5-124">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="360a5-125">Desative a função atribuída.</span><span class="sxs-lookup"><span data-stu-id="360a5-125">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="360a5-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="360a5-126">Properties</span></span>
| <span data-ttu-id="360a5-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="360a5-127">Property</span></span>     | <span data-ttu-id="360a5-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="360a5-128">Type</span></span>   |<span data-ttu-id="360a5-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="360a5-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="360a5-130">id</span><span class="sxs-lookup"><span data-stu-id="360a5-130">id</span></span>|<span data-ttu-id="360a5-131">string</span><span class="sxs-lookup"><span data-stu-id="360a5-131">string</span></span>|<span data-ttu-id="360a5-132">O identificador exclusivo para a função de administrador.</span><span class="sxs-lookup"><span data-stu-id="360a5-132">The unique identifier for administrator role.</span></span> <span data-ttu-id="360a5-133">É uma cadeia de caracteres GUID e tem o mesmo valor que a identificação do modelo de função do Azure AD para uma determinada função.</span><span class="sxs-lookup"><span data-stu-id="360a5-133">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="360a5-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="360a5-134">Read-only.</span></span>|
|<span data-ttu-id="360a5-135">name</span><span class="sxs-lookup"><span data-stu-id="360a5-135">name</span></span>|<span data-ttu-id="360a5-136">string</span><span class="sxs-lookup"><span data-stu-id="360a5-136">string</span></span>|<span data-ttu-id="360a5-137">Nome da função.</span><span class="sxs-lookup"><span data-stu-id="360a5-137">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="360a5-138">Relações</span><span class="sxs-lookup"><span data-stu-id="360a5-138">Relationships</span></span>
| <span data-ttu-id="360a5-139">Relação</span><span class="sxs-lookup"><span data-stu-id="360a5-139">Relationship</span></span> | <span data-ttu-id="360a5-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="360a5-140">Type</span></span>   |<span data-ttu-id="360a5-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="360a5-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="360a5-142">assignments</span><span class="sxs-lookup"><span data-stu-id="360a5-142">assignments</span></span>|<span data-ttu-id="360a5-143">coleção [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="360a5-143">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="360a5-144">As atribuições para essa função.</span><span class="sxs-lookup"><span data-stu-id="360a5-144">The assignments for this role.</span></span> <span data-ttu-id="360a5-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="360a5-145">Read-only.</span></span> <span data-ttu-id="360a5-146">Anulável.</span><span class="sxs-lookup"><span data-stu-id="360a5-146">Nullable.</span></span>|
|<span data-ttu-id="360a5-147">configurações</span><span class="sxs-lookup"><span data-stu-id="360a5-147">settings</span></span>|[<span data-ttu-id="360a5-148">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="360a5-148">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="360a5-149">As configurações para essa função.</span><span class="sxs-lookup"><span data-stu-id="360a5-149">The settings for this role.</span></span> <span data-ttu-id="360a5-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="360a5-150">Read-only.</span></span> <span data-ttu-id="360a5-151">Anulável.</span><span class="sxs-lookup"><span data-stu-id="360a5-151">Nullable.</span></span>|
|<span data-ttu-id="360a5-152">Resumo</span><span class="sxs-lookup"><span data-stu-id="360a5-152">summary</span></span>|[<span data-ttu-id="360a5-153">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="360a5-153">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="360a5-154">As informações de resumo para essa função.</span><span class="sxs-lookup"><span data-stu-id="360a5-154">The summary information for this role.</span></span> <span data-ttu-id="360a5-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="360a5-155">Read-only.</span></span> <span data-ttu-id="360a5-156">Anulável.</span><span class="sxs-lookup"><span data-stu-id="360a5-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="360a5-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="360a5-157">JSON representation</span></span>

<span data-ttu-id="360a5-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="360a5-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->