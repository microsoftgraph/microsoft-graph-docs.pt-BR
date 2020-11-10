---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função. A tabela a seguir lista as operações.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 76829c502e83b4218241df74d9fc51e43c0eeb86
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965458"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="14749-104">Criar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="14749-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="14749-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14749-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14749-106">Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="14749-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="14749-107">A tabela a seguir lista as operações.</span><span class="sxs-lookup"><span data-stu-id="14749-107">The following table lists the operations.</span></span>

| <span data-ttu-id="14749-108">Operation</span><span class="sxs-lookup"><span data-stu-id="14749-108">Operation</span></span>                                   | <span data-ttu-id="14749-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="14749-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="14749-110">Atribuir uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="14749-110">Assign a role assignment</span></span>                    | <span data-ttu-id="14749-111">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="14749-111">AdminAdd</span></span>    |
| <span data-ttu-id="14749-112">Ativar uma atribuição de função qualificada</span><span class="sxs-lookup"><span data-stu-id="14749-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="14749-113">UserAdd</span><span class="sxs-lookup"><span data-stu-id="14749-113">UserAdd</span></span>     |
| <span data-ttu-id="14749-114">Desativar uma atribuição de função ativada</span><span class="sxs-lookup"><span data-stu-id="14749-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="14749-115">Userremove</span><span class="sxs-lookup"><span data-stu-id="14749-115">UserRemove</span></span>  |
| <span data-ttu-id="14749-116">Remover uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="14749-116">Remove a role assignment</span></span>                    | <span data-ttu-id="14749-117">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="14749-117">AdminRemove</span></span> |
| <span data-ttu-id="14749-118">Atualizar uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="14749-118">Update a role assignment</span></span>                    | <span data-ttu-id="14749-119">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="14749-119">AdminUpdate</span></span> |
| <span data-ttu-id="14749-120">Solicitação para estender minha atribuição de função</span><span class="sxs-lookup"><span data-stu-id="14749-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="14749-121">Userextend</span><span class="sxs-lookup"><span data-stu-id="14749-121">UserExtend</span></span>  |
| <span data-ttu-id="14749-122">Estender uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="14749-122">Extend a role assignment</span></span>                    | <span data-ttu-id="14749-123">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="14749-123">AdminExtend</span></span> |
| <span data-ttu-id="14749-124">Solicitação para renovar minha atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="14749-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="14749-125">Userrenew</span><span class="sxs-lookup"><span data-stu-id="14749-125">UserRenew</span></span>   |
| <span data-ttu-id="14749-126">Renovar uma atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="14749-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="14749-127">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="14749-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="14749-128">Permissões</span><span class="sxs-lookup"><span data-stu-id="14749-128">Permissions</span></span>

<span data-ttu-id="14749-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="14749-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="14749-131">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="14749-131">Azure resources</span></span>

| <span data-ttu-id="14749-132">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14749-132">Permission type</span></span> | <span data-ttu-id="14749-133">Permissões</span><span class="sxs-lookup"><span data-stu-id="14749-133">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="14749-134">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14749-134">Delegated (work or school account)</span></span> | <span data-ttu-id="14749-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="14749-135">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="14749-136">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14749-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14749-137">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14749-137">Not supported.</span></span> |
| <span data-ttu-id="14749-138">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14749-138">Application</span></span> | <span data-ttu-id="14749-139">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14749-139">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="14749-140">Azure AD</span><span class="sxs-lookup"><span data-stu-id="14749-140">Azure AD</span></span>

| <span data-ttu-id="14749-141">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14749-141">Permission type</span></span> | <span data-ttu-id="14749-142">Permissões</span><span class="sxs-lookup"><span data-stu-id="14749-142">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="14749-143">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14749-143">Delegated (work or school account)</span></span> | <span data-ttu-id="14749-144">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="14749-144">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="14749-145">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14749-145">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14749-146">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14749-146">Not supported.</span></span> |
| <span data-ttu-id="14749-147">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14749-147">Application</span></span> | <span data-ttu-id="14749-148">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14749-148">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="14749-149">Grupos</span><span class="sxs-lookup"><span data-stu-id="14749-149">Groups</span></span>

