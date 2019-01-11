---
title: tipo de recurso de privilegedRole
description: 'Representa uma função de administrador do Azure AD, tais como: **Administrador Global, administrador de faturamento, administrador de serviço, administrador do usuário, senha de administrador**, etc.'
localization_priority: Normal
ms.openlocfilehash: 75763e18731cb969623cc4df6360d50abc018b41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860855"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="73bf9-103">tipo de recurso de privilegedRole</span><span class="sxs-lookup"><span data-stu-id="73bf9-103">privilegedRole resource type</span></span>

> <span data-ttu-id="73bf9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="73bf9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73bf9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="73bf9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73bf9-106">Representa uma função de administrador do Azure AD, tais como: **Administrador Global, administrador de faturamento, administrador de serviço, administrador do usuário, senha de administrador**, etc.</span><span class="sxs-lookup"><span data-stu-id="73bf9-106">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="73bf9-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="73bf9-107">Methods</span></span>

| <span data-ttu-id="73bf9-108">Método</span><span class="sxs-lookup"><span data-stu-id="73bf9-108">Method</span></span>           | <span data-ttu-id="73bf9-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="73bf9-109">Return Type</span></span>    |<span data-ttu-id="73bf9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="73bf9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="73bf9-111">Objetos de privilegedRole List</span><span class="sxs-lookup"><span data-stu-id="73bf9-111">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="73bf9-112">coleção [privilegedRole](privilegedrole.md)</span><span class="sxs-lookup"><span data-stu-id="73bf9-112">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="73bf9-113">Obtenha a coleção de privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="73bf9-113">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="73bf9-114">Obter privilegedRole</span><span class="sxs-lookup"><span data-stu-id="73bf9-114">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="73bf9-115">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="73bf9-115">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="73bf9-116">Leia as propriedades e os relacionamentos do objeto privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="73bf9-116">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="73bf9-117">Lista de atribuições</span><span class="sxs-lookup"><span data-stu-id="73bf9-117">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="73bf9-118">coleção [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="73bf9-118">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="73bf9-119">Obtenha uma coleção de objetos de atribuição para essa função.</span><span class="sxs-lookup"><span data-stu-id="73bf9-119">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="73bf9-120">selfActivate</span><span class="sxs-lookup"><span data-stu-id="73bf9-120">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="73bf9-121">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="73bf9-121">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="73bf9-122">Ative a função atribuída.</span><span class="sxs-lookup"><span data-stu-id="73bf9-122">Activate the assigned role.</span></span>|
|[<span data-ttu-id="73bf9-123">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="73bf9-123">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="73bf9-124">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="73bf9-124">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="73bf9-125">Desative a função atribuída.</span><span class="sxs-lookup"><span data-stu-id="73bf9-125">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="73bf9-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73bf9-126">Properties</span></span>
| <span data-ttu-id="73bf9-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73bf9-127">Property</span></span>     | <span data-ttu-id="73bf9-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="73bf9-128">Type</span></span>   |<span data-ttu-id="73bf9-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="73bf9-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73bf9-130">id</span><span class="sxs-lookup"><span data-stu-id="73bf9-130">id</span></span>|<span data-ttu-id="73bf9-131">string</span><span class="sxs-lookup"><span data-stu-id="73bf9-131">string</span></span>|<span data-ttu-id="73bf9-132">O identificador exclusivo para a função de administrador.</span><span class="sxs-lookup"><span data-stu-id="73bf9-132">The unique identifier for administrator role.</span></span> <span data-ttu-id="73bf9-133">É uma cadeia de caracteres GUID e tem o mesmo valor que a identificação do modelo de função do Azure AD para uma determinada função.</span><span class="sxs-lookup"><span data-stu-id="73bf9-133">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="73bf9-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73bf9-134">Read-only.</span></span>|
|<span data-ttu-id="73bf9-135">name</span><span class="sxs-lookup"><span data-stu-id="73bf9-135">name</span></span>|<span data-ttu-id="73bf9-136">string</span><span class="sxs-lookup"><span data-stu-id="73bf9-136">string</span></span>|<span data-ttu-id="73bf9-137">Nome da função.</span><span class="sxs-lookup"><span data-stu-id="73bf9-137">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73bf9-138">Relações</span><span class="sxs-lookup"><span data-stu-id="73bf9-138">Relationships</span></span>
| <span data-ttu-id="73bf9-139">Relação</span><span class="sxs-lookup"><span data-stu-id="73bf9-139">Relationship</span></span> | <span data-ttu-id="73bf9-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="73bf9-140">Type</span></span>   |<span data-ttu-id="73bf9-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="73bf9-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73bf9-142">assignments</span><span class="sxs-lookup"><span data-stu-id="73bf9-142">assignments</span></span>|<span data-ttu-id="73bf9-143">coleção [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="73bf9-143">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="73bf9-144">As atribuições para essa função.</span><span class="sxs-lookup"><span data-stu-id="73bf9-144">The assignments for this role.</span></span> <span data-ttu-id="73bf9-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73bf9-145">Read-only.</span></span> <span data-ttu-id="73bf9-146">Anulável.</span><span class="sxs-lookup"><span data-stu-id="73bf9-146">Nullable.</span></span>|
|<span data-ttu-id="73bf9-147">configurações</span><span class="sxs-lookup"><span data-stu-id="73bf9-147">settings</span></span>|[<span data-ttu-id="73bf9-148">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="73bf9-148">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="73bf9-149">As configurações para essa função.</span><span class="sxs-lookup"><span data-stu-id="73bf9-149">The settings for this role.</span></span> <span data-ttu-id="73bf9-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73bf9-150">Read-only.</span></span> <span data-ttu-id="73bf9-151">Anulável.</span><span class="sxs-lookup"><span data-stu-id="73bf9-151">Nullable.</span></span>|
|<span data-ttu-id="73bf9-152">Resumo</span><span class="sxs-lookup"><span data-stu-id="73bf9-152">summary</span></span>|[<span data-ttu-id="73bf9-153">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="73bf9-153">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="73bf9-154">As informações de resumo para essa função.</span><span class="sxs-lookup"><span data-stu-id="73bf9-154">The summary information for this role.</span></span> <span data-ttu-id="73bf9-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73bf9-155">Read-only.</span></span> <span data-ttu-id="73bf9-156">Anulável.</span><span class="sxs-lookup"><span data-stu-id="73bf9-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73bf9-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73bf9-157">JSON representation</span></span>

<span data-ttu-id="73bf9-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73bf9-158">Here is a JSON representation of the resource.</span></span>

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
