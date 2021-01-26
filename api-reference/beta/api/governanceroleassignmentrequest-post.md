---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação que você deseja em uma atribuição de função. A tabela a seguir lista as operações.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 19ca4988977807f410a2525110b1b3479d6ea326
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983402"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="9c024-104">Criar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="9c024-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="9c024-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c024-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c024-106">Crie uma solicitação de atribuição de função para representar a operação que você deseja em uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="9c024-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="9c024-107">A tabela a seguir lista as operações.</span><span class="sxs-lookup"><span data-stu-id="9c024-107">The following table lists the operations.</span></span>

| <span data-ttu-id="9c024-108">Operação</span><span class="sxs-lookup"><span data-stu-id="9c024-108">Operation</span></span>                                   | <span data-ttu-id="9c024-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c024-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="9c024-110">Atribuir uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="9c024-110">Assign a role assignment</span></span>                    | <span data-ttu-id="9c024-111">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="9c024-111">AdminAdd</span></span>    |
| <span data-ttu-id="9c024-112">Ativar uma atribuição de função qualificada</span><span class="sxs-lookup"><span data-stu-id="9c024-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="9c024-113">UserAdd</span><span class="sxs-lookup"><span data-stu-id="9c024-113">UserAdd</span></span>     |
| <span data-ttu-id="9c024-114">Desativar uma atribuição de função ativada</span><span class="sxs-lookup"><span data-stu-id="9c024-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="9c024-115">UserRemove</span><span class="sxs-lookup"><span data-stu-id="9c024-115">UserRemove</span></span>  |
| <span data-ttu-id="9c024-116">Remover uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="9c024-116">Remove a role assignment</span></span>                    | <span data-ttu-id="9c024-117">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="9c024-117">AdminRemove</span></span> |
| <span data-ttu-id="9c024-118">Atualizar uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="9c024-118">Update a role assignment</span></span>                    | <span data-ttu-id="9c024-119">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="9c024-119">AdminUpdate</span></span> |
| <span data-ttu-id="9c024-120">Solicitação para estender minha atribuição de função</span><span class="sxs-lookup"><span data-stu-id="9c024-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="9c024-121">UserExtend</span><span class="sxs-lookup"><span data-stu-id="9c024-121">UserExtend</span></span>  |
| <span data-ttu-id="9c024-122">Estender uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="9c024-122">Extend a role assignment</span></span>                    | <span data-ttu-id="9c024-123">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="9c024-123">AdminExtend</span></span> |
| <span data-ttu-id="9c024-124">Solicitação para renovar minha atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="9c024-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="9c024-125">UserRenew</span><span class="sxs-lookup"><span data-stu-id="9c024-125">UserRenew</span></span>   |
| <span data-ttu-id="9c024-126">Renovar uma atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="9c024-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="9c024-127">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="9c024-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="9c024-128">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c024-128">Permissions</span></span>

<span data-ttu-id="9c024-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="9c024-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="9c024-131">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="9c024-131">Azure resources</span></span>

| <span data-ttu-id="9c024-132">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c024-132">Permission type</span></span> | <span data-ttu-id="9c024-133">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c024-133">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="9c024-134">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c024-134">Delegated (work or school account)</span></span> | <span data-ttu-id="9c024-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9c024-135">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="9c024-136">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c024-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c024-137">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c024-137">Not supported.</span></span> |
| <span data-ttu-id="9c024-138">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c024-138">Application</span></span> | <span data-ttu-id="9c024-139">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c024-139">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="9c024-140">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="9c024-140">Azure AD</span></span>

| <span data-ttu-id="9c024-141">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c024-141">Permission type</span></span> | <span data-ttu-id="9c024-142">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c024-142">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="9c024-143">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c024-143">Delegated (work or school account)</span></span> | <span data-ttu-id="9c024-144">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="9c024-144">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="9c024-145">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c024-145">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c024-146">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c024-146">Not supported.</span></span> |
| <span data-ttu-id="9c024-147">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c024-147">Application</span></span> | <span data-ttu-id="9c024-148">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c024-148">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="9c024-149">Grupos</span><span class="sxs-lookup"><span data-stu-id="9c024-149">Groups</span></span>