|<span data-ttu-id="14749-150">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14749-150">Permission type</span></span> | <span data-ttu-id="14749-151">Permissões</span><span class="sxs-lookup"><span data-stu-id="14749-151">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="14749-152">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14749-152">Delegated (work or school account)</span></span> | <span data-ttu-id="14749-153">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="14749-153">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="14749-154">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14749-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14749-155">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14749-155">Not supported.</span></span> |
| <span data-ttu-id="14749-156">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14749-156">Application</span></span> | <span data-ttu-id="14749-157">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14749-157">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="14749-158">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14749-158">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="14749-159">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14749-159">Request headers</span></span>

| <span data-ttu-id="14749-160">Nome</span><span class="sxs-lookup"><span data-stu-id="14749-160">Name</span></span>          | <span data-ttu-id="14749-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="14749-161">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="14749-162">Authorization</span><span class="sxs-lookup"><span data-stu-id="14749-162">Authorization</span></span> | <span data-ttu-id="14749-163">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="14749-163">Bearer {code}</span></span>    |
| <span data-ttu-id="14749-164">Content-type</span><span class="sxs-lookup"><span data-stu-id="14749-164">Content-type</span></span>  | <span data-ttu-id="14749-165">application/json</span><span class="sxs-lookup"><span data-stu-id="14749-165">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="14749-166">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14749-166">Request body</span></span>

