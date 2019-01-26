---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação desejado em uma atribuição de função. A tabela a seguir lista as operações.
localization_priority: Normal
ms.openlocfilehash: 0fc8d96585daf63f53bc6b33985a289e8f810d6b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572364"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="03a6a-104">Criar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="03a6a-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03a6a-105">Crie uma solicitação de atribuição de função para representar a operação desejado em uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="03a6a-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="03a6a-106">A tabela a seguir lista as operações.</span><span class="sxs-lookup"><span data-stu-id="03a6a-106">The following table lists the operations.</span></span>

| <span data-ttu-id="03a6a-107">Operation</span><span class="sxs-lookup"><span data-stu-id="03a6a-107">Operation</span></span>       | <span data-ttu-id="03a6a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="03a6a-108">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="03a6a-109">Atribuir uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="03a6a-109">Assign a role assignment</span></span>| <span data-ttu-id="03a6a-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="03a6a-110">AdminAdd</span></span> |
| <span data-ttu-id="03a6a-111">Ativar uma atribuição de função elegíveis</span><span class="sxs-lookup"><span data-stu-id="03a6a-111">Activate an eligible role assignment</span></span>| <span data-ttu-id="03a6a-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="03a6a-112">UserAdd</span></span> | 
| <span data-ttu-id="03a6a-113">Desativar uma atribuição de função ativada</span><span class="sxs-lookup"><span data-stu-id="03a6a-113">Deactivate an activated role assignment</span></span>| <span data-ttu-id="03a6a-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="03a6a-114">UserRemove</span></span> | 
| <span data-ttu-id="03a6a-115">Remover uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="03a6a-115">Remove a role assignment</span></span>| <span data-ttu-id="03a6a-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="03a6a-116">AdminRemove</span></span> |
| <span data-ttu-id="03a6a-117">Atualizar uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="03a6a-117">Update a role assignment</span></span>| <span data-ttu-id="03a6a-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="03a6a-118">AdminUpdate</span></span> |
| <span data-ttu-id="03a6a-119">Solicitação para estender minha atribuição de função</span><span class="sxs-lookup"><span data-stu-id="03a6a-119">Request to extend my role assignment</span></span>| <span data-ttu-id="03a6a-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="03a6a-120">UserExtend</span></span> | 
| <span data-ttu-id="03a6a-121">Estender uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="03a6a-121">Extend a role assignment</span></span>| <span data-ttu-id="03a6a-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="03a6a-122">AdminExtend</span></span> | 
| <span data-ttu-id="03a6a-123">Solicitação de renovação minha atribuição de função expirados</span><span class="sxs-lookup"><span data-stu-id="03a6a-123">Request to renew my expired role assignment</span></span>| <span data-ttu-id="03a6a-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="03a6a-124">UserRenew</span></span> | 
| <span data-ttu-id="03a6a-125">Renovar uma atribuição de função expirados</span><span class="sxs-lookup"><span data-stu-id="03a6a-125">Renew an expired role assignment</span></span>| <span data-ttu-id="03a6a-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="03a6a-126">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="03a6a-127">Permissões</span><span class="sxs-lookup"><span data-stu-id="03a6a-127">Permissions</span></span>
<span data-ttu-id="03a6a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03a6a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03a6a-130">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03a6a-130">Permission type</span></span>      | <span data-ttu-id="03a6a-131">Permissões</span><span class="sxs-lookup"><span data-stu-id="03a6a-131">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03a6a-132">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03a6a-132">Delegated (work or school account)</span></span> | <span data-ttu-id="03a6a-133">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="03a6a-133">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="03a6a-134">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03a6a-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03a6a-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03a6a-135">Not supported.</span></span>    |
|<span data-ttu-id="03a6a-136">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03a6a-136">Application</span></span> | <span data-ttu-id="03a6a-137">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="03a6a-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="03a6a-138">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03a6a-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="03a6a-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03a6a-139">Request headers</span></span>
| <span data-ttu-id="03a6a-140">Nome</span><span class="sxs-lookup"><span data-stu-id="03a6a-140">Name</span></span>       | <span data-ttu-id="03a6a-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="03a6a-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="03a6a-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="03a6a-142">Authorization</span></span>  | <span data-ttu-id="03a6a-143">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="03a6a-143">Bearer {code}</span></span>|
| <span data-ttu-id="03a6a-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="03a6a-144">Content-type</span></span>  | <span data-ttu-id="03a6a-145">application/json</span><span class="sxs-lookup"><span data-stu-id="03a6a-145">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03a6a-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03a6a-146">Request body</span></span>
<span data-ttu-id="03a6a-147">No corpo da solicitação, fornece uma representação JSON de um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="03a6a-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="03a6a-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03a6a-148">Property</span></span>     | <span data-ttu-id="03a6a-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="03a6a-149">Type</span></span>    |<span data-ttu-id="03a6a-150">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="03a6a-150">Required</span></span>|  <span data-ttu-id="03a6a-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="03a6a-151">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="03a6a-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="03a6a-152">resourceId</span></span>|<span data-ttu-id="03a6a-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03a6a-153">String</span></span>|<span data-ttu-id="03a6a-154">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-154">Yes</span></span>|<span data-ttu-id="03a6a-155">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="03a6a-155">The ID of the resource.</span></span>|
|<span data-ttu-id="03a6a-156">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="03a6a-156">roleDefinitionId</span></span>|<span data-ttu-id="03a6a-157">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-157">String</span></span>|<span data-ttu-id="03a6a-158">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-158">Yes</span></span>|<span data-ttu-id="03a6a-159">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="03a6a-159">The ID of the role definition.</span></span>|
|<span data-ttu-id="03a6a-160">subjectId</span><span class="sxs-lookup"><span data-stu-id="03a6a-160">subjectId</span></span>|<span data-ttu-id="03a6a-161">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-161">String</span></span>|<span data-ttu-id="03a6a-162">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-162">Yes</span></span>|<span data-ttu-id="03a6a-163">A identificação do assunto.</span><span class="sxs-lookup"><span data-stu-id="03a6a-163">The ID of the subject.</span></span>|
|<span data-ttu-id="03a6a-164">assignmentState</span><span class="sxs-lookup"><span data-stu-id="03a6a-164">assignmentState</span></span>|<span data-ttu-id="03a6a-165">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-165">String</span></span>|<span data-ttu-id="03a6a-166">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-166">Yes</span></span>|<span data-ttu-id="03a6a-167">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="03a6a-167">The state of assignment.</span></span> <span data-ttu-id="03a6a-168">O valor pode ser ``Eligible`` e ``Active``.</span><span class="sxs-lookup"><span data-stu-id="03a6a-168">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="03a6a-169">type</span><span class="sxs-lookup"><span data-stu-id="03a6a-169">type</span></span>|<span data-ttu-id="03a6a-170">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-170">String</span></span>|<span data-ttu-id="03a6a-171">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-171">Yes</span></span>|<span data-ttu-id="03a6a-172">O tipo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="03a6a-172">The request type.</span></span> <span data-ttu-id="03a6a-173">O valor pode ser `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`e `AdminExtend`.</span><span class="sxs-lookup"><span data-stu-id="03a6a-173">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="03a6a-174">motivo</span><span class="sxs-lookup"><span data-stu-id="03a6a-174">reason</span></span>|<span data-ttu-id="03a6a-175">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-175">String</span></span>| |<span data-ttu-id="03a6a-176">O motivo pelo qual deve ser fornecido para a solicitação de atribuição de função de auditoria e revise finalidade.</span><span class="sxs-lookup"><span data-stu-id="03a6a-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="03a6a-177">agenda</span><span class="sxs-lookup"><span data-stu-id="03a6a-177">schedule</span></span>|[<span data-ttu-id="03a6a-178">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="03a6a-178">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="03a6a-179">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="03a6a-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="03a6a-180">Tipo de solicitação de `UserAdd`, `AdminAdd`, `AdminUpdate`, e `AdminExtend`, é necessário.</span><span class="sxs-lookup"><span data-stu-id="03a6a-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="03a6a-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="03a6a-181">Response</span></span>
<span data-ttu-id="03a6a-182">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03a6a-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="03a6a-183">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="03a6a-183">Error codes</span></span>
<span data-ttu-id="03a6a-184">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="03a6a-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="03a6a-185">Além disso, ele também retorna os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="03a6a-185">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="03a6a-186">Código de erro</span><span class="sxs-lookup"><span data-stu-id="03a6a-186">Error code</span></span>     | <span data-ttu-id="03a6a-187">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="03a6a-187">Error message</span></span>              | <span data-ttu-id="03a6a-188">Detalhes</span><span class="sxs-lookup"><span data-stu-id="03a6a-188">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="03a6a-189">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="03a6a-189">400 BadRequest</span></span> | <span data-ttu-id="03a6a-190">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="03a6a-190">RoleNotFound</span></span>    | <span data-ttu-id="03a6a-191">O `roleDefinitionId` fornecida na solicitação de corpo não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="03a6a-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="03a6a-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="03a6a-192">400 BadRequest</span></span> | <span data-ttu-id="03a6a-193">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="03a6a-193">ResourceIsLocked</span></span>    | <span data-ttu-id="03a6a-194">O recurso fornecido no corpo da solicitação está em estado de `Locked` e não pode criar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="03a6a-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="03a6a-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="03a6a-195">400 BadRequest</span></span> | <span data-ttu-id="03a6a-196">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="03a6a-196">SubjectNotFound</span></span>    | <span data-ttu-id="03a6a-197">O `subjectId` fornecida na solicitação de corpo não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="03a6a-197">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="03a6a-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="03a6a-198">400 BadRequest</span></span> | <span data-ttu-id="03a6a-199">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="03a6a-199">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="03a6a-200">Já existe uma pendente [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no sistema.</span><span class="sxs-lookup"><span data-stu-id="03a6a-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="03a6a-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="03a6a-201">400 BadRequest</span></span> | <span data-ttu-id="03a6a-202">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="03a6a-202">RoleAssignmentExists</span></span>    | <span data-ttu-id="03a6a-203">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criada já existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="03a6a-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="03a6a-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="03a6a-204">400 BadRequest</span></span> | <span data-ttu-id="03a6a-205">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="03a6a-205">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="03a6a-206">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="03a6a-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="03a6a-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="03a6a-207">400 BadRequest</span></span> | <span data-ttu-id="03a6a-208">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="03a6a-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="03a6a-209">O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não atende às políticas internas e não pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="03a6a-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="03a6a-210">Exemplos</span><span class="sxs-lookup"><span data-stu-id="03a6a-210">Examples</span></span>
<span data-ttu-id="03a6a-211">Os exemplos a seguir mostram como usar essa API.</span><span class="sxs-lookup"><span data-stu-id="03a6a-211">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="03a6a-212">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="03a6a-212">Example 1</span></span>
<span data-ttu-id="03a6a-213">Neste exemplo, os administradores atribuem nawu@fimdev.net usuário à função Leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="03a6a-213">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="03a6a-214">**Observação:** Além de permissão, este exemplo exige que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="03a6a-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="03a6a-215">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03a6a-215">Property</span></span>     | <span data-ttu-id="03a6a-216">Tipo</span><span class="sxs-lookup"><span data-stu-id="03a6a-216">Type</span></span>    |<span data-ttu-id="03a6a-217">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="03a6a-217">Required</span></span>|  <span data-ttu-id="03a6a-218">Valor</span><span class="sxs-lookup"><span data-stu-id="03a6a-218">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="03a6a-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="03a6a-219">resourceId</span></span>|<span data-ttu-id="03a6a-220">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03a6a-220">String</span></span>|<span data-ttu-id="03a6a-221">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-221">Yes</span></span>|<span data-ttu-id="03a6a-222">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-222">\<resourceId\></span></span>|
|<span data-ttu-id="03a6a-223">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="03a6a-223">roleDefinitionId</span></span>|<span data-ttu-id="03a6a-224">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-224">String</span></span>|<span data-ttu-id="03a6a-225">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-225">Yes</span></span>|<span data-ttu-id="03a6a-226">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-226">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="03a6a-227">subjectId</span><span class="sxs-lookup"><span data-stu-id="03a6a-227">subjectId</span></span>|<span data-ttu-id="03a6a-228">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-228">String</span></span>|<span data-ttu-id="03a6a-229">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-229">Yes</span></span>|<span data-ttu-id="03a6a-230">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-230">\<subjectId\></span></span>|
|<span data-ttu-id="03a6a-231">assignmentState</span><span class="sxs-lookup"><span data-stu-id="03a6a-231">assignmentState</span></span>|<span data-ttu-id="03a6a-232">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-232">String</span></span>|<span data-ttu-id="03a6a-233">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-233">Yes</span></span>| <span data-ttu-id="03a6a-234">Elegíveis / ativo</span><span class="sxs-lookup"><span data-stu-id="03a6a-234">Eligible / Active</span></span>|
|<span data-ttu-id="03a6a-235">type</span><span class="sxs-lookup"><span data-stu-id="03a6a-235">type</span></span>|<span data-ttu-id="03a6a-236">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-236">String</span></span>|<span data-ttu-id="03a6a-237">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-237">Yes</span></span>| <span data-ttu-id="03a6a-238">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="03a6a-238">AdminAdd</span></span>|
|<span data-ttu-id="03a6a-239">motivo</span><span class="sxs-lookup"><span data-stu-id="03a6a-239">reason</span></span>|<span data-ttu-id="03a6a-240">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-240">String</span></span>| <span data-ttu-id="03a6a-241">depende de configurações de função</span><span class="sxs-lookup"><span data-stu-id="03a6a-241">depends on role Settings</span></span>||
|<span data-ttu-id="03a6a-242">agenda</span><span class="sxs-lookup"><span data-stu-id="03a6a-242">schedule</span></span>|[<span data-ttu-id="03a6a-243">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="03a6a-243">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="03a6a-244">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-244">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="03a6a-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03a6a-245">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Eligible",
"type":"AdminAdd",
"reason":"Assign an eligible role",
"schedule":{
  "startDateTime":"2018-05-12T23:37:43.356Z",
  "endDateTime":"2018-11-08T23:37:43.356Z",
  "type":"Once"
  }
}
```
##### <a name="response"></a><span data-ttu-id="03a6a-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="03a6a-246">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

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

### <a name="example-2"></a><span data-ttu-id="03a6a-247">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="03a6a-247">Example 2</span></span>
<span data-ttu-id="03a6a-248">Neste exemplo, nawu@fimdev.net o usuário ativa a função de leitor de faturamento elegível.</span><span class="sxs-lookup"><span data-stu-id="03a6a-248">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="03a6a-249">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03a6a-249">Property</span></span>     | <span data-ttu-id="03a6a-250">Tipo</span><span class="sxs-lookup"><span data-stu-id="03a6a-250">Type</span></span>    |<span data-ttu-id="03a6a-251">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="03a6a-251">Required</span></span>|  <span data-ttu-id="03a6a-252">Valor</span><span class="sxs-lookup"><span data-stu-id="03a6a-252">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="03a6a-253">resourceId</span><span class="sxs-lookup"><span data-stu-id="03a6a-253">resourceId</span></span>|<span data-ttu-id="03a6a-254">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03a6a-254">String</span></span>|<span data-ttu-id="03a6a-255">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-255">Yes</span></span>|<span data-ttu-id="03a6a-256">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-256">\<resourceId\></span></span>|
|<span data-ttu-id="03a6a-257">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="03a6a-257">roleDefinitionId</span></span>|<span data-ttu-id="03a6a-258">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-258">String</span></span>|<span data-ttu-id="03a6a-259">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-259">Yes</span></span>|<span data-ttu-id="03a6a-260">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-260">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="03a6a-261">subjectId</span><span class="sxs-lookup"><span data-stu-id="03a6a-261">subjectId</span></span>|<span data-ttu-id="03a6a-262">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-262">String</span></span>|<span data-ttu-id="03a6a-263">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-263">Yes</span></span>|<span data-ttu-id="03a6a-264">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-264">\<subjectId\></span></span>|
|<span data-ttu-id="03a6a-265">assignmentState</span><span class="sxs-lookup"><span data-stu-id="03a6a-265">assignmentState</span></span>|<span data-ttu-id="03a6a-266">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-266">String</span></span>|<span data-ttu-id="03a6a-267">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-267">Yes</span></span>| <span data-ttu-id="03a6a-268">Ativo</span><span class="sxs-lookup"><span data-stu-id="03a6a-268">Active</span></span>|
|<span data-ttu-id="03a6a-269">type</span><span class="sxs-lookup"><span data-stu-id="03a6a-269">type</span></span>|<span data-ttu-id="03a6a-270">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-270">String</span></span>|<span data-ttu-id="03a6a-271">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-271">Yes</span></span>| <span data-ttu-id="03a6a-272">UserAdd</span><span class="sxs-lookup"><span data-stu-id="03a6a-272">UserAdd</span></span>|
|<span data-ttu-id="03a6a-273">motivo</span><span class="sxs-lookup"><span data-stu-id="03a6a-273">reason</span></span>|<span data-ttu-id="03a6a-274">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-274">String</span></span>| <span data-ttu-id="03a6a-275">depende de configurações de função</span><span class="sxs-lookup"><span data-stu-id="03a6a-275">depends on role Settings</span></span>||
|<span data-ttu-id="03a6a-276">agenda</span><span class="sxs-lookup"><span data-stu-id="03a6a-276">schedule</span></span>|[<span data-ttu-id="03a6a-277">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="03a6a-277">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="03a6a-278">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-278">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="03a6a-279">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03a6a-279">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"8b4d1d51-08e9-4254-b0a6-b16177aae376",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserAdd",
"reason": "Activate the owner role",
"schedule":{
  "type":"Once",
  "startDateTime":"2018-05-12T23:28:43.537Z",
  "duration":"PT9H"
  },
"linkedEligibleRoleAssignmentId":"e327f4be-42a0-47a2-8579-0a39b025b394"
}
```
##### <a name="response"></a><span data-ttu-id="03a6a-280">Resposta</span><span class="sxs-lookup"><span data-stu-id="03a6a-280">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
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

### <a name="example-3"></a><span data-ttu-id="03a6a-281">Exemplo 3</span><span class="sxs-lookup"><span data-stu-id="03a6a-281">Example 3</span></span>
<span data-ttu-id="03a6a-282">Neste exemplo, o nawu@fimdev.net usuário desativa a função de leitor de cobrança ativa.</span><span class="sxs-lookup"><span data-stu-id="03a6a-282">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="03a6a-283">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03a6a-283">Property</span></span>     | <span data-ttu-id="03a6a-284">Tipo</span><span class="sxs-lookup"><span data-stu-id="03a6a-284">Type</span></span>    |<span data-ttu-id="03a6a-285">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="03a6a-285">Required</span></span>|  <span data-ttu-id="03a6a-286">Valor</span><span class="sxs-lookup"><span data-stu-id="03a6a-286">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="03a6a-287">resourceId</span><span class="sxs-lookup"><span data-stu-id="03a6a-287">resourceId</span></span>|<span data-ttu-id="03a6a-288">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03a6a-288">String</span></span>|<span data-ttu-id="03a6a-289">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-289">Yes</span></span>|<span data-ttu-id="03a6a-290">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-290">\<resourceId\></span></span>|
|<span data-ttu-id="03a6a-291">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="03a6a-291">roleDefinitionId</span></span>|<span data-ttu-id="03a6a-292">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-292">String</span></span>|<span data-ttu-id="03a6a-293">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-293">Yes</span></span>|<span data-ttu-id="03a6a-294">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-294">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="03a6a-295">subjectId</span><span class="sxs-lookup"><span data-stu-id="03a6a-295">subjectId</span></span>|<span data-ttu-id="03a6a-296">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-296">String</span></span>|<span data-ttu-id="03a6a-297">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-297">Yes</span></span>|<span data-ttu-id="03a6a-298">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-298">\<subjectId\></span></span>|
|<span data-ttu-id="03a6a-299">assignmentState</span><span class="sxs-lookup"><span data-stu-id="03a6a-299">assignmentState</span></span>|<span data-ttu-id="03a6a-300">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-300">String</span></span>|<span data-ttu-id="03a6a-301">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-301">Yes</span></span>| <span data-ttu-id="03a6a-302">Ativo</span><span class="sxs-lookup"><span data-stu-id="03a6a-302">Active</span></span>|
|<span data-ttu-id="03a6a-303">type</span><span class="sxs-lookup"><span data-stu-id="03a6a-303">type</span></span>|<span data-ttu-id="03a6a-304">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-304">String</span></span>|<span data-ttu-id="03a6a-305">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-305">Yes</span></span>| <span data-ttu-id="03a6a-306">UserRemove</span><span class="sxs-lookup"><span data-stu-id="03a6a-306">UserRemove</span></span>|
|<span data-ttu-id="03a6a-307">motivo</span><span class="sxs-lookup"><span data-stu-id="03a6a-307">reason</span></span>|<span data-ttu-id="03a6a-308">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-308">String</span></span>| <span data-ttu-id="03a6a-309">Não</span><span class="sxs-lookup"><span data-stu-id="03a6a-309">No</span></span>||
|<span data-ttu-id="03a6a-310">agenda</span><span class="sxs-lookup"><span data-stu-id="03a6a-310">schedule</span></span>|[<span data-ttu-id="03a6a-311">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="03a6a-311">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="03a6a-312">Não</span><span class="sxs-lookup"><span data-stu-id="03a6a-312">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="03a6a-313">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03a6a-313">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"bc75b4e6-7403-4243-bf2f-d1f6990be122",
"resourceId":"fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserRemove",
"reason":"Deactivate the role",
"linkedEligibleRoleAssignmentId":"cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```
##### <a name="response"></a><span data-ttu-id="03a6a-314">Resposta</span><span class="sxs-lookup"><span data-stu-id="03a6a-314">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

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

### <a name="example-4"></a><span data-ttu-id="03a6a-315">Exemplo 4</span><span class="sxs-lookup"><span data-stu-id="03a6a-315">Example 4</span></span>
<span data-ttu-id="03a6a-316">Neste exemplo, os administradores remover nawu@fimdev.net o usuário da função Leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="03a6a-316">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="03a6a-317">**Observação:** Além de permissão, este exemplo exige que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="03a6a-317">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="03a6a-318">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03a6a-318">Property</span></span>     | <span data-ttu-id="03a6a-319">Tipo</span><span class="sxs-lookup"><span data-stu-id="03a6a-319">Type</span></span>    |<span data-ttu-id="03a6a-320">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="03a6a-320">Required</span></span>|  <span data-ttu-id="03a6a-321">Valor</span><span class="sxs-lookup"><span data-stu-id="03a6a-321">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="03a6a-322">resourceId</span><span class="sxs-lookup"><span data-stu-id="03a6a-322">resourceId</span></span>|<span data-ttu-id="03a6a-323">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03a6a-323">String</span></span>|<span data-ttu-id="03a6a-324">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-324">Yes</span></span>|<span data-ttu-id="03a6a-325">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-325">\<resourceId\></span></span>|
|<span data-ttu-id="03a6a-326">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="03a6a-326">roleDefinitionId</span></span>|<span data-ttu-id="03a6a-327">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-327">String</span></span>|<span data-ttu-id="03a6a-328">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-328">Yes</span></span>|<span data-ttu-id="03a6a-329">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-329">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="03a6a-330">subjectId</span><span class="sxs-lookup"><span data-stu-id="03a6a-330">subjectId</span></span>|<span data-ttu-id="03a6a-331">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-331">String</span></span>|<span data-ttu-id="03a6a-332">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-332">Yes</span></span>|<span data-ttu-id="03a6a-333">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-333">\<subjectId\></span></span>|
|<span data-ttu-id="03a6a-334">assignmentState</span><span class="sxs-lookup"><span data-stu-id="03a6a-334">assignmentState</span></span>|<span data-ttu-id="03a6a-335">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-335">String</span></span>|<span data-ttu-id="03a6a-336">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-336">Yes</span></span>| <span data-ttu-id="03a6a-337">Elegíveis / ativo</span><span class="sxs-lookup"><span data-stu-id="03a6a-337">Eligible / Active</span></span>|
|<span data-ttu-id="03a6a-338">type</span><span class="sxs-lookup"><span data-stu-id="03a6a-338">type</span></span>|<span data-ttu-id="03a6a-339">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-339">String</span></span>|<span data-ttu-id="03a6a-340">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-340">Yes</span></span>| <span data-ttu-id="03a6a-341">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="03a6a-341">AdminRemove</span></span>|
|<span data-ttu-id="03a6a-342">motivo</span><span class="sxs-lookup"><span data-stu-id="03a6a-342">reason</span></span>|<span data-ttu-id="03a6a-343">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-343">String</span></span>| <span data-ttu-id="03a6a-344">Não</span><span class="sxs-lookup"><span data-stu-id="03a6a-344">No</span></span>||
|<span data-ttu-id="03a6a-345">agenda</span><span class="sxs-lookup"><span data-stu-id="03a6a-345">schedule</span></span>|[<span data-ttu-id="03a6a-346">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="03a6a-346">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="03a6a-347">Não</span><span class="sxs-lookup"><span data-stu-id="03a6a-347">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="03a6a-348">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03a6a-348">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminRemove"
}
```
##### <a name="response"></a><span data-ttu-id="03a6a-349">Resposta</span><span class="sxs-lookup"><span data-stu-id="03a6a-349">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminRemove",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```

### <a name="example-5"></a><span data-ttu-id="03a6a-350">Exemplo 5</span><span class="sxs-lookup"><span data-stu-id="03a6a-350">Example 5</span></span>
<span data-ttu-id="03a6a-351">Neste exemplo, os administradores atualizar a atribuição de função para o usuário de nawu@fimdev.net ao proprietário.</span><span class="sxs-lookup"><span data-stu-id="03a6a-351">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="03a6a-352">**Observação:** Além de permissão, este exemplo exige que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="03a6a-352">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="03a6a-353">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03a6a-353">Property</span></span>     | <span data-ttu-id="03a6a-354">Tipo</span><span class="sxs-lookup"><span data-stu-id="03a6a-354">Type</span></span>    |<span data-ttu-id="03a6a-355">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="03a6a-355">Required</span></span>|  <span data-ttu-id="03a6a-356">Valor</span><span class="sxs-lookup"><span data-stu-id="03a6a-356">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="03a6a-357">resourceId</span><span class="sxs-lookup"><span data-stu-id="03a6a-357">resourceId</span></span>|<span data-ttu-id="03a6a-358">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03a6a-358">String</span></span>|<span data-ttu-id="03a6a-359">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-359">Yes</span></span>|<span data-ttu-id="03a6a-360">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-360">\<resourceId\></span></span>|
|<span data-ttu-id="03a6a-361">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="03a6a-361">roleDefinitionId</span></span>|<span data-ttu-id="03a6a-362">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-362">String</span></span>|<span data-ttu-id="03a6a-363">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-363">Yes</span></span>|<span data-ttu-id="03a6a-364">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-364">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="03a6a-365">subjectId</span><span class="sxs-lookup"><span data-stu-id="03a6a-365">subjectId</span></span>|<span data-ttu-id="03a6a-366">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-366">String</span></span>|<span data-ttu-id="03a6a-367">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-367">Yes</span></span>|<span data-ttu-id="03a6a-368">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-368">\<subjectId\></span></span>|
|<span data-ttu-id="03a6a-369">assignmentState</span><span class="sxs-lookup"><span data-stu-id="03a6a-369">assignmentState</span></span>|<span data-ttu-id="03a6a-370">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-370">String</span></span>|<span data-ttu-id="03a6a-371">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-371">Yes</span></span>| <span data-ttu-id="03a6a-372">Elegíveis / ativo</span><span class="sxs-lookup"><span data-stu-id="03a6a-372">Eligible / Active</span></span>|
|<span data-ttu-id="03a6a-373">type</span><span class="sxs-lookup"><span data-stu-id="03a6a-373">type</span></span>|<span data-ttu-id="03a6a-374">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-374">String</span></span>|<span data-ttu-id="03a6a-375">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-375">Yes</span></span>| <span data-ttu-id="03a6a-376">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="03a6a-376">AdminUpdate</span></span>|
|<span data-ttu-id="03a6a-377">motivo</span><span class="sxs-lookup"><span data-stu-id="03a6a-377">reason</span></span>|<span data-ttu-id="03a6a-378">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-378">String</span></span>| <span data-ttu-id="03a6a-379">depende roleSettings</span><span class="sxs-lookup"><span data-stu-id="03a6a-379">depends on roleSettings</span></span>||
|<span data-ttu-id="03a6a-380">agenda</span><span class="sxs-lookup"><span data-stu-id="03a6a-380">schedule</span></span>|[<span data-ttu-id="03a6a-381">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="03a6a-381">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="03a6a-382">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-382">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="03a6a-383">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03a6a-383">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState":"Eligible",
  "type":"AdminUpdate",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31.000Z"
  }
}
```
##### <a name="response"></a><span data-ttu-id="03a6a-384">Resposta</span><span class="sxs-lookup"><span data-stu-id="03a6a-384">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminUpdate",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "reason":null,
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31Z",
    "duration":"PT0S"
  }
}
```

### <a name="example-6"></a><span data-ttu-id="03a6a-385">Exemplo 6</span><span class="sxs-lookup"><span data-stu-id="03a6a-385">Example 6</span></span>
<span data-ttu-id="03a6a-386">Este exemplo estende a atribuição de função expirar para usuário ANUJCUSER Colaborador do serviço de gerenciamento de API.</span><span class="sxs-lookup"><span data-stu-id="03a6a-386">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="03a6a-387">**Observação:** Additon à permissão, este exemplo exige que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="03a6a-387">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="03a6a-388">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03a6a-388">Property</span></span>     | <span data-ttu-id="03a6a-389">Tipo</span><span class="sxs-lookup"><span data-stu-id="03a6a-389">Type</span></span>    |<span data-ttu-id="03a6a-390">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="03a6a-390">Required</span></span>|  <span data-ttu-id="03a6a-391">Valor</span><span class="sxs-lookup"><span data-stu-id="03a6a-391">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="03a6a-392">resourceId</span><span class="sxs-lookup"><span data-stu-id="03a6a-392">resourceId</span></span>|<span data-ttu-id="03a6a-393">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03a6a-393">String</span></span>|<span data-ttu-id="03a6a-394">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-394">Yes</span></span>|<span data-ttu-id="03a6a-395">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-395">\<resourceId\></span></span>|
|<span data-ttu-id="03a6a-396">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="03a6a-396">roleDefinitionId</span></span>|<span data-ttu-id="03a6a-397">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-397">String</span></span>|<span data-ttu-id="03a6a-398">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-398">Yes</span></span>|<span data-ttu-id="03a6a-399">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-399">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="03a6a-400">subjectId</span><span class="sxs-lookup"><span data-stu-id="03a6a-400">subjectId</span></span>|<span data-ttu-id="03a6a-401">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-401">String</span></span>|<span data-ttu-id="03a6a-402">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-402">Yes</span></span>|<span data-ttu-id="03a6a-403">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="03a6a-403">\<subjectId\></span></span>|
|<span data-ttu-id="03a6a-404">assignmentState</span><span class="sxs-lookup"><span data-stu-id="03a6a-404">assignmentState</span></span>|<span data-ttu-id="03a6a-405">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-405">String</span></span>|<span data-ttu-id="03a6a-406">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-406">Yes</span></span>| <span data-ttu-id="03a6a-407">Elegíveis / ativo</span><span class="sxs-lookup"><span data-stu-id="03a6a-407">Eligible / Active</span></span> |
|<span data-ttu-id="03a6a-408">type</span><span class="sxs-lookup"><span data-stu-id="03a6a-408">type</span></span>|<span data-ttu-id="03a6a-409">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-409">String</span></span>|<span data-ttu-id="03a6a-410">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-410">Yes</span></span>| <span data-ttu-id="03a6a-411">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="03a6a-411">AdminExtend</span></span>|
|<span data-ttu-id="03a6a-412">motivo</span><span class="sxs-lookup"><span data-stu-id="03a6a-412">reason</span></span>|<span data-ttu-id="03a6a-413">String</span><span class="sxs-lookup"><span data-stu-id="03a6a-413">String</span></span>| <span data-ttu-id="03a6a-414">depende roleSettings</span><span class="sxs-lookup"><span data-stu-id="03a6a-414">depends on roleSettings</span></span>||
|<span data-ttu-id="03a6a-415">agenda</span><span class="sxs-lookup"><span data-stu-id="03a6a-415">schedule</span></span>|[<span data-ttu-id="03a6a-416">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="03a6a-416">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="03a6a-417">Sim</span><span class="sxs-lookup"><span data-stu-id="03a6a-417">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="03a6a-418">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03a6a-418">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminExtend",
  "reason":"extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z"
  }
}
```
##### <a name="response"></a><span data-ttu-id="03a6a-419">Resposta</span><span class="sxs-lookup"><span data-stu-id="03a6a-419">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminExtend",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "reason":"extend role assignment",
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z",
    "duration":"PT0S"
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
