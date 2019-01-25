---
title: tipo de recurso de privilegedRoleAssignment
description: 'Representa uma atribuição de função privilegiado para um usuário específico. '
localization_priority: Normal
ms.openlocfilehash: 479b6d46dc479134fd0abb46b1a9ffe478611a82
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515115"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="79700-103">tipo de recurso de privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="79700-103">privilegedRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79700-104">Representa uma atribuição de função privilegiado para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="79700-104">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="79700-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="79700-105">Methods</span></span>

| <span data-ttu-id="79700-106">Método</span><span class="sxs-lookup"><span data-stu-id="79700-106">Method</span></span>           | <span data-ttu-id="79700-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="79700-107">Return Type</span></span>    |<span data-ttu-id="79700-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="79700-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="79700-109">Coleção de privilegedRoleAssignment de lista</span><span class="sxs-lookup"><span data-stu-id="79700-109">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="79700-110">coleção [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="79700-110">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="79700-111">Obtenha a coleção de objetos privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="79700-111">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="79700-112">Obter privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="79700-112">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="79700-113">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="79700-113">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="79700-114">Leia as propriedades e os relacionamentos do objeto privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="79700-114">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="79700-115">Criar atribuição</span><span class="sxs-lookup"><span data-stu-id="79700-115">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="79700-116">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="79700-116">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="79700-117">Crie uma nova atribuição de lançamento para a coleção assignments.</span><span class="sxs-lookup"><span data-stu-id="79700-117">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="79700-118">Delete</span><span class="sxs-lookup"><span data-stu-id="79700-118">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="79700-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79700-119">None</span></span> |<span data-ttu-id="79700-120">Exclua objeto privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="79700-120">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="79700-121">makePermanent</span><span class="sxs-lookup"><span data-stu-id="79700-121">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="79700-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="79700-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="79700-123">Fazer a atribuição de função como permanente.</span><span class="sxs-lookup"><span data-stu-id="79700-123">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="79700-124">makeEligible</span><span class="sxs-lookup"><span data-stu-id="79700-124">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="79700-125">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="79700-125">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="79700-126">Fazer a atribuição de função como qualificado.</span><span class="sxs-lookup"><span data-stu-id="79700-126">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="79700-127">Pessoal</span><span class="sxs-lookup"><span data-stu-id="79700-127">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="79700-128">coleção [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="79700-128">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="79700-129">Obtenha as atribuições de função privilegiado do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="79700-129">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="79700-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79700-130">Properties</span></span>
| <span data-ttu-id="79700-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79700-131">Property</span></span>     | <span data-ttu-id="79700-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="79700-132">Type</span></span>   |<span data-ttu-id="79700-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="79700-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79700-134">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="79700-134">expirationDateTime</span></span>|<span data-ttu-id="79700-135">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79700-135">dateTimeOffset</span></span>|<span data-ttu-id="79700-136">DateTime UTC quando a atribuição de função privilegiado temporário será expirada.</span><span class="sxs-lookup"><span data-stu-id="79700-136">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="79700-137">Para atribuição de função permanente, o valor é nulo.</span><span class="sxs-lookup"><span data-stu-id="79700-137">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="79700-138">id</span><span class="sxs-lookup"><span data-stu-id="79700-138">id</span></span>|<span data-ttu-id="79700-139">string</span><span class="sxs-lookup"><span data-stu-id="79700-139">string</span></span>| <span data-ttu-id="79700-140">O identificador exclusivo para a atribuição de função privilegiado.</span><span class="sxs-lookup"><span data-stu-id="79700-140">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="79700-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="79700-141">Read-only.</span></span> <span data-ttu-id="79700-142">É no formato de 'userId_roleId', onde userId é a cadeia de caracteres do GUID para id de usuário do Windows Azure AD e roleId é a cadeia de caracteres do GUID para id de função de administrador do Azure.</span><span class="sxs-lookup"><span data-stu-id="79700-142">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="79700-143">isElevated</span><span class="sxs-lookup"><span data-stu-id="79700-143">isElevated</span></span>|<span data-ttu-id="79700-144">booliano</span><span class="sxs-lookup"><span data-stu-id="79700-144">boolean</span></span>|<span data-ttu-id="79700-145">**true** se a atribuição de função é ativada.</span><span class="sxs-lookup"><span data-stu-id="79700-145">**true** if the role assignment is activated.</span></span> <span data-ttu-id="79700-146">**false** se a atribuição de função é desativada.</span><span class="sxs-lookup"><span data-stu-id="79700-146">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="79700-147">resultMessage</span><span class="sxs-lookup"><span data-stu-id="79700-147">resultMessage</span></span>|<span data-ttu-id="79700-148">string</span><span class="sxs-lookup"><span data-stu-id="79700-148">string</span></span>|<span data-ttu-id="79700-149">Mensagem de resultado definido pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="79700-149">Result message set by the service.</span></span>|
|<span data-ttu-id="79700-150">roleId</span><span class="sxs-lookup"><span data-stu-id="79700-150">roleId</span></span>|<span data-ttu-id="79700-151">string</span><span class="sxs-lookup"><span data-stu-id="79700-151">string</span></span>|<span data-ttu-id="79700-152">identificador de função</span><span class="sxs-lookup"><span data-stu-id="79700-152">Role identifier.</span></span> <span data-ttu-id="79700-153">No formato de cadeia de caracteres GUID.</span><span class="sxs-lookup"><span data-stu-id="79700-153">In GUID string format.</span></span>|
|<span data-ttu-id="79700-154">userId</span><span class="sxs-lookup"><span data-stu-id="79700-154">userId</span></span>|<span data-ttu-id="79700-155">string</span><span class="sxs-lookup"><span data-stu-id="79700-155">string</span></span>|<span data-ttu-id="79700-156">Identificador de usuário.</span><span class="sxs-lookup"><span data-stu-id="79700-156">User identifier.</span></span> <span data-ttu-id="79700-157">No formato de cadeia de caracteres GUID.</span><span class="sxs-lookup"><span data-stu-id="79700-157">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79700-158">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="79700-158">Relationships</span></span>
| <span data-ttu-id="79700-159">Relação</span><span class="sxs-lookup"><span data-stu-id="79700-159">Relationship</span></span> | <span data-ttu-id="79700-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="79700-160">Type</span></span>   |<span data-ttu-id="79700-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="79700-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79700-162">roleInfo</span><span class="sxs-lookup"><span data-stu-id="79700-162">roleInfo</span></span>|[<span data-ttu-id="79700-163">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="79700-163">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="79700-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="79700-164">Read-only.</span></span> <span data-ttu-id="79700-165">Anulável.</span><span class="sxs-lookup"><span data-stu-id="79700-165">Nullable.</span></span> <span data-ttu-id="79700-166">As informações de função associada.</span><span class="sxs-lookup"><span data-stu-id="79700-166">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="79700-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79700-167">JSON representation</span></span>

<span data-ttu-id="79700-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79700-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedroleassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
