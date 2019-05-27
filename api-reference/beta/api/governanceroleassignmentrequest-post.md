---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função. A tabela a seguir lista as operações.
localization_priority: Normal
ms.openlocfilehash: be27c8e0bab24f6a83e970b9aae46d0742be7c10
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422364"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="97048-104">Criar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="97048-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97048-105">Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="97048-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="97048-106">A tabela a seguir lista as operações.</span><span class="sxs-lookup"><span data-stu-id="97048-106">The following table lists the operations.</span></span>

| <span data-ttu-id="97048-107">Operation</span><span class="sxs-lookup"><span data-stu-id="97048-107">Operation</span></span>                                   | <span data-ttu-id="97048-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="97048-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="97048-109">Atribuir uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="97048-109">Assign a role assignment</span></span>                    | <span data-ttu-id="97048-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="97048-110">AdminAdd</span></span>    |
| <span data-ttu-id="97048-111">Ativar uma atribuição de função qualificada</span><span class="sxs-lookup"><span data-stu-id="97048-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="97048-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="97048-112">UserAdd</span></span>     |
| <span data-ttu-id="97048-113">Desativar uma atribuição de função ativada</span><span class="sxs-lookup"><span data-stu-id="97048-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="97048-114">Userremove</span><span class="sxs-lookup"><span data-stu-id="97048-114">UserRemove</span></span>  |
| <span data-ttu-id="97048-115">Remover uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="97048-115">Remove a role assignment</span></span>                    | <span data-ttu-id="97048-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="97048-116">AdminRemove</span></span> |
| <span data-ttu-id="97048-117">Atualizar uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="97048-117">Update a role assignment</span></span>                    | <span data-ttu-id="97048-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="97048-118">AdminUpdate</span></span> |
| <span data-ttu-id="97048-119">Solicitação para estender minha atribuição de função</span><span class="sxs-lookup"><span data-stu-id="97048-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="97048-120">Userextend</span><span class="sxs-lookup"><span data-stu-id="97048-120">UserExtend</span></span>  |
| <span data-ttu-id="97048-121">Estender uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="97048-121">Extend a role assignment</span></span>                    | <span data-ttu-id="97048-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="97048-122">AdminExtend</span></span> |
| <span data-ttu-id="97048-123">Solicitação para renovar minha atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="97048-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="97048-124">Userrenew</span><span class="sxs-lookup"><span data-stu-id="97048-124">UserRenew</span></span>   |
| <span data-ttu-id="97048-125">Renovar uma atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="97048-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="97048-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="97048-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="97048-127">Permissões</span><span class="sxs-lookup"><span data-stu-id="97048-127">Permissions</span></span>

<span data-ttu-id="97048-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97048-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97048-130">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97048-130">Permission type</span></span>                        | <span data-ttu-id="97048-131">Permissões</span><span class="sxs-lookup"><span data-stu-id="97048-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="97048-132">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97048-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="97048-133">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="97048-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="97048-134">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97048-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97048-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97048-135">Not supported.</span></span>                            |
| <span data-ttu-id="97048-136">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97048-136">Application</span></span>                            | <span data-ttu-id="97048-137">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97048-137">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97048-138">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97048-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="97048-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97048-139">Request headers</span></span>

| <span data-ttu-id="97048-140">Nome</span><span class="sxs-lookup"><span data-stu-id="97048-140">Name</span></span>          | <span data-ttu-id="97048-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="97048-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="97048-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="97048-142">Authorization</span></span> | <span data-ttu-id="97048-143">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="97048-143">Bearer {code}</span></span>    |
| <span data-ttu-id="97048-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="97048-144">Content-type</span></span>  | <span data-ttu-id="97048-145">application/json</span><span class="sxs-lookup"><span data-stu-id="97048-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="97048-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97048-146">Request body</span></span>

