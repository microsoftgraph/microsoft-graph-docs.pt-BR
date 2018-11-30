---
title: tipo de recurso de privilegedRoleAssignment
description: 'Representa uma atribuição de função privilegiado para um usuário específico. '
ms.openlocfilehash: 40cfe6487184171fc0d120f9a0e2cd98070f96f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035250"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="571ed-103">tipo de recurso de privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="571ed-103">privilegedRoleAssignment resource type</span></span>

> <span data-ttu-id="571ed-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="571ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="571ed-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="571ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="571ed-106">Representa uma atribuição de função privilegiado para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="571ed-106">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="571ed-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="571ed-107">Methods</span></span>

| <span data-ttu-id="571ed-108">Método</span><span class="sxs-lookup"><span data-stu-id="571ed-108">Method</span></span>           | <span data-ttu-id="571ed-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="571ed-109">Return Type</span></span>    |<span data-ttu-id="571ed-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="571ed-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="571ed-111">Coleção de privilegedRoleAssignment de lista</span><span class="sxs-lookup"><span data-stu-id="571ed-111">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="571ed-112">coleção [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="571ed-112">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="571ed-113">Obtenha a coleção de objetos privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="571ed-113">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="571ed-114">Obter privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="571ed-114">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="571ed-115">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="571ed-115">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="571ed-116">Leia as propriedades e os relacionamentos do objeto privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="571ed-116">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="571ed-117">Criar atribuição</span><span class="sxs-lookup"><span data-stu-id="571ed-117">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="571ed-118">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="571ed-118">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="571ed-119">Crie uma nova atribuição de lançamento para a coleção assignments.</span><span class="sxs-lookup"><span data-stu-id="571ed-119">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="571ed-120">Delete</span><span class="sxs-lookup"><span data-stu-id="571ed-120">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="571ed-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="571ed-121">None</span></span> |<span data-ttu-id="571ed-122">Exclua objeto privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="571ed-122">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="571ed-123">makePermanent</span><span class="sxs-lookup"><span data-stu-id="571ed-123">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="571ed-124">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="571ed-124">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="571ed-125">Fazer a atribuição de função como permanente.</span><span class="sxs-lookup"><span data-stu-id="571ed-125">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="571ed-126">makeEligible</span><span class="sxs-lookup"><span data-stu-id="571ed-126">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="571ed-127">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="571ed-127">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="571ed-128">Fazer a atribuição de função como qualificado.</span><span class="sxs-lookup"><span data-stu-id="571ed-128">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="571ed-129">Minha</span><span class="sxs-lookup"><span data-stu-id="571ed-129">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="571ed-130">coleção [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="571ed-130">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="571ed-131">Obtenha as atribuições de função privilegiado do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="571ed-131">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="571ed-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="571ed-132">Properties</span></span>
| <span data-ttu-id="571ed-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="571ed-133">Property</span></span>     | <span data-ttu-id="571ed-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="571ed-134">Type</span></span>   |<span data-ttu-id="571ed-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="571ed-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="571ed-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="571ed-136">expirationDateTime</span></span>|<span data-ttu-id="571ed-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="571ed-137">dateTimeOffset</span></span>|<span data-ttu-id="571ed-138">DateTime UTC quando a atribuição de função privilegiado temporário será expirada.</span><span class="sxs-lookup"><span data-stu-id="571ed-138">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="571ed-139">Para atribuição de função permanente, o valor é nulo.</span><span class="sxs-lookup"><span data-stu-id="571ed-139">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="571ed-140">id</span><span class="sxs-lookup"><span data-stu-id="571ed-140">id</span></span>|<span data-ttu-id="571ed-141">string</span><span class="sxs-lookup"><span data-stu-id="571ed-141">string</span></span>| <span data-ttu-id="571ed-142">O identificador exclusivo para a atribuição de função privilegiado.</span><span class="sxs-lookup"><span data-stu-id="571ed-142">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="571ed-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="571ed-143">Read-only.</span></span> <span data-ttu-id="571ed-144">É no formato de 'userId_roleId', onde userId é a cadeia de caracteres do GUID para id de usuário do Windows Azure AD e roleId é a cadeia de caracteres do GUID para id de função de administrador do Azure.</span><span class="sxs-lookup"><span data-stu-id="571ed-144">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="571ed-145">isElevated</span><span class="sxs-lookup"><span data-stu-id="571ed-145">isElevated</span></span>|<span data-ttu-id="571ed-146">booliano</span><span class="sxs-lookup"><span data-stu-id="571ed-146">boolean</span></span>|<span data-ttu-id="571ed-147">**true** se a atribuição de função é ativada.</span><span class="sxs-lookup"><span data-stu-id="571ed-147">**true** if the role assignment is activated.</span></span> <span data-ttu-id="571ed-148">**false** se a atribuição de função é desativada.</span><span class="sxs-lookup"><span data-stu-id="571ed-148">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="571ed-149">resultMessage</span><span class="sxs-lookup"><span data-stu-id="571ed-149">resultMessage</span></span>|<span data-ttu-id="571ed-150">string</span><span class="sxs-lookup"><span data-stu-id="571ed-150">string</span></span>|<span data-ttu-id="571ed-151">Mensagem de resultado definido pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="571ed-151">Result message set by the service.</span></span>|
|<span data-ttu-id="571ed-152">roleId</span><span class="sxs-lookup"><span data-stu-id="571ed-152">roleId</span></span>|<span data-ttu-id="571ed-153">string</span><span class="sxs-lookup"><span data-stu-id="571ed-153">string</span></span>|<span data-ttu-id="571ed-154">Identificador de função.</span><span class="sxs-lookup"><span data-stu-id="571ed-154">Role identifier.</span></span> <span data-ttu-id="571ed-155">No formato de cadeia de caracteres GUID.</span><span class="sxs-lookup"><span data-stu-id="571ed-155">In GUID string format.</span></span>|
|<span data-ttu-id="571ed-156">userId</span><span class="sxs-lookup"><span data-stu-id="571ed-156">userId</span></span>|<span data-ttu-id="571ed-157">string</span><span class="sxs-lookup"><span data-stu-id="571ed-157">string</span></span>|<span data-ttu-id="571ed-158">Identificador de usuário.</span><span class="sxs-lookup"><span data-stu-id="571ed-158">User identifier.</span></span> <span data-ttu-id="571ed-159">No formato de cadeia de caracteres GUID.</span><span class="sxs-lookup"><span data-stu-id="571ed-159">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="571ed-160">Relações</span><span class="sxs-lookup"><span data-stu-id="571ed-160">Relationships</span></span>
| <span data-ttu-id="571ed-161">Relação</span><span class="sxs-lookup"><span data-stu-id="571ed-161">Relationship</span></span> | <span data-ttu-id="571ed-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="571ed-162">Type</span></span>   |<span data-ttu-id="571ed-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="571ed-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="571ed-164">roleInfo</span><span class="sxs-lookup"><span data-stu-id="571ed-164">roleInfo</span></span>|[<span data-ttu-id="571ed-165">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="571ed-165">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="571ed-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="571ed-166">Read-only.</span></span> <span data-ttu-id="571ed-167">Anulável.</span><span class="sxs-lookup"><span data-stu-id="571ed-167">Nullable.</span></span> <span data-ttu-id="571ed-168">As informações de função associada.</span><span class="sxs-lookup"><span data-stu-id="571ed-168">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="571ed-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="571ed-169">JSON representation</span></span>

<span data-ttu-id="571ed-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="571ed-170">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->