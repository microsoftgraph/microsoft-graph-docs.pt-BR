---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função. A tabela a seguir lista as operações.
localization_priority: Normal
ms.openlocfilehash: 104ab1a0d4909bc2181df70bc4fc895fc4558260
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503274"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="eac76-104">Criar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="eac76-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eac76-105">Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="eac76-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="eac76-106">A tabela a seguir lista as operações.</span><span class="sxs-lookup"><span data-stu-id="eac76-106">The following table lists the operations.</span></span>

| <span data-ttu-id="eac76-107">Operation</span><span class="sxs-lookup"><span data-stu-id="eac76-107">Operation</span></span>                                   | <span data-ttu-id="eac76-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="eac76-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="eac76-109">Atribuir uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="eac76-109">Assign a role assignment</span></span>                    | <span data-ttu-id="eac76-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="eac76-110">AdminAdd</span></span>    |
| <span data-ttu-id="eac76-111">Ativar uma atribuição de função qualificada</span><span class="sxs-lookup"><span data-stu-id="eac76-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="eac76-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="eac76-112">UserAdd</span></span>     |
| <span data-ttu-id="eac76-113">Desativar uma atribuição de função ativada</span><span class="sxs-lookup"><span data-stu-id="eac76-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="eac76-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="eac76-114">UserRemove</span></span>  |
| <span data-ttu-id="eac76-115">Remover uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="eac76-115">Remove a role assignment</span></span>                    | <span data-ttu-id="eac76-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="eac76-116">AdminRemove</span></span> |
| <span data-ttu-id="eac76-117">Atualizar uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="eac76-117">Update a role assignment</span></span>                    | <span data-ttu-id="eac76-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="eac76-118">AdminUpdate</span></span> |
| <span data-ttu-id="eac76-119">Solicitação para estender minha atribuição de função</span><span class="sxs-lookup"><span data-stu-id="eac76-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="eac76-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="eac76-120">UserExtend</span></span>  |
| <span data-ttu-id="eac76-121">Estender uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="eac76-121">Extend a role assignment</span></span>                    | <span data-ttu-id="eac76-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="eac76-122">AdminExtend</span></span> |
| <span data-ttu-id="eac76-123">Solicitação para renovar minha atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="eac76-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="eac76-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="eac76-124">UserRenew</span></span>   |
| <span data-ttu-id="eac76-125">ReNovar uma atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="eac76-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="eac76-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="eac76-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="eac76-127">Permissões</span><span class="sxs-lookup"><span data-stu-id="eac76-127">Permissions</span></span>

<span data-ttu-id="eac76-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eac76-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eac76-130">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eac76-130">Permission type</span></span>                        | <span data-ttu-id="eac76-131">Permissões</span><span class="sxs-lookup"><span data-stu-id="eac76-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="eac76-132">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eac76-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="eac76-133">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="eac76-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="eac76-134">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eac76-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eac76-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eac76-135">Not supported.</span></span>                            |
| <span data-ttu-id="eac76-136">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eac76-136">Application</span></span>                            | <span data-ttu-id="eac76-137">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="eac76-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="eac76-138">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eac76-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="eac76-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eac76-139">Request headers</span></span>

| <span data-ttu-id="eac76-140">Nome</span><span class="sxs-lookup"><span data-stu-id="eac76-140">Name</span></span>          | <span data-ttu-id="eac76-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="eac76-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="eac76-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="eac76-142">Authorization</span></span> | <span data-ttu-id="eac76-143">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="eac76-143">Bearer {code}</span></span>    |
| <span data-ttu-id="eac76-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="eac76-144">Content-type</span></span>  | <span data-ttu-id="eac76-145">application/json</span><span class="sxs-lookup"><span data-stu-id="eac76-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="eac76-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eac76-146">Request body</span></span>

