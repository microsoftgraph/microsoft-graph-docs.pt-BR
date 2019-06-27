---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função. A tabela a seguir lista as operações.
localization_priority: Normal
ms.openlocfilehash: 2765018430f4747815fc18428750cdfae4983765
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263536"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="af997-104">Criar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="af997-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af997-105">Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="af997-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="af997-106">A tabela a seguir lista as operações.</span><span class="sxs-lookup"><span data-stu-id="af997-106">The following table lists the operations.</span></span>

| <span data-ttu-id="af997-107">Operation</span><span class="sxs-lookup"><span data-stu-id="af997-107">Operation</span></span>                                   | <span data-ttu-id="af997-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="af997-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="af997-109">Atribuir uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="af997-109">Assign a role assignment</span></span>                    | <span data-ttu-id="af997-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="af997-110">AdminAdd</span></span>    |
| <span data-ttu-id="af997-111">Ativar uma atribuição de função qualificada</span><span class="sxs-lookup"><span data-stu-id="af997-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="af997-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="af997-112">UserAdd</span></span>     |
| <span data-ttu-id="af997-113">Desativar uma atribuição de função ativada</span><span class="sxs-lookup"><span data-stu-id="af997-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="af997-114">Userremove</span><span class="sxs-lookup"><span data-stu-id="af997-114">UserRemove</span></span>  |
| <span data-ttu-id="af997-115">Remover uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="af997-115">Remove a role assignment</span></span>                    | <span data-ttu-id="af997-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="af997-116">AdminRemove</span></span> |
| <span data-ttu-id="af997-117">Atualizar uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="af997-117">Update a role assignment</span></span>                    | <span data-ttu-id="af997-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="af997-118">AdminUpdate</span></span> |
| <span data-ttu-id="af997-119">Solicitação para estender minha atribuição de função</span><span class="sxs-lookup"><span data-stu-id="af997-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="af997-120">Userextend</span><span class="sxs-lookup"><span data-stu-id="af997-120">UserExtend</span></span>  |
| <span data-ttu-id="af997-121">Estender uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="af997-121">Extend a role assignment</span></span>                    | <span data-ttu-id="af997-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="af997-122">AdminExtend</span></span> |
| <span data-ttu-id="af997-123">Solicitação para renovar minha atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="af997-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="af997-124">Userrenew</span><span class="sxs-lookup"><span data-stu-id="af997-124">UserRenew</span></span>   |
| <span data-ttu-id="af997-125">Renovar uma atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="af997-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="af997-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="af997-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="af997-127">Permissões</span><span class="sxs-lookup"><span data-stu-id="af997-127">Permissions</span></span>

<span data-ttu-id="af997-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af997-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="af997-130">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af997-130">Permission type</span></span>                        | <span data-ttu-id="af997-131">Permissões</span><span class="sxs-lookup"><span data-stu-id="af997-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="af997-132">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af997-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="af997-133">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="af997-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="af997-134">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af997-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af997-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af997-135">Not supported.</span></span>                            |
| <span data-ttu-id="af997-136">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af997-136">Application</span></span>                            | <span data-ttu-id="af997-137">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af997-137">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="af997-138">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af997-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="af997-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af997-139">Request headers</span></span>

| <span data-ttu-id="af997-140">Nome</span><span class="sxs-lookup"><span data-stu-id="af997-140">Name</span></span>          | <span data-ttu-id="af997-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="af997-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="af997-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="af997-142">Authorization</span></span> | <span data-ttu-id="af997-143">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="af997-143">Bearer {code}</span></span>    |
| <span data-ttu-id="af997-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="af997-144">Content-type</span></span>  | <span data-ttu-id="af997-145">application/json</span><span class="sxs-lookup"><span data-stu-id="af997-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="af997-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af997-146">Request body</span></span>

