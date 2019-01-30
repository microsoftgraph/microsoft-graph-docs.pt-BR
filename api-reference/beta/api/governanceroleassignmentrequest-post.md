---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação desejado em uma atribuição de função. A tabela a seguir lista as operações.
localization_priority: Normal
ms.openlocfilehash: c936a6cd0ba061fc1dd3758533781d7270673939
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641264"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="25cfa-104">Criar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="25cfa-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25cfa-105">Crie uma solicitação de atribuição de função para representar a operação desejado em uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="25cfa-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="25cfa-106">A tabela a seguir lista as operações.</span><span class="sxs-lookup"><span data-stu-id="25cfa-106">The following table lists the operations.</span></span>

| <span data-ttu-id="25cfa-107">Operação</span><span class="sxs-lookup"><span data-stu-id="25cfa-107">Operation</span></span>       | <span data-ttu-id="25cfa-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="25cfa-108">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="25cfa-109">Atribuir uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="25cfa-109">Assign a role assignment</span></span>| <span data-ttu-id="25cfa-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="25cfa-110">AdminAdd</span></span> |
| <span data-ttu-id="25cfa-111">Ativar uma atribuição de função elegíveis</span><span class="sxs-lookup"><span data-stu-id="25cfa-111">Activate an eligible role assignment</span></span>| <span data-ttu-id="25cfa-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="25cfa-112">UserAdd</span></span> | 
| <span data-ttu-id="25cfa-113">Desativar uma atribuição de função ativada</span><span class="sxs-lookup"><span data-stu-id="25cfa-113">Deactivate an activated role assignment</span></span>| <span data-ttu-id="25cfa-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="25cfa-114">UserRemove</span></span> | 
| <span data-ttu-id="25cfa-115">Remover uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="25cfa-115">Remove a role assignment</span></span>| <span data-ttu-id="25cfa-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="25cfa-116">AdminRemove</span></span> |
| <span data-ttu-id="25cfa-117">Atualizar uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="25cfa-117">Update a role assignment</span></span>| <span data-ttu-id="25cfa-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="25cfa-118">AdminUpdate</span></span> |
| <span data-ttu-id="25cfa-119">Solicitação para estender minha atribuição de função</span><span class="sxs-lookup"><span data-stu-id="25cfa-119">Request to extend my role assignment</span></span>| <span data-ttu-id="25cfa-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="25cfa-120">UserExtend</span></span> | 
| <span data-ttu-id="25cfa-121">Estender uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="25cfa-121">Extend a role assignment</span></span>| <span data-ttu-id="25cfa-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="25cfa-122">AdminExtend</span></span> | 
| <span data-ttu-id="25cfa-123">Solicitação de renovação minha atribuição de função expirados</span><span class="sxs-lookup"><span data-stu-id="25cfa-123">Request to renew my expired role assignment</span></span>| <span data-ttu-id="25cfa-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="25cfa-124">UserRenew</span></span> | 
| <span data-ttu-id="25cfa-125">Renovar uma atribuição de função expirados</span><span class="sxs-lookup"><span data-stu-id="25cfa-125">Renew an expired role assignment</span></span>| <span data-ttu-id="25cfa-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="25cfa-126">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="25cfa-127">Permissões</span><span class="sxs-lookup"><span data-stu-id="25cfa-127">Permissions</span></span>
<span data-ttu-id="25cfa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25cfa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25cfa-130">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25cfa-130">Permission type</span></span>      | <span data-ttu-id="25cfa-131">Permissões</span><span class="sxs-lookup"><span data-stu-id="25cfa-131">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25cfa-132">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25cfa-132">Delegated (work or school account)</span></span> | <span data-ttu-id="25cfa-133">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="25cfa-133">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="25cfa-134">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25cfa-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25cfa-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25cfa-135">Not supported.</span></span>    |
|<span data-ttu-id="25cfa-136">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25cfa-136">Application</span></span> | <span data-ttu-id="25cfa-137">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="25cfa-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="25cfa-138">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25cfa-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="25cfa-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25cfa-139">Request headers</span></span>
| <span data-ttu-id="25cfa-140">Nome</span><span class="sxs-lookup"><span data-stu-id="25cfa-140">Name</span></span>       | <span data-ttu-id="25cfa-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="25cfa-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="25cfa-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="25cfa-142">Authorization</span></span>  | <span data-ttu-id="25cfa-143">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="25cfa-143">Bearer {code}</span></span>|
| <span data-ttu-id="25cfa-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="25cfa-144">Content-type</span></span>  | <span data-ttu-id="25cfa-145">application/json</span><span class="sxs-lookup"><span data-stu-id="25cfa-145">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25cfa-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25cfa-146">Request body</span></span>
<span data-ttu-id="25cfa-147">No corpo da solicitação, fornece uma representação JSON de um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="25cfa-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="25cfa-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25cfa-148">Property</span></span>     | <span data-ttu-id="25cfa-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="25cfa-149">Type</span></span>    |<span data-ttu-id="25cfa-150">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="25cfa-150">Required</span></span>|  <span data-ttu-id="25cfa-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="25cfa-151">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="25cfa-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="25cfa-152">resourceId</span></span>|<span data-ttu-id="25cfa-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25cfa-153">String</span></span>|<span data-ttu-id="25cfa-154">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-154">Yes</span></span>|<span data-ttu-id="25cfa-155">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="25cfa-155">The ID of the resource.</span></span>|
|<span data-ttu-id="25cfa-156">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="25cfa-156">roleDefinitionId</span></span>|<span data-ttu-id="25cfa-157">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-157">String</span></span>|<span data-ttu-id="25cfa-158">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-158">Yes</span></span>|<span data-ttu-id="25cfa-159">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="25cfa-159">The ID of the role definition.</span></span>|
|<span data-ttu-id="25cfa-160">subjectId</span><span class="sxs-lookup"><span data-stu-id="25cfa-160">subjectId</span></span>|<span data-ttu-id="25cfa-161">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-161">String</span></span>|<span data-ttu-id="25cfa-162">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-162">Yes</span></span>|<span data-ttu-id="25cfa-163">A identificação do assunto.</span><span class="sxs-lookup"><span data-stu-id="25cfa-163">The ID of the subject.</span></span>|
|<span data-ttu-id="25cfa-164">assignmentState</span><span class="sxs-lookup"><span data-stu-id="25cfa-164">assignmentState</span></span>|<span data-ttu-id="25cfa-165">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-165">String</span></span>|<span data-ttu-id="25cfa-166">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-166">Yes</span></span>|<span data-ttu-id="25cfa-167">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="25cfa-167">The state of assignment.</span></span> <span data-ttu-id="25cfa-168">O valor pode ser ``Eligible`` e ``Active``.</span><span class="sxs-lookup"><span data-stu-id="25cfa-168">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="25cfa-169">type</span><span class="sxs-lookup"><span data-stu-id="25cfa-169">type</span></span>|<span data-ttu-id="25cfa-170">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-170">String</span></span>|<span data-ttu-id="25cfa-171">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-171">Yes</span></span>|<span data-ttu-id="25cfa-172">O tipo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="25cfa-172">The request type.</span></span> <span data-ttu-id="25cfa-173">O valor pode ser `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`e `AdminExtend`.</span><span class="sxs-lookup"><span data-stu-id="25cfa-173">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="25cfa-174">motivo</span><span class="sxs-lookup"><span data-stu-id="25cfa-174">reason</span></span>|<span data-ttu-id="25cfa-175">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-175">String</span></span>| |<span data-ttu-id="25cfa-176">O motivo pelo qual deve ser fornecido para a solicitação de atribuição de função de auditoria e revise finalidade.</span><span class="sxs-lookup"><span data-stu-id="25cfa-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="25cfa-177">agenda</span><span class="sxs-lookup"><span data-stu-id="25cfa-177">schedule</span></span>|[<span data-ttu-id="25cfa-178">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="25cfa-178">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="25cfa-179">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="25cfa-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="25cfa-180">Tipo de solicitação de `UserAdd`, `AdminAdd`, `AdminUpdate`, e `AdminExtend`, é necessário.</span><span class="sxs-lookup"><span data-stu-id="25cfa-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="25cfa-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="25cfa-181">Response</span></span>
<span data-ttu-id="25cfa-182">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25cfa-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="25cfa-183">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="25cfa-183">Error codes</span></span>
<span data-ttu-id="25cfa-184">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="25cfa-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="25cfa-185">Além disso, ele também retorna os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="25cfa-185">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="25cfa-186">Código de erro</span><span class="sxs-lookup"><span data-stu-id="25cfa-186">Error code</span></span>     | <span data-ttu-id="25cfa-187">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="25cfa-187">Error message</span></span>              | <span data-ttu-id="25cfa-188">Detalhes</span><span class="sxs-lookup"><span data-stu-id="25cfa-188">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="25cfa-189">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="25cfa-189">400 BadRequest</span></span> | <span data-ttu-id="25cfa-190">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="25cfa-190">RoleNotFound</span></span>    | <span data-ttu-id="25cfa-191">O `roleDefinitionId` fornecida na solicitação de corpo não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="25cfa-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="25cfa-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="25cfa-192">400 BadRequest</span></span> | <span data-ttu-id="25cfa-193">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="25cfa-193">ResourceIsLocked</span></span>    | <span data-ttu-id="25cfa-194">O recurso fornecido no corpo da solicitação está em estado de `Locked` e não pode criar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="25cfa-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="25cfa-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="25cfa-195">400 BadRequest</span></span> | <span data-ttu-id="25cfa-196">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="25cfa-196">SubjectNotFound</span></span>    | <span data-ttu-id="25cfa-197">O `subjectId` fornecida na solicitação de corpo não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="25cfa-197">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="25cfa-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="25cfa-198">400 BadRequest</span></span> | <span data-ttu-id="25cfa-199">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="25cfa-199">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="25cfa-200">Já existe uma pendente [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no sistema.</span><span class="sxs-lookup"><span data-stu-id="25cfa-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="25cfa-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="25cfa-201">400 BadRequest</span></span> | <span data-ttu-id="25cfa-202">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="25cfa-202">RoleAssignmentExists</span></span>    | <span data-ttu-id="25cfa-203">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criada já existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="25cfa-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="25cfa-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="25cfa-204">400 BadRequest</span></span> | <span data-ttu-id="25cfa-205">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="25cfa-205">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="25cfa-206">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="25cfa-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="25cfa-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="25cfa-207">400 BadRequest</span></span> | <span data-ttu-id="25cfa-208">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="25cfa-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="25cfa-209">O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não atende às políticas internas e não pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="25cfa-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="25cfa-210">Exemplos</span><span class="sxs-lookup"><span data-stu-id="25cfa-210">Examples</span></span>
<span data-ttu-id="25cfa-211">Os exemplos a seguir mostram como usar essa API.</span><span class="sxs-lookup"><span data-stu-id="25cfa-211">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="25cfa-212">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="25cfa-212">Example 1</span></span>
<span data-ttu-id="25cfa-213">Neste exemplo, os administradores atribuem nawu@fimdev.net usuário à função Leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="25cfa-213">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="25cfa-214">**Observação:** Além de permissão, este exemplo exige que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="25cfa-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="25cfa-215">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25cfa-215">Property</span></span>     | <span data-ttu-id="25cfa-216">Tipo</span><span class="sxs-lookup"><span data-stu-id="25cfa-216">Type</span></span>    |<span data-ttu-id="25cfa-217">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="25cfa-217">Required</span></span>|  <span data-ttu-id="25cfa-218">Valor</span><span class="sxs-lookup"><span data-stu-id="25cfa-218">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="25cfa-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="25cfa-219">resourceId</span></span>|<span data-ttu-id="25cfa-220">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25cfa-220">String</span></span>|<span data-ttu-id="25cfa-221">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-221">Yes</span></span>|<span data-ttu-id="25cfa-222">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-222">\<resourceId\></span></span>|
|<span data-ttu-id="25cfa-223">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="25cfa-223">roleDefinitionId</span></span>|<span data-ttu-id="25cfa-224">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-224">String</span></span>|<span data-ttu-id="25cfa-225">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-225">Yes</span></span>|<span data-ttu-id="25cfa-226">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-226">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="25cfa-227">subjectId</span><span class="sxs-lookup"><span data-stu-id="25cfa-227">subjectId</span></span>|<span data-ttu-id="25cfa-228">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-228">String</span></span>|<span data-ttu-id="25cfa-229">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-229">Yes</span></span>|<span data-ttu-id="25cfa-230">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-230">\<subjectId\></span></span>|
|<span data-ttu-id="25cfa-231">assignmentState</span><span class="sxs-lookup"><span data-stu-id="25cfa-231">assignmentState</span></span>|<span data-ttu-id="25cfa-232">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-232">String</span></span>|<span data-ttu-id="25cfa-233">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-233">Yes</span></span>| <span data-ttu-id="25cfa-234">Elegíveis / ativo</span><span class="sxs-lookup"><span data-stu-id="25cfa-234">Eligible / Active</span></span>|
|<span data-ttu-id="25cfa-235">type</span><span class="sxs-lookup"><span data-stu-id="25cfa-235">type</span></span>|<span data-ttu-id="25cfa-236">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-236">String</span></span>|<span data-ttu-id="25cfa-237">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-237">Yes</span></span>| <span data-ttu-id="25cfa-238">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="25cfa-238">AdminAdd</span></span>|
|<span data-ttu-id="25cfa-239">motivo</span><span class="sxs-lookup"><span data-stu-id="25cfa-239">reason</span></span>|<span data-ttu-id="25cfa-240">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-240">String</span></span>| <span data-ttu-id="25cfa-241">depende de configurações de função</span><span class="sxs-lookup"><span data-stu-id="25cfa-241">depends on role Settings</span></span>||
|<span data-ttu-id="25cfa-242">agenda</span><span class="sxs-lookup"><span data-stu-id="25cfa-242">schedule</span></span>|[<span data-ttu-id="25cfa-243">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="25cfa-243">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="25cfa-244">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-244">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="25cfa-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25cfa-245">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="25cfa-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="25cfa-246">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="25cfa-247">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="25cfa-247">Example 2</span></span>
<span data-ttu-id="25cfa-248">Neste exemplo, nawu@fimdev.net o usuário ativa a função de leitor de faturamento elegível.</span><span class="sxs-lookup"><span data-stu-id="25cfa-248">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="25cfa-249">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25cfa-249">Property</span></span>     | <span data-ttu-id="25cfa-250">Tipo</span><span class="sxs-lookup"><span data-stu-id="25cfa-250">Type</span></span>    |<span data-ttu-id="25cfa-251">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="25cfa-251">Required</span></span>|  <span data-ttu-id="25cfa-252">Valor</span><span class="sxs-lookup"><span data-stu-id="25cfa-252">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="25cfa-253">resourceId</span><span class="sxs-lookup"><span data-stu-id="25cfa-253">resourceId</span></span>|<span data-ttu-id="25cfa-254">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25cfa-254">String</span></span>|<span data-ttu-id="25cfa-255">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-255">Yes</span></span>|<span data-ttu-id="25cfa-256">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-256">\<resourceId\></span></span>|
|<span data-ttu-id="25cfa-257">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="25cfa-257">roleDefinitionId</span></span>|<span data-ttu-id="25cfa-258">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-258">String</span></span>|<span data-ttu-id="25cfa-259">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-259">Yes</span></span>|<span data-ttu-id="25cfa-260">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-260">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="25cfa-261">subjectId</span><span class="sxs-lookup"><span data-stu-id="25cfa-261">subjectId</span></span>|<span data-ttu-id="25cfa-262">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-262">String</span></span>|<span data-ttu-id="25cfa-263">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-263">Yes</span></span>|<span data-ttu-id="25cfa-264">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-264">\<subjectId\></span></span>|
|<span data-ttu-id="25cfa-265">assignmentState</span><span class="sxs-lookup"><span data-stu-id="25cfa-265">assignmentState</span></span>|<span data-ttu-id="25cfa-266">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-266">String</span></span>|<span data-ttu-id="25cfa-267">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-267">Yes</span></span>| <span data-ttu-id="25cfa-268">Ativo</span><span class="sxs-lookup"><span data-stu-id="25cfa-268">Active</span></span>|
|<span data-ttu-id="25cfa-269">type</span><span class="sxs-lookup"><span data-stu-id="25cfa-269">type</span></span>|<span data-ttu-id="25cfa-270">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-270">String</span></span>|<span data-ttu-id="25cfa-271">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-271">Yes</span></span>| <span data-ttu-id="25cfa-272">UserAdd</span><span class="sxs-lookup"><span data-stu-id="25cfa-272">UserAdd</span></span>|
|<span data-ttu-id="25cfa-273">motivo</span><span class="sxs-lookup"><span data-stu-id="25cfa-273">reason</span></span>|<span data-ttu-id="25cfa-274">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-274">String</span></span>| <span data-ttu-id="25cfa-275">depende de configurações de função</span><span class="sxs-lookup"><span data-stu-id="25cfa-275">depends on role Settings</span></span>||
|<span data-ttu-id="25cfa-276">agenda</span><span class="sxs-lookup"><span data-stu-id="25cfa-276">schedule</span></span>|[<span data-ttu-id="25cfa-277">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="25cfa-277">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="25cfa-278">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-278">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="25cfa-279">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25cfa-279">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="25cfa-280">Resposta</span><span class="sxs-lookup"><span data-stu-id="25cfa-280">Response</span></span>
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

### <a name="example-3"></a><span data-ttu-id="25cfa-281">Exemplo 3</span><span class="sxs-lookup"><span data-stu-id="25cfa-281">Example 3</span></span>
<span data-ttu-id="25cfa-282">Neste exemplo, o nawu@fimdev.net usuário desativa a função de leitor de cobrança ativa.</span><span class="sxs-lookup"><span data-stu-id="25cfa-282">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="25cfa-283">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25cfa-283">Property</span></span>     | <span data-ttu-id="25cfa-284">Tipo</span><span class="sxs-lookup"><span data-stu-id="25cfa-284">Type</span></span>    |<span data-ttu-id="25cfa-285">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="25cfa-285">Required</span></span>|  <span data-ttu-id="25cfa-286">Valor</span><span class="sxs-lookup"><span data-stu-id="25cfa-286">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="25cfa-287">resourceId</span><span class="sxs-lookup"><span data-stu-id="25cfa-287">resourceId</span></span>|<span data-ttu-id="25cfa-288">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25cfa-288">String</span></span>|<span data-ttu-id="25cfa-289">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-289">Yes</span></span>|<span data-ttu-id="25cfa-290">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-290">\<resourceId\></span></span>|
|<span data-ttu-id="25cfa-291">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="25cfa-291">roleDefinitionId</span></span>|<span data-ttu-id="25cfa-292">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-292">String</span></span>|<span data-ttu-id="25cfa-293">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-293">Yes</span></span>|<span data-ttu-id="25cfa-294">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-294">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="25cfa-295">subjectId</span><span class="sxs-lookup"><span data-stu-id="25cfa-295">subjectId</span></span>|<span data-ttu-id="25cfa-296">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-296">String</span></span>|<span data-ttu-id="25cfa-297">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-297">Yes</span></span>|<span data-ttu-id="25cfa-298">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-298">\<subjectId\></span></span>|
|<span data-ttu-id="25cfa-299">assignmentState</span><span class="sxs-lookup"><span data-stu-id="25cfa-299">assignmentState</span></span>|<span data-ttu-id="25cfa-300">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-300">String</span></span>|<span data-ttu-id="25cfa-301">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-301">Yes</span></span>| <span data-ttu-id="25cfa-302">Ativo</span><span class="sxs-lookup"><span data-stu-id="25cfa-302">Active</span></span>|
|<span data-ttu-id="25cfa-303">type</span><span class="sxs-lookup"><span data-stu-id="25cfa-303">type</span></span>|<span data-ttu-id="25cfa-304">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-304">String</span></span>|<span data-ttu-id="25cfa-305">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-305">Yes</span></span>| <span data-ttu-id="25cfa-306">UserRemove</span><span class="sxs-lookup"><span data-stu-id="25cfa-306">UserRemove</span></span>|
|<span data-ttu-id="25cfa-307">motivo</span><span class="sxs-lookup"><span data-stu-id="25cfa-307">reason</span></span>|<span data-ttu-id="25cfa-308">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-308">String</span></span>| <span data-ttu-id="25cfa-309">Não</span><span class="sxs-lookup"><span data-stu-id="25cfa-309">No</span></span>||
|<span data-ttu-id="25cfa-310">agenda</span><span class="sxs-lookup"><span data-stu-id="25cfa-310">schedule</span></span>|[<span data-ttu-id="25cfa-311">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="25cfa-311">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="25cfa-312">Não</span><span class="sxs-lookup"><span data-stu-id="25cfa-312">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="25cfa-313">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25cfa-313">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="25cfa-314">Resposta</span><span class="sxs-lookup"><span data-stu-id="25cfa-314">Response</span></span>
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

### <a name="example-4"></a><span data-ttu-id="25cfa-315">Exemplo 4</span><span class="sxs-lookup"><span data-stu-id="25cfa-315">Example 4</span></span>
<span data-ttu-id="25cfa-316">Neste exemplo, os administradores remover nawu@fimdev.net o usuário da função Leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="25cfa-316">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="25cfa-317">**Observação:** Além de permissão, este exemplo exige que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="25cfa-317">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="25cfa-318">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25cfa-318">Property</span></span>     | <span data-ttu-id="25cfa-319">Tipo</span><span class="sxs-lookup"><span data-stu-id="25cfa-319">Type</span></span>    |<span data-ttu-id="25cfa-320">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="25cfa-320">Required</span></span>|  <span data-ttu-id="25cfa-321">Valor</span><span class="sxs-lookup"><span data-stu-id="25cfa-321">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="25cfa-322">resourceId</span><span class="sxs-lookup"><span data-stu-id="25cfa-322">resourceId</span></span>|<span data-ttu-id="25cfa-323">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25cfa-323">String</span></span>|<span data-ttu-id="25cfa-324">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-324">Yes</span></span>|<span data-ttu-id="25cfa-325">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-325">\<resourceId\></span></span>|
|<span data-ttu-id="25cfa-326">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="25cfa-326">roleDefinitionId</span></span>|<span data-ttu-id="25cfa-327">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-327">String</span></span>|<span data-ttu-id="25cfa-328">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-328">Yes</span></span>|<span data-ttu-id="25cfa-329">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-329">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="25cfa-330">subjectId</span><span class="sxs-lookup"><span data-stu-id="25cfa-330">subjectId</span></span>|<span data-ttu-id="25cfa-331">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-331">String</span></span>|<span data-ttu-id="25cfa-332">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-332">Yes</span></span>|<span data-ttu-id="25cfa-333">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-333">\<subjectId\></span></span>|
|<span data-ttu-id="25cfa-334">assignmentState</span><span class="sxs-lookup"><span data-stu-id="25cfa-334">assignmentState</span></span>|<span data-ttu-id="25cfa-335">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-335">String</span></span>|<span data-ttu-id="25cfa-336">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-336">Yes</span></span>| <span data-ttu-id="25cfa-337">Elegíveis / ativo</span><span class="sxs-lookup"><span data-stu-id="25cfa-337">Eligible / Active</span></span>|
|<span data-ttu-id="25cfa-338">type</span><span class="sxs-lookup"><span data-stu-id="25cfa-338">type</span></span>|<span data-ttu-id="25cfa-339">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-339">String</span></span>|<span data-ttu-id="25cfa-340">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-340">Yes</span></span>| <span data-ttu-id="25cfa-341">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="25cfa-341">AdminRemove</span></span>|
|<span data-ttu-id="25cfa-342">motivo</span><span class="sxs-lookup"><span data-stu-id="25cfa-342">reason</span></span>|<span data-ttu-id="25cfa-343">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-343">String</span></span>| <span data-ttu-id="25cfa-344">Não</span><span class="sxs-lookup"><span data-stu-id="25cfa-344">No</span></span>||
|<span data-ttu-id="25cfa-345">agenda</span><span class="sxs-lookup"><span data-stu-id="25cfa-345">schedule</span></span>|[<span data-ttu-id="25cfa-346">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="25cfa-346">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="25cfa-347">Não</span><span class="sxs-lookup"><span data-stu-id="25cfa-347">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="25cfa-348">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25cfa-348">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="25cfa-349">Resposta</span><span class="sxs-lookup"><span data-stu-id="25cfa-349">Response</span></span>
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

### <a name="example-5"></a><span data-ttu-id="25cfa-350">Exemplo 5</span><span class="sxs-lookup"><span data-stu-id="25cfa-350">Example 5</span></span>
<span data-ttu-id="25cfa-351">Neste exemplo, os administradores atualizar a atribuição de função para o usuário de nawu@fimdev.net ao proprietário.</span><span class="sxs-lookup"><span data-stu-id="25cfa-351">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="25cfa-352">**Observação:** Além de permissão, este exemplo exige que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="25cfa-352">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="25cfa-353">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25cfa-353">Property</span></span>     | <span data-ttu-id="25cfa-354">Tipo</span><span class="sxs-lookup"><span data-stu-id="25cfa-354">Type</span></span>    |<span data-ttu-id="25cfa-355">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="25cfa-355">Required</span></span>|  <span data-ttu-id="25cfa-356">Valor</span><span class="sxs-lookup"><span data-stu-id="25cfa-356">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="25cfa-357">resourceId</span><span class="sxs-lookup"><span data-stu-id="25cfa-357">resourceId</span></span>|<span data-ttu-id="25cfa-358">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25cfa-358">String</span></span>|<span data-ttu-id="25cfa-359">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-359">Yes</span></span>|<span data-ttu-id="25cfa-360">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-360">\<resourceId\></span></span>|
|<span data-ttu-id="25cfa-361">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="25cfa-361">roleDefinitionId</span></span>|<span data-ttu-id="25cfa-362">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-362">String</span></span>|<span data-ttu-id="25cfa-363">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-363">Yes</span></span>|<span data-ttu-id="25cfa-364">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-364">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="25cfa-365">subjectId</span><span class="sxs-lookup"><span data-stu-id="25cfa-365">subjectId</span></span>|<span data-ttu-id="25cfa-366">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-366">String</span></span>|<span data-ttu-id="25cfa-367">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-367">Yes</span></span>|<span data-ttu-id="25cfa-368">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-368">\<subjectId\></span></span>|
|<span data-ttu-id="25cfa-369">assignmentState</span><span class="sxs-lookup"><span data-stu-id="25cfa-369">assignmentState</span></span>|<span data-ttu-id="25cfa-370">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-370">String</span></span>|<span data-ttu-id="25cfa-371">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-371">Yes</span></span>| <span data-ttu-id="25cfa-372">Elegíveis / ativo</span><span class="sxs-lookup"><span data-stu-id="25cfa-372">Eligible / Active</span></span>|
|<span data-ttu-id="25cfa-373">type</span><span class="sxs-lookup"><span data-stu-id="25cfa-373">type</span></span>|<span data-ttu-id="25cfa-374">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-374">String</span></span>|<span data-ttu-id="25cfa-375">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-375">Yes</span></span>| <span data-ttu-id="25cfa-376">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="25cfa-376">AdminUpdate</span></span>|
|<span data-ttu-id="25cfa-377">motivo</span><span class="sxs-lookup"><span data-stu-id="25cfa-377">reason</span></span>|<span data-ttu-id="25cfa-378">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-378">String</span></span>| <span data-ttu-id="25cfa-379">depende roleSettings</span><span class="sxs-lookup"><span data-stu-id="25cfa-379">depends on roleSettings</span></span>||
|<span data-ttu-id="25cfa-380">agenda</span><span class="sxs-lookup"><span data-stu-id="25cfa-380">schedule</span></span>|[<span data-ttu-id="25cfa-381">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="25cfa-381">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="25cfa-382">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-382">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="25cfa-383">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25cfa-383">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="25cfa-384">Resposta</span><span class="sxs-lookup"><span data-stu-id="25cfa-384">Response</span></span>
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

### <a name="example-6"></a><span data-ttu-id="25cfa-385">Exemplo 6</span><span class="sxs-lookup"><span data-stu-id="25cfa-385">Example 6</span></span>
<span data-ttu-id="25cfa-386">Este exemplo estende a atribuição de função expirar para usuário ANUJCUSER Colaborador do serviço de gerenciamento de API.</span><span class="sxs-lookup"><span data-stu-id="25cfa-386">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="25cfa-387">**Observação:** Additon à permissão, este exemplo exige que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="25cfa-387">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="25cfa-388">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25cfa-388">Property</span></span>     | <span data-ttu-id="25cfa-389">Tipo</span><span class="sxs-lookup"><span data-stu-id="25cfa-389">Type</span></span>    |<span data-ttu-id="25cfa-390">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="25cfa-390">Required</span></span>|  <span data-ttu-id="25cfa-391">Valor</span><span class="sxs-lookup"><span data-stu-id="25cfa-391">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="25cfa-392">resourceId</span><span class="sxs-lookup"><span data-stu-id="25cfa-392">resourceId</span></span>|<span data-ttu-id="25cfa-393">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25cfa-393">String</span></span>|<span data-ttu-id="25cfa-394">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-394">Yes</span></span>|<span data-ttu-id="25cfa-395">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-395">\<resourceId\></span></span>|
|<span data-ttu-id="25cfa-396">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="25cfa-396">roleDefinitionId</span></span>|<span data-ttu-id="25cfa-397">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-397">String</span></span>|<span data-ttu-id="25cfa-398">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-398">Yes</span></span>|<span data-ttu-id="25cfa-399">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-399">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="25cfa-400">subjectId</span><span class="sxs-lookup"><span data-stu-id="25cfa-400">subjectId</span></span>|<span data-ttu-id="25cfa-401">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-401">String</span></span>|<span data-ttu-id="25cfa-402">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-402">Yes</span></span>|<span data-ttu-id="25cfa-403">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="25cfa-403">\<subjectId\></span></span>|
|<span data-ttu-id="25cfa-404">assignmentState</span><span class="sxs-lookup"><span data-stu-id="25cfa-404">assignmentState</span></span>|<span data-ttu-id="25cfa-405">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-405">String</span></span>|<span data-ttu-id="25cfa-406">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-406">Yes</span></span>| <span data-ttu-id="25cfa-407">Elegíveis / ativo</span><span class="sxs-lookup"><span data-stu-id="25cfa-407">Eligible / Active</span></span> |
|<span data-ttu-id="25cfa-408">type</span><span class="sxs-lookup"><span data-stu-id="25cfa-408">type</span></span>|<span data-ttu-id="25cfa-409">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-409">String</span></span>|<span data-ttu-id="25cfa-410">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-410">Yes</span></span>| <span data-ttu-id="25cfa-411">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="25cfa-411">AdminExtend</span></span>|
|<span data-ttu-id="25cfa-412">motivo</span><span class="sxs-lookup"><span data-stu-id="25cfa-412">reason</span></span>|<span data-ttu-id="25cfa-413">String</span><span class="sxs-lookup"><span data-stu-id="25cfa-413">String</span></span>| <span data-ttu-id="25cfa-414">depende roleSettings</span><span class="sxs-lookup"><span data-stu-id="25cfa-414">depends on roleSettings</span></span>||
|<span data-ttu-id="25cfa-415">agenda</span><span class="sxs-lookup"><span data-stu-id="25cfa-415">schedule</span></span>|[<span data-ttu-id="25cfa-416">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="25cfa-416">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="25cfa-417">Sim</span><span class="sxs-lookup"><span data-stu-id="25cfa-417">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="25cfa-418">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25cfa-418">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="25cfa-419">Resposta</span><span class="sxs-lookup"><span data-stu-id="25cfa-419">Response</span></span>
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