<span data-ttu-id="14749-167">No corpo da solicitação, forneça uma representação JSON de um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="14749-167">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="14749-168">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14749-168">Property</span></span>         | <span data-ttu-id="14749-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="14749-169">Type</span></span>                                                     | <span data-ttu-id="14749-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="14749-170">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="14749-171">resourceId</span><span class="sxs-lookup"><span data-stu-id="14749-171">resourceId</span></span>       | <span data-ttu-id="14749-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14749-172">String</span></span>                                                   | <span data-ttu-id="14749-173">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="14749-173">The ID of the resource.</span></span> <span data-ttu-id="14749-174">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14749-174">Required.</span></span> |
| <span data-ttu-id="14749-175">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="14749-175">roleDefinitionId</span></span> | <span data-ttu-id="14749-176">String</span><span class="sxs-lookup"><span data-stu-id="14749-176">String</span></span>                                                   | <span data-ttu-id="14749-177">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="14749-177">The ID of the role definition.</span></span> <span data-ttu-id="14749-178">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14749-178">Required.</span></span> |
| <span data-ttu-id="14749-179">SubjectID</span><span class="sxs-lookup"><span data-stu-id="14749-179">subjectId</span></span>        | <span data-ttu-id="14749-180">String</span><span class="sxs-lookup"><span data-stu-id="14749-180">String</span></span>                                                   | <span data-ttu-id="14749-181">A ID do assunto.</span><span class="sxs-lookup"><span data-stu-id="14749-181">The ID of the subject.</span></span> <span data-ttu-id="14749-182">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14749-182">Required.</span></span> |
| <span data-ttu-id="14749-183">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="14749-183">assignmentState</span></span>  | <span data-ttu-id="14749-184">String</span><span class="sxs-lookup"><span data-stu-id="14749-184">String</span></span>                                                   | <span data-ttu-id="14749-185">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="14749-185">The state of assignment.</span></span> <span data-ttu-id="14749-186">O valor pode ser `Eligible` e `Active` .</span><span class="sxs-lookup"><span data-stu-id="14749-186">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="14749-187">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14749-187">Required.</span></span> |
| <span data-ttu-id="14749-188">tipo</span><span class="sxs-lookup"><span data-stu-id="14749-188">type</span></span>             | <span data-ttu-id="14749-189">String</span><span class="sxs-lookup"><span data-stu-id="14749-189">String</span></span>                                                   | <span data-ttu-id="14749-190">O tipo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14749-190">The request type.</span></span> <span data-ttu-id="14749-191">O valor pode ser,,,,,, `AdminAdd` `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew` `AdminRenew` e `AdminExtend` .</span><span class="sxs-lookup"><span data-stu-id="14749-191">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="14749-192">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14749-192">Required.</span></span> |
| <span data-ttu-id="14749-193">motivo</span><span class="sxs-lookup"><span data-stu-id="14749-193">reason</span></span>           | <span data-ttu-id="14749-194">String</span><span class="sxs-lookup"><span data-stu-id="14749-194">String</span></span>                                                   | <span data-ttu-id="14749-195">O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e análise.</span><span class="sxs-lookup"><span data-stu-id="14749-195">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="14749-196">Cronograma</span><span class="sxs-lookup"><span data-stu-id="14749-196">schedule</span></span>         | [<span data-ttu-id="14749-197">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="14749-197">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="14749-198">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="14749-198">The schedule of the role assignment request.</span></span> <span data-ttu-id="14749-199">Para o tipo de solicitação de,,, `UserAdd` `AdminAdd` `AdminUpdate` e `AdminExtend` , é necessário.</span><span class="sxs-lookup"><span data-stu-id="14749-199">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="14749-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="14749-200">Response</span></span>

<span data-ttu-id="14749-201">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14749-201">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="14749-202">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="14749-202">Error codes</span></span>

<span data-ttu-id="14749-203">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="14749-203">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="14749-204">Além disso, ele também retorna os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="14749-204">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="14749-205">Código de erro</span><span class="sxs-lookup"><span data-stu-id="14749-205">Error code</span></span>     | <span data-ttu-id="14749-206">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="14749-206">Error message</span></span>                               | <span data-ttu-id="14749-207">Detalhes</span><span class="sxs-lookup"><span data-stu-id="14749-207">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="14749-208">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="14749-208">400 BadRequest</span></span> | <span data-ttu-id="14749-209">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="14749-209">RoleNotFound</span></span>                                | <span data-ttu-id="14749-210">O `roleDefinitionId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="14749-210">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="14749-211">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="14749-211">400 BadRequest</span></span> | <span data-ttu-id="14749-212">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="14749-212">ResourceIsLocked</span></span>                            | <span data-ttu-id="14749-213">O recurso fornecido no corpo da solicitação está no estado de `Locked` e não pode criar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="14749-213">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="14749-214">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="14749-214">400 BadRequest</span></span> | <span data-ttu-id="14749-215">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="14749-215">SubjectNotFound</span></span>                             | <span data-ttu-id="14749-216">O `subjectId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="14749-216">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="14749-217">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="14749-217">400 BadRequest</span></span> | <span data-ttu-id="14749-218">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="14749-218">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="14749-219">Já existe um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) pendente no sistema.</span><span class="sxs-lookup"><span data-stu-id="14749-219">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="14749-220">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="14749-220">400 BadRequest</span></span> | <span data-ttu-id="14749-221">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="14749-221">RoleAssignmentExists</span></span>                        | <span data-ttu-id="14749-222">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criado já existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="14749-222">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="14749-223">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="14749-223">400 BadRequest</span></span> | <span data-ttu-id="14749-224">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="14749-224">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="14749-225">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="14749-225">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="14749-226">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="14749-226">400 BadRequest</span></span> | <span data-ttu-id="14749-227">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="14749-227">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="14749-228">O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não atende às políticas internas e não pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="14749-228">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="14749-229">Exemplos</span><span class="sxs-lookup"><span data-stu-id="14749-229">Examples</span></span>

