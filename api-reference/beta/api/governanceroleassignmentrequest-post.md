---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função. A tabela a seguir lista as operações.
localization_priority: Normal
ms.openlocfilehash: b9b5f701f3f8ad283f589d07b250ce8ea63aa479
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329608"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="f2ddd-104">Criar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f2ddd-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2ddd-105">Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="f2ddd-106">A tabela a seguir lista as operações.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-106">The following table lists the operations.</span></span>

| <span data-ttu-id="f2ddd-107">Operação</span><span class="sxs-lookup"><span data-stu-id="f2ddd-107">Operation</span></span>                                   | <span data-ttu-id="f2ddd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="f2ddd-109">Atribuir uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="f2ddd-109">Assign a role assignment</span></span>                    | <span data-ttu-id="f2ddd-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="f2ddd-110">AdminAdd</span></span>    |
| <span data-ttu-id="f2ddd-111">Ativar uma atribuição de função qualificada</span><span class="sxs-lookup"><span data-stu-id="f2ddd-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="f2ddd-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="f2ddd-112">UserAdd</span></span>     |
| <span data-ttu-id="f2ddd-113">Desativar uma atribuição de função ativada</span><span class="sxs-lookup"><span data-stu-id="f2ddd-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="f2ddd-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="f2ddd-114">UserRemove</span></span>  |
| <span data-ttu-id="f2ddd-115">Remover uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="f2ddd-115">Remove a role assignment</span></span>                    | <span data-ttu-id="f2ddd-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="f2ddd-116">AdminRemove</span></span> |
| <span data-ttu-id="f2ddd-117">Atualizar uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="f2ddd-117">Update a role assignment</span></span>                    | <span data-ttu-id="f2ddd-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="f2ddd-118">AdminUpdate</span></span> |
| <span data-ttu-id="f2ddd-119">Solicitação para estender minha atribuição de função</span><span class="sxs-lookup"><span data-stu-id="f2ddd-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="f2ddd-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="f2ddd-120">UserExtend</span></span>  |
| <span data-ttu-id="f2ddd-121">Estender uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="f2ddd-121">Extend a role assignment</span></span>                    | <span data-ttu-id="f2ddd-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="f2ddd-122">AdminExtend</span></span> |
| <span data-ttu-id="f2ddd-123">Solicitação para renovar minha atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="f2ddd-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="f2ddd-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="f2ddd-124">UserRenew</span></span>   |
| <span data-ttu-id="f2ddd-125">ReNovar uma atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="f2ddd-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="f2ddd-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="f2ddd-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="f2ddd-127">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2ddd-127">Permissions</span></span>

<span data-ttu-id="f2ddd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2ddd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2ddd-130">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2ddd-130">Permission type</span></span>                        | <span data-ttu-id="f2ddd-131">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2ddd-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="f2ddd-132">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2ddd-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2ddd-133">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="f2ddd-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="f2ddd-134">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2ddd-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2ddd-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-135">Not supported.</span></span>                            |
| <span data-ttu-id="f2ddd-136">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-136">Application</span></span>                            | <span data-ttu-id="f2ddd-137">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="f2ddd-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2ddd-138">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2ddd-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="f2ddd-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2ddd-139">Request headers</span></span>

| <span data-ttu-id="f2ddd-140">Nome</span><span class="sxs-lookup"><span data-stu-id="f2ddd-140">Name</span></span>          | <span data-ttu-id="f2ddd-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2ddd-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="f2ddd-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2ddd-142">Authorization</span></span> | <span data-ttu-id="f2ddd-143">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f2ddd-143">Bearer {code}</span></span>    |
| <span data-ttu-id="f2ddd-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="f2ddd-144">Content-type</span></span>  | <span data-ttu-id="f2ddd-145">application/json</span><span class="sxs-lookup"><span data-stu-id="f2ddd-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2ddd-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2ddd-146">Request body</span></span>

