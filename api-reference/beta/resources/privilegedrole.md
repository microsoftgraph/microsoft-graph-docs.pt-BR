---
title: tipo de recurso de privilegedRole
description: 'Representa uma função de administrador do Azure AD, tais como: **Administrador Global, administrador de faturamento, administrador de serviço, administrador do usuário, senha de administrador**, etc.'
localization_priority: Normal
ms.openlocfilehash: 131999f52a583400b018e98d2319118f69ca87e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513743"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="b22cb-103">tipo de recurso de privilegedRole</span><span class="sxs-lookup"><span data-stu-id="b22cb-103">privilegedRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b22cb-104">Representa uma função de administrador do Azure AD, tais como: **Administrador Global, administrador de faturamento, administrador de serviço, administrador do usuário, senha de administrador**, etc.</span><span class="sxs-lookup"><span data-stu-id="b22cb-104">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="b22cb-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="b22cb-105">Methods</span></span>

| <span data-ttu-id="b22cb-106">Método</span><span class="sxs-lookup"><span data-stu-id="b22cb-106">Method</span></span>           | <span data-ttu-id="b22cb-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b22cb-107">Return Type</span></span>    |<span data-ttu-id="b22cb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b22cb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b22cb-109">Objetos de privilegedRole List</span><span class="sxs-lookup"><span data-stu-id="b22cb-109">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="b22cb-110">coleção [privilegedRole](privilegedrole.md)</span><span class="sxs-lookup"><span data-stu-id="b22cb-110">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="b22cb-111">Obtenha a coleção de privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="b22cb-111">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="b22cb-112">Obter privilegedRole</span><span class="sxs-lookup"><span data-stu-id="b22cb-112">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="b22cb-113">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="b22cb-113">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="b22cb-114">Leia as propriedades e os relacionamentos do objeto privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="b22cb-114">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="b22cb-115">Lista de atribuições</span><span class="sxs-lookup"><span data-stu-id="b22cb-115">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="b22cb-116">coleção [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b22cb-116">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="b22cb-117">Obtenha uma coleção de objetos de atribuição para essa função.</span><span class="sxs-lookup"><span data-stu-id="b22cb-117">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="b22cb-118">selfActivate</span><span class="sxs-lookup"><span data-stu-id="b22cb-118">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="b22cb-119">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b22cb-119">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="b22cb-120">Ative a função atribuída.</span><span class="sxs-lookup"><span data-stu-id="b22cb-120">Activate the assigned role.</span></span>|
|[<span data-ttu-id="b22cb-121">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="b22cb-121">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="b22cb-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b22cb-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="b22cb-123">Desative a função atribuída.</span><span class="sxs-lookup"><span data-stu-id="b22cb-123">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="b22cb-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b22cb-124">Properties</span></span>
| <span data-ttu-id="b22cb-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b22cb-125">Property</span></span>     | <span data-ttu-id="b22cb-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="b22cb-126">Type</span></span>   |<span data-ttu-id="b22cb-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="b22cb-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b22cb-128">id</span><span class="sxs-lookup"><span data-stu-id="b22cb-128">id</span></span>|<span data-ttu-id="b22cb-129">string</span><span class="sxs-lookup"><span data-stu-id="b22cb-129">string</span></span>|<span data-ttu-id="b22cb-130">O identificador exclusivo para a função de administrador.</span><span class="sxs-lookup"><span data-stu-id="b22cb-130">The unique identifier for administrator role.</span></span> <span data-ttu-id="b22cb-131">É uma cadeia de caracteres GUID e tem o mesmo valor que a identificação do modelo de função do Azure AD para uma determinada função.</span><span class="sxs-lookup"><span data-stu-id="b22cb-131">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="b22cb-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b22cb-132">Read-only.</span></span>|
|<span data-ttu-id="b22cb-133">name</span><span class="sxs-lookup"><span data-stu-id="b22cb-133">name</span></span>|<span data-ttu-id="b22cb-134">string</span><span class="sxs-lookup"><span data-stu-id="b22cb-134">string</span></span>|<span data-ttu-id="b22cb-135">Nome da função.</span><span class="sxs-lookup"><span data-stu-id="b22cb-135">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b22cb-136">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="b22cb-136">Relationships</span></span>
| <span data-ttu-id="b22cb-137">Relação</span><span class="sxs-lookup"><span data-stu-id="b22cb-137">Relationship</span></span> | <span data-ttu-id="b22cb-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="b22cb-138">Type</span></span>   |<span data-ttu-id="b22cb-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="b22cb-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b22cb-140">assignments</span><span class="sxs-lookup"><span data-stu-id="b22cb-140">assignments</span></span>|<span data-ttu-id="b22cb-141">coleção [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b22cb-141">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="b22cb-142">As atribuições para essa função.</span><span class="sxs-lookup"><span data-stu-id="b22cb-142">The assignments for this role.</span></span> <span data-ttu-id="b22cb-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b22cb-143">Read-only.</span></span> <span data-ttu-id="b22cb-144">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b22cb-144">Nullable.</span></span>|
|<span data-ttu-id="b22cb-145">configurações</span><span class="sxs-lookup"><span data-stu-id="b22cb-145">settings</span></span>|[<span data-ttu-id="b22cb-146">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="b22cb-146">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="b22cb-147">As configurações para essa função.</span><span class="sxs-lookup"><span data-stu-id="b22cb-147">The settings for this role.</span></span> <span data-ttu-id="b22cb-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b22cb-148">Read-only.</span></span> <span data-ttu-id="b22cb-149">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b22cb-149">Nullable.</span></span>|
|<span data-ttu-id="b22cb-150">Resumo</span><span class="sxs-lookup"><span data-stu-id="b22cb-150">summary</span></span>|[<span data-ttu-id="b22cb-151">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="b22cb-151">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="b22cb-152">As informações de resumo para essa função.</span><span class="sxs-lookup"><span data-stu-id="b22cb-152">The summary information for this role.</span></span> <span data-ttu-id="b22cb-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b22cb-153">Read-only.</span></span> <span data-ttu-id="b22cb-154">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b22cb-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b22cb-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b22cb-155">JSON representation</span></span>

<span data-ttu-id="b22cb-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b22cb-156">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
