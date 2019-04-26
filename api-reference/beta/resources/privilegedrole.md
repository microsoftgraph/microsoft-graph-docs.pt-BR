---
title: tipo de recurso privilegedRole
description: Representa uma função de administrador do Azure AD, como um **administrador global, administrador de cobrança, administrador de serviço, administrador de usuário, administrador de senha**, etc.
localization_priority: Normal
ms.openlocfilehash: 131999f52a583400b018e98d2319118f69ca87e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563378"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="4d7b8-103">tipo de recurso privilegedRole</span><span class="sxs-lookup"><span data-stu-id="4d7b8-103">privilegedRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d7b8-104">Representa uma função de administrador do Azure AD, como um **administrador global, administrador de cobrança, administrador de serviço, administrador de usuário, administrador de senha**, etc.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-104">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="4d7b8-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="4d7b8-105">Methods</span></span>

| <span data-ttu-id="4d7b8-106">Método</span><span class="sxs-lookup"><span data-stu-id="4d7b8-106">Method</span></span>           | <span data-ttu-id="4d7b8-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4d7b8-107">Return Type</span></span>    |<span data-ttu-id="4d7b8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d7b8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4d7b8-109">Listar objetos privilegedRole</span><span class="sxs-lookup"><span data-stu-id="4d7b8-109">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="4d7b8-110">[privilegedRole](privilegedrole.md) collection</span><span class="sxs-lookup"><span data-stu-id="4d7b8-110">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="4d7b8-111">Obtenha a coleção de privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-111">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="4d7b8-112">Get privilegedRole</span><span class="sxs-lookup"><span data-stu-id="4d7b8-112">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="4d7b8-113">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="4d7b8-113">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="4d7b8-114">Leia as propriedades e os relacionamentos do objeto privilegedRole.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-114">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="4d7b8-115">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="4d7b8-115">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="4d7b8-116">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="4d7b8-116">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="4d7b8-117">Obtenha uma coleção de objetos Assignment para essa função.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-117">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="4d7b8-118">selfActivate</span><span class="sxs-lookup"><span data-stu-id="4d7b8-118">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="4d7b8-119">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4d7b8-119">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="4d7b8-120">Ative a função atribuída.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-120">Activate the assigned role.</span></span>|
|[<span data-ttu-id="4d7b8-121">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="4d7b8-121">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="4d7b8-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4d7b8-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="4d7b8-123">DesAtive a função atribuída.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-123">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="4d7b8-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d7b8-124">Properties</span></span>
| <span data-ttu-id="4d7b8-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d7b8-125">Property</span></span>     | <span data-ttu-id="4d7b8-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d7b8-126">Type</span></span>   |<span data-ttu-id="4d7b8-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d7b8-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d7b8-128">id</span><span class="sxs-lookup"><span data-stu-id="4d7b8-128">id</span></span>|<span data-ttu-id="4d7b8-129">string</span><span class="sxs-lookup"><span data-stu-id="4d7b8-129">string</span></span>|<span data-ttu-id="4d7b8-130">O identificador exclusivo para a função de administrador.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-130">The unique identifier for administrator role.</span></span> <span data-ttu-id="4d7b8-131">É uma cadeia de caracteres GUID e tem o mesmo valor que a ID de modelo de função do Azure AD para a função determinada.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-131">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="4d7b8-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-132">Read-only.</span></span>|
|<span data-ttu-id="4d7b8-133">name</span><span class="sxs-lookup"><span data-stu-id="4d7b8-133">name</span></span>|<span data-ttu-id="4d7b8-134">string</span><span class="sxs-lookup"><span data-stu-id="4d7b8-134">string</span></span>|<span data-ttu-id="4d7b8-135">Nome da função.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-135">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d7b8-136">Relações</span><span class="sxs-lookup"><span data-stu-id="4d7b8-136">Relationships</span></span>
| <span data-ttu-id="4d7b8-137">Relação</span><span class="sxs-lookup"><span data-stu-id="4d7b8-137">Relationship</span></span> | <span data-ttu-id="4d7b8-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d7b8-138">Type</span></span>   |<span data-ttu-id="4d7b8-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d7b8-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d7b8-140">assignments</span><span class="sxs-lookup"><span data-stu-id="4d7b8-140">assignments</span></span>|<span data-ttu-id="4d7b8-141">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="4d7b8-141">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="4d7b8-142">As atribuições para essa função.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-142">The assignments for this role.</span></span> <span data-ttu-id="4d7b8-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-143">Read-only.</span></span> <span data-ttu-id="4d7b8-144">Anulável.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-144">Nullable.</span></span>|
|<span data-ttu-id="4d7b8-145">settings</span><span class="sxs-lookup"><span data-stu-id="4d7b8-145">settings</span></span>|[<span data-ttu-id="4d7b8-146">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="4d7b8-146">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="4d7b8-147">As configurações dessa função.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-147">The settings for this role.</span></span> <span data-ttu-id="4d7b8-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-148">Read-only.</span></span> <span data-ttu-id="4d7b8-149">Anulável.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-149">Nullable.</span></span>|
|<span data-ttu-id="4d7b8-150">summary</span><span class="sxs-lookup"><span data-stu-id="4d7b8-150">summary</span></span>|[<span data-ttu-id="4d7b8-151">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="4d7b8-151">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="4d7b8-152">As informações resumidas para essa função.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-152">The summary information for this role.</span></span> <span data-ttu-id="4d7b8-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-153">Read-only.</span></span> <span data-ttu-id="4d7b8-154">Anulável.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d7b8-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d7b8-155">JSON representation</span></span>

<span data-ttu-id="4d7b8-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4d7b8-156">Here is a JSON representation of the resource.</span></span>

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