<span data-ttu-id="f2ddd-147">No corpo da solicitação, forneça uma representação JSON de um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="f2ddd-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="f2ddd-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2ddd-148">Property</span></span>         | <span data-ttu-id="f2ddd-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-149">Type</span></span>                                                     | <span data-ttu-id="f2ddd-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2ddd-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="f2ddd-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="f2ddd-151">resourceId</span></span>       | <span data-ttu-id="f2ddd-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2ddd-152">String</span></span>                                                   | <span data-ttu-id="f2ddd-153">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-153">The ID of the resource.</span></span> <span data-ttu-id="f2ddd-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-154">Required.</span></span> |
| <span data-ttu-id="f2ddd-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f2ddd-155">roleDefinitionId</span></span> | <span data-ttu-id="f2ddd-156">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-156">String</span></span>                                                   | <span data-ttu-id="f2ddd-157">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-157">The ID of the role definition.</span></span> <span data-ttu-id="f2ddd-158">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-158">Required.</span></span> |
| <span data-ttu-id="f2ddd-159">SubjectID</span><span class="sxs-lookup"><span data-stu-id="f2ddd-159">subjectId</span></span>        | <span data-ttu-id="f2ddd-160">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-160">String</span></span>                                                   | <span data-ttu-id="f2ddd-161">A ID do assunto.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-161">The ID of the subject.</span></span> <span data-ttu-id="f2ddd-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-162">Required.</span></span> |
| <span data-ttu-id="f2ddd-163">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="f2ddd-163">assignmentState</span></span>  | <span data-ttu-id="f2ddd-164">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-164">String</span></span>                                                   | <span data-ttu-id="f2ddd-165">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-165">The state of assignment.</span></span> <span data-ttu-id="f2ddd-166">O valor pode ser `Eligible` e `Active`.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="f2ddd-167">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-167">Required.</span></span> |
| <span data-ttu-id="f2ddd-168">tipo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-168">type</span></span>             | <span data-ttu-id="f2ddd-169">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-169">String</span></span>                                                   | <span data-ttu-id="f2ddd-170">O tipo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-170">The request type.</span></span> <span data-ttu-id="f2ddd-171">O valor pode ser `AdminAdd`, `UserAdd`, `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew`,,,, `AdminRenew`e. `AdminExtend`</span><span class="sxs-lookup"><span data-stu-id="f2ddd-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="f2ddd-172">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-172">Required.</span></span> |
| <span data-ttu-id="f2ddd-173">motivos</span><span class="sxs-lookup"><span data-stu-id="f2ddd-173">reason</span></span>           | <span data-ttu-id="f2ddd-174">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-174">String</span></span>                                                   | <span data-ttu-id="f2ddd-175">O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e análise.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="f2ddd-176">futebol</span><span class="sxs-lookup"><span data-stu-id="f2ddd-176">schedule</span></span>         | [<span data-ttu-id="f2ddd-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f2ddd-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="f2ddd-178">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="f2ddd-179">Para o tipo de `UserAdd`solicitação `AdminAdd`de `AdminUpdate`,, `AdminExtend`, e, é necessário.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="f2ddd-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2ddd-180">Response</span></span>

<span data-ttu-id="f2ddd-181">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="f2ddd-182">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="f2ddd-182">Error codes</span></span>

<span data-ttu-id="f2ddd-183">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="f2ddd-184">Além disso, ele também retorna os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="f2ddd-185">Código de erro</span><span class="sxs-lookup"><span data-stu-id="f2ddd-185">Error code</span></span>     | <span data-ttu-id="f2ddd-186">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="f2ddd-186">Error message</span></span>                               | <span data-ttu-id="f2ddd-187">Detalhes</span><span class="sxs-lookup"><span data-stu-id="f2ddd-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="f2ddd-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2ddd-188">400 BadRequest</span></span> | <span data-ttu-id="f2ddd-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="f2ddd-189">RoleNotFound</span></span>                                | <span data-ttu-id="f2ddd-190">O `roleDefinitionId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="f2ddd-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2ddd-191">400 BadRequest</span></span> | <span data-ttu-id="f2ddd-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="f2ddd-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="f2ddd-193">O recurso fornecido no corpo da solicitação está no estado de `Locked` e não pode criar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="f2ddd-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2ddd-194">400 BadRequest</span></span> | <span data-ttu-id="f2ddd-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="f2ddd-195">SubjectNotFound</span></span>                             | <span data-ttu-id="f2ddd-196">O `subjectId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="f2ddd-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2ddd-197">400 BadRequest</span></span> | <span data-ttu-id="f2ddd-198">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f2ddd-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="f2ddd-199">Já existe um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) pendente no sistema.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="f2ddd-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2ddd-200">400 BadRequest</span></span> | <span data-ttu-id="f2ddd-201">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="f2ddd-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="f2ddd-202">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criado já existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="f2ddd-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2ddd-203">400 BadRequest</span></span> | <span data-ttu-id="f2ddd-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="f2ddd-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="f2ddd-205">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="f2ddd-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2ddd-206">400 BadRequest</span></span> | <span data-ttu-id="f2ddd-207">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="f2ddd-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="f2ddd-208">O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não atende às políticas internas e não pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="f2ddd-209">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f2ddd-209">Examples</span></span>

