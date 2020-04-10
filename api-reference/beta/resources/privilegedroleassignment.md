---
title: tipo de recurso privilegedRoleAssignment
description: 'Representa uma atribuição de função privilegiada para um usuário específico. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: aef2b3962601a20df30f27c19ccd1abf23b0c561
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217901"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="18f02-103">tipo de recurso privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="18f02-103">privilegedRoleAssignment resource type</span></span>

<span data-ttu-id="18f02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18f02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18f02-105">Representa uma atribuição de função privilegiada para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="18f02-105">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="18f02-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="18f02-106">Methods</span></span>

| <span data-ttu-id="18f02-107">Método</span><span class="sxs-lookup"><span data-stu-id="18f02-107">Method</span></span>           | <span data-ttu-id="18f02-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="18f02-108">Return Type</span></span>    |<span data-ttu-id="18f02-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="18f02-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="18f02-110">Listar privilegedRoleAssignment coleção</span><span class="sxs-lookup"><span data-stu-id="18f02-110">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="18f02-111">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="18f02-111">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="18f02-112">Obtenha a coleção de objetos privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="18f02-112">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="18f02-113">Get privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="18f02-113">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="18f02-114">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="18f02-114">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="18f02-115">Leia as propriedades e os relacionamentos do objeto privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="18f02-115">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="18f02-116">Criar tarefa</span><span class="sxs-lookup"><span data-stu-id="18f02-116">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="18f02-117">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="18f02-117">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="18f02-118">Crie uma nova atribuição postando na coleção assignments.</span><span class="sxs-lookup"><span data-stu-id="18f02-118">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="18f02-119">Delete</span><span class="sxs-lookup"><span data-stu-id="18f02-119">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="18f02-120">None</span><span class="sxs-lookup"><span data-stu-id="18f02-120">None</span></span> |<span data-ttu-id="18f02-121">Exclua um objeto privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="18f02-121">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="18f02-122">makePermanent</span><span class="sxs-lookup"><span data-stu-id="18f02-122">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="18f02-123">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="18f02-123">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="18f02-124">Torne a atribuição de função como permanente.</span><span class="sxs-lookup"><span data-stu-id="18f02-124">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="18f02-125">makeEligible</span><span class="sxs-lookup"><span data-stu-id="18f02-125">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="18f02-126">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="18f02-126">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="18f02-127">Tornar a atribuição de função como qualificada.</span><span class="sxs-lookup"><span data-stu-id="18f02-127">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="18f02-128">my</span><span class="sxs-lookup"><span data-stu-id="18f02-128">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="18f02-129">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="18f02-129">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="18f02-130">Obtenha as atribuições de função privilegiada do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="18f02-130">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="18f02-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18f02-131">Properties</span></span>
| <span data-ttu-id="18f02-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18f02-132">Property</span></span>     | <span data-ttu-id="18f02-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="18f02-133">Type</span></span>   |<span data-ttu-id="18f02-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="18f02-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18f02-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="18f02-135">expirationDateTime</span></span>|<span data-ttu-id="18f02-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18f02-136">dateTimeOffset</span></span>|<span data-ttu-id="18f02-137">A data e hora UTC em que a atribuição de função privilegiada temporária será expirada.</span><span class="sxs-lookup"><span data-stu-id="18f02-137">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="18f02-138">Para atribuição de função permanente, o valor é NULL.</span><span class="sxs-lookup"><span data-stu-id="18f02-138">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="18f02-139">id</span><span class="sxs-lookup"><span data-stu-id="18f02-139">id</span></span>|<span data-ttu-id="18f02-140">string</span><span class="sxs-lookup"><span data-stu-id="18f02-140">string</span></span>| <span data-ttu-id="18f02-141">O identificador exclusivo da atribuição de função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="18f02-141">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="18f02-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="18f02-142">Read-only.</span></span> <span data-ttu-id="18f02-143">Ele está no formato de ' userId_roleId ', onde userId é a cadeia de caracteres GUID da ID de usuário do Azure AD e RoleID é a cadeia de caracteres GUID da ID da função de administrador do Azure.</span><span class="sxs-lookup"><span data-stu-id="18f02-143">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="18f02-144">iselevados</span><span class="sxs-lookup"><span data-stu-id="18f02-144">isElevated</span></span>|<span data-ttu-id="18f02-145">booliano</span><span class="sxs-lookup"><span data-stu-id="18f02-145">boolean</span></span>|<span data-ttu-id="18f02-146">**true** se a atribuição de função é ativada.</span><span class="sxs-lookup"><span data-stu-id="18f02-146">**true** if the role assignment is activated.</span></span> <span data-ttu-id="18f02-147">**false** se a atribuição de função é desativada.</span><span class="sxs-lookup"><span data-stu-id="18f02-147">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="18f02-148">resultMessage</span><span class="sxs-lookup"><span data-stu-id="18f02-148">resultMessage</span></span>|<span data-ttu-id="18f02-149">string</span><span class="sxs-lookup"><span data-stu-id="18f02-149">string</span></span>|<span data-ttu-id="18f02-150">Mensagem de resultado definida pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="18f02-150">Result message set by the service.</span></span>|
|<span data-ttu-id="18f02-151">roleId</span><span class="sxs-lookup"><span data-stu-id="18f02-151">roleId</span></span>|<span data-ttu-id="18f02-152">string</span><span class="sxs-lookup"><span data-stu-id="18f02-152">string</span></span>|<span data-ttu-id="18f02-153">Identificador de função.</span><span class="sxs-lookup"><span data-stu-id="18f02-153">Role identifier.</span></span> <span data-ttu-id="18f02-154">Em formato de cadeia de caracteres GUID.</span><span class="sxs-lookup"><span data-stu-id="18f02-154">In GUID string format.</span></span>|
|<span data-ttu-id="18f02-155">userId</span><span class="sxs-lookup"><span data-stu-id="18f02-155">userId</span></span>|<span data-ttu-id="18f02-156">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18f02-156">string</span></span>|<span data-ttu-id="18f02-157">Identificador de usuário.</span><span class="sxs-lookup"><span data-stu-id="18f02-157">User identifier.</span></span> <span data-ttu-id="18f02-158">Em formato de cadeia de caracteres GUID.</span><span class="sxs-lookup"><span data-stu-id="18f02-158">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18f02-159">Relações</span><span class="sxs-lookup"><span data-stu-id="18f02-159">Relationships</span></span>
| <span data-ttu-id="18f02-160">Relação</span><span class="sxs-lookup"><span data-stu-id="18f02-160">Relationship</span></span> | <span data-ttu-id="18f02-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="18f02-161">Type</span></span>   |<span data-ttu-id="18f02-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="18f02-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18f02-163">roleInfo</span><span class="sxs-lookup"><span data-stu-id="18f02-163">roleInfo</span></span>|[<span data-ttu-id="18f02-164">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="18f02-164">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="18f02-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="18f02-165">Read-only.</span></span> <span data-ttu-id="18f02-166">Anulável.</span><span class="sxs-lookup"><span data-stu-id="18f02-166">Nullable.</span></span> <span data-ttu-id="18f02-167">As informações da função associada.</span><span class="sxs-lookup"><span data-stu-id="18f02-167">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18f02-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18f02-168">JSON representation</span></span>

<span data-ttu-id="18f02-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18f02-169">Here is a JSON representation of the resource.</span></span>

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