<span data-ttu-id="af997-147">No corpo da solicitação, forneça uma representação JSON de um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="af997-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="af997-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af997-148">Property</span></span>         | <span data-ttu-id="af997-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="af997-149">Type</span></span>                                                     | <span data-ttu-id="af997-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="af997-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="af997-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="af997-151">resourceId</span></span>       | <span data-ttu-id="af997-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af997-152">String</span></span>                                                   | <span data-ttu-id="af997-153">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="af997-153">The ID of the resource.</span></span> <span data-ttu-id="af997-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af997-154">Required.</span></span> |
| <span data-ttu-id="af997-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="af997-155">roleDefinitionId</span></span> | <span data-ttu-id="af997-156">String</span><span class="sxs-lookup"><span data-stu-id="af997-156">String</span></span>                                                   | <span data-ttu-id="af997-157">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="af997-157">The ID of the role definition.</span></span> <span data-ttu-id="af997-158">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af997-158">Required.</span></span> |
| <span data-ttu-id="af997-159">SubjectID</span><span class="sxs-lookup"><span data-stu-id="af997-159">subjectId</span></span>        | <span data-ttu-id="af997-160">String</span><span class="sxs-lookup"><span data-stu-id="af997-160">String</span></span>                                                   | <span data-ttu-id="af997-161">A ID do assunto.</span><span class="sxs-lookup"><span data-stu-id="af997-161">The ID of the subject.</span></span> <span data-ttu-id="af997-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af997-162">Required.</span></span> |
| <span data-ttu-id="af997-163">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="af997-163">assignmentState</span></span>  | <span data-ttu-id="af997-164">String</span><span class="sxs-lookup"><span data-stu-id="af997-164">String</span></span>                                                   | <span data-ttu-id="af997-165">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="af997-165">The state of assignment.</span></span> <span data-ttu-id="af997-166">O valor pode ser `Eligible` e `Active`.</span><span class="sxs-lookup"><span data-stu-id="af997-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="af997-167">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af997-167">Required.</span></span> |
| <span data-ttu-id="af997-168">type</span><span class="sxs-lookup"><span data-stu-id="af997-168">type</span></span>             | <span data-ttu-id="af997-169">String</span><span class="sxs-lookup"><span data-stu-id="af997-169">String</span></span>                                                   | <span data-ttu-id="af997-170">O tipo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="af997-170">The request type.</span></span> <span data-ttu-id="af997-171">O valor pode ser `AdminAdd`, `UserAdd`, `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew`,,,, `AdminRenew`e. `AdminExtend`</span><span class="sxs-lookup"><span data-stu-id="af997-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="af997-172">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af997-172">Required.</span></span> |
| <span data-ttu-id="af997-173">motivos</span><span class="sxs-lookup"><span data-stu-id="af997-173">reason</span></span>           | <span data-ttu-id="af997-174">String</span><span class="sxs-lookup"><span data-stu-id="af997-174">String</span></span>                                                   | <span data-ttu-id="af997-175">O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e análise.</span><span class="sxs-lookup"><span data-stu-id="af997-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="af997-176">Cronograma</span><span class="sxs-lookup"><span data-stu-id="af997-176">schedule</span></span>         | [<span data-ttu-id="af997-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="af997-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="af997-178">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="af997-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="af997-179">Para o tipo de `UserAdd`solicitação `AdminAdd`de `AdminUpdate`,, `AdminExtend`, e, é necessário.</span><span class="sxs-lookup"><span data-stu-id="af997-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="af997-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="af997-180">Response</span></span>

<span data-ttu-id="af997-181">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af997-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="af997-182">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="af997-182">Error codes</span></span>