<span data-ttu-id="eac76-147">No corpo da solicitação, forneça uma representação JSON de um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="eac76-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="eac76-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eac76-148">Property</span></span>         | <span data-ttu-id="eac76-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="eac76-149">Type</span></span>                                                     | <span data-ttu-id="eac76-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="eac76-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="eac76-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="eac76-151">resourceId</span></span>       | <span data-ttu-id="eac76-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eac76-152">String</span></span>                                                   | <span data-ttu-id="eac76-153">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="eac76-153">The ID of the resource.</span></span> <span data-ttu-id="eac76-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eac76-154">Required.</span></span> |
| <span data-ttu-id="eac76-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="eac76-155">roleDefinitionId</span></span> | <span data-ttu-id="eac76-156">String</span><span class="sxs-lookup"><span data-stu-id="eac76-156">String</span></span>                                                   | <span data-ttu-id="eac76-157">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="eac76-157">The ID of the role definition.</span></span> <span data-ttu-id="eac76-158">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eac76-158">Required.</span></span> |
| <span data-ttu-id="eac76-159">SubjectID</span><span class="sxs-lookup"><span data-stu-id="eac76-159">subjectId</span></span>        | <span data-ttu-id="eac76-160">String</span><span class="sxs-lookup"><span data-stu-id="eac76-160">String</span></span>                                                   | <span data-ttu-id="eac76-161">A ID do assunto.</span><span class="sxs-lookup"><span data-stu-id="eac76-161">The ID of the subject.</span></span> <span data-ttu-id="eac76-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eac76-162">Required.</span></span> |
| <span data-ttu-id="eac76-163">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="eac76-163">assignmentState</span></span>  | <span data-ttu-id="eac76-164">String</span><span class="sxs-lookup"><span data-stu-id="eac76-164">String</span></span>                                                   | <span data-ttu-id="eac76-165">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="eac76-165">The state of assignment.</span></span> <span data-ttu-id="eac76-166">O valor pode ser `Eligible` e `Active`.</span><span class="sxs-lookup"><span data-stu-id="eac76-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="eac76-167">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eac76-167">Required.</span></span> |
| <span data-ttu-id="eac76-168">type</span><span class="sxs-lookup"><span data-stu-id="eac76-168">type</span></span>             | <span data-ttu-id="eac76-169">String</span><span class="sxs-lookup"><span data-stu-id="eac76-169">String</span></span>                                                   | <span data-ttu-id="eac76-170">O tipo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eac76-170">The request type.</span></span> <span data-ttu-id="eac76-171">O valor pode ser `AdminAdd`, `UserAdd`, `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew`,,,, `AdminRenew`e. `AdminExtend`</span><span class="sxs-lookup"><span data-stu-id="eac76-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="eac76-172">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eac76-172">Required.</span></span> |
| <span data-ttu-id="eac76-173">motivos</span><span class="sxs-lookup"><span data-stu-id="eac76-173">reason</span></span>           | <span data-ttu-id="eac76-174">String</span><span class="sxs-lookup"><span data-stu-id="eac76-174">String</span></span>                                                   | <span data-ttu-id="eac76-175">O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e análise.</span><span class="sxs-lookup"><span data-stu-id="eac76-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="eac76-176">futebol</span><span class="sxs-lookup"><span data-stu-id="eac76-176">schedule</span></span>         | [<span data-ttu-id="eac76-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="eac76-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="eac76-178">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="eac76-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="eac76-179">Para o tipo de `UserAdd`solicitação `AdminAdd`de `AdminUpdate`,, `AdminExtend`, e, é necessário.</span><span class="sxs-lookup"><span data-stu-id="eac76-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="eac76-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="eac76-180">Response</span></span>

<span data-ttu-id="eac76-181">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eac76-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="eac76-182">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="eac76-182">Error codes</span></span>