<span data-ttu-id="f2ddd-210">Os exemplos a seguir mostram como usar essa API.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="f2ddd-211">Exemplo 1: o administrador atribui um usuário a uma função</span><span class="sxs-lookup"><span data-stu-id="f2ddd-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="f2ddd-212">Neste exemplo, um administrador atribui o usuário nawu@fimdev.net à função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="f2ddd-213">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="f2ddd-214">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2ddd-214">Property</span></span>         | <span data-ttu-id="f2ddd-215">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-215">Type</span></span>                                                     | <span data-ttu-id="f2ddd-216">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="f2ddd-216">Required</span></span>                 | <span data-ttu-id="f2ddd-217">Valor</span><span class="sxs-lookup"><span data-stu-id="f2ddd-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="f2ddd-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="f2ddd-218">resourceId</span></span>       | <span data-ttu-id="f2ddd-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2ddd-219">String</span></span>                                                   | <span data-ttu-id="f2ddd-220">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-220">Yes</span></span>                      | <span data-ttu-id="f2ddd-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-221">\<resourceId\></span></span> |
| <span data-ttu-id="f2ddd-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f2ddd-222">roleDefinitionId</span></span> | <span data-ttu-id="f2ddd-223">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-223">String</span></span>                                                   | <span data-ttu-id="f2ddd-224">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-224">Yes</span></span>                      | <span data-ttu-id="f2ddd-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="f2ddd-226">SubjectID</span><span class="sxs-lookup"><span data-stu-id="f2ddd-226">subjectId</span></span>        | <span data-ttu-id="f2ddd-227">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-227">String</span></span>                                                   | <span data-ttu-id="f2ddd-228">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-228">Yes</span></span>                      | <span data-ttu-id="f2ddd-229">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-229">\<subjectId\></span></span> |
| <span data-ttu-id="f2ddd-230">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="f2ddd-230">assignmentState</span></span>  | <span data-ttu-id="f2ddd-231">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-231">String</span></span>                                                   | <span data-ttu-id="f2ddd-232">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-232">Yes</span></span>                      | <span data-ttu-id="f2ddd-233">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-233">Eligible / Active</span></span> |
| <span data-ttu-id="f2ddd-234">tipo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-234">type</span></span>             | <span data-ttu-id="f2ddd-235">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-235">String</span></span>                                                   | <span data-ttu-id="f2ddd-236">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-236">Yes</span></span>                      | <span data-ttu-id="f2ddd-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="f2ddd-237">AdminAdd</span></span> |
| <span data-ttu-id="f2ddd-238">motivos</span><span class="sxs-lookup"><span data-stu-id="f2ddd-238">reason</span></span>           | <span data-ttu-id="f2ddd-239">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-239">String</span></span>                                                   | <span data-ttu-id="f2ddd-240">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="f2ddd-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="f2ddd-241">futebol</span><span class="sxs-lookup"><span data-stu-id="f2ddd-241">schedule</span></span>         | [<span data-ttu-id="f2ddd-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f2ddd-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="f2ddd-243">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="f2ddd-244">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2ddd-244">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="f2ddd-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2ddd-245">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="f2ddd-246">Exemplo 2: o usuário ativa a função qualificada</span><span class="sxs-lookup"><span data-stu-id="f2ddd-246">Example 2: User activates eligible role</span></span>

<span data-ttu-id="f2ddd-247">Neste exemplo, o usuário nawu@fimdev.net ativa a função de leitor de cobrança qualificado.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-247">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="f2ddd-248">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2ddd-248">Property</span></span>         | <span data-ttu-id="f2ddd-249">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-249">Type</span></span>                                                     | <span data-ttu-id="f2ddd-250">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="f2ddd-250">Required</span></span>                 | <span data-ttu-id="f2ddd-251">Valor</span><span class="sxs-lookup"><span data-stu-id="f2ddd-251">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="f2ddd-252">resourceId</span><span class="sxs-lookup"><span data-stu-id="f2ddd-252">resourceId</span></span>       | <span data-ttu-id="f2ddd-253">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2ddd-253">String</span></span>                                                   | <span data-ttu-id="f2ddd-254">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-254">Yes</span></span>                      | <span data-ttu-id="f2ddd-255">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-255">\<resourceId\></span></span> |
| <span data-ttu-id="f2ddd-256">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f2ddd-256">roleDefinitionId</span></span> | <span data-ttu-id="f2ddd-257">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-257">String</span></span>                                                   | <span data-ttu-id="f2ddd-258">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-258">Yes</span></span>                      | <span data-ttu-id="f2ddd-259">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-259">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="f2ddd-260">SubjectID</span><span class="sxs-lookup"><span data-stu-id="f2ddd-260">subjectId</span></span>        | <span data-ttu-id="f2ddd-261">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-261">String</span></span>                                                   | <span data-ttu-id="f2ddd-262">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-262">Yes</span></span>                      | <span data-ttu-id="f2ddd-263">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-263">\<subjectId\></span></span> |
| <span data-ttu-id="f2ddd-264">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="f2ddd-264">assignmentState</span></span>  | <span data-ttu-id="f2ddd-265">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-265">String</span></span>                                                   | <span data-ttu-id="f2ddd-266">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-266">Yes</span></span>                      | <span data-ttu-id="f2ddd-267">Ativo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-267">Active</span></span> |
| <span data-ttu-id="f2ddd-268">tipo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-268">type</span></span>             | <span data-ttu-id="f2ddd-269">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-269">String</span></span>                                                   | <span data-ttu-id="f2ddd-270">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-270">Yes</span></span>                      | <span data-ttu-id="f2ddd-271">UserAdd</span><span class="sxs-lookup"><span data-stu-id="f2ddd-271">UserAdd</span></span> |
| <span data-ttu-id="f2ddd-272">motivos</span><span class="sxs-lookup"><span data-stu-id="f2ddd-272">reason</span></span>           | <span data-ttu-id="f2ddd-273">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-273">String</span></span>                                                   | <span data-ttu-id="f2ddd-274">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="f2ddd-274">depends on role Settings</span></span> |   |
| <span data-ttu-id="f2ddd-275">futebol</span><span class="sxs-lookup"><span data-stu-id="f2ddd-275">schedule</span></span>         | [<span data-ttu-id="f2ddd-276">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f2ddd-276">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="f2ddd-277">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-277">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="f2ddd-278">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2ddd-278">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="f2ddd-279">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2ddd-279">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="f2ddd-280">Exemplo 3: o usuário desativa uma função atribuída</span><span class="sxs-lookup"><span data-stu-id="f2ddd-280">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="f2ddd-281">Neste exemplo, o usuário nawu@fimdev.net desativa a função de leitor de cobrança ativa.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-281">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="f2ddd-282">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2ddd-282">Property</span></span>         | <span data-ttu-id="f2ddd-283">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-283">Type</span></span>                                                     | <span data-ttu-id="f2ddd-284">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="f2ddd-284">Required</span></span> | <span data-ttu-id="f2ddd-285">Valor</span><span class="sxs-lookup"><span data-stu-id="f2ddd-285">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="f2ddd-286">resourceId</span><span class="sxs-lookup"><span data-stu-id="f2ddd-286">resourceId</span></span>       | <span data-ttu-id="f2ddd-287">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2ddd-287">String</span></span>                                                   | <span data-ttu-id="f2ddd-288">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-288">Yes</span></span>      | <span data-ttu-id="f2ddd-289">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-289">\<resourceId\></span></span> |
| <span data-ttu-id="f2ddd-290">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f2ddd-290">roleDefinitionId</span></span> | <span data-ttu-id="f2ddd-291">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-291">String</span></span>                                                   | <span data-ttu-id="f2ddd-292">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-292">Yes</span></span>      | <span data-ttu-id="f2ddd-293">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-293">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="f2ddd-294">SubjectID</span><span class="sxs-lookup"><span data-stu-id="f2ddd-294">subjectId</span></span>        | <span data-ttu-id="f2ddd-295">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-295">String</span></span>                                                   | <span data-ttu-id="f2ddd-296">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-296">Yes</span></span>      | <span data-ttu-id="f2ddd-297">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-297">\<subjectId\></span></span> |
| <span data-ttu-id="f2ddd-298">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="f2ddd-298">assignmentState</span></span>  | <span data-ttu-id="f2ddd-299">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-299">String</span></span>                                                   | <span data-ttu-id="f2ddd-300">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-300">Yes</span></span>      | <span data-ttu-id="f2ddd-301">Ativo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-301">Active</span></span> |
| <span data-ttu-id="f2ddd-302">tipo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-302">type</span></span>             | <span data-ttu-id="f2ddd-303">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-303">String</span></span>                                                   | <span data-ttu-id="f2ddd-304">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-304">Yes</span></span>      | <span data-ttu-id="f2ddd-305">UserRemove</span><span class="sxs-lookup"><span data-stu-id="f2ddd-305">UserRemove</span></span> |
| <span data-ttu-id="f2ddd-306">motivos</span><span class="sxs-lookup"><span data-stu-id="f2ddd-306">reason</span></span>           | <span data-ttu-id="f2ddd-307">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-307">String</span></span>                                                   | <span data-ttu-id="f2ddd-308">Não</span><span class="sxs-lookup"><span data-stu-id="f2ddd-308">No</span></span>       |   |
| <span data-ttu-id="f2ddd-309">futebol</span><span class="sxs-lookup"><span data-stu-id="f2ddd-309">schedule</span></span>         | [<span data-ttu-id="f2ddd-310">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f2ddd-310">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="f2ddd-311">Não</span><span class="sxs-lookup"><span data-stu-id="f2ddd-311">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="f2ddd-312">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2ddd-312">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="f2ddd-313">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2ddd-313">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="f2ddd-314">Exemplo 4: o administrador remove o usuário de uma função</span><span class="sxs-lookup"><span data-stu-id="f2ddd-314">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="f2ddd-315">Neste exemplo, um administrador remove o usuário nawu@fimdev.net da função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-315">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="f2ddd-316">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-316">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="f2ddd-317">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2ddd-317">Property</span></span>         | <span data-ttu-id="f2ddd-318">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-318">Type</span></span>                                                     | <span data-ttu-id="f2ddd-319">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="f2ddd-319">Required</span></span> | <span data-ttu-id="f2ddd-320">Valor</span><span class="sxs-lookup"><span data-stu-id="f2ddd-320">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="f2ddd-321">resourceId</span><span class="sxs-lookup"><span data-stu-id="f2ddd-321">resourceId</span></span>       | <span data-ttu-id="f2ddd-322">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2ddd-322">String</span></span>                                                   | <span data-ttu-id="f2ddd-323">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-323">Yes</span></span>      | <span data-ttu-id="f2ddd-324">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-324">\<resourceId\></span></span> |
| <span data-ttu-id="f2ddd-325">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f2ddd-325">roleDefinitionId</span></span> | <span data-ttu-id="f2ddd-326">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-326">String</span></span>                                                   | <span data-ttu-id="f2ddd-327">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-327">Yes</span></span>      | <span data-ttu-id="f2ddd-328">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-328">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="f2ddd-329">SubjectID</span><span class="sxs-lookup"><span data-stu-id="f2ddd-329">subjectId</span></span>        | <span data-ttu-id="f2ddd-330">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-330">String</span></span>                                                   | <span data-ttu-id="f2ddd-331">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-331">Yes</span></span>      | <span data-ttu-id="f2ddd-332">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-332">\<subjectId\></span></span> |
| <span data-ttu-id="f2ddd-333">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="f2ddd-333">assignmentState</span></span>  | <span data-ttu-id="f2ddd-334">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-334">String</span></span>                                                   | <span data-ttu-id="f2ddd-335">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-335">Yes</span></span>      | <span data-ttu-id="f2ddd-336">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-336">Eligible / Active</span></span> |
| <span data-ttu-id="f2ddd-337">tipo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-337">type</span></span>             | <span data-ttu-id="f2ddd-338">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-338">String</span></span>                                                   | <span data-ttu-id="f2ddd-339">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-339">Yes</span></span>      | <span data-ttu-id="f2ddd-340">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="f2ddd-340">AdminRemove</span></span> |
| <span data-ttu-id="f2ddd-341">motivos</span><span class="sxs-lookup"><span data-stu-id="f2ddd-341">reason</span></span>           | <span data-ttu-id="f2ddd-342">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-342">String</span></span>                                                   | <span data-ttu-id="f2ddd-343">Não</span><span class="sxs-lookup"><span data-stu-id="f2ddd-343">No</span></span>       |   |
| <span data-ttu-id="f2ddd-344">futebol</span><span class="sxs-lookup"><span data-stu-id="f2ddd-344">schedule</span></span>         | [<span data-ttu-id="f2ddd-345">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f2ddd-345">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="f2ddd-346">Não</span><span class="sxs-lookup"><span data-stu-id="f2ddd-346">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="f2ddd-347">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2ddd-347">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="f2ddd-348">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2ddd-348">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="f2ddd-349">Exemplo 5: atribuição de função de atualização do administrador</span><span class="sxs-lookup"><span data-stu-id="f2ddd-349">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="f2ddd-350">Neste exemplo, os administradores atualizam a atribuição de função para o usuário nawu@fimdev.net para o proprietário.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-350">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="f2ddd-351">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-351">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="f2ddd-352">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2ddd-352">Property</span></span>         | <span data-ttu-id="f2ddd-353">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-353">Type</span></span>                                                     | <span data-ttu-id="f2ddd-354">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="f2ddd-354">Required</span></span>                | <span data-ttu-id="f2ddd-355">Valor</span><span class="sxs-lookup"><span data-stu-id="f2ddd-355">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="f2ddd-356">resourceId</span><span class="sxs-lookup"><span data-stu-id="f2ddd-356">resourceId</span></span>       | <span data-ttu-id="f2ddd-357">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2ddd-357">String</span></span>                                                   | <span data-ttu-id="f2ddd-358">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-358">Yes</span></span>                     | <span data-ttu-id="f2ddd-359">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-359">\<resourceId\></span></span> |
| <span data-ttu-id="f2ddd-360">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f2ddd-360">roleDefinitionId</span></span> | <span data-ttu-id="f2ddd-361">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-361">String</span></span>                                                   | <span data-ttu-id="f2ddd-362">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-362">Yes</span></span>                     | <span data-ttu-id="f2ddd-363">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-363">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="f2ddd-364">SubjectID</span><span class="sxs-lookup"><span data-stu-id="f2ddd-364">subjectId</span></span>        | <span data-ttu-id="f2ddd-365">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-365">String</span></span>                                                   | <span data-ttu-id="f2ddd-366">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-366">Yes</span></span>                     | <span data-ttu-id="f2ddd-367">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-367">\<subjectId\></span></span> |
| <span data-ttu-id="f2ddd-368">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="f2ddd-368">assignmentState</span></span>  | <span data-ttu-id="f2ddd-369">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-369">String</span></span>                                                   | <span data-ttu-id="f2ddd-370">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-370">Yes</span></span>                     | <span data-ttu-id="f2ddd-371">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-371">Eligible / Active</span></span> |
| <span data-ttu-id="f2ddd-372">tipo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-372">type</span></span>             | <span data-ttu-id="f2ddd-373">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-373">String</span></span>                                                   | <span data-ttu-id="f2ddd-374">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-374">Yes</span></span>                     | <span data-ttu-id="f2ddd-375">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="f2ddd-375">AdminUpdate</span></span> |
| <span data-ttu-id="f2ddd-376">motivos</span><span class="sxs-lookup"><span data-stu-id="f2ddd-376">reason</span></span>           | <span data-ttu-id="f2ddd-377">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-377">String</span></span>                                                   | <span data-ttu-id="f2ddd-378">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="f2ddd-378">depends on roleSettings</span></span> |   |
| <span data-ttu-id="f2ddd-379">futebol</span><span class="sxs-lookup"><span data-stu-id="f2ddd-379">schedule</span></span>         | [<span data-ttu-id="f2ddd-380">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f2ddd-380">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="f2ddd-381">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-381">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="f2ddd-382">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2ddd-382">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="f2ddd-383">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2ddd-383">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="f2ddd-384">Exemplo 6: administrador estende a atribuição de função de expiração</span><span class="sxs-lookup"><span data-stu-id="f2ddd-384">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="f2ddd-385">Este exemplo estende a atribuição de função de expiração para o usuário ANUJCUSER para o colaborador do serviço de gerenciamento de API.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-385">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="f2ddd-386">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="f2ddd-386">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="f2ddd-387">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2ddd-387">Property</span></span>         | <span data-ttu-id="f2ddd-388">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-388">Type</span></span>                                                     | <span data-ttu-id="f2ddd-389">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="f2ddd-389">Required</span></span>                | <span data-ttu-id="f2ddd-390">Valor</span><span class="sxs-lookup"><span data-stu-id="f2ddd-390">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="f2ddd-391">resourceId</span><span class="sxs-lookup"><span data-stu-id="f2ddd-391">resourceId</span></span>       | <span data-ttu-id="f2ddd-392">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2ddd-392">String</span></span>                                                   | <span data-ttu-id="f2ddd-393">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-393">Yes</span></span>                     | <span data-ttu-id="f2ddd-394">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-394">\<resourceId\></span></span> |
| <span data-ttu-id="f2ddd-395">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f2ddd-395">roleDefinitionId</span></span> | <span data-ttu-id="f2ddd-396">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-396">String</span></span>                                                   | <span data-ttu-id="f2ddd-397">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-397">Yes</span></span>                     | <span data-ttu-id="f2ddd-398">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-398">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="f2ddd-399">SubjectID</span><span class="sxs-lookup"><span data-stu-id="f2ddd-399">subjectId</span></span>        | <span data-ttu-id="f2ddd-400">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-400">String</span></span>                                                   | <span data-ttu-id="f2ddd-401">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-401">Yes</span></span>                     | <span data-ttu-id="f2ddd-402">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="f2ddd-402">\<subjectId\></span></span> |
| <span data-ttu-id="f2ddd-403">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="f2ddd-403">assignmentState</span></span>  | <span data-ttu-id="f2ddd-404">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-404">String</span></span>                                                   | <span data-ttu-id="f2ddd-405">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-405">Yes</span></span>                     | <span data-ttu-id="f2ddd-406">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-406">Eligible / Active</span></span> |
| <span data-ttu-id="f2ddd-407">tipo</span><span class="sxs-lookup"><span data-stu-id="f2ddd-407">type</span></span>             | <span data-ttu-id="f2ddd-408">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-408">String</span></span>                                                   | <span data-ttu-id="f2ddd-409">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-409">Yes</span></span>                     | <span data-ttu-id="f2ddd-410">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="f2ddd-410">AdminExtend</span></span> |
| <span data-ttu-id="f2ddd-411">motivos</span><span class="sxs-lookup"><span data-stu-id="f2ddd-411">reason</span></span>           | <span data-ttu-id="f2ddd-412">String</span><span class="sxs-lookup"><span data-stu-id="f2ddd-412">String</span></span>                                                   | <span data-ttu-id="f2ddd-413">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="f2ddd-413">depends on roleSettings</span></span> |   |
| <span data-ttu-id="f2ddd-414">futebol</span><span class="sxs-lookup"><span data-stu-id="f2ddd-414">schedule</span></span>         | [<span data-ttu-id="f2ddd-415">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f2ddd-415">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="f2ddd-416">Sim</span><span class="sxs-lookup"><span data-stu-id="f2ddd-416">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="f2ddd-417">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2ddd-417">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="f2ddd-418">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2ddd-418">Response</span></span>

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
  "suppressions": []
}
-->