<span data-ttu-id="af997-183">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="af997-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="af997-184">Além disso, ele também retorna os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="af997-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="af997-185">Código de erro</span><span class="sxs-lookup"><span data-stu-id="af997-185">Error code</span></span>     | <span data-ttu-id="af997-186">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="af997-186">Error message</span></span>                               | <span data-ttu-id="af997-187">Detalhes</span><span class="sxs-lookup"><span data-stu-id="af997-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="af997-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="af997-188">400 BadRequest</span></span> | <span data-ttu-id="af997-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="af997-189">RoleNotFound</span></span>                                | <span data-ttu-id="af997-190">O `roleDefinitionId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="af997-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="af997-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="af997-191">400 BadRequest</span></span> | <span data-ttu-id="af997-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="af997-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="af997-193">O recurso fornecido no corpo da solicitação está no estado de `Locked` e não pode criar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="af997-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="af997-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="af997-194">400 BadRequest</span></span> | <span data-ttu-id="af997-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="af997-195">SubjectNotFound</span></span>                             | <span data-ttu-id="af997-196">O `subjectId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="af997-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="af997-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="af997-197">400 BadRequest</span></span> | <span data-ttu-id="af997-198">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="af997-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="af997-199">Já existe um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) pendente no sistema.</span><span class="sxs-lookup"><span data-stu-id="af997-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="af997-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="af997-200">400 BadRequest</span></span> | <span data-ttu-id="af997-201">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="af997-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="af997-202">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criado já existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="af997-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="af997-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="af997-203">400 BadRequest</span></span> | <span data-ttu-id="af997-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="af997-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="af997-205">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="af997-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="af997-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="af997-206">400 BadRequest</span></span> | <span data-ttu-id="af997-207">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="af997-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="af997-208">O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não atende às políticas internas e não pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="af997-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="af997-209">Exemplos</span><span class="sxs-lookup"><span data-stu-id="af997-209">Examples</span></span>

<span data-ttu-id="af997-210">Os exemplos a seguir mostram como usar essa API.</span><span class="sxs-lookup"><span data-stu-id="af997-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="af997-211">Exemplo 1: o administrador atribui um usuário a uma função</span><span class="sxs-lookup"><span data-stu-id="af997-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="af997-212">Neste exemplo, um administrador atribui o usuário nawu@fimdev.net à função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="af997-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="af997-213">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="af997-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="af997-214">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af997-214">Property</span></span>         | <span data-ttu-id="af997-215">Tipo</span><span class="sxs-lookup"><span data-stu-id="af997-215">Type</span></span>                                                     | <span data-ttu-id="af997-216">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="af997-216">Required</span></span>                 | <span data-ttu-id="af997-217">Valor</span><span class="sxs-lookup"><span data-stu-id="af997-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="af997-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="af997-218">resourceId</span></span>       | <span data-ttu-id="af997-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af997-219">String</span></span>                                                   | <span data-ttu-id="af997-220">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-220">Yes</span></span>                      | <span data-ttu-id="af997-221">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="af997-221">\<resourceId\></span></span> |
| <span data-ttu-id="af997-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="af997-222">roleDefinitionId</span></span> | <span data-ttu-id="af997-223">String</span><span class="sxs-lookup"><span data-stu-id="af997-223">String</span></span>                                                   | <span data-ttu-id="af997-224">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-224">Yes</span></span>                      | <span data-ttu-id="af997-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="af997-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="af997-226">SubjectID</span><span class="sxs-lookup"><span data-stu-id="af997-226">subjectId</span></span>        | <span data-ttu-id="af997-227">String</span><span class="sxs-lookup"><span data-stu-id="af997-227">String</span></span>                                                   | <span data-ttu-id="af997-228">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-228">Yes</span></span>                      | <span data-ttu-id="af997-229">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="af997-229">\<subjectId\></span></span> |
| <span data-ttu-id="af997-230">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="af997-230">assignmentState</span></span>  | <span data-ttu-id="af997-231">String</span><span class="sxs-lookup"><span data-stu-id="af997-231">String</span></span>                                                   | <span data-ttu-id="af997-232">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-232">Yes</span></span>                      | <span data-ttu-id="af997-233">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="af997-233">Eligible / Active</span></span> |
| <span data-ttu-id="af997-234">type</span><span class="sxs-lookup"><span data-stu-id="af997-234">type</span></span>             | <span data-ttu-id="af997-235">String</span><span class="sxs-lookup"><span data-stu-id="af997-235">String</span></span>                                                   | <span data-ttu-id="af997-236">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-236">Yes</span></span>                      | <span data-ttu-id="af997-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="af997-237">AdminAdd</span></span> |
| <span data-ttu-id="af997-238">motivos</span><span class="sxs-lookup"><span data-stu-id="af997-238">reason</span></span>           | <span data-ttu-id="af997-239">String</span><span class="sxs-lookup"><span data-stu-id="af997-239">String</span></span>                                                   | <span data-ttu-id="af997-240">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="af997-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="af997-241">Cronograma</span><span class="sxs-lookup"><span data-stu-id="af997-241">schedule</span></span>         | [<span data-ttu-id="af997-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="af997-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="af997-243">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="af997-244">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af997-244">Request</span></span>

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

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="af997-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="af997-245">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="af997-246">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="af997-246">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="af997-247">C#</span><span class="sxs-lookup"><span data-stu-id="af997-247">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/governanceroleassignmentrequest_post-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="af997-248">Javascript</span><span class="sxs-lookup"><span data-stu-id="af997-248">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/governanceroleassignmentrequest_post-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="af997-249">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="af997-249">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/governanceroleassignmentrequest_post-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="af997-250">Exemplo 2: o usuário ativa a função qualificada</span><span class="sxs-lookup"><span data-stu-id="af997-250">Example 2: User activates eligible role</span></span>

<span data-ttu-id="af997-251">Neste exemplo, o usuário nawu@fimdev.net ativa a função de leitor de cobrança qualificado.</span><span class="sxs-lookup"><span data-stu-id="af997-251">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="af997-252">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af997-252">Property</span></span>         | <span data-ttu-id="af997-253">Tipo</span><span class="sxs-lookup"><span data-stu-id="af997-253">Type</span></span>                                                     | <span data-ttu-id="af997-254">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="af997-254">Required</span></span>                 | <span data-ttu-id="af997-255">Valor</span><span class="sxs-lookup"><span data-stu-id="af997-255">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="af997-256">resourceId</span><span class="sxs-lookup"><span data-stu-id="af997-256">resourceId</span></span>       | <span data-ttu-id="af997-257">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af997-257">String</span></span>                                                   | <span data-ttu-id="af997-258">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-258">Yes</span></span>                      | <span data-ttu-id="af997-259">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="af997-259">\<resourceId\></span></span> |
| <span data-ttu-id="af997-260">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="af997-260">roleDefinitionId</span></span> | <span data-ttu-id="af997-261">String</span><span class="sxs-lookup"><span data-stu-id="af997-261">String</span></span>                                                   | <span data-ttu-id="af997-262">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-262">Yes</span></span>                      | <span data-ttu-id="af997-263">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="af997-263">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="af997-264">SubjectID</span><span class="sxs-lookup"><span data-stu-id="af997-264">subjectId</span></span>        | <span data-ttu-id="af997-265">String</span><span class="sxs-lookup"><span data-stu-id="af997-265">String</span></span>                                                   | <span data-ttu-id="af997-266">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-266">Yes</span></span>                      | <span data-ttu-id="af997-267">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="af997-267">\<subjectId\></span></span> |
| <span data-ttu-id="af997-268">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="af997-268">assignmentState</span></span>  | <span data-ttu-id="af997-269">String</span><span class="sxs-lookup"><span data-stu-id="af997-269">String</span></span>                                                   | <span data-ttu-id="af997-270">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-270">Yes</span></span>                      | <span data-ttu-id="af997-271">Ativo</span><span class="sxs-lookup"><span data-stu-id="af997-271">Active</span></span> |
| <span data-ttu-id="af997-272">type</span><span class="sxs-lookup"><span data-stu-id="af997-272">type</span></span>             | <span data-ttu-id="af997-273">String</span><span class="sxs-lookup"><span data-stu-id="af997-273">String</span></span>                                                   | <span data-ttu-id="af997-274">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-274">Yes</span></span>                      | <span data-ttu-id="af997-275">UserAdd</span><span class="sxs-lookup"><span data-stu-id="af997-275">UserAdd</span></span> |
| <span data-ttu-id="af997-276">motivos</span><span class="sxs-lookup"><span data-stu-id="af997-276">reason</span></span>           | <span data-ttu-id="af997-277">String</span><span class="sxs-lookup"><span data-stu-id="af997-277">String</span></span>                                                   | <span data-ttu-id="af997-278">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="af997-278">depends on role Settings</span></span> |   |
| <span data-ttu-id="af997-279">Cronograma</span><span class="sxs-lookup"><span data-stu-id="af997-279">schedule</span></span>         | [<span data-ttu-id="af997-280">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="af997-280">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="af997-281">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-281">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="af997-282">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af997-282">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="af997-283">Resposta</span><span class="sxs-lookup"><span data-stu-id="af997-283">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="af997-284">Exemplo 3: o usuário desativa uma função atribuída</span><span class="sxs-lookup"><span data-stu-id="af997-284">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="af997-285">Neste exemplo, o usuário nawu@fimdev.net desativa a função de leitor de cobrança ativa.</span><span class="sxs-lookup"><span data-stu-id="af997-285">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="af997-286">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af997-286">Property</span></span>         | <span data-ttu-id="af997-287">Tipo</span><span class="sxs-lookup"><span data-stu-id="af997-287">Type</span></span>                                                     | <span data-ttu-id="af997-288">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="af997-288">Required</span></span> | <span data-ttu-id="af997-289">Valor</span><span class="sxs-lookup"><span data-stu-id="af997-289">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="af997-290">resourceId</span><span class="sxs-lookup"><span data-stu-id="af997-290">resourceId</span></span>       | <span data-ttu-id="af997-291">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af997-291">String</span></span>                                                   | <span data-ttu-id="af997-292">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-292">Yes</span></span>      | <span data-ttu-id="af997-293">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="af997-293">\<resourceId\></span></span> |
| <span data-ttu-id="af997-294">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="af997-294">roleDefinitionId</span></span> | <span data-ttu-id="af997-295">String</span><span class="sxs-lookup"><span data-stu-id="af997-295">String</span></span>                                                   | <span data-ttu-id="af997-296">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-296">Yes</span></span>      | <span data-ttu-id="af997-297">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="af997-297">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="af997-298">SubjectID</span><span class="sxs-lookup"><span data-stu-id="af997-298">subjectId</span></span>        | <span data-ttu-id="af997-299">String</span><span class="sxs-lookup"><span data-stu-id="af997-299">String</span></span>                                                   | <span data-ttu-id="af997-300">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-300">Yes</span></span>      | <span data-ttu-id="af997-301">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="af997-301">\<subjectId\></span></span> |
| <span data-ttu-id="af997-302">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="af997-302">assignmentState</span></span>  | <span data-ttu-id="af997-303">String</span><span class="sxs-lookup"><span data-stu-id="af997-303">String</span></span>                                                   | <span data-ttu-id="af997-304">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-304">Yes</span></span>      | <span data-ttu-id="af997-305">Ativo</span><span class="sxs-lookup"><span data-stu-id="af997-305">Active</span></span> |
| <span data-ttu-id="af997-306">type</span><span class="sxs-lookup"><span data-stu-id="af997-306">type</span></span>             | <span data-ttu-id="af997-307">String</span><span class="sxs-lookup"><span data-stu-id="af997-307">String</span></span>                                                   | <span data-ttu-id="af997-308">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-308">Yes</span></span>      | <span data-ttu-id="af997-309">Userremove</span><span class="sxs-lookup"><span data-stu-id="af997-309">UserRemove</span></span> |
| <span data-ttu-id="af997-310">motivos</span><span class="sxs-lookup"><span data-stu-id="af997-310">reason</span></span>           | <span data-ttu-id="af997-311">String</span><span class="sxs-lookup"><span data-stu-id="af997-311">String</span></span>                                                   | <span data-ttu-id="af997-312">Não</span><span class="sxs-lookup"><span data-stu-id="af997-312">No</span></span>       |   |
| <span data-ttu-id="af997-313">Cronograma</span><span class="sxs-lookup"><span data-stu-id="af997-313">schedule</span></span>         | [<span data-ttu-id="af997-314">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="af997-314">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="af997-315">Não</span><span class="sxs-lookup"><span data-stu-id="af997-315">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="af997-316">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af997-316">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="af997-317">Resposta</span><span class="sxs-lookup"><span data-stu-id="af997-317">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="af997-318">Exemplo 4: o administrador remove o usuário de uma função</span><span class="sxs-lookup"><span data-stu-id="af997-318">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="af997-319">Neste exemplo, um administrador remove o usuário nawu@fimdev.net da função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="af997-319">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="af997-320">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="af997-320">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="af997-321">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af997-321">Property</span></span>         | <span data-ttu-id="af997-322">Tipo</span><span class="sxs-lookup"><span data-stu-id="af997-322">Type</span></span>                                                     | <span data-ttu-id="af997-323">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="af997-323">Required</span></span> | <span data-ttu-id="af997-324">Valor</span><span class="sxs-lookup"><span data-stu-id="af997-324">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="af997-325">resourceId</span><span class="sxs-lookup"><span data-stu-id="af997-325">resourceId</span></span>       | <span data-ttu-id="af997-326">String</span><span class="sxs-lookup"><span data-stu-id="af997-326">String</span></span>                                                   | <span data-ttu-id="af997-327">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-327">Yes</span></span>      | <span data-ttu-id="af997-328">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="af997-328">\<resourceId\></span></span> |
| <span data-ttu-id="af997-329">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="af997-329">roleDefinitionId</span></span> | <span data-ttu-id="af997-330">String</span><span class="sxs-lookup"><span data-stu-id="af997-330">String</span></span>                                                   | <span data-ttu-id="af997-331">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-331">Yes</span></span>      | <span data-ttu-id="af997-332">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="af997-332">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="af997-333">SubjectID</span><span class="sxs-lookup"><span data-stu-id="af997-333">subjectId</span></span>        | <span data-ttu-id="af997-334">String</span><span class="sxs-lookup"><span data-stu-id="af997-334">String</span></span>                                                   | <span data-ttu-id="af997-335">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-335">Yes</span></span>      | <span data-ttu-id="af997-336">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="af997-336">\<subjectId\></span></span> |
| <span data-ttu-id="af997-337">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="af997-337">assignmentState</span></span>  | <span data-ttu-id="af997-338">String</span><span class="sxs-lookup"><span data-stu-id="af997-338">String</span></span>                                                   | <span data-ttu-id="af997-339">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-339">Yes</span></span>      | <span data-ttu-id="af997-340">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="af997-340">Eligible / Active</span></span> |
| <span data-ttu-id="af997-341">type</span><span class="sxs-lookup"><span data-stu-id="af997-341">type</span></span>             | <span data-ttu-id="af997-342">String</span><span class="sxs-lookup"><span data-stu-id="af997-342">String</span></span>                                                   | <span data-ttu-id="af997-343">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-343">Yes</span></span>      | <span data-ttu-id="af997-344">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="af997-344">AdminRemove</span></span> |
| <span data-ttu-id="af997-345">motivos</span><span class="sxs-lookup"><span data-stu-id="af997-345">reason</span></span>           | <span data-ttu-id="af997-346">String</span><span class="sxs-lookup"><span data-stu-id="af997-346">String</span></span>                                                   | <span data-ttu-id="af997-347">Não</span><span class="sxs-lookup"><span data-stu-id="af997-347">No</span></span>       |   |
| <span data-ttu-id="af997-348">Cronograma</span><span class="sxs-lookup"><span data-stu-id="af997-348">schedule</span></span>         | [<span data-ttu-id="af997-349">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="af997-349">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="af997-350">Não</span><span class="sxs-lookup"><span data-stu-id="af997-350">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="af997-351">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af997-351">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="af997-352">Resposta</span><span class="sxs-lookup"><span data-stu-id="af997-352">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="af997-353">Exemplo 5: atribuição de função de atualização do administrador</span><span class="sxs-lookup"><span data-stu-id="af997-353">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="af997-354">Neste exemplo, os administradores atualizam a atribuição de função para o usuário nawu@fimdev.net para o proprietário.</span><span class="sxs-lookup"><span data-stu-id="af997-354">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="af997-355">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="af997-355">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="af997-356">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af997-356">Property</span></span>         | <span data-ttu-id="af997-357">Tipo</span><span class="sxs-lookup"><span data-stu-id="af997-357">Type</span></span>                                                     | <span data-ttu-id="af997-358">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="af997-358">Required</span></span>                | <span data-ttu-id="af997-359">Valor</span><span class="sxs-lookup"><span data-stu-id="af997-359">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="af997-360">resourceId</span><span class="sxs-lookup"><span data-stu-id="af997-360">resourceId</span></span>       | <span data-ttu-id="af997-361">String</span><span class="sxs-lookup"><span data-stu-id="af997-361">String</span></span>                                                   | <span data-ttu-id="af997-362">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-362">Yes</span></span>                     | <span data-ttu-id="af997-363">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="af997-363">\<resourceId\></span></span> |
| <span data-ttu-id="af997-364">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="af997-364">roleDefinitionId</span></span> | <span data-ttu-id="af997-365">String</span><span class="sxs-lookup"><span data-stu-id="af997-365">String</span></span>                                                   | <span data-ttu-id="af997-366">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-366">Yes</span></span>                     | <span data-ttu-id="af997-367">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="af997-367">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="af997-368">SubjectID</span><span class="sxs-lookup"><span data-stu-id="af997-368">subjectId</span></span>        | <span data-ttu-id="af997-369">String</span><span class="sxs-lookup"><span data-stu-id="af997-369">String</span></span>                                                   | <span data-ttu-id="af997-370">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-370">Yes</span></span>                     | <span data-ttu-id="af997-371">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="af997-371">\<subjectId\></span></span> |
| <span data-ttu-id="af997-372">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="af997-372">assignmentState</span></span>  | <span data-ttu-id="af997-373">String</span><span class="sxs-lookup"><span data-stu-id="af997-373">String</span></span>                                                   | <span data-ttu-id="af997-374">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-374">Yes</span></span>                     | <span data-ttu-id="af997-375">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="af997-375">Eligible / Active</span></span> |
| <span data-ttu-id="af997-376">type</span><span class="sxs-lookup"><span data-stu-id="af997-376">type</span></span>             | <span data-ttu-id="af997-377">String</span><span class="sxs-lookup"><span data-stu-id="af997-377">String</span></span>                                                   | <span data-ttu-id="af997-378">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-378">Yes</span></span>                     | <span data-ttu-id="af997-379">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="af997-379">AdminUpdate</span></span> |
| <span data-ttu-id="af997-380">motivos</span><span class="sxs-lookup"><span data-stu-id="af997-380">reason</span></span>           | <span data-ttu-id="af997-381">String</span><span class="sxs-lookup"><span data-stu-id="af997-381">String</span></span>                                                   | <span data-ttu-id="af997-382">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="af997-382">depends on roleSettings</span></span> |   |
| <span data-ttu-id="af997-383">Cronograma</span><span class="sxs-lookup"><span data-stu-id="af997-383">schedule</span></span>         | [<span data-ttu-id="af997-384">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="af997-384">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="af997-385">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-385">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="af997-386">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af997-386">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="af997-387">Resposta</span><span class="sxs-lookup"><span data-stu-id="af997-387">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="af997-388">Exemplo 6: administrador estende a atribuição de função de expiração</span><span class="sxs-lookup"><span data-stu-id="af997-388">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="af997-389">Este exemplo estende a atribuição de função de expiração para o usuário ANUJCUSER para o colaborador do serviço de gerenciamento de API.</span><span class="sxs-lookup"><span data-stu-id="af997-389">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="af997-390">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="af997-390">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="af997-391">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af997-391">Property</span></span>         | <span data-ttu-id="af997-392">Tipo</span><span class="sxs-lookup"><span data-stu-id="af997-392">Type</span></span>                                                     | <span data-ttu-id="af997-393">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="af997-393">Required</span></span>                | <span data-ttu-id="af997-394">Valor</span><span class="sxs-lookup"><span data-stu-id="af997-394">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="af997-395">resourceId</span><span class="sxs-lookup"><span data-stu-id="af997-395">resourceId</span></span>       | <span data-ttu-id="af997-396">String</span><span class="sxs-lookup"><span data-stu-id="af997-396">String</span></span>                                                   | <span data-ttu-id="af997-397">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-397">Yes</span></span>                     | <span data-ttu-id="af997-398">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="af997-398">\<resourceId\></span></span> |
| <span data-ttu-id="af997-399">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="af997-399">roleDefinitionId</span></span> | <span data-ttu-id="af997-400">String</span><span class="sxs-lookup"><span data-stu-id="af997-400">String</span></span>                                                   | <span data-ttu-id="af997-401">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-401">Yes</span></span>                     | <span data-ttu-id="af997-402">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="af997-402">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="af997-403">SubjectID</span><span class="sxs-lookup"><span data-stu-id="af997-403">subjectId</span></span>        | <span data-ttu-id="af997-404">String</span><span class="sxs-lookup"><span data-stu-id="af997-404">String</span></span>                                                   | <span data-ttu-id="af997-405">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-405">Yes</span></span>                     | <span data-ttu-id="af997-406">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="af997-406">\<subjectId\></span></span> |
| <span data-ttu-id="af997-407">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="af997-407">assignmentState</span></span>  | <span data-ttu-id="af997-408">String</span><span class="sxs-lookup"><span data-stu-id="af997-408">String</span></span>                                                   | <span data-ttu-id="af997-409">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-409">Yes</span></span>                     | <span data-ttu-id="af997-410">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="af997-410">Eligible / Active</span></span> |
| <span data-ttu-id="af997-411">type</span><span class="sxs-lookup"><span data-stu-id="af997-411">type</span></span>             | <span data-ttu-id="af997-412">String</span><span class="sxs-lookup"><span data-stu-id="af997-412">String</span></span>                                                   | <span data-ttu-id="af997-413">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-413">Yes</span></span>                     | <span data-ttu-id="af997-414">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="af997-414">AdminExtend</span></span> |
| <span data-ttu-id="af997-415">motivos</span><span class="sxs-lookup"><span data-stu-id="af997-415">reason</span></span>           | <span data-ttu-id="af997-416">String</span><span class="sxs-lookup"><span data-stu-id="af997-416">String</span></span>                                                   | <span data-ttu-id="af997-417">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="af997-417">depends on roleSettings</span></span> |   |
| <span data-ttu-id="af997-418">Cronograma</span><span class="sxs-lookup"><span data-stu-id="af997-418">schedule</span></span>         | [<span data-ttu-id="af997-419">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="af997-419">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="af997-420">Sim</span><span class="sxs-lookup"><span data-stu-id="af997-420">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="af997-421">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af997-421">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="af997-422">Resposta</span><span class="sxs-lookup"><span data-stu-id="af997-422">Response</span></span>

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
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