<span data-ttu-id="eac76-183">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="eac76-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="eac76-184">Além disso, ele também retorna os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="eac76-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="eac76-185">Código de erro</span><span class="sxs-lookup"><span data-stu-id="eac76-185">Error code</span></span>     | <span data-ttu-id="eac76-186">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="eac76-186">Error message</span></span>                               | <span data-ttu-id="eac76-187">Detalhes</span><span class="sxs-lookup"><span data-stu-id="eac76-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="eac76-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="eac76-188">400 BadRequest</span></span> | <span data-ttu-id="eac76-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="eac76-189">RoleNotFound</span></span>                                | <span data-ttu-id="eac76-190">O `roleDefinitionId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="eac76-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="eac76-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="eac76-191">400 BadRequest</span></span> | <span data-ttu-id="eac76-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="eac76-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="eac76-193">O recurso fornecido no corpo da solicitação está no estado de `Locked` e não pode criar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="eac76-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="eac76-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="eac76-194">400 BadRequest</span></span> | <span data-ttu-id="eac76-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="eac76-195">SubjectNotFound</span></span>                             | <span data-ttu-id="eac76-196">O `subjectId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="eac76-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="eac76-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="eac76-197">400 BadRequest</span></span> | <span data-ttu-id="eac76-198">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="eac76-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="eac76-199">Já existe um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) pendente no sistema.</span><span class="sxs-lookup"><span data-stu-id="eac76-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="eac76-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="eac76-200">400 BadRequest</span></span> | <span data-ttu-id="eac76-201">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="eac76-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="eac76-202">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criado já existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="eac76-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="eac76-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="eac76-203">400 BadRequest</span></span> | <span data-ttu-id="eac76-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="eac76-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="eac76-205">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="eac76-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="eac76-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="eac76-206">400 BadRequest</span></span> | <span data-ttu-id="eac76-207">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="eac76-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="eac76-208">O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não atende às políticas internas e não pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="eac76-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="eac76-209">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eac76-209">Examples</span></span>

<span data-ttu-id="eac76-210">Os exemplos a seguir mostram como usar essa API.</span><span class="sxs-lookup"><span data-stu-id="eac76-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="eac76-211">Exemplo 1: o administrador atribui um usuário a uma função</span><span class="sxs-lookup"><span data-stu-id="eac76-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="eac76-212">Neste exemplo, um administrador atribui o usuário nawu@fimdev.net à função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="eac76-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="eac76-213">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="eac76-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="eac76-214">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eac76-214">Property</span></span>         | <span data-ttu-id="eac76-215">Tipo</span><span class="sxs-lookup"><span data-stu-id="eac76-215">Type</span></span>                                                     | <span data-ttu-id="eac76-216">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="eac76-216">Required</span></span>                 | <span data-ttu-id="eac76-217">Valor</span><span class="sxs-lookup"><span data-stu-id="eac76-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="eac76-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="eac76-218">resourceId</span></span>       | <span data-ttu-id="eac76-219">String</span><span class="sxs-lookup"><span data-stu-id="eac76-219">String</span></span>                                                   | <span data-ttu-id="eac76-220">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-220">Yes</span></span>                      | <span data-ttu-id="eac76-221">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="eac76-221">\<resourceId\></span></span> |
| <span data-ttu-id="eac76-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="eac76-222">roleDefinitionId</span></span> | <span data-ttu-id="eac76-223">String</span><span class="sxs-lookup"><span data-stu-id="eac76-223">String</span></span>                                                   | <span data-ttu-id="eac76-224">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-224">Yes</span></span>                      | <span data-ttu-id="eac76-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="eac76-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="eac76-226">SubjectID</span><span class="sxs-lookup"><span data-stu-id="eac76-226">subjectId</span></span>        | <span data-ttu-id="eac76-227">String</span><span class="sxs-lookup"><span data-stu-id="eac76-227">String</span></span>                                                   | <span data-ttu-id="eac76-228">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-228">Yes</span></span>                      | <span data-ttu-id="eac76-229">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="eac76-229">\<subjectId\></span></span> |
| <span data-ttu-id="eac76-230">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="eac76-230">assignmentState</span></span>  | <span data-ttu-id="eac76-231">String</span><span class="sxs-lookup"><span data-stu-id="eac76-231">String</span></span>                                                   | <span data-ttu-id="eac76-232">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-232">Yes</span></span>                      | <span data-ttu-id="eac76-233">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="eac76-233">Eligible / Active</span></span> |
| <span data-ttu-id="eac76-234">type</span><span class="sxs-lookup"><span data-stu-id="eac76-234">type</span></span>             | <span data-ttu-id="eac76-235">String</span><span class="sxs-lookup"><span data-stu-id="eac76-235">String</span></span>                                                   | <span data-ttu-id="eac76-236">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-236">Yes</span></span>                      | <span data-ttu-id="eac76-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="eac76-237">AdminAdd</span></span> |
| <span data-ttu-id="eac76-238">motivos</span><span class="sxs-lookup"><span data-stu-id="eac76-238">reason</span></span>           | <span data-ttu-id="eac76-239">String</span><span class="sxs-lookup"><span data-stu-id="eac76-239">String</span></span>                                                   | <span data-ttu-id="eac76-240">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="eac76-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="eac76-241">futebol</span><span class="sxs-lookup"><span data-stu-id="eac76-241">schedule</span></span>         | [<span data-ttu-id="eac76-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="eac76-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="eac76-243">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="eac76-244">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eac76-244">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="eac76-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="eac76-245">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="eac76-246">Exemplo 2: o usuário ativa a função qualificada</span><span class="sxs-lookup"><span data-stu-id="eac76-246">Example 2: User activates eligible role</span></span>

<span data-ttu-id="eac76-247">Neste exemplo, o usuário nawu@fimdev.net ativa a função de leitor de cobrança qualificado.</span><span class="sxs-lookup"><span data-stu-id="eac76-247">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="eac76-248">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eac76-248">Property</span></span>         | <span data-ttu-id="eac76-249">Tipo</span><span class="sxs-lookup"><span data-stu-id="eac76-249">Type</span></span>                                                     | <span data-ttu-id="eac76-250">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="eac76-250">Required</span></span>                 | <span data-ttu-id="eac76-251">Valor</span><span class="sxs-lookup"><span data-stu-id="eac76-251">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="eac76-252">resourceId</span><span class="sxs-lookup"><span data-stu-id="eac76-252">resourceId</span></span>       | <span data-ttu-id="eac76-253">String</span><span class="sxs-lookup"><span data-stu-id="eac76-253">String</span></span>                                                   | <span data-ttu-id="eac76-254">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-254">Yes</span></span>                      | <span data-ttu-id="eac76-255">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="eac76-255">\<resourceId\></span></span> |
| <span data-ttu-id="eac76-256">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="eac76-256">roleDefinitionId</span></span> | <span data-ttu-id="eac76-257">String</span><span class="sxs-lookup"><span data-stu-id="eac76-257">String</span></span>                                                   | <span data-ttu-id="eac76-258">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-258">Yes</span></span>                      | <span data-ttu-id="eac76-259">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="eac76-259">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="eac76-260">SubjectID</span><span class="sxs-lookup"><span data-stu-id="eac76-260">subjectId</span></span>        | <span data-ttu-id="eac76-261">String</span><span class="sxs-lookup"><span data-stu-id="eac76-261">String</span></span>                                                   | <span data-ttu-id="eac76-262">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-262">Yes</span></span>                      | <span data-ttu-id="eac76-263">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="eac76-263">\<subjectId\></span></span> |
| <span data-ttu-id="eac76-264">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="eac76-264">assignmentState</span></span>  | <span data-ttu-id="eac76-265">String</span><span class="sxs-lookup"><span data-stu-id="eac76-265">String</span></span>                                                   | <span data-ttu-id="eac76-266">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-266">Yes</span></span>                      | <span data-ttu-id="eac76-267">Ativo</span><span class="sxs-lookup"><span data-stu-id="eac76-267">Active</span></span> |
| <span data-ttu-id="eac76-268">type</span><span class="sxs-lookup"><span data-stu-id="eac76-268">type</span></span>             | <span data-ttu-id="eac76-269">String</span><span class="sxs-lookup"><span data-stu-id="eac76-269">String</span></span>                                                   | <span data-ttu-id="eac76-270">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-270">Yes</span></span>                      | <span data-ttu-id="eac76-271">UserAdd</span><span class="sxs-lookup"><span data-stu-id="eac76-271">UserAdd</span></span> |
| <span data-ttu-id="eac76-272">motivos</span><span class="sxs-lookup"><span data-stu-id="eac76-272">reason</span></span>           | <span data-ttu-id="eac76-273">String</span><span class="sxs-lookup"><span data-stu-id="eac76-273">String</span></span>                                                   | <span data-ttu-id="eac76-274">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="eac76-274">depends on role Settings</span></span> |   |
| <span data-ttu-id="eac76-275">futebol</span><span class="sxs-lookup"><span data-stu-id="eac76-275">schedule</span></span>         | [<span data-ttu-id="eac76-276">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="eac76-276">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="eac76-277">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-277">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="eac76-278">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eac76-278">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="eac76-279">Resposta</span><span class="sxs-lookup"><span data-stu-id="eac76-279">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="eac76-280">Exemplo 3: o usuário desativa uma função atribuída</span><span class="sxs-lookup"><span data-stu-id="eac76-280">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="eac76-281">Neste exemplo, o usuário nawu@fimdev.net desativa a função de leitor de cobrança ativa.</span><span class="sxs-lookup"><span data-stu-id="eac76-281">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="eac76-282">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eac76-282">Property</span></span>         | <span data-ttu-id="eac76-283">Tipo</span><span class="sxs-lookup"><span data-stu-id="eac76-283">Type</span></span>                                                     | <span data-ttu-id="eac76-284">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="eac76-284">Required</span></span> | <span data-ttu-id="eac76-285">Valor</span><span class="sxs-lookup"><span data-stu-id="eac76-285">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="eac76-286">resourceId</span><span class="sxs-lookup"><span data-stu-id="eac76-286">resourceId</span></span>       | <span data-ttu-id="eac76-287">String</span><span class="sxs-lookup"><span data-stu-id="eac76-287">String</span></span>                                                   | <span data-ttu-id="eac76-288">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-288">Yes</span></span>      | <span data-ttu-id="eac76-289">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="eac76-289">\<resourceId\></span></span> |
| <span data-ttu-id="eac76-290">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="eac76-290">roleDefinitionId</span></span> | <span data-ttu-id="eac76-291">String</span><span class="sxs-lookup"><span data-stu-id="eac76-291">String</span></span>                                                   | <span data-ttu-id="eac76-292">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-292">Yes</span></span>      | <span data-ttu-id="eac76-293">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="eac76-293">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="eac76-294">SubjectID</span><span class="sxs-lookup"><span data-stu-id="eac76-294">subjectId</span></span>        | <span data-ttu-id="eac76-295">String</span><span class="sxs-lookup"><span data-stu-id="eac76-295">String</span></span>                                                   | <span data-ttu-id="eac76-296">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-296">Yes</span></span>      | <span data-ttu-id="eac76-297">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="eac76-297">\<subjectId\></span></span> |
| <span data-ttu-id="eac76-298">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="eac76-298">assignmentState</span></span>  | <span data-ttu-id="eac76-299">String</span><span class="sxs-lookup"><span data-stu-id="eac76-299">String</span></span>                                                   | <span data-ttu-id="eac76-300">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-300">Yes</span></span>      | <span data-ttu-id="eac76-301">Ativo</span><span class="sxs-lookup"><span data-stu-id="eac76-301">Active</span></span> |
| <span data-ttu-id="eac76-302">type</span><span class="sxs-lookup"><span data-stu-id="eac76-302">type</span></span>             | <span data-ttu-id="eac76-303">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eac76-303">String</span></span>                                                   | <span data-ttu-id="eac76-304">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-304">Yes</span></span>      | <span data-ttu-id="eac76-305">UserRemove</span><span class="sxs-lookup"><span data-stu-id="eac76-305">UserRemove</span></span> |
| <span data-ttu-id="eac76-306">motivos</span><span class="sxs-lookup"><span data-stu-id="eac76-306">reason</span></span>           | <span data-ttu-id="eac76-307">String</span><span class="sxs-lookup"><span data-stu-id="eac76-307">String</span></span>                                                   | <span data-ttu-id="eac76-308">Não</span><span class="sxs-lookup"><span data-stu-id="eac76-308">No</span></span>       |   |
| <span data-ttu-id="eac76-309">futebol</span><span class="sxs-lookup"><span data-stu-id="eac76-309">schedule</span></span>         | [<span data-ttu-id="eac76-310">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="eac76-310">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="eac76-311">Não</span><span class="sxs-lookup"><span data-stu-id="eac76-311">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="eac76-312">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eac76-312">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="eac76-313">Resposta</span><span class="sxs-lookup"><span data-stu-id="eac76-313">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="eac76-314">Exemplo 4: o administrador remove o usuário de uma função</span><span class="sxs-lookup"><span data-stu-id="eac76-314">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="eac76-315">Neste exemplo, um administrador remove o usuário nawu@fimdev.net da função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="eac76-315">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="eac76-316">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="eac76-316">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="eac76-317">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eac76-317">Property</span></span>         | <span data-ttu-id="eac76-318">Tipo</span><span class="sxs-lookup"><span data-stu-id="eac76-318">Type</span></span>                                                     | <span data-ttu-id="eac76-319">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="eac76-319">Required</span></span> | <span data-ttu-id="eac76-320">Valor</span><span class="sxs-lookup"><span data-stu-id="eac76-320">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="eac76-321">resourceId</span><span class="sxs-lookup"><span data-stu-id="eac76-321">resourceId</span></span>       | <span data-ttu-id="eac76-322">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eac76-322">String</span></span>                                                   | <span data-ttu-id="eac76-323">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-323">Yes</span></span>      | <span data-ttu-id="eac76-324">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="eac76-324">\<resourceId\></span></span> |
| <span data-ttu-id="eac76-325">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="eac76-325">roleDefinitionId</span></span> | <span data-ttu-id="eac76-326">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eac76-326">String</span></span>                                                   | <span data-ttu-id="eac76-327">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-327">Yes</span></span>      | <span data-ttu-id="eac76-328">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="eac76-328">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="eac76-329">SubjectID</span><span class="sxs-lookup"><span data-stu-id="eac76-329">subjectId</span></span>        | <span data-ttu-id="eac76-330">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eac76-330">String</span></span>                                                   | <span data-ttu-id="eac76-331">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-331">Yes</span></span>      | <span data-ttu-id="eac76-332">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="eac76-332">\<subjectId\></span></span> |
| <span data-ttu-id="eac76-333">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="eac76-333">assignmentState</span></span>  | <span data-ttu-id="eac76-334">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eac76-334">String</span></span>                                                   | <span data-ttu-id="eac76-335">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-335">Yes</span></span>      | <span data-ttu-id="eac76-336">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="eac76-336">Eligible / Active</span></span> |
| <span data-ttu-id="eac76-337">type</span><span class="sxs-lookup"><span data-stu-id="eac76-337">type</span></span>             | <span data-ttu-id="eac76-338">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eac76-338">String</span></span>                                                   | <span data-ttu-id="eac76-339">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-339">Yes</span></span>      | <span data-ttu-id="eac76-340">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="eac76-340">AdminRemove</span></span> |
| <span data-ttu-id="eac76-341">motivos</span><span class="sxs-lookup"><span data-stu-id="eac76-341">reason</span></span>           | <span data-ttu-id="eac76-342">String</span><span class="sxs-lookup"><span data-stu-id="eac76-342">String</span></span>                                                   | <span data-ttu-id="eac76-343">Não</span><span class="sxs-lookup"><span data-stu-id="eac76-343">No</span></span>       |   |
| <span data-ttu-id="eac76-344">futebol</span><span class="sxs-lookup"><span data-stu-id="eac76-344">schedule</span></span>         | [<span data-ttu-id="eac76-345">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="eac76-345">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="eac76-346">Não</span><span class="sxs-lookup"><span data-stu-id="eac76-346">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="eac76-347">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eac76-347">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="eac76-348">Resposta</span><span class="sxs-lookup"><span data-stu-id="eac76-348">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="eac76-349">Exemplo 5: atribuição de função de atualização do administrador</span><span class="sxs-lookup"><span data-stu-id="eac76-349">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="eac76-350">Neste exemplo, os administradores atualizam a atribuição de função para o usuário nawu@fimdev.net para o proprietário.</span><span class="sxs-lookup"><span data-stu-id="eac76-350">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="eac76-351">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="eac76-351">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="eac76-352">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eac76-352">Property</span></span>         | <span data-ttu-id="eac76-353">Tipo</span><span class="sxs-lookup"><span data-stu-id="eac76-353">Type</span></span>                                                     | <span data-ttu-id="eac76-354">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="eac76-354">Required</span></span>                | <span data-ttu-id="eac76-355">Valor</span><span class="sxs-lookup"><span data-stu-id="eac76-355">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="eac76-356">resourceId</span><span class="sxs-lookup"><span data-stu-id="eac76-356">resourceId</span></span>       | <span data-ttu-id="eac76-357">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eac76-357">String</span></span>                                                   | <span data-ttu-id="eac76-358">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-358">Yes</span></span>                     | <span data-ttu-id="eac76-359">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="eac76-359">\<resourceId\></span></span> |
| <span data-ttu-id="eac76-360">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="eac76-360">roleDefinitionId</span></span> | <span data-ttu-id="eac76-361">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eac76-361">String</span></span>                                                   | <span data-ttu-id="eac76-362">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-362">Yes</span></span>                     | <span data-ttu-id="eac76-363">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="eac76-363">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="eac76-364">SubjectID</span><span class="sxs-lookup"><span data-stu-id="eac76-364">subjectId</span></span>        | <span data-ttu-id="eac76-365">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eac76-365">String</span></span>                                                   | <span data-ttu-id="eac76-366">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-366">Yes</span></span>                     | <span data-ttu-id="eac76-367">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="eac76-367">\<subjectId\></span></span> |
| <span data-ttu-id="eac76-368">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="eac76-368">assignmentState</span></span>  | <span data-ttu-id="eac76-369">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eac76-369">String</span></span>                                                   | <span data-ttu-id="eac76-370">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-370">Yes</span></span>                     | <span data-ttu-id="eac76-371">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="eac76-371">Eligible / Active</span></span> |
| <span data-ttu-id="eac76-372">type</span><span class="sxs-lookup"><span data-stu-id="eac76-372">type</span></span>             | <span data-ttu-id="eac76-373">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eac76-373">String</span></span>                                                   | <span data-ttu-id="eac76-374">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-374">Yes</span></span>                     | <span data-ttu-id="eac76-375">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="eac76-375">AdminUpdate</span></span> |
| <span data-ttu-id="eac76-376">motivos</span><span class="sxs-lookup"><span data-stu-id="eac76-376">reason</span></span>           | <span data-ttu-id="eac76-377">String</span><span class="sxs-lookup"><span data-stu-id="eac76-377">String</span></span>                                                   | <span data-ttu-id="eac76-378">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="eac76-378">depends on roleSettings</span></span> |   |
| <span data-ttu-id="eac76-379">futebol</span><span class="sxs-lookup"><span data-stu-id="eac76-379">schedule</span></span>         | [<span data-ttu-id="eac76-380">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="eac76-380">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="eac76-381">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-381">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="eac76-382">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eac76-382">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="eac76-383">Resposta</span><span class="sxs-lookup"><span data-stu-id="eac76-383">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="eac76-384">Exemplo 6: administrador estende a atribuição de função de expiração</span><span class="sxs-lookup"><span data-stu-id="eac76-384">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="eac76-385">Este exemplo estende a atribuição de função de expiração para o usuário ANUJCUSER para o colaborador do serviço de gerenciamento de API.</span><span class="sxs-lookup"><span data-stu-id="eac76-385">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="eac76-386">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="eac76-386">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="eac76-387">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eac76-387">Property</span></span>         | <span data-ttu-id="eac76-388">Tipo</span><span class="sxs-lookup"><span data-stu-id="eac76-388">Type</span></span>                                                     | <span data-ttu-id="eac76-389">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="eac76-389">Required</span></span>                | <span data-ttu-id="eac76-390">Valor</span><span class="sxs-lookup"><span data-stu-id="eac76-390">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="eac76-391">resourceId</span><span class="sxs-lookup"><span data-stu-id="eac76-391">resourceId</span></span>       | <span data-ttu-id="eac76-392">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eac76-392">String</span></span>                                                   | <span data-ttu-id="eac76-393">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-393">Yes</span></span>                     | <span data-ttu-id="eac76-394">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="eac76-394">\<resourceId\></span></span> |
| <span data-ttu-id="eac76-395">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="eac76-395">roleDefinitionId</span></span> | <span data-ttu-id="eac76-396">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eac76-396">String</span></span>                                                   | <span data-ttu-id="eac76-397">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-397">Yes</span></span>                     | <span data-ttu-id="eac76-398">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="eac76-398">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="eac76-399">SubjectID</span><span class="sxs-lookup"><span data-stu-id="eac76-399">subjectId</span></span>        | <span data-ttu-id="eac76-400">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eac76-400">String</span></span>                                                   | <span data-ttu-id="eac76-401">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-401">Yes</span></span>                     | <span data-ttu-id="eac76-402">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="eac76-402">\<subjectId\></span></span> |
| <span data-ttu-id="eac76-403">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="eac76-403">assignmentState</span></span>  | <span data-ttu-id="eac76-404">String</span><span class="sxs-lookup"><span data-stu-id="eac76-404">String</span></span>                                                   | <span data-ttu-id="eac76-405">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-405">Yes</span></span>                     | <span data-ttu-id="eac76-406">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="eac76-406">Eligible / Active</span></span> |
| <span data-ttu-id="eac76-407">type</span><span class="sxs-lookup"><span data-stu-id="eac76-407">type</span></span>             | <span data-ttu-id="eac76-408">String</span><span class="sxs-lookup"><span data-stu-id="eac76-408">String</span></span>                                                   | <span data-ttu-id="eac76-409">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-409">Yes</span></span>                     | <span data-ttu-id="eac76-410">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="eac76-410">AdminExtend</span></span> |
| <span data-ttu-id="eac76-411">motivos</span><span class="sxs-lookup"><span data-stu-id="eac76-411">reason</span></span>           | <span data-ttu-id="eac76-412">String</span><span class="sxs-lookup"><span data-stu-id="eac76-412">String</span></span>                                                   | <span data-ttu-id="eac76-413">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="eac76-413">depends on roleSettings</span></span> |   |
| <span data-ttu-id="eac76-414">futebol</span><span class="sxs-lookup"><span data-stu-id="eac76-414">schedule</span></span>         | [<span data-ttu-id="eac76-415">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="eac76-415">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="eac76-416">Sim</span><span class="sxs-lookup"><span data-stu-id="eac76-416">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="eac76-417">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eac76-417">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="eac76-418">Resposta</span><span class="sxs-lookup"><span data-stu-id="eac76-418">Response</span></span>

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
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