|<span data-ttu-id="9c024-150">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c024-150">Permission type</span></span> | <span data-ttu-id="9c024-151">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c024-151">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="9c024-152">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c024-152">Delegated (work or school account)</span></span> | <span data-ttu-id="9c024-153">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="9c024-153">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="9c024-154">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c024-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c024-155">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c024-155">Not supported.</span></span> |
| <span data-ttu-id="9c024-156">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c024-156">Application</span></span> | <span data-ttu-id="9c024-157">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c024-157">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c024-158">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c024-158">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="9c024-159">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c024-159">Request headers</span></span>

| <span data-ttu-id="9c024-160">Nome</span><span class="sxs-lookup"><span data-stu-id="9c024-160">Name</span></span>          | <span data-ttu-id="9c024-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c024-161">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="9c024-162">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c024-162">Authorization</span></span> | <span data-ttu-id="9c024-163">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9c024-163">Bearer {code}</span></span>    |
| <span data-ttu-id="9c024-164">Content-type</span><span class="sxs-lookup"><span data-stu-id="9c024-164">Content-type</span></span>  | <span data-ttu-id="9c024-165">application/json</span><span class="sxs-lookup"><span data-stu-id="9c024-165">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c024-166">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c024-166">Request body</span></span>

<span data-ttu-id="9c024-167">No corpo da solicitação, fornece uma representação JSON de um [objeto governanceRoleAssignmentRequest.](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="9c024-167">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="9c024-168">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c024-168">Property</span></span>         | <span data-ttu-id="9c024-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c024-169">Type</span></span>                                                     | <span data-ttu-id="9c024-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c024-170">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="9c024-171">resourceId</span><span class="sxs-lookup"><span data-stu-id="9c024-171">resourceId</span></span>       | <span data-ttu-id="9c024-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-172">String</span></span>                                                   | <span data-ttu-id="9c024-173">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c024-173">The ID of the resource.</span></span> <span data-ttu-id="9c024-174">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c024-174">Required.</span></span> |
| <span data-ttu-id="9c024-175">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="9c024-175">roleDefinitionId</span></span> | <span data-ttu-id="9c024-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-176">String</span></span>                                                   | <span data-ttu-id="9c024-177">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="9c024-177">The ID of the role definition.</span></span> <span data-ttu-id="9c024-178">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c024-178">Required.</span></span> |
| <span data-ttu-id="9c024-179">subjectId</span><span class="sxs-lookup"><span data-stu-id="9c024-179">subjectId</span></span>        | <span data-ttu-id="9c024-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-180">String</span></span>                                                   | <span data-ttu-id="9c024-181">A ID do assunto.</span><span class="sxs-lookup"><span data-stu-id="9c024-181">The ID of the subject.</span></span> <span data-ttu-id="9c024-182">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c024-182">Required.</span></span> |
| <span data-ttu-id="9c024-183">assignmentState</span><span class="sxs-lookup"><span data-stu-id="9c024-183">assignmentState</span></span>  | <span data-ttu-id="9c024-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-184">String</span></span>                                                   | <span data-ttu-id="9c024-185">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="9c024-185">The state of assignment.</span></span> <span data-ttu-id="9c024-186">O valor pode ser `Eligible` e `Active` .</span><span class="sxs-lookup"><span data-stu-id="9c024-186">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="9c024-187">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c024-187">Required.</span></span> |
| <span data-ttu-id="9c024-188">type</span><span class="sxs-lookup"><span data-stu-id="9c024-188">type</span></span>             | <span data-ttu-id="9c024-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-189">String</span></span>                                                   | <span data-ttu-id="9c024-190">O tipo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c024-190">The request type.</span></span> <span data-ttu-id="9c024-191">O valor pode `AdminAdd` ser , , , , e `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew` `AdminRenew` `AdminExtend` .</span><span class="sxs-lookup"><span data-stu-id="9c024-191">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="9c024-192">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c024-192">Required.</span></span> |
| <span data-ttu-id="9c024-193">motivo</span><span class="sxs-lookup"><span data-stu-id="9c024-193">reason</span></span>           | <span data-ttu-id="9c024-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-194">String</span></span>                                                   | <span data-ttu-id="9c024-195">O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e revisão.</span><span class="sxs-lookup"><span data-stu-id="9c024-195">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="9c024-196">Cronograma</span><span class="sxs-lookup"><span data-stu-id="9c024-196">schedule</span></span>         | [<span data-ttu-id="9c024-197">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="9c024-197">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="9c024-198">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="9c024-198">The schedule of the role assignment request.</span></span> <span data-ttu-id="9c024-199">Para o tipo de `UserAdd` `AdminAdd` solicitação `AdminUpdate` de , e , `AdminExtend` é necessário.</span><span class="sxs-lookup"><span data-stu-id="9c024-199">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="9c024-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c024-200">Response</span></span>

<span data-ttu-id="9c024-201">Se bem-sucedido, este método retorna um código de resposta e um objeto `201 Created` [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c024-201">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="9c024-202">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="9c024-202">Error codes</span></span>

<span data-ttu-id="9c024-203">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="9c024-203">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="9c024-204">Além disso, ele também retorna os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="9c024-204">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="9c024-205">Código de erro</span><span class="sxs-lookup"><span data-stu-id="9c024-205">Error code</span></span>     | <span data-ttu-id="9c024-206">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="9c024-206">Error message</span></span>                               | <span data-ttu-id="9c024-207">Detalhes</span><span class="sxs-lookup"><span data-stu-id="9c024-207">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="9c024-208">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c024-208">400 BadRequest</span></span> | <span data-ttu-id="9c024-209">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="9c024-209">RoleNotFound</span></span>                                | <span data-ttu-id="9c024-210">O `roleDefinitionId` fornecido no corpo da solicitação não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="9c024-210">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="9c024-211">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c024-211">400 BadRequest</span></span> | <span data-ttu-id="9c024-212">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="9c024-212">ResourceIsLocked</span></span>                            | <span data-ttu-id="9c024-213">O recurso fornecido no corpo da solicitação está no estado e não pode criar `Locked` solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="9c024-213">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="9c024-214">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c024-214">400 BadRequest</span></span> | <span data-ttu-id="9c024-215">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="9c024-215">SubjectNotFound</span></span>                             | <span data-ttu-id="9c024-216">O `subjectId` fornecido no corpo da solicitação não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="9c024-216">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="9c024-217">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c024-217">400 BadRequest</span></span> | <span data-ttu-id="9c024-218">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="9c024-218">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="9c024-219">Já existe uma [governança pendenteRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no sistema.</span><span class="sxs-lookup"><span data-stu-id="9c024-219">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="9c024-220">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c024-220">400 BadRequest</span></span> | <span data-ttu-id="9c024-221">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="9c024-221">RoleAssignmentExists</span></span>                        | <span data-ttu-id="9c024-222">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criado já existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="9c024-222">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="9c024-223">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c024-223">400 BadRequest</span></span> | <span data-ttu-id="9c024-224">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="9c024-224">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="9c024-225">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="9c024-225">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="9c024-226">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c024-226">400 BadRequest</span></span> | <span data-ttu-id="9c024-227">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="9c024-227">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="9c024-228">O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não está de acordo com as políticas internas e não pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="9c024-228">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="9c024-229">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9c024-229">Examples</span></span>

<span data-ttu-id="9c024-230">Os exemplos a seguir mostram como usar essa API.</span><span class="sxs-lookup"><span data-stu-id="9c024-230">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="9c024-231">Exemplo 1: O administrador atribui um usuário a uma função</span><span class="sxs-lookup"><span data-stu-id="9c024-231">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="9c024-232">Neste exemplo, um administrador atribui o usuário nawu@contoso.com à função Leitor de Cobrança.</span><span class="sxs-lookup"><span data-stu-id="9c024-232">In this example, an administrator assigns user nawu@contoso.com to the Billing Reader role.</span></span>

 ><span data-ttu-id="9c024-233">**Observação:** Além da permissão, este exemplo exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` `owner` `user access administrator` (ou) no recurso.</span><span class="sxs-lookup"><span data-stu-id="9c024-233">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="9c024-234">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c024-234">Property</span></span>         | <span data-ttu-id="9c024-235">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c024-235">Type</span></span>                                                     | <span data-ttu-id="9c024-236">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="9c024-236">Required</span></span>                 | <span data-ttu-id="9c024-237">Valor</span><span class="sxs-lookup"><span data-stu-id="9c024-237">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="9c024-238">resourceId</span><span class="sxs-lookup"><span data-stu-id="9c024-238">resourceId</span></span>       | <span data-ttu-id="9c024-239">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-239">String</span></span>                                                   | <span data-ttu-id="9c024-240">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-240">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="9c024-241">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="9c024-241">roleDefinitionId</span></span> | <span data-ttu-id="9c024-242">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-242">String</span></span>                                                   | <span data-ttu-id="9c024-243">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-243">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="9c024-244">subjectId</span><span class="sxs-lookup"><span data-stu-id="9c024-244">subjectId</span></span>        | <span data-ttu-id="9c024-245">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-245">String</span></span>                                                   | <span data-ttu-id="9c024-246">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-246">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="9c024-247">assignmentState</span><span class="sxs-lookup"><span data-stu-id="9c024-247">assignmentState</span></span>  | <span data-ttu-id="9c024-248">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-248">String</span></span>                                                   | <span data-ttu-id="9c024-249">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-249">Yes</span></span>                      | <span data-ttu-id="9c024-250">Qualificado/Ativo</span><span class="sxs-lookup"><span data-stu-id="9c024-250">Eligible / Active</span></span> |
| <span data-ttu-id="9c024-251">type</span><span class="sxs-lookup"><span data-stu-id="9c024-251">type</span></span>             | <span data-ttu-id="9c024-252">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-252">String</span></span>                                                   | <span data-ttu-id="9c024-253">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-253">Yes</span></span>                      | <span data-ttu-id="9c024-254">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="9c024-254">AdminAdd</span></span> |
| <span data-ttu-id="9c024-255">motivo</span><span class="sxs-lookup"><span data-stu-id="9c024-255">reason</span></span>           | <span data-ttu-id="9c024-256">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-256">String</span></span>                                                   | <span data-ttu-id="9c024-257">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="9c024-257">depends on role Settings</span></span> |   |
| <span data-ttu-id="9c024-258">Cronograma</span><span class="sxs-lookup"><span data-stu-id="9c024-258">schedule</span></span>         | [<span data-ttu-id="9c024-259">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="9c024-259">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="9c024-260">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-260">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="9c024-261">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c024-261">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9c024-262">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c024-262">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Eligible",
  "type": "AdminAdd",
  "reason": "Assign an eligible role",
  "schedule": {
    "startDateTime": "2018-05-12T23:37:43.356Z",
    "endDateTime": "2018-11-08T23:37:43.356Z",
    "type": "Once"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="9c024-263">C#</span><span class="sxs-lookup"><span data-stu-id="9c024-263">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c024-264">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c024-264">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c024-265">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c024-265">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c024-266">Java</span><span class="sxs-lookup"><span data-stu-id="9c024-266">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="9c024-267">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c024-267">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "1232e4ea-741a-4be5-8044-5edabdd61672",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminAdd",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "Evaluate Only",
  "status": {
    "status": "InProgress",
    "subStatus": "Granted",
    "statusDetails": [
      {
        "key": "AdminRequestRule",
        "value": "Grant"
      },
      {
        "key": "ExpirationRule",
        "value": "Grant"
      },
      {
        "key": "MfaRule",
        "value": "Grant"
      }
    ]
  },
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:37:43.356Z",
    "endDateTime": "2018-11-08T23:37:43.356Z",
    "duration": "PT0S"
  }
}
```

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="9c024-268">Exemplo 2: o usuário ativa a função qualificada</span><span class="sxs-lookup"><span data-stu-id="9c024-268">Example 2: User activates eligible role</span></span>

<span data-ttu-id="9c024-269">Neste exemplo, o usuário nawu@contoso.com ativa a função leitor de cobrança qualificada.</span><span class="sxs-lookup"><span data-stu-id="9c024-269">In this example, the user nawu@contoso.com activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="9c024-270">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c024-270">Property</span></span>         | <span data-ttu-id="9c024-271">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c024-271">Type</span></span>                                                     | <span data-ttu-id="9c024-272">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="9c024-272">Required</span></span>                 | <span data-ttu-id="9c024-273">Valor</span><span class="sxs-lookup"><span data-stu-id="9c024-273">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="9c024-274">resourceId</span><span class="sxs-lookup"><span data-stu-id="9c024-274">resourceId</span></span>       | <span data-ttu-id="9c024-275">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-275">String</span></span>                                                   | <span data-ttu-id="9c024-276">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-276">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="9c024-277">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="9c024-277">roleDefinitionId</span></span> | <span data-ttu-id="9c024-278">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-278">String</span></span>                                                   | <span data-ttu-id="9c024-279">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-279">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="9c024-280">subjectId</span><span class="sxs-lookup"><span data-stu-id="9c024-280">subjectId</span></span>        | <span data-ttu-id="9c024-281">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-281">String</span></span>                                                   | <span data-ttu-id="9c024-282">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-282">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="9c024-283">assignmentState</span><span class="sxs-lookup"><span data-stu-id="9c024-283">assignmentState</span></span>  | <span data-ttu-id="9c024-284">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-284">String</span></span>                                                   | <span data-ttu-id="9c024-285">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-285">Yes</span></span>                      | <span data-ttu-id="9c024-286">Ativo</span><span class="sxs-lookup"><span data-stu-id="9c024-286">Active</span></span> |
| <span data-ttu-id="9c024-287">type</span><span class="sxs-lookup"><span data-stu-id="9c024-287">type</span></span>             | <span data-ttu-id="9c024-288">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-288">String</span></span>                                                   | <span data-ttu-id="9c024-289">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-289">Yes</span></span>                      | <span data-ttu-id="9c024-290">UserAdd</span><span class="sxs-lookup"><span data-stu-id="9c024-290">UserAdd</span></span> |
| <span data-ttu-id="9c024-291">motivo</span><span class="sxs-lookup"><span data-stu-id="9c024-291">reason</span></span>           | <span data-ttu-id="9c024-292">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-292">String</span></span>                                                   | <span data-ttu-id="9c024-293">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="9c024-293">depends on role Settings</span></span> |   |
| <span data-ttu-id="9c024-294">Cronograma</span><span class="sxs-lookup"><span data-stu-id="9c024-294">schedule</span></span>         | [<span data-ttu-id="9c024-295">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="9c024-295">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="9c024-296">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-296">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="9c024-297">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c024-297">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserAdd",
  "reason": "Activate the owner role",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:28:43.537Z",
    "duration": "PT9H"
  },
  "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394"
}
```

#### <a name="response"></a><span data-ttu-id="9c024-298">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c024-298">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "3ad49a7c-918e-4d86-9f84-fab28f8658c0",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394",
  "type": "UserAdd",
  "assignmentState": "Active",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "Activate the owner role",
  "status": {
    "status": "InProgress",
    "subStatus": "Granted",
    "statusDetails": [
      {
        "key": "EligibilityRule",
        "value": "Grant"
      },
      {
        "key": "ExpirationRule",
        "value": "Grant"
      },
      {
        "key": "MfaRule",
        "value": "Grant"
      },
      {
        "key": "JustificationRule",
        "value": "Grant"
      },
      {
        "key": "ActivationDayRule",
        "value": "Grant"
      },
      {
        "key": "ApprovalRule",
        "value": "Grant"
      }
    ]
  },
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:28:43.537Z",
    "endDateTime": "0001-01-01T00:00:00Z",
    "duration": "PT9H"
  }
}
```

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="9c024-299">Exemplo 3: o usuário desativa uma função atribuída</span><span class="sxs-lookup"><span data-stu-id="9c024-299">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="9c024-300">Neste exemplo, o usuário nawu@contoso.com desativa a função de Leitor de Cobrança ativa.</span><span class="sxs-lookup"><span data-stu-id="9c024-300">In this example, the user nawu@contoso.com deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="9c024-301">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c024-301">Property</span></span>         | <span data-ttu-id="9c024-302">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c024-302">Type</span></span>                                                     | <span data-ttu-id="9c024-303">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="9c024-303">Required</span></span> | <span data-ttu-id="9c024-304">Valor</span><span class="sxs-lookup"><span data-stu-id="9c024-304">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="9c024-305">resourceId</span><span class="sxs-lookup"><span data-stu-id="9c024-305">resourceId</span></span>       | <span data-ttu-id="9c024-306">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-306">String</span></span>                                                   | <span data-ttu-id="9c024-307">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-307">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="9c024-308">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="9c024-308">roleDefinitionId</span></span> | <span data-ttu-id="9c024-309">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-309">String</span></span>                                                   | <span data-ttu-id="9c024-310">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-310">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="9c024-311">subjectId</span><span class="sxs-lookup"><span data-stu-id="9c024-311">subjectId</span></span>        | <span data-ttu-id="9c024-312">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-312">String</span></span>                                                   | <span data-ttu-id="9c024-313">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-313">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="9c024-314">assignmentState</span><span class="sxs-lookup"><span data-stu-id="9c024-314">assignmentState</span></span>  | <span data-ttu-id="9c024-315">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-315">String</span></span>                                                   | <span data-ttu-id="9c024-316">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-316">Yes</span></span>      | <span data-ttu-id="9c024-317">Ativo</span><span class="sxs-lookup"><span data-stu-id="9c024-317">Active</span></span> |
| <span data-ttu-id="9c024-318">type</span><span class="sxs-lookup"><span data-stu-id="9c024-318">type</span></span>             | <span data-ttu-id="9c024-319">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-319">String</span></span>                                                   | <span data-ttu-id="9c024-320">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-320">Yes</span></span>      | <span data-ttu-id="9c024-321">UserRemove</span><span class="sxs-lookup"><span data-stu-id="9c024-321">UserRemove</span></span> |
| <span data-ttu-id="9c024-322">motivo</span><span class="sxs-lookup"><span data-stu-id="9c024-322">reason</span></span>           | <span data-ttu-id="9c024-323">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-323">String</span></span>                                                   | <span data-ttu-id="9c024-324">Não</span><span class="sxs-lookup"><span data-stu-id="9c024-324">No</span></span>       |   |
| <span data-ttu-id="9c024-325">Cronograma</span><span class="sxs-lookup"><span data-stu-id="9c024-325">schedule</span></span>         | [<span data-ttu-id="9c024-326">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="9c024-326">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="9c024-327">Não</span><span class="sxs-lookup"><span data-stu-id="9c024-327">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="9c024-328">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c024-328">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
  "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserRemove",
  "reason": "Deactivate the role",
  "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```

#### <a name="response"></a><span data-ttu-id="9c024-329">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c024-329">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "abfcdb57-8e5d-42a0-ae67-7598b96fddb1",
  "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
  "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec",
  "type": "UserRemove",
  "assignmentState": "Active",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "Evaluate only",
  "schedule": null,
  "status": {
    "status": "Closed",
    "subStatus": "Revoked",
    "statusDetails": []
  }
}
```

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="9c024-330">Exemplo 4: O administrador remove o usuário de uma função</span><span class="sxs-lookup"><span data-stu-id="9c024-330">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="9c024-331">Neste exemplo, um administrador remove o usuário nawu@contoso.com da função Leitor de Cobrança.</span><span class="sxs-lookup"><span data-stu-id="9c024-331">In this example, an administrator removes the user nawu@contoso.com from the Billing Reader role.</span></span>

 ><span data-ttu-id="9c024-332">**Observação:** Além da permissão, este exemplo exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` `owner` `user access administrator` (ou) no recurso.</span><span class="sxs-lookup"><span data-stu-id="9c024-332">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="9c024-333">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c024-333">Property</span></span>         | <span data-ttu-id="9c024-334">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c024-334">Type</span></span>                                                     | <span data-ttu-id="9c024-335">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="9c024-335">Required</span></span> | <span data-ttu-id="9c024-336">Valor</span><span class="sxs-lookup"><span data-stu-id="9c024-336">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="9c024-337">resourceId</span><span class="sxs-lookup"><span data-stu-id="9c024-337">resourceId</span></span>       | <span data-ttu-id="9c024-338">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-338">String</span></span>                                                   | <span data-ttu-id="9c024-339">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-339">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="9c024-340">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="9c024-340">roleDefinitionId</span></span> | <span data-ttu-id="9c024-341">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-341">String</span></span>                                                   | <span data-ttu-id="9c024-342">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-342">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="9c024-343">subjectId</span><span class="sxs-lookup"><span data-stu-id="9c024-343">subjectId</span></span>        | <span data-ttu-id="9c024-344">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-344">String</span></span>                                                   | <span data-ttu-id="9c024-345">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-345">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="9c024-346">assignmentState</span><span class="sxs-lookup"><span data-stu-id="9c024-346">assignmentState</span></span>  | <span data-ttu-id="9c024-347">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-347">String</span></span>                                                   | <span data-ttu-id="9c024-348">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-348">Yes</span></span>      | <span data-ttu-id="9c024-349">Qualificado/Ativo</span><span class="sxs-lookup"><span data-stu-id="9c024-349">Eligible / Active</span></span> |
| <span data-ttu-id="9c024-350">type</span><span class="sxs-lookup"><span data-stu-id="9c024-350">type</span></span>             | <span data-ttu-id="9c024-351">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-351">String</span></span>                                                   | <span data-ttu-id="9c024-352">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-352">Yes</span></span>      | <span data-ttu-id="9c024-353">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="9c024-353">AdminRemove</span></span> |
| <span data-ttu-id="9c024-354">motivo</span><span class="sxs-lookup"><span data-stu-id="9c024-354">reason</span></span>           | <span data-ttu-id="9c024-355">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-355">String</span></span>                                                   | <span data-ttu-id="9c024-356">Não</span><span class="sxs-lookup"><span data-stu-id="9c024-356">No</span></span>       |   |
| <span data-ttu-id="9c024-357">Cronograma</span><span class="sxs-lookup"><span data-stu-id="9c024-357">schedule</span></span>         | [<span data-ttu-id="9c024-358">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="9c024-358">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="9c024-359">Não</span><span class="sxs-lookup"><span data-stu-id="9c024-359">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="9c024-360">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c024-360">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminRemove"
}
```

#### <a name="response"></a><span data-ttu-id="9c024-361">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c024-361">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminRemove",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
  "status": {
    "status": "Closed",
    "subStatus": "Revoked",
    "statusDetails": []
  },
  "schedule": null
}
```

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="9c024-362">Exemplo 5: O administrador atualiza a atribuição de função</span><span class="sxs-lookup"><span data-stu-id="9c024-362">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="9c024-363">Neste exemplo, os administradores atualizam a atribuição de função do usuário nawu@contoso.com para Proprietário.</span><span class="sxs-lookup"><span data-stu-id="9c024-363">In this example, administrators update the role assignment for the user nawu@contoso.com to Owner.</span></span>

 ><span data-ttu-id="9c024-364">**Observação:** Além da permissão, este exemplo exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` `owner` `user access administrator` (ou) no recurso.</span><span class="sxs-lookup"><span data-stu-id="9c024-364">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="9c024-365">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c024-365">Property</span></span>         | <span data-ttu-id="9c024-366">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c024-366">Type</span></span>                                                     | <span data-ttu-id="9c024-367">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="9c024-367">Required</span></span>                | <span data-ttu-id="9c024-368">Valor</span><span class="sxs-lookup"><span data-stu-id="9c024-368">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="9c024-369">resourceId</span><span class="sxs-lookup"><span data-stu-id="9c024-369">resourceId</span></span>       | <span data-ttu-id="9c024-370">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-370">String</span></span>                                                   | <span data-ttu-id="9c024-371">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-371">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="9c024-372">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="9c024-372">roleDefinitionId</span></span> | <span data-ttu-id="9c024-373">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-373">String</span></span>                                                   | <span data-ttu-id="9c024-374">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-374">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="9c024-375">subjectId</span><span class="sxs-lookup"><span data-stu-id="9c024-375">subjectId</span></span>        | <span data-ttu-id="9c024-376">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-376">String</span></span>                                                   | <span data-ttu-id="9c024-377">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-377">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="9c024-378">assignmentState</span><span class="sxs-lookup"><span data-stu-id="9c024-378">assignmentState</span></span>  | <span data-ttu-id="9c024-379">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-379">String</span></span>                                                   | <span data-ttu-id="9c024-380">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-380">Yes</span></span>                     | <span data-ttu-id="9c024-381">Qualificado/Ativo</span><span class="sxs-lookup"><span data-stu-id="9c024-381">Eligible / Active</span></span> |
| <span data-ttu-id="9c024-382">type</span><span class="sxs-lookup"><span data-stu-id="9c024-382">type</span></span>             | <span data-ttu-id="9c024-383">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-383">String</span></span>                                                   | <span data-ttu-id="9c024-384">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-384">Yes</span></span>                     | <span data-ttu-id="9c024-385">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="9c024-385">AdminUpdate</span></span> |
| <span data-ttu-id="9c024-386">motivo</span><span class="sxs-lookup"><span data-stu-id="9c024-386">reason</span></span>           | <span data-ttu-id="9c024-387">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-387">String</span></span>                                                   | <span data-ttu-id="9c024-388">depende de roleSettings</span><span class="sxs-lookup"><span data-stu-id="9c024-388">depends on roleSettings</span></span> |   |
| <span data-ttu-id="9c024-389">Cronograma</span><span class="sxs-lookup"><span data-stu-id="9c024-389">schedule</span></span>         | [<span data-ttu-id="9c024-390">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="9c024-390">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="9c024-391">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-391">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="9c024-392">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c024-392">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState": "Eligible",
  "type": "AdminUpdate",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31.000Z"
  }
}
```

#### <a name="response"></a><span data-ttu-id="9c024-393">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c024-393">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminUpdate",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
  "status": {
    "status": "InProgress",
    "subStatus": "Granted",
    "statusDetails": [
      {
        "key": "AdminRequestRule",
        "value": "Grant"
      },
      {
        "key": "ExpirationRule",
        "value": "Grant"
      },
      {
        "key": "MfaRule",
        "value": "Grant"
      }
    ]
  },
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31Z",
    "duration": "PT0S"
  }
}
```

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="9c024-394">Exemplo 6: O administrador estende a atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="9c024-394">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="9c024-395">Este exemplo estende a atribuição de função expirada para o usuário ANUJCUSER para o Colaborador do Serviço de Gerenciamento de API.</span><span class="sxs-lookup"><span data-stu-id="9c024-395">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="9c024-396">**Observação:** Além da permissão, este exemplo exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` `owner` `user access administrator` (ou) no recurso.</span><span class="sxs-lookup"><span data-stu-id="9c024-396">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="9c024-397">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c024-397">Property</span></span>         | <span data-ttu-id="9c024-398">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c024-398">Type</span></span>                                                     | <span data-ttu-id="9c024-399">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="9c024-399">Required</span></span>                | <span data-ttu-id="9c024-400">Valor</span><span class="sxs-lookup"><span data-stu-id="9c024-400">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="9c024-401">resourceId</span><span class="sxs-lookup"><span data-stu-id="9c024-401">resourceId</span></span>       | <span data-ttu-id="9c024-402">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-402">String</span></span>                                                   | <span data-ttu-id="9c024-403">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-403">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="9c024-404">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="9c024-404">roleDefinitionId</span></span> | <span data-ttu-id="9c024-405">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-405">String</span></span>                                                   | <span data-ttu-id="9c024-406">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-406">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="9c024-407">subjectId</span><span class="sxs-lookup"><span data-stu-id="9c024-407">subjectId</span></span>        | <span data-ttu-id="9c024-408">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-408">String</span></span>                                                   | <span data-ttu-id="9c024-409">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-409">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="9c024-410">assignmentState</span><span class="sxs-lookup"><span data-stu-id="9c024-410">assignmentState</span></span>  | <span data-ttu-id="9c024-411">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-411">String</span></span>                                                   | <span data-ttu-id="9c024-412">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-412">Yes</span></span>                     | <span data-ttu-id="9c024-413">Qualificado/Ativo</span><span class="sxs-lookup"><span data-stu-id="9c024-413">Eligible / Active</span></span> |
| <span data-ttu-id="9c024-414">type</span><span class="sxs-lookup"><span data-stu-id="9c024-414">type</span></span>             | <span data-ttu-id="9c024-415">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-415">String</span></span>                                                   | <span data-ttu-id="9c024-416">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-416">Yes</span></span>                     | <span data-ttu-id="9c024-417">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="9c024-417">AdminExtend</span></span> |
| <span data-ttu-id="9c024-418">motivo</span><span class="sxs-lookup"><span data-stu-id="9c024-418">reason</span></span>           | <span data-ttu-id="9c024-419">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c024-419">String</span></span>                                                   | <span data-ttu-id="9c024-420">depende de roleSettings</span><span class="sxs-lookup"><span data-stu-id="9c024-420">depends on roleSettings</span></span> |   |
| <span data-ttu-id="9c024-421">Cronograma</span><span class="sxs-lookup"><span data-stu-id="9c024-421">schedule</span></span>         | [<span data-ttu-id="9c024-422">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="9c024-422">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="9c024-423">Sim</span><span class="sxs-lookup"><span data-stu-id="9c024-423">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="9c024-424">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c024-424">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminExtend",
  "reason": "extend role assignment",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z"
  }
}
```

#### <a name="response"></a><span data-ttu-id="9c024-425">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c024-425">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminExtend",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "extend role assignment",
  "status": {
    "status": "InProgress",
    "subStatus": "Granted",
    "statusDetails": [
      {
        "key": "AdminRequestRule",
        "value": "Grant"
      },
      {
        "key": "ExpirationRule",
        "value": "Grant"
      },
      {
        "key": "MfaRule",
        "value": "Grant"
      }
    ]
  },
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z",
    "duration": "PT0S"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