<span data-ttu-id="97048-147">No corpo da solicitação, forneça uma representação JSON de um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="97048-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="97048-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97048-148">Property</span></span>         | <span data-ttu-id="97048-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="97048-149">Type</span></span>                                                     | <span data-ttu-id="97048-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="97048-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="97048-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="97048-151">resourceId</span></span>       | <span data-ttu-id="97048-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97048-152">String</span></span>                                                   | <span data-ttu-id="97048-153">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="97048-153">The ID of the resource.</span></span> <span data-ttu-id="97048-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97048-154">Required.</span></span> |
| <span data-ttu-id="97048-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="97048-155">roleDefinitionId</span></span> | <span data-ttu-id="97048-156">String</span><span class="sxs-lookup"><span data-stu-id="97048-156">String</span></span>                                                   | <span data-ttu-id="97048-157">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="97048-157">The ID of the role definition.</span></span> <span data-ttu-id="97048-158">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97048-158">Required.</span></span> |
| <span data-ttu-id="97048-159">SubjectID</span><span class="sxs-lookup"><span data-stu-id="97048-159">subjectId</span></span>        | <span data-ttu-id="97048-160">String</span><span class="sxs-lookup"><span data-stu-id="97048-160">String</span></span>                                                   | <span data-ttu-id="97048-161">A ID do assunto.</span><span class="sxs-lookup"><span data-stu-id="97048-161">The ID of the subject.</span></span> <span data-ttu-id="97048-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97048-162">Required.</span></span> |
| <span data-ttu-id="97048-163">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="97048-163">assignmentState</span></span>  | <span data-ttu-id="97048-164">String</span><span class="sxs-lookup"><span data-stu-id="97048-164">String</span></span>                                                   | <span data-ttu-id="97048-165">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="97048-165">The state of assignment.</span></span> <span data-ttu-id="97048-166">O valor pode ser `Eligible` e `Active`.</span><span class="sxs-lookup"><span data-stu-id="97048-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="97048-167">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97048-167">Required.</span></span> |
| <span data-ttu-id="97048-168">type</span><span class="sxs-lookup"><span data-stu-id="97048-168">type</span></span>             | <span data-ttu-id="97048-169">String</span><span class="sxs-lookup"><span data-stu-id="97048-169">String</span></span>                                                   | <span data-ttu-id="97048-170">O tipo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="97048-170">The request type.</span></span> <span data-ttu-id="97048-171">O valor pode ser `AdminAdd`, `UserAdd`, `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew`,,,, `AdminRenew`e. `AdminExtend`</span><span class="sxs-lookup"><span data-stu-id="97048-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="97048-172">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97048-172">Required.</span></span> |
| <span data-ttu-id="97048-173">motivos</span><span class="sxs-lookup"><span data-stu-id="97048-173">reason</span></span>           | <span data-ttu-id="97048-174">String</span><span class="sxs-lookup"><span data-stu-id="97048-174">String</span></span>                                                   | <span data-ttu-id="97048-175">O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e análise.</span><span class="sxs-lookup"><span data-stu-id="97048-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="97048-176">Cronograma</span><span class="sxs-lookup"><span data-stu-id="97048-176">schedule</span></span>         | [<span data-ttu-id="97048-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="97048-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="97048-178">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="97048-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="97048-179">Para o tipo de `UserAdd`solicitação `AdminAdd`de `AdminUpdate`,, `AdminExtend`, e, é necessário.</span><span class="sxs-lookup"><span data-stu-id="97048-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="97048-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="97048-180">Response</span></span>

<span data-ttu-id="97048-181">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97048-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="97048-182">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="97048-182">Error codes</span></span>

