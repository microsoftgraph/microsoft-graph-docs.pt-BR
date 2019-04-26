---
title: tipo de recurso privilegedRoleAssignment
description: 'Representa uma atribuição de função privilegiada para um usuário específico. '
localization_priority: Normal
ms.openlocfilehash: 1e58f144eb3dda19225a836aa966f9479d3a9350
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344210"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="a97b6-103">tipo de recurso privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a97b6-103">privilegedRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a97b6-104">Representa uma atribuição de função privilegiada para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="a97b6-104">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="a97b6-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="a97b6-105">Methods</span></span>

| <span data-ttu-id="a97b6-106">Método</span><span class="sxs-lookup"><span data-stu-id="a97b6-106">Method</span></span>           | <span data-ttu-id="a97b6-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a97b6-107">Return Type</span></span>    |<span data-ttu-id="a97b6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a97b6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a97b6-109">Listar privilegedRoleAssignment coleção</span><span class="sxs-lookup"><span data-stu-id="a97b6-109">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="a97b6-110">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="a97b6-110">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="a97b6-111">Obtenha a coleção de objetos privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="a97b6-111">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="a97b6-112">Get privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a97b6-112">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="a97b6-113">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a97b6-113">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="a97b6-114">Leia as propriedades e os relacionamentos do objeto privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="a97b6-114">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="a97b6-115">Criar tarefa</span><span class="sxs-lookup"><span data-stu-id="a97b6-115">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="a97b6-116">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a97b6-116">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="a97b6-117">Crie uma nova atribuição postando na coleção assignments.</span><span class="sxs-lookup"><span data-stu-id="a97b6-117">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="a97b6-118">Delete</span><span class="sxs-lookup"><span data-stu-id="a97b6-118">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="a97b6-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a97b6-119">None</span></span> |<span data-ttu-id="a97b6-120">Exclua um objeto privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="a97b6-120">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="a97b6-121">makePermanent</span><span class="sxs-lookup"><span data-stu-id="a97b6-121">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="a97b6-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a97b6-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="a97b6-123">Torne a atribuição de função como permanente.</span><span class="sxs-lookup"><span data-stu-id="a97b6-123">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="a97b6-124">makeEligible</span><span class="sxs-lookup"><span data-stu-id="a97b6-124">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="a97b6-125">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a97b6-125">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="a97b6-126">Tornar a atribuição de função como qualificada.</span><span class="sxs-lookup"><span data-stu-id="a97b6-126">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="a97b6-127">my</span><span class="sxs-lookup"><span data-stu-id="a97b6-127">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="a97b6-128">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="a97b6-128">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="a97b6-129">Obtenha as atribuições de função privilegiada do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="a97b6-129">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="a97b6-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a97b6-130">Properties</span></span>
| <span data-ttu-id="a97b6-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a97b6-131">Property</span></span>     | <span data-ttu-id="a97b6-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a97b6-132">Type</span></span>   |<span data-ttu-id="a97b6-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a97b6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a97b6-134">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a97b6-134">expirationDateTime</span></span>|<span data-ttu-id="a97b6-135">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a97b6-135">dateTimeOffset</span></span>|<span data-ttu-id="a97b6-136">A data e hora UTC em que a atribuição de função privilegiada temporária será expirada.</span><span class="sxs-lookup"><span data-stu-id="a97b6-136">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="a97b6-137">Para atribuição de função permanente, o valor é NULL.</span><span class="sxs-lookup"><span data-stu-id="a97b6-137">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="a97b6-138">id</span><span class="sxs-lookup"><span data-stu-id="a97b6-138">id</span></span>|<span data-ttu-id="a97b6-139">string</span><span class="sxs-lookup"><span data-stu-id="a97b6-139">string</span></span>| <span data-ttu-id="a97b6-140">O identificador exclusivo da atribuição de função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="a97b6-140">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="a97b6-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a97b6-141">Read-only.</span></span> <span data-ttu-id="a97b6-142">Ele está no formato de ' userId_roleId ', onde userId é a cadeia de caracteres GUID da ID de usuário do Azure AD e RoleID é a cadeia de caracteres GUID da ID de função do administrador do Azure.</span><span class="sxs-lookup"><span data-stu-id="a97b6-142">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="a97b6-143">isElevados</span><span class="sxs-lookup"><span data-stu-id="a97b6-143">isElevated</span></span>|<span data-ttu-id="a97b6-144">booliano</span><span class="sxs-lookup"><span data-stu-id="a97b6-144">boolean</span></span>|<span data-ttu-id="a97b6-145">**true** se a atribuição de função é ativada.</span><span class="sxs-lookup"><span data-stu-id="a97b6-145">**true** if the role assignment is activated.</span></span> <span data-ttu-id="a97b6-146">**false** se a atribuição de função é desativada.</span><span class="sxs-lookup"><span data-stu-id="a97b6-146">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="a97b6-147">resultMessage</span><span class="sxs-lookup"><span data-stu-id="a97b6-147">resultMessage</span></span>|<span data-ttu-id="a97b6-148">string</span><span class="sxs-lookup"><span data-stu-id="a97b6-148">string</span></span>|<span data-ttu-id="a97b6-149">Mensagem de resultado definida pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="a97b6-149">Result message set by the service.</span></span>|
|<span data-ttu-id="a97b6-150">roleId</span><span class="sxs-lookup"><span data-stu-id="a97b6-150">roleId</span></span>|<span data-ttu-id="a97b6-151">string</span><span class="sxs-lookup"><span data-stu-id="a97b6-151">string</span></span>|<span data-ttu-id="a97b6-152">Identificador de função.</span><span class="sxs-lookup"><span data-stu-id="a97b6-152">Role identifier.</span></span> <span data-ttu-id="a97b6-153">Em formato de cadeia de caracteres GUID.</span><span class="sxs-lookup"><span data-stu-id="a97b6-153">In GUID string format.</span></span>|
|<span data-ttu-id="a97b6-154">userId</span><span class="sxs-lookup"><span data-stu-id="a97b6-154">userId</span></span>|<span data-ttu-id="a97b6-155">string</span><span class="sxs-lookup"><span data-stu-id="a97b6-155">string</span></span>|<span data-ttu-id="a97b6-156">Identificador de usuário.</span><span class="sxs-lookup"><span data-stu-id="a97b6-156">User identifier.</span></span> <span data-ttu-id="a97b6-157">Em formato de cadeia de caracteres GUID.</span><span class="sxs-lookup"><span data-stu-id="a97b6-157">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a97b6-158">Relações</span><span class="sxs-lookup"><span data-stu-id="a97b6-158">Relationships</span></span>
| <span data-ttu-id="a97b6-159">Relação</span><span class="sxs-lookup"><span data-stu-id="a97b6-159">Relationship</span></span> | <span data-ttu-id="a97b6-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="a97b6-160">Type</span></span>   |<span data-ttu-id="a97b6-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="a97b6-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a97b6-162">roleInfo</span><span class="sxs-lookup"><span data-stu-id="a97b6-162">roleInfo</span></span>|[<span data-ttu-id="a97b6-163">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="a97b6-163">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="a97b6-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a97b6-164">Read-only.</span></span> <span data-ttu-id="a97b6-165">Anulável.</span><span class="sxs-lookup"><span data-stu-id="a97b6-165">Nullable.</span></span> <span data-ttu-id="a97b6-166">As informações da função associada.</span><span class="sxs-lookup"><span data-stu-id="a97b6-166">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a97b6-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a97b6-167">JSON representation</span></span>

<span data-ttu-id="a97b6-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a97b6-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
}-->

```json
{
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isElevated": true,
  "resultMessage": "string",
  "roleId": "string",
  "userId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