<span data-ttu-id="14749-230">Os exemplos a seguir mostram como usar essa API.</span><span class="sxs-lookup"><span data-stu-id="14749-230">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="14749-231">Exemplo 1: o administrador atribui um usuário a uma função</span><span class="sxs-lookup"><span data-stu-id="14749-231">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="14749-232">Neste exemplo, um administrador atribui o usuário nawu@fimdev.net à função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="14749-232">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="14749-233">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma atribuição de `Active` função de administrador ( `owner` ou `user access administrator` ) no recurso.</span><span class="sxs-lookup"><span data-stu-id="14749-233">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="14749-234">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14749-234">Property</span></span>         | <span data-ttu-id="14749-235">Tipo</span><span class="sxs-lookup"><span data-stu-id="14749-235">Type</span></span>                                                     | <span data-ttu-id="14749-236">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="14749-236">Required</span></span>                 | <span data-ttu-id="14749-237">Valor</span><span class="sxs-lookup"><span data-stu-id="14749-237">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="14749-238">resourceId</span><span class="sxs-lookup"><span data-stu-id="14749-238">resourceId</span></span>       | <span data-ttu-id="14749-239">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14749-239">String</span></span>                                                   | <span data-ttu-id="14749-240">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-240">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="14749-241">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="14749-241">roleDefinitionId</span></span> | <span data-ttu-id="14749-242">String</span><span class="sxs-lookup"><span data-stu-id="14749-242">String</span></span>                                                   | <span data-ttu-id="14749-243">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-243">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="14749-244">SubjectID</span><span class="sxs-lookup"><span data-stu-id="14749-244">subjectId</span></span>        | <span data-ttu-id="14749-245">String</span><span class="sxs-lookup"><span data-stu-id="14749-245">String</span></span>                                                   | <span data-ttu-id="14749-246">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-246">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="14749-247">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="14749-247">assignmentState</span></span>  | <span data-ttu-id="14749-248">String</span><span class="sxs-lookup"><span data-stu-id="14749-248">String</span></span>                                                   | <span data-ttu-id="14749-249">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-249">Yes</span></span>                      | <span data-ttu-id="14749-250">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="14749-250">Eligible / Active</span></span> |
| <span data-ttu-id="14749-251">tipo</span><span class="sxs-lookup"><span data-stu-id="14749-251">type</span></span>             | <span data-ttu-id="14749-252">String</span><span class="sxs-lookup"><span data-stu-id="14749-252">String</span></span>                                                   | <span data-ttu-id="14749-253">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-253">Yes</span></span>                      | <span data-ttu-id="14749-254">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="14749-254">AdminAdd</span></span> |
| <span data-ttu-id="14749-255">motivo</span><span class="sxs-lookup"><span data-stu-id="14749-255">reason</span></span>           | <span data-ttu-id="14749-256">String</span><span class="sxs-lookup"><span data-stu-id="14749-256">String</span></span>                                                   | <span data-ttu-id="14749-257">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="14749-257">depends on role Settings</span></span> |   |
| <span data-ttu-id="14749-258">Cronograma</span><span class="sxs-lookup"><span data-stu-id="14749-258">schedule</span></span>         | [<span data-ttu-id="14749-259">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="14749-259">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="14749-260">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-260">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="14749-261">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14749-261">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="14749-262">HTTP</span><span class="sxs-lookup"><span data-stu-id="14749-262">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="14749-263">C#</span><span class="sxs-lookup"><span data-stu-id="14749-263">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14749-264">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14749-264">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14749-265">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14749-265">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14749-266">Java</span><span class="sxs-lookup"><span data-stu-id="14749-266">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="14749-267">Resposta</span><span class="sxs-lookup"><span data-stu-id="14749-267">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="14749-268">Exemplo 2: o usuário ativa a função qualificada</span><span class="sxs-lookup"><span data-stu-id="14749-268">Example 2: User activates eligible role</span></span>

<span data-ttu-id="14749-269">Neste exemplo, o usuário nawu@fimdev.net ativa a função de leitor de cobrança qualificado.</span><span class="sxs-lookup"><span data-stu-id="14749-269">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="14749-270">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14749-270">Property</span></span>         | <span data-ttu-id="14749-271">Tipo</span><span class="sxs-lookup"><span data-stu-id="14749-271">Type</span></span>                                                     | <span data-ttu-id="14749-272">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="14749-272">Required</span></span>                 | <span data-ttu-id="14749-273">Valor</span><span class="sxs-lookup"><span data-stu-id="14749-273">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="14749-274">resourceId</span><span class="sxs-lookup"><span data-stu-id="14749-274">resourceId</span></span>       | <span data-ttu-id="14749-275">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14749-275">String</span></span>                                                   | <span data-ttu-id="14749-276">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-276">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="14749-277">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="14749-277">roleDefinitionId</span></span> | <span data-ttu-id="14749-278">String</span><span class="sxs-lookup"><span data-stu-id="14749-278">String</span></span>                                                   | <span data-ttu-id="14749-279">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-279">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="14749-280">SubjectID</span><span class="sxs-lookup"><span data-stu-id="14749-280">subjectId</span></span>        | <span data-ttu-id="14749-281">String</span><span class="sxs-lookup"><span data-stu-id="14749-281">String</span></span>                                                   | <span data-ttu-id="14749-282">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-282">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="14749-283">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="14749-283">assignmentState</span></span>  | <span data-ttu-id="14749-284">String</span><span class="sxs-lookup"><span data-stu-id="14749-284">String</span></span>                                                   | <span data-ttu-id="14749-285">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-285">Yes</span></span>                      | <span data-ttu-id="14749-286">Ativo</span><span class="sxs-lookup"><span data-stu-id="14749-286">Active</span></span> |
| <span data-ttu-id="14749-287">tipo</span><span class="sxs-lookup"><span data-stu-id="14749-287">type</span></span>             | <span data-ttu-id="14749-288">String</span><span class="sxs-lookup"><span data-stu-id="14749-288">String</span></span>                                                   | <span data-ttu-id="14749-289">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-289">Yes</span></span>                      | <span data-ttu-id="14749-290">UserAdd</span><span class="sxs-lookup"><span data-stu-id="14749-290">UserAdd</span></span> |
| <span data-ttu-id="14749-291">motivo</span><span class="sxs-lookup"><span data-stu-id="14749-291">reason</span></span>           | <span data-ttu-id="14749-292">String</span><span class="sxs-lookup"><span data-stu-id="14749-292">String</span></span>                                                   | <span data-ttu-id="14749-293">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="14749-293">depends on role Settings</span></span> |   |
| <span data-ttu-id="14749-294">Cronograma</span><span class="sxs-lookup"><span data-stu-id="14749-294">schedule</span></span>         | [<span data-ttu-id="14749-295">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="14749-295">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="14749-296">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-296">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="14749-297">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14749-297">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="14749-298">Resposta</span><span class="sxs-lookup"><span data-stu-id="14749-298">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="14749-299">Exemplo 3: o usuário desativa uma função atribuída</span><span class="sxs-lookup"><span data-stu-id="14749-299">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="14749-300">Neste exemplo, o usuário nawu@fimdev.net desativa a função de leitor de cobrança ativa.</span><span class="sxs-lookup"><span data-stu-id="14749-300">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="14749-301">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14749-301">Property</span></span>         | <span data-ttu-id="14749-302">Tipo</span><span class="sxs-lookup"><span data-stu-id="14749-302">Type</span></span>                                                     | <span data-ttu-id="14749-303">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="14749-303">Required</span></span> | <span data-ttu-id="14749-304">Valor</span><span class="sxs-lookup"><span data-stu-id="14749-304">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="14749-305">resourceId</span><span class="sxs-lookup"><span data-stu-id="14749-305">resourceId</span></span>       | <span data-ttu-id="14749-306">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14749-306">String</span></span>                                                   | <span data-ttu-id="14749-307">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-307">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="14749-308">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="14749-308">roleDefinitionId</span></span> | <span data-ttu-id="14749-309">String</span><span class="sxs-lookup"><span data-stu-id="14749-309">String</span></span>                                                   | <span data-ttu-id="14749-310">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-310">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="14749-311">SubjectID</span><span class="sxs-lookup"><span data-stu-id="14749-311">subjectId</span></span>        | <span data-ttu-id="14749-312">String</span><span class="sxs-lookup"><span data-stu-id="14749-312">String</span></span>                                                   | <span data-ttu-id="14749-313">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-313">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="14749-314">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="14749-314">assignmentState</span></span>  | <span data-ttu-id="14749-315">String</span><span class="sxs-lookup"><span data-stu-id="14749-315">String</span></span>                                                   | <span data-ttu-id="14749-316">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-316">Yes</span></span>      | <span data-ttu-id="14749-317">Ativo</span><span class="sxs-lookup"><span data-stu-id="14749-317">Active</span></span> |
| <span data-ttu-id="14749-318">tipo</span><span class="sxs-lookup"><span data-stu-id="14749-318">type</span></span>             | <span data-ttu-id="14749-319">String</span><span class="sxs-lookup"><span data-stu-id="14749-319">String</span></span>                                                   | <span data-ttu-id="14749-320">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-320">Yes</span></span>      | <span data-ttu-id="14749-321">Userremove</span><span class="sxs-lookup"><span data-stu-id="14749-321">UserRemove</span></span> |
| <span data-ttu-id="14749-322">motivo</span><span class="sxs-lookup"><span data-stu-id="14749-322">reason</span></span>           | <span data-ttu-id="14749-323">String</span><span class="sxs-lookup"><span data-stu-id="14749-323">String</span></span>                                                   | <span data-ttu-id="14749-324">Não</span><span class="sxs-lookup"><span data-stu-id="14749-324">No</span></span>       |   |
| <span data-ttu-id="14749-325">Cronograma</span><span class="sxs-lookup"><span data-stu-id="14749-325">schedule</span></span>         | [<span data-ttu-id="14749-326">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="14749-326">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="14749-327">Não</span><span class="sxs-lookup"><span data-stu-id="14749-327">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="14749-328">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14749-328">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="14749-329">Resposta</span><span class="sxs-lookup"><span data-stu-id="14749-329">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="14749-330">Exemplo 4: o administrador remove o usuário de uma função</span><span class="sxs-lookup"><span data-stu-id="14749-330">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="14749-331">Neste exemplo, um administrador remove o usuário nawu@fimdev.net da função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="14749-331">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="14749-332">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma atribuição de `Active` função de administrador ( `owner` ou `user access administrator` ) no recurso.</span><span class="sxs-lookup"><span data-stu-id="14749-332">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="14749-333">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14749-333">Property</span></span>         | <span data-ttu-id="14749-334">Tipo</span><span class="sxs-lookup"><span data-stu-id="14749-334">Type</span></span>                                                     | <span data-ttu-id="14749-335">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="14749-335">Required</span></span> | <span data-ttu-id="14749-336">Valor</span><span class="sxs-lookup"><span data-stu-id="14749-336">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="14749-337">resourceId</span><span class="sxs-lookup"><span data-stu-id="14749-337">resourceId</span></span>       | <span data-ttu-id="14749-338">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14749-338">String</span></span>                                                   | <span data-ttu-id="14749-339">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-339">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="14749-340">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="14749-340">roleDefinitionId</span></span> | <span data-ttu-id="14749-341">String</span><span class="sxs-lookup"><span data-stu-id="14749-341">String</span></span>                                                   | <span data-ttu-id="14749-342">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-342">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="14749-343">SubjectID</span><span class="sxs-lookup"><span data-stu-id="14749-343">subjectId</span></span>        | <span data-ttu-id="14749-344">String</span><span class="sxs-lookup"><span data-stu-id="14749-344">String</span></span>                                                   | <span data-ttu-id="14749-345">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-345">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="14749-346">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="14749-346">assignmentState</span></span>  | <span data-ttu-id="14749-347">String</span><span class="sxs-lookup"><span data-stu-id="14749-347">String</span></span>                                                   | <span data-ttu-id="14749-348">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-348">Yes</span></span>      | <span data-ttu-id="14749-349">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="14749-349">Eligible / Active</span></span> |
| <span data-ttu-id="14749-350">tipo</span><span class="sxs-lookup"><span data-stu-id="14749-350">type</span></span>             | <span data-ttu-id="14749-351">String</span><span class="sxs-lookup"><span data-stu-id="14749-351">String</span></span>                                                   | <span data-ttu-id="14749-352">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-352">Yes</span></span>      | <span data-ttu-id="14749-353">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="14749-353">AdminRemove</span></span> |
| <span data-ttu-id="14749-354">motivo</span><span class="sxs-lookup"><span data-stu-id="14749-354">reason</span></span>           | <span data-ttu-id="14749-355">String</span><span class="sxs-lookup"><span data-stu-id="14749-355">String</span></span>                                                   | <span data-ttu-id="14749-356">Não</span><span class="sxs-lookup"><span data-stu-id="14749-356">No</span></span>       |   |
| <span data-ttu-id="14749-357">Cronograma</span><span class="sxs-lookup"><span data-stu-id="14749-357">schedule</span></span>         | [<span data-ttu-id="14749-358">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="14749-358">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="14749-359">Não</span><span class="sxs-lookup"><span data-stu-id="14749-359">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="14749-360">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14749-360">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="14749-361">Resposta</span><span class="sxs-lookup"><span data-stu-id="14749-361">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="14749-362">Exemplo 5: atribuição de função de atualização do administrador</span><span class="sxs-lookup"><span data-stu-id="14749-362">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="14749-363">Neste exemplo, os administradores atualizam a atribuição de função para o usuário nawu@fimdev.net para o proprietário.</span><span class="sxs-lookup"><span data-stu-id="14749-363">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="14749-364">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma atribuição de `Active` função de administrador ( `owner` ou `user access administrator` ) no recurso.</span><span class="sxs-lookup"><span data-stu-id="14749-364">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="14749-365">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14749-365">Property</span></span>         | <span data-ttu-id="14749-366">Tipo</span><span class="sxs-lookup"><span data-stu-id="14749-366">Type</span></span>                                                     | <span data-ttu-id="14749-367">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="14749-367">Required</span></span>                | <span data-ttu-id="14749-368">Valor</span><span class="sxs-lookup"><span data-stu-id="14749-368">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="14749-369">resourceId</span><span class="sxs-lookup"><span data-stu-id="14749-369">resourceId</span></span>       | <span data-ttu-id="14749-370">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14749-370">String</span></span>                                                   | <span data-ttu-id="14749-371">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-371">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="14749-372">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="14749-372">roleDefinitionId</span></span> | <span data-ttu-id="14749-373">String</span><span class="sxs-lookup"><span data-stu-id="14749-373">String</span></span>                                                   | <span data-ttu-id="14749-374">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-374">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="14749-375">SubjectID</span><span class="sxs-lookup"><span data-stu-id="14749-375">subjectId</span></span>        | <span data-ttu-id="14749-376">String</span><span class="sxs-lookup"><span data-stu-id="14749-376">String</span></span>                                                   | <span data-ttu-id="14749-377">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-377">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="14749-378">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="14749-378">assignmentState</span></span>  | <span data-ttu-id="14749-379">String</span><span class="sxs-lookup"><span data-stu-id="14749-379">String</span></span>                                                   | <span data-ttu-id="14749-380">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-380">Yes</span></span>                     | <span data-ttu-id="14749-381">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="14749-381">Eligible / Active</span></span> |
| <span data-ttu-id="14749-382">tipo</span><span class="sxs-lookup"><span data-stu-id="14749-382">type</span></span>             | <span data-ttu-id="14749-383">String</span><span class="sxs-lookup"><span data-stu-id="14749-383">String</span></span>                                                   | <span data-ttu-id="14749-384">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-384">Yes</span></span>                     | <span data-ttu-id="14749-385">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="14749-385">AdminUpdate</span></span> |
| <span data-ttu-id="14749-386">motivo</span><span class="sxs-lookup"><span data-stu-id="14749-386">reason</span></span>           | <span data-ttu-id="14749-387">String</span><span class="sxs-lookup"><span data-stu-id="14749-387">String</span></span>                                                   | <span data-ttu-id="14749-388">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="14749-388">depends on roleSettings</span></span> |   |
| <span data-ttu-id="14749-389">Cronograma</span><span class="sxs-lookup"><span data-stu-id="14749-389">schedule</span></span>         | [<span data-ttu-id="14749-390">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="14749-390">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="14749-391">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-391">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="14749-392">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14749-392">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="14749-393">Resposta</span><span class="sxs-lookup"><span data-stu-id="14749-393">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="14749-394">Exemplo 6: administrador estende a atribuição de função de expiração</span><span class="sxs-lookup"><span data-stu-id="14749-394">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="14749-395">Este exemplo estende a atribuição de função de expiração para o usuário ANUJCUSER para o colaborador do serviço de gerenciamento de API.</span><span class="sxs-lookup"><span data-stu-id="14749-395">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="14749-396">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma atribuição de `Active` função de administrador ( `owner` ou `user access administrator` ) no recurso.</span><span class="sxs-lookup"><span data-stu-id="14749-396">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="14749-397">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14749-397">Property</span></span>         | <span data-ttu-id="14749-398">Tipo</span><span class="sxs-lookup"><span data-stu-id="14749-398">Type</span></span>                                                     | <span data-ttu-id="14749-399">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="14749-399">Required</span></span>                | <span data-ttu-id="14749-400">Valor</span><span class="sxs-lookup"><span data-stu-id="14749-400">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="14749-401">resourceId</span><span class="sxs-lookup"><span data-stu-id="14749-401">resourceId</span></span>       | <span data-ttu-id="14749-402">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14749-402">String</span></span>                                                   | <span data-ttu-id="14749-403">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-403">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="14749-404">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="14749-404">roleDefinitionId</span></span> | <span data-ttu-id="14749-405">String</span><span class="sxs-lookup"><span data-stu-id="14749-405">String</span></span>                                                   | <span data-ttu-id="14749-406">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-406">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="14749-407">SubjectID</span><span class="sxs-lookup"><span data-stu-id="14749-407">subjectId</span></span>        | <span data-ttu-id="14749-408">String</span><span class="sxs-lookup"><span data-stu-id="14749-408">String</span></span>                                                   | <span data-ttu-id="14749-409">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-409">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="14749-410">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="14749-410">assignmentState</span></span>  | <span data-ttu-id="14749-411">String</span><span class="sxs-lookup"><span data-stu-id="14749-411">String</span></span>                                                   | <span data-ttu-id="14749-412">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-412">Yes</span></span>                     | <span data-ttu-id="14749-413">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="14749-413">Eligible / Active</span></span> |
| <span data-ttu-id="14749-414">tipo</span><span class="sxs-lookup"><span data-stu-id="14749-414">type</span></span>             | <span data-ttu-id="14749-415">String</span><span class="sxs-lookup"><span data-stu-id="14749-415">String</span></span>                                                   | <span data-ttu-id="14749-416">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-416">Yes</span></span>                     | <span data-ttu-id="14749-417">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="14749-417">AdminExtend</span></span> |
| <span data-ttu-id="14749-418">motivo</span><span class="sxs-lookup"><span data-stu-id="14749-418">reason</span></span>           | <span data-ttu-id="14749-419">String</span><span class="sxs-lookup"><span data-stu-id="14749-419">String</span></span>                                                   | <span data-ttu-id="14749-420">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="14749-420">depends on roleSettings</span></span> |   |
| <span data-ttu-id="14749-421">Cronograma</span><span class="sxs-lookup"><span data-stu-id="14749-421">schedule</span></span>         | [<span data-ttu-id="14749-422">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="14749-422">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="14749-423">Sim</span><span class="sxs-lookup"><span data-stu-id="14749-423">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="14749-424">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14749-424">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="14749-425">Resposta</span><span class="sxs-lookup"><span data-stu-id="14749-425">Response</span></span>

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


