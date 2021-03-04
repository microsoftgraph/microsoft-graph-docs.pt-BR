---
title: Tipo de recurso privilegedRoleAssignment
description: 'Representa uma atribuição de função privilegiada para um usuário específico. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 55b37c195777659b172e668d4e02b60de4f78c0d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440141"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="fb7af-103">Tipo de recurso privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="fb7af-103">privilegedRoleAssignment resource type</span></span>

<span data-ttu-id="fb7af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb7af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb7af-105">Representa uma atribuição de função privilegiada para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="fb7af-105">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="fb7af-106">Methods</span><span class="sxs-lookup"><span data-stu-id="fb7af-106">Methods</span></span>

| <span data-ttu-id="fb7af-107">Método</span><span class="sxs-lookup"><span data-stu-id="fb7af-107">Method</span></span>           | <span data-ttu-id="fb7af-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fb7af-108">Return Type</span></span>    |<span data-ttu-id="fb7af-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb7af-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fb7af-110">Listar coleção privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="fb7af-110">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="fb7af-111">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="fb7af-111">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="fb7af-112">Obter a coleção de objetos privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="fb7af-112">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="fb7af-113">Get privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="fb7af-113">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="fb7af-114">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="fb7af-114">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="fb7af-115">Ler propriedades e relações do objeto privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="fb7af-115">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="fb7af-116">Criar tarefa</span><span class="sxs-lookup"><span data-stu-id="fb7af-116">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="fb7af-117">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="fb7af-117">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="fb7af-118">Crie uma nova atribuição postando na coleção de atribuições.</span><span class="sxs-lookup"><span data-stu-id="fb7af-118">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="fb7af-119">Delete</span><span class="sxs-lookup"><span data-stu-id="fb7af-119">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="fb7af-120">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="fb7af-120">None</span></span> |<span data-ttu-id="fb7af-121">Exclua um objeto privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="fb7af-121">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="fb7af-122">makePermanent</span><span class="sxs-lookup"><span data-stu-id="fb7af-122">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="fb7af-123">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="fb7af-123">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="fb7af-124">Torne a atribuição de função como permanente.</span><span class="sxs-lookup"><span data-stu-id="fb7af-124">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="fb7af-125">makeEligible</span><span class="sxs-lookup"><span data-stu-id="fb7af-125">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="fb7af-126">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="fb7af-126">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="fb7af-127">Tornar a atribuição de função como qualificada.</span><span class="sxs-lookup"><span data-stu-id="fb7af-127">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="fb7af-128">my</span><span class="sxs-lookup"><span data-stu-id="fb7af-128">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="fb7af-129">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="fb7af-129">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="fb7af-130">Obter as atribuições de função privilegiada do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="fb7af-130">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="fb7af-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb7af-131">Properties</span></span>
| <span data-ttu-id="fb7af-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb7af-132">Property</span></span>     | <span data-ttu-id="fb7af-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb7af-133">Type</span></span>   |<span data-ttu-id="fb7af-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb7af-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb7af-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fb7af-135">expirationDateTime</span></span>|<span data-ttu-id="fb7af-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb7af-136">dateTimeOffset</span></span>|<span data-ttu-id="fb7af-137">O UTC DateTime quando a atribuição de função privilegiada temporária será expirada.</span><span class="sxs-lookup"><span data-stu-id="fb7af-137">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="fb7af-138">Para atribuição de função permanente, o valor é nulo.</span><span class="sxs-lookup"><span data-stu-id="fb7af-138">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="fb7af-139">id</span><span class="sxs-lookup"><span data-stu-id="fb7af-139">id</span></span>|<span data-ttu-id="fb7af-140">string</span><span class="sxs-lookup"><span data-stu-id="fb7af-140">string</span></span>| <span data-ttu-id="fb7af-141">O identificador exclusivo da atribuição de função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="fb7af-141">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="fb7af-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fb7af-142">Read-only.</span></span> <span data-ttu-id="fb7af-143">Está no formato de "userId_roleId", onde userId é a cadeia de caracteres GUID para id de usuário do Azure AD e roleId é a cadeia de caracteres GUID para id de função de administrador do Azure.</span><span class="sxs-lookup"><span data-stu-id="fb7af-143">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="fb7af-144">isElevated</span><span class="sxs-lookup"><span data-stu-id="fb7af-144">isElevated</span></span>|<span data-ttu-id="fb7af-145">booliano</span><span class="sxs-lookup"><span data-stu-id="fb7af-145">boolean</span></span>|<span data-ttu-id="fb7af-146">**true** se a atribuição de função estiver ativada.</span><span class="sxs-lookup"><span data-stu-id="fb7af-146">**true** if the role assignment is activated.</span></span> <span data-ttu-id="fb7af-147">**false** se a atribuição de função for desativada.</span><span class="sxs-lookup"><span data-stu-id="fb7af-147">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="fb7af-148">resultMessage</span><span class="sxs-lookup"><span data-stu-id="fb7af-148">resultMessage</span></span>|<span data-ttu-id="fb7af-149">string</span><span class="sxs-lookup"><span data-stu-id="fb7af-149">string</span></span>|<span data-ttu-id="fb7af-150">Mensagem de resultado definida pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="fb7af-150">Result message set by the service.</span></span>|
|<span data-ttu-id="fb7af-151">roleId</span><span class="sxs-lookup"><span data-stu-id="fb7af-151">roleId</span></span>|<span data-ttu-id="fb7af-152">string</span><span class="sxs-lookup"><span data-stu-id="fb7af-152">string</span></span>|<span data-ttu-id="fb7af-153">Identificador de função.</span><span class="sxs-lookup"><span data-stu-id="fb7af-153">Role identifier.</span></span> <span data-ttu-id="fb7af-154">No formato de cadeia de caracteres GUID.</span><span class="sxs-lookup"><span data-stu-id="fb7af-154">In GUID string format.</span></span>|
|<span data-ttu-id="fb7af-155">userId</span><span class="sxs-lookup"><span data-stu-id="fb7af-155">userId</span></span>|<span data-ttu-id="fb7af-156">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb7af-156">string</span></span>|<span data-ttu-id="fb7af-157">Identificador de usuário.</span><span class="sxs-lookup"><span data-stu-id="fb7af-157">User identifier.</span></span> <span data-ttu-id="fb7af-158">No formato de cadeia de caracteres GUID.</span><span class="sxs-lookup"><span data-stu-id="fb7af-158">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb7af-159">Relações</span><span class="sxs-lookup"><span data-stu-id="fb7af-159">Relationships</span></span>
| <span data-ttu-id="fb7af-160">Relação</span><span class="sxs-lookup"><span data-stu-id="fb7af-160">Relationship</span></span> | <span data-ttu-id="fb7af-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb7af-161">Type</span></span>   |<span data-ttu-id="fb7af-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb7af-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb7af-163">roleInfo</span><span class="sxs-lookup"><span data-stu-id="fb7af-163">roleInfo</span></span>|[<span data-ttu-id="fb7af-164">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="fb7af-164">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="fb7af-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fb7af-165">Read-only.</span></span> <span data-ttu-id="fb7af-166">Anulável.</span><span class="sxs-lookup"><span data-stu-id="fb7af-166">Nullable.</span></span> <span data-ttu-id="fb7af-167">As informações de função associadas.</span><span class="sxs-lookup"><span data-stu-id="fb7af-167">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb7af-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb7af-168">JSON representation</span></span>

<span data-ttu-id="fb7af-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fb7af-169">Here is a JSON representation of the resource.</span></span>

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