<span data-ttu-id="97048-183">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="97048-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="97048-184">Além disso, ele também retorna os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="97048-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="97048-185">Código de erro</span><span class="sxs-lookup"><span data-stu-id="97048-185">Error code</span></span>     | <span data-ttu-id="97048-186">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="97048-186">Error message</span></span>                               | <span data-ttu-id="97048-187">Detalhes</span><span class="sxs-lookup"><span data-stu-id="97048-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="97048-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="97048-188">400 BadRequest</span></span> | <span data-ttu-id="97048-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="97048-189">RoleNotFound</span></span>                                | <span data-ttu-id="97048-190">O `roleDefinitionId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="97048-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="97048-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="97048-191">400 BadRequest</span></span> | <span data-ttu-id="97048-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="97048-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="97048-193">O recurso fornecido no corpo da solicitação está no estado de `Locked` e não pode criar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="97048-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="97048-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="97048-194">400 BadRequest</span></span> | <span data-ttu-id="97048-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="97048-195">SubjectNotFound</span></span>                             | <span data-ttu-id="97048-196">O `subjectId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="97048-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="97048-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="97048-197">400 BadRequest</span></span> | <span data-ttu-id="97048-198">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="97048-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="97048-199">Já existe um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) pendente no sistema.</span><span class="sxs-lookup"><span data-stu-id="97048-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="97048-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="97048-200">400 BadRequest</span></span> | <span data-ttu-id="97048-201">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="97048-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="97048-202">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criado já existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="97048-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="97048-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="97048-203">400 BadRequest</span></span> | <span data-ttu-id="97048-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="97048-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="97048-205">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="97048-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="97048-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="97048-206">400 BadRequest</span></span> | <span data-ttu-id="97048-207">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="97048-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="97048-208">O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não atende às políticas internas e não pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="97048-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="97048-209">Exemplos</span><span class="sxs-lookup"><span data-stu-id="97048-209">Examples</span></span>

<span data-ttu-id="97048-210">Os exemplos a seguir mostram como usar essa API.</span><span class="sxs-lookup"><span data-stu-id="97048-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="97048-211">Exemplo 1: o administrador atribui um usuário a uma função</span><span class="sxs-lookup"><span data-stu-id="97048-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="97048-212">Neste exemplo, um administrador atribui o usuário nawu@fimdev.net à função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="97048-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="97048-213">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="97048-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="97048-214">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97048-214">Property</span></span>         | <span data-ttu-id="97048-215">Tipo</span><span class="sxs-lookup"><span data-stu-id="97048-215">Type</span></span>                                                     | <span data-ttu-id="97048-216">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="97048-216">Required</span></span>                 | <span data-ttu-id="97048-217">Valor</span><span class="sxs-lookup"><span data-stu-id="97048-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="97048-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="97048-218">resourceId</span></span>       | <span data-ttu-id="97048-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97048-219">String</span></span>                                                   | <span data-ttu-id="97048-220">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-220">Yes</span></span>                      | <span data-ttu-id="97048-221">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="97048-221">\<resourceId\></span></span> |
| <span data-ttu-id="97048-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="97048-222">roleDefinitionId</span></span> | <span data-ttu-id="97048-223">String</span><span class="sxs-lookup"><span data-stu-id="97048-223">String</span></span>                                                   | <span data-ttu-id="97048-224">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-224">Yes</span></span>                      | <span data-ttu-id="97048-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="97048-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="97048-226">SubjectID</span><span class="sxs-lookup"><span data-stu-id="97048-226">subjectId</span></span>        | <span data-ttu-id="97048-227">String</span><span class="sxs-lookup"><span data-stu-id="97048-227">String</span></span>                                                   | <span data-ttu-id="97048-228">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-228">Yes</span></span>                      | <span data-ttu-id="97048-229">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="97048-229">\<subjectId\></span></span> |
| <span data-ttu-id="97048-230">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="97048-230">assignmentState</span></span>  | <span data-ttu-id="97048-231">String</span><span class="sxs-lookup"><span data-stu-id="97048-231">String</span></span>                                                   | <span data-ttu-id="97048-232">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-232">Yes</span></span>                      | <span data-ttu-id="97048-233">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="97048-233">Eligible / Active</span></span> |
| <span data-ttu-id="97048-234">type</span><span class="sxs-lookup"><span data-stu-id="97048-234">type</span></span>             | <span data-ttu-id="97048-235">String</span><span class="sxs-lookup"><span data-stu-id="97048-235">String</span></span>                                                   | <span data-ttu-id="97048-236">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-236">Yes</span></span>                      | <span data-ttu-id="97048-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="97048-237">AdminAdd</span></span> |
| <span data-ttu-id="97048-238">motivos</span><span class="sxs-lookup"><span data-stu-id="97048-238">reason</span></span>           | <span data-ttu-id="97048-239">String</span><span class="sxs-lookup"><span data-stu-id="97048-239">String</span></span>                                                   | <span data-ttu-id="97048-240">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="97048-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="97048-241">Cronograma</span><span class="sxs-lookup"><span data-stu-id="97048-241">schedule</span></span>         | [<span data-ttu-id="97048-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="97048-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="97048-243">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="97048-244">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97048-244">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="97048-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="97048-245">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="97048-246">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="97048-246">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="97048-247">C#</span><span class="sxs-lookup"><span data-stu-id="97048-247">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/governanceroleassignmentrequest_post-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97048-248">Javascript</span><span class="sxs-lookup"><span data-stu-id="97048-248">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/governanceroleassignmentrequest_post-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="97048-249">Exemplo 2: o usuário ativa a função qualificada</span><span class="sxs-lookup"><span data-stu-id="97048-249">Example 2: User activates eligible role</span></span>

<span data-ttu-id="97048-250">Neste exemplo, o usuário nawu@fimdev.net ativa a função de leitor de cobrança qualificado.</span><span class="sxs-lookup"><span data-stu-id="97048-250">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="97048-251">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97048-251">Property</span></span>         | <span data-ttu-id="97048-252">Tipo</span><span class="sxs-lookup"><span data-stu-id="97048-252">Type</span></span>                                                     | <span data-ttu-id="97048-253">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="97048-253">Required</span></span>                 | <span data-ttu-id="97048-254">Valor</span><span class="sxs-lookup"><span data-stu-id="97048-254">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="97048-255">resourceId</span><span class="sxs-lookup"><span data-stu-id="97048-255">resourceId</span></span>       | <span data-ttu-id="97048-256">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97048-256">String</span></span>                                                   | <span data-ttu-id="97048-257">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-257">Yes</span></span>                      | <span data-ttu-id="97048-258">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="97048-258">\<resourceId\></span></span> |
| <span data-ttu-id="97048-259">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="97048-259">roleDefinitionId</span></span> | <span data-ttu-id="97048-260">String</span><span class="sxs-lookup"><span data-stu-id="97048-260">String</span></span>                                                   | <span data-ttu-id="97048-261">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-261">Yes</span></span>                      | <span data-ttu-id="97048-262">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="97048-262">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="97048-263">SubjectID</span><span class="sxs-lookup"><span data-stu-id="97048-263">subjectId</span></span>        | <span data-ttu-id="97048-264">String</span><span class="sxs-lookup"><span data-stu-id="97048-264">String</span></span>                                                   | <span data-ttu-id="97048-265">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-265">Yes</span></span>                      | <span data-ttu-id="97048-266">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="97048-266">\<subjectId\></span></span> |
| <span data-ttu-id="97048-267">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="97048-267">assignmentState</span></span>  | <span data-ttu-id="97048-268">String</span><span class="sxs-lookup"><span data-stu-id="97048-268">String</span></span>                                                   | <span data-ttu-id="97048-269">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-269">Yes</span></span>                      | <span data-ttu-id="97048-270">Ativo</span><span class="sxs-lookup"><span data-stu-id="97048-270">Active</span></span> |
| <span data-ttu-id="97048-271">type</span><span class="sxs-lookup"><span data-stu-id="97048-271">type</span></span>             | <span data-ttu-id="97048-272">String</span><span class="sxs-lookup"><span data-stu-id="97048-272">String</span></span>                                                   | <span data-ttu-id="97048-273">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-273">Yes</span></span>                      | <span data-ttu-id="97048-274">UserAdd</span><span class="sxs-lookup"><span data-stu-id="97048-274">UserAdd</span></span> |
| <span data-ttu-id="97048-275">motivos</span><span class="sxs-lookup"><span data-stu-id="97048-275">reason</span></span>           | <span data-ttu-id="97048-276">String</span><span class="sxs-lookup"><span data-stu-id="97048-276">String</span></span>                                                   | <span data-ttu-id="97048-277">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="97048-277">depends on role Settings</span></span> |   |
| <span data-ttu-id="97048-278">Cronograma</span><span class="sxs-lookup"><span data-stu-id="97048-278">schedule</span></span>         | [<span data-ttu-id="97048-279">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="97048-279">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="97048-280">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-280">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="97048-281">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97048-281">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="97048-282">Resposta</span><span class="sxs-lookup"><span data-stu-id="97048-282">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="97048-283">Exemplo 3: o usuário desativa uma função atribuída</span><span class="sxs-lookup"><span data-stu-id="97048-283">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="97048-284">Neste exemplo, o usuário nawu@fimdev.net desativa a função de leitor de cobrança ativa.</span><span class="sxs-lookup"><span data-stu-id="97048-284">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="97048-285">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97048-285">Property</span></span>         | <span data-ttu-id="97048-286">Tipo</span><span class="sxs-lookup"><span data-stu-id="97048-286">Type</span></span>                                                     | <span data-ttu-id="97048-287">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="97048-287">Required</span></span> | <span data-ttu-id="97048-288">Valor</span><span class="sxs-lookup"><span data-stu-id="97048-288">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="97048-289">resourceId</span><span class="sxs-lookup"><span data-stu-id="97048-289">resourceId</span></span>       | <span data-ttu-id="97048-290">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97048-290">String</span></span>                                                   | <span data-ttu-id="97048-291">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-291">Yes</span></span>      | <span data-ttu-id="97048-292">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="97048-292">\<resourceId\></span></span> |
| <span data-ttu-id="97048-293">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="97048-293">roleDefinitionId</span></span> | <span data-ttu-id="97048-294">String</span><span class="sxs-lookup"><span data-stu-id="97048-294">String</span></span>                                                   | <span data-ttu-id="97048-295">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-295">Yes</span></span>      | <span data-ttu-id="97048-296">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="97048-296">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="97048-297">SubjectID</span><span class="sxs-lookup"><span data-stu-id="97048-297">subjectId</span></span>        | <span data-ttu-id="97048-298">String</span><span class="sxs-lookup"><span data-stu-id="97048-298">String</span></span>                                                   | <span data-ttu-id="97048-299">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-299">Yes</span></span>      | <span data-ttu-id="97048-300">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="97048-300">\<subjectId\></span></span> |
| <span data-ttu-id="97048-301">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="97048-301">assignmentState</span></span>  | <span data-ttu-id="97048-302">String</span><span class="sxs-lookup"><span data-stu-id="97048-302">String</span></span>                                                   | <span data-ttu-id="97048-303">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-303">Yes</span></span>      | <span data-ttu-id="97048-304">Ativo</span><span class="sxs-lookup"><span data-stu-id="97048-304">Active</span></span> |
| <span data-ttu-id="97048-305">type</span><span class="sxs-lookup"><span data-stu-id="97048-305">type</span></span>             | <span data-ttu-id="97048-306">String</span><span class="sxs-lookup"><span data-stu-id="97048-306">String</span></span>                                                   | <span data-ttu-id="97048-307">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-307">Yes</span></span>      | <span data-ttu-id="97048-308">Userremove</span><span class="sxs-lookup"><span data-stu-id="97048-308">UserRemove</span></span> |
| <span data-ttu-id="97048-309">motivos</span><span class="sxs-lookup"><span data-stu-id="97048-309">reason</span></span>           | <span data-ttu-id="97048-310">String</span><span class="sxs-lookup"><span data-stu-id="97048-310">String</span></span>                                                   | <span data-ttu-id="97048-311">Não</span><span class="sxs-lookup"><span data-stu-id="97048-311">No</span></span>       |   |
| <span data-ttu-id="97048-312">Cronograma</span><span class="sxs-lookup"><span data-stu-id="97048-312">schedule</span></span>         | [<span data-ttu-id="97048-313">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="97048-313">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="97048-314">Não</span><span class="sxs-lookup"><span data-stu-id="97048-314">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="97048-315">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97048-315">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="97048-316">Resposta</span><span class="sxs-lookup"><span data-stu-id="97048-316">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="97048-317">Exemplo 4: o administrador remove o usuário de uma função</span><span class="sxs-lookup"><span data-stu-id="97048-317">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="97048-318">Neste exemplo, um administrador remove o usuário nawu@fimdev.net da função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="97048-318">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="97048-319">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="97048-319">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="97048-320">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97048-320">Property</span></span>         | <span data-ttu-id="97048-321">Tipo</span><span class="sxs-lookup"><span data-stu-id="97048-321">Type</span></span>                                                     | <span data-ttu-id="97048-322">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="97048-322">Required</span></span> | <span data-ttu-id="97048-323">Valor</span><span class="sxs-lookup"><span data-stu-id="97048-323">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="97048-324">resourceId</span><span class="sxs-lookup"><span data-stu-id="97048-324">resourceId</span></span>       | <span data-ttu-id="97048-325">String</span><span class="sxs-lookup"><span data-stu-id="97048-325">String</span></span>                                                   | <span data-ttu-id="97048-326">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-326">Yes</span></span>      | <span data-ttu-id="97048-327">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="97048-327">\<resourceId\></span></span> |
| <span data-ttu-id="97048-328">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="97048-328">roleDefinitionId</span></span> | <span data-ttu-id="97048-329">String</span><span class="sxs-lookup"><span data-stu-id="97048-329">String</span></span>                                                   | <span data-ttu-id="97048-330">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-330">Yes</span></span>      | <span data-ttu-id="97048-331">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="97048-331">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="97048-332">SubjectID</span><span class="sxs-lookup"><span data-stu-id="97048-332">subjectId</span></span>        | <span data-ttu-id="97048-333">String</span><span class="sxs-lookup"><span data-stu-id="97048-333">String</span></span>                                                   | <span data-ttu-id="97048-334">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-334">Yes</span></span>      | <span data-ttu-id="97048-335">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="97048-335">\<subjectId\></span></span> |
| <span data-ttu-id="97048-336">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="97048-336">assignmentState</span></span>  | <span data-ttu-id="97048-337">String</span><span class="sxs-lookup"><span data-stu-id="97048-337">String</span></span>                                                   | <span data-ttu-id="97048-338">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-338">Yes</span></span>      | <span data-ttu-id="97048-339">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="97048-339">Eligible / Active</span></span> |
| <span data-ttu-id="97048-340">type</span><span class="sxs-lookup"><span data-stu-id="97048-340">type</span></span>             | <span data-ttu-id="97048-341">String</span><span class="sxs-lookup"><span data-stu-id="97048-341">String</span></span>                                                   | <span data-ttu-id="97048-342">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-342">Yes</span></span>      | <span data-ttu-id="97048-343">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="97048-343">AdminRemove</span></span> |
| <span data-ttu-id="97048-344">motivos</span><span class="sxs-lookup"><span data-stu-id="97048-344">reason</span></span>           | <span data-ttu-id="97048-345">String</span><span class="sxs-lookup"><span data-stu-id="97048-345">String</span></span>                                                   | <span data-ttu-id="97048-346">Não</span><span class="sxs-lookup"><span data-stu-id="97048-346">No</span></span>       |   |
| <span data-ttu-id="97048-347">Cronograma</span><span class="sxs-lookup"><span data-stu-id="97048-347">schedule</span></span>         | [<span data-ttu-id="97048-348">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="97048-348">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="97048-349">Não</span><span class="sxs-lookup"><span data-stu-id="97048-349">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="97048-350">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97048-350">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="97048-351">Resposta</span><span class="sxs-lookup"><span data-stu-id="97048-351">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="97048-352">Exemplo 5: atribuição de função de atualização do administrador</span><span class="sxs-lookup"><span data-stu-id="97048-352">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="97048-353">Neste exemplo, os administradores atualizam a atribuição de função para o usuário nawu@fimdev.net para o proprietário.</span><span class="sxs-lookup"><span data-stu-id="97048-353">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="97048-354">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="97048-354">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="97048-355">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97048-355">Property</span></span>         | <span data-ttu-id="97048-356">Tipo</span><span class="sxs-lookup"><span data-stu-id="97048-356">Type</span></span>                                                     | <span data-ttu-id="97048-357">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="97048-357">Required</span></span>                | <span data-ttu-id="97048-358">Valor</span><span class="sxs-lookup"><span data-stu-id="97048-358">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="97048-359">resourceId</span><span class="sxs-lookup"><span data-stu-id="97048-359">resourceId</span></span>       | <span data-ttu-id="97048-360">String</span><span class="sxs-lookup"><span data-stu-id="97048-360">String</span></span>                                                   | <span data-ttu-id="97048-361">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-361">Yes</span></span>                     | <span data-ttu-id="97048-362">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="97048-362">\<resourceId\></span></span> |
| <span data-ttu-id="97048-363">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="97048-363">roleDefinitionId</span></span> | <span data-ttu-id="97048-364">String</span><span class="sxs-lookup"><span data-stu-id="97048-364">String</span></span>                                                   | <span data-ttu-id="97048-365">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-365">Yes</span></span>                     | <span data-ttu-id="97048-366">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="97048-366">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="97048-367">SubjectID</span><span class="sxs-lookup"><span data-stu-id="97048-367">subjectId</span></span>        | <span data-ttu-id="97048-368">String</span><span class="sxs-lookup"><span data-stu-id="97048-368">String</span></span>                                                   | <span data-ttu-id="97048-369">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-369">Yes</span></span>                     | <span data-ttu-id="97048-370">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="97048-370">\<subjectId\></span></span> |
| <span data-ttu-id="97048-371">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="97048-371">assignmentState</span></span>  | <span data-ttu-id="97048-372">String</span><span class="sxs-lookup"><span data-stu-id="97048-372">String</span></span>                                                   | <span data-ttu-id="97048-373">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-373">Yes</span></span>                     | <span data-ttu-id="97048-374">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="97048-374">Eligible / Active</span></span> |
| <span data-ttu-id="97048-375">type</span><span class="sxs-lookup"><span data-stu-id="97048-375">type</span></span>             | <span data-ttu-id="97048-376">String</span><span class="sxs-lookup"><span data-stu-id="97048-376">String</span></span>                                                   | <span data-ttu-id="97048-377">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-377">Yes</span></span>                     | <span data-ttu-id="97048-378">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="97048-378">AdminUpdate</span></span> |
| <span data-ttu-id="97048-379">motivos</span><span class="sxs-lookup"><span data-stu-id="97048-379">reason</span></span>           | <span data-ttu-id="97048-380">String</span><span class="sxs-lookup"><span data-stu-id="97048-380">String</span></span>                                                   | <span data-ttu-id="97048-381">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="97048-381">depends on roleSettings</span></span> |   |
| <span data-ttu-id="97048-382">Cronograma</span><span class="sxs-lookup"><span data-stu-id="97048-382">schedule</span></span>         | [<span data-ttu-id="97048-383">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="97048-383">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="97048-384">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-384">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="97048-385">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97048-385">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="97048-386">Resposta</span><span class="sxs-lookup"><span data-stu-id="97048-386">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="97048-387">Exemplo 6: administrador estende a atribuição de função de expiração</span><span class="sxs-lookup"><span data-stu-id="97048-387">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="97048-388">Este exemplo estende a atribuição de função de expiração para o usuário ANUJCUSER para o colaborador do serviço de gerenciamento de API.</span><span class="sxs-lookup"><span data-stu-id="97048-388">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="97048-389">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="97048-389">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="97048-390">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97048-390">Property</span></span>         | <span data-ttu-id="97048-391">Tipo</span><span class="sxs-lookup"><span data-stu-id="97048-391">Type</span></span>                                                     | <span data-ttu-id="97048-392">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="97048-392">Required</span></span>                | <span data-ttu-id="97048-393">Valor</span><span class="sxs-lookup"><span data-stu-id="97048-393">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="97048-394">resourceId</span><span class="sxs-lookup"><span data-stu-id="97048-394">resourceId</span></span>       | <span data-ttu-id="97048-395">String</span><span class="sxs-lookup"><span data-stu-id="97048-395">String</span></span>                                                   | <span data-ttu-id="97048-396">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-396">Yes</span></span>                     | <span data-ttu-id="97048-397">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="97048-397">\<resourceId\></span></span> |
| <span data-ttu-id="97048-398">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="97048-398">roleDefinitionId</span></span> | <span data-ttu-id="97048-399">String</span><span class="sxs-lookup"><span data-stu-id="97048-399">String</span></span>                                                   | <span data-ttu-id="97048-400">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-400">Yes</span></span>                     | <span data-ttu-id="97048-401">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="97048-401">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="97048-402">SubjectID</span><span class="sxs-lookup"><span data-stu-id="97048-402">subjectId</span></span>        | <span data-ttu-id="97048-403">String</span><span class="sxs-lookup"><span data-stu-id="97048-403">String</span></span>                                                   | <span data-ttu-id="97048-404">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-404">Yes</span></span>                     | <span data-ttu-id="97048-405">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="97048-405">\<subjectId\></span></span> |
| <span data-ttu-id="97048-406">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="97048-406">assignmentState</span></span>  | <span data-ttu-id="97048-407">String</span><span class="sxs-lookup"><span data-stu-id="97048-407">String</span></span>                                                   | <span data-ttu-id="97048-408">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-408">Yes</span></span>                     | <span data-ttu-id="97048-409">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="97048-409">Eligible / Active</span></span> |
| <span data-ttu-id="97048-410">type</span><span class="sxs-lookup"><span data-stu-id="97048-410">type</span></span>             | <span data-ttu-id="97048-411">String</span><span class="sxs-lookup"><span data-stu-id="97048-411">String</span></span>                                                   | <span data-ttu-id="97048-412">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-412">Yes</span></span>                     | <span data-ttu-id="97048-413">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="97048-413">AdminExtend</span></span> |
| <span data-ttu-id="97048-414">motivos</span><span class="sxs-lookup"><span data-stu-id="97048-414">reason</span></span>           | <span data-ttu-id="97048-415">String</span><span class="sxs-lookup"><span data-stu-id="97048-415">String</span></span>                                                   | <span data-ttu-id="97048-416">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="97048-416">depends on roleSettings</span></span> |   |
| <span data-ttu-id="97048-417">Cronograma</span><span class="sxs-lookup"><span data-stu-id="97048-417">schedule</span></span>         | [<span data-ttu-id="97048-418">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="97048-418">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="97048-419">Sim</span><span class="sxs-lookup"><span data-stu-id="97048-419">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="97048-420">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97048-420">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="97048-421">Resposta</span><span class="sxs-lookup"><span data-stu-id="97048-421">Response</span></span>

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
