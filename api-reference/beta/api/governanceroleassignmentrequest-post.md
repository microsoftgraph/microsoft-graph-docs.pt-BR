---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação desejado em uma atribuição de função. A tabela a seguir lista as operações.
ms.openlocfilehash: b0d9edab1182d4a6fa620cfb953df1cb8af20c66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036014"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="c9124-104">Criar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="c9124-104">Create governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="c9124-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c9124-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9124-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c9124-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9124-107">Crie uma solicitação de atribuição de função para representar a operação desejado em uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="c9124-107">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="c9124-108">A tabela a seguir lista as operações.</span><span class="sxs-lookup"><span data-stu-id="c9124-108">The following table lists the operations.</span></span>

| <span data-ttu-id="c9124-109">Operação</span><span class="sxs-lookup"><span data-stu-id="c9124-109">Operation</span></span>       | <span data-ttu-id="c9124-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9124-110">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="c9124-111">Atribuir uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="c9124-111">Assign a role assignment</span></span>| <span data-ttu-id="c9124-112">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="c9124-112">AdminAdd</span></span> |
| <span data-ttu-id="c9124-113">Ativar uma atribuição de função elegíveis</span><span class="sxs-lookup"><span data-stu-id="c9124-113">Activate an eligible role assignment</span></span>| <span data-ttu-id="c9124-114">UserAdd</span><span class="sxs-lookup"><span data-stu-id="c9124-114">UserAdd</span></span> | 
| <span data-ttu-id="c9124-115">Desativar uma atribuição de função ativada</span><span class="sxs-lookup"><span data-stu-id="c9124-115">Deactivate an activated role assignment</span></span>| <span data-ttu-id="c9124-116">UserRemove</span><span class="sxs-lookup"><span data-stu-id="c9124-116">UserRemove</span></span> | 
| <span data-ttu-id="c9124-117">Remover uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="c9124-117">Remove a role assignment</span></span>| <span data-ttu-id="c9124-118">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="c9124-118">AdminRemove</span></span> |
| <span data-ttu-id="c9124-119">Atualizar uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="c9124-119">Update a role assignment</span></span>| <span data-ttu-id="c9124-120">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="c9124-120">AdminUpdate</span></span> |
| <span data-ttu-id="c9124-121">Solicitação para estender minha atribuição de função</span><span class="sxs-lookup"><span data-stu-id="c9124-121">Request to extend my role assignment</span></span>| <span data-ttu-id="c9124-122">UserExtend</span><span class="sxs-lookup"><span data-stu-id="c9124-122">UserExtend</span></span> | 
| <span data-ttu-id="c9124-123">Estender uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="c9124-123">Extend a role assignment</span></span>| <span data-ttu-id="c9124-124">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="c9124-124">AdminExtend</span></span> | 
| <span data-ttu-id="c9124-125">Solicitação de renovação minha atribuição de função expirados</span><span class="sxs-lookup"><span data-stu-id="c9124-125">Request to renew my expired role assignment</span></span>| <span data-ttu-id="c9124-126">UserRenew</span><span class="sxs-lookup"><span data-stu-id="c9124-126">UserRenew</span></span> | 
| <span data-ttu-id="c9124-127">Renovar uma atribuição de função expirados</span><span class="sxs-lookup"><span data-stu-id="c9124-127">Renew an expired role assignment</span></span>| <span data-ttu-id="c9124-128">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="c9124-128">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="c9124-129">Permissions</span><span class="sxs-lookup"><span data-stu-id="c9124-129">Permissions</span></span>
<span data-ttu-id="c9124-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9124-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9124-132">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9124-132">Permission type</span></span>      | <span data-ttu-id="c9124-133">Permissions</span><span class="sxs-lookup"><span data-stu-id="c9124-133">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9124-134">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9124-134">Delegated (work or school account)</span></span> | <span data-ttu-id="c9124-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c9124-135">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="c9124-136">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9124-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9124-137">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9124-137">Not supported.</span></span>    |
|<span data-ttu-id="c9124-138">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9124-138">Application</span></span> | <span data-ttu-id="c9124-139">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c9124-139">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9124-140">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9124-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9124-141">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c9124-141">Optional query parameters</span></span>
<span data-ttu-id="c9124-142">Esse método não **suporte [parâmetros de consulta OData](/graph/query-parameters)** .</span><span class="sxs-lookup"><span data-stu-id="c9124-142">This method does **not** support [OData query parameters](/graph/query-parameters).</span></span>

### <a name="request-headers"></a><span data-ttu-id="c9124-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9124-143">Request headers</span></span>
| <span data-ttu-id="c9124-144">Nome</span><span class="sxs-lookup"><span data-stu-id="c9124-144">Name</span></span>       | <span data-ttu-id="c9124-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9124-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c9124-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9124-146">Authorization</span></span>  | <span data-ttu-id="c9124-147">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="c9124-147">Bearer {code}</span></span>|
| <span data-ttu-id="c9124-148">Content-type</span><span class="sxs-lookup"><span data-stu-id="c9124-148">Content-type</span></span>  | <span data-ttu-id="c9124-149">application/json</span><span class="sxs-lookup"><span data-stu-id="c9124-149">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="c9124-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9124-150">Request body</span></span>
<span data-ttu-id="c9124-151">No corpo da solicitação, fornece uma representação JSON do objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="c9124-151">In the request body, supply a JSON representation of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="c9124-152">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9124-152">Property</span></span>     | <span data-ttu-id="c9124-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9124-153">Type</span></span>    |<span data-ttu-id="c9124-154">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c9124-154">Required</span></span>|  <span data-ttu-id="c9124-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9124-155">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="c9124-156">resourceId</span><span class="sxs-lookup"><span data-stu-id="c9124-156">resourceId</span></span>|<span data-ttu-id="c9124-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9124-157">String</span></span>|<span data-ttu-id="c9124-158">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-158">Yes</span></span>|<span data-ttu-id="c9124-159">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9124-159">The ID of the resource.</span></span>|
|<span data-ttu-id="c9124-160">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c9124-160">roleDefinitionId</span></span>|<span data-ttu-id="c9124-161">String</span><span class="sxs-lookup"><span data-stu-id="c9124-161">String</span></span>|<span data-ttu-id="c9124-162">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-162">Yes</span></span>|<span data-ttu-id="c9124-163">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="c9124-163">The ID of the role definition.</span></span>|
|<span data-ttu-id="c9124-164">subjectId</span><span class="sxs-lookup"><span data-stu-id="c9124-164">subjectId</span></span>|<span data-ttu-id="c9124-165">String</span><span class="sxs-lookup"><span data-stu-id="c9124-165">String</span></span>|<span data-ttu-id="c9124-166">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-166">Yes</span></span>|<span data-ttu-id="c9124-167">A identificação do assunto.</span><span class="sxs-lookup"><span data-stu-id="c9124-167">The ID of the subject.</span></span>|
|<span data-ttu-id="c9124-168">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c9124-168">assignmentState</span></span>|<span data-ttu-id="c9124-169">String</span><span class="sxs-lookup"><span data-stu-id="c9124-169">String</span></span>|<span data-ttu-id="c9124-170">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-170">Yes</span></span>|<span data-ttu-id="c9124-171">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="c9124-171">The state of assignment.</span></span> <span data-ttu-id="c9124-172">O valor pode ser ``Eligible`` e ``Active``.</span><span class="sxs-lookup"><span data-stu-id="c9124-172">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="c9124-173">type</span><span class="sxs-lookup"><span data-stu-id="c9124-173">type</span></span>|<span data-ttu-id="c9124-174">String</span><span class="sxs-lookup"><span data-stu-id="c9124-174">String</span></span>|<span data-ttu-id="c9124-175">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-175">Yes</span></span>|<span data-ttu-id="c9124-176">O tipo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9124-176">The request type.</span></span> <span data-ttu-id="c9124-177">O valor pode ser `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`e `AdminExtend`.</span><span class="sxs-lookup"><span data-stu-id="c9124-177">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="c9124-178">motivo</span><span class="sxs-lookup"><span data-stu-id="c9124-178">reason</span></span>|<span data-ttu-id="c9124-179">String</span><span class="sxs-lookup"><span data-stu-id="c9124-179">String</span></span>| |<span data-ttu-id="c9124-180">O motivo pelo qual deve ser fornecido para a solicitação de atribuição de função de auditoria e revise finalidade.</span><span class="sxs-lookup"><span data-stu-id="c9124-180">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="c9124-181">agenda</span><span class="sxs-lookup"><span data-stu-id="c9124-181">schedule</span></span>|[<span data-ttu-id="c9124-182">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c9124-182">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="c9124-183">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="c9124-183">The schedule of the role assignment request.</span></span> <span data-ttu-id="c9124-184">Tipo de solicitação de `UserAdd`, `AdminAdd`, `AdminUpdate`, e `AdminExtend`, é necessário.</span><span class="sxs-lookup"><span data-stu-id="c9124-184">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

### <a name="response"></a><span data-ttu-id="c9124-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9124-185">Response</span></span>
<span data-ttu-id="c9124-186">Se tiver êxito, este método retornará um `201, Created` código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9124-186">If successful, this method returns a `201, Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="error-codes"></a><span data-ttu-id="c9124-187">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="c9124-187">Error codes</span></span>
<span data-ttu-id="c9124-188">Essa API segue o padrão dos códigos HTTP, além dos códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="c9124-188">This API follows the standard of HTTP codes, in addition to the error codes listed in the following table.</span></span>

|<span data-ttu-id="c9124-189">Código de erro</span><span class="sxs-lookup"><span data-stu-id="c9124-189">Error code</span></span>     | <span data-ttu-id="c9124-190">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="c9124-190">Error message</span></span>              | <span data-ttu-id="c9124-191">Detalhes</span><span class="sxs-lookup"><span data-stu-id="c9124-191">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="c9124-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c9124-192">400 BadRequest</span></span> | <span data-ttu-id="c9124-193">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="c9124-193">RoleNotFound</span></span>    | <span data-ttu-id="c9124-194">O `roleDefinitionId` fornecida na solicitação de corpo não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="c9124-194">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="c9124-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c9124-195">400 BadRequest</span></span> | <span data-ttu-id="c9124-196">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="c9124-196">ResourceIsLocked</span></span>    | <span data-ttu-id="c9124-197">O recurso fornecido no corpo da solicitação está em estado de `Locked` e não pode criar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="c9124-197">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="c9124-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c9124-198">400 BadRequest</span></span> | <span data-ttu-id="c9124-199">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="c9124-199">SubjectNotFound</span></span>    | <span data-ttu-id="c9124-200">O `subjectId` fornecida na solicitação de corpo não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="c9124-200">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="c9124-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c9124-201">400 BadRequest</span></span> | <span data-ttu-id="c9124-202">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="c9124-202">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="c9124-203">Já existe uma pendente [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no sistema.</span><span class="sxs-lookup"><span data-stu-id="c9124-203">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="c9124-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c9124-204">400 BadRequest</span></span> | <span data-ttu-id="c9124-205">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="c9124-205">RoleAssignmentExists</span></span>    | <span data-ttu-id="c9124-206">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criada já existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="c9124-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="c9124-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c9124-207">400 BadRequest</span></span> | <span data-ttu-id="c9124-208">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="c9124-208">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="c9124-209">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="c9124-209">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="c9124-210">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c9124-210">400 BadRequest</span></span> | <span data-ttu-id="c9124-211">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="c9124-211">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="c9124-212">O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não atende às políticas internas e não pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="c9124-212">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="example-1"></a><span data-ttu-id="c9124-213">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="c9124-213">Example 1</span></span>
<span data-ttu-id="c9124-214">Neste exemplo, os administradores atribuem nawu@fimdev.net usuário à função Leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="c9124-214">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="c9124-215">**Observação:** Além de permissão, este exemplo requer o solicitante ter pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="c9124-215">**Note:** Besides the permission, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="c9124-216">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9124-216">Property</span></span>     | <span data-ttu-id="c9124-217">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9124-217">Type</span></span>    |<span data-ttu-id="c9124-218">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c9124-218">Required</span></span>|  <span data-ttu-id="c9124-219">Valor</span><span class="sxs-lookup"><span data-stu-id="c9124-219">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="c9124-220">resourceId</span><span class="sxs-lookup"><span data-stu-id="c9124-220">resourceId</span></span>|<span data-ttu-id="c9124-221">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9124-221">String</span></span>|<span data-ttu-id="c9124-222">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-222">Yes</span></span>|<span data-ttu-id="c9124-223">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c9124-223">\<resourceId\></span></span>|
|<span data-ttu-id="c9124-224">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c9124-224">roleDefinitionId</span></span>|<span data-ttu-id="c9124-225">String</span><span class="sxs-lookup"><span data-stu-id="c9124-225">String</span></span>|<span data-ttu-id="c9124-226">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-226">Yes</span></span>|<span data-ttu-id="c9124-227">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c9124-227">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="c9124-228">subjectId</span><span class="sxs-lookup"><span data-stu-id="c9124-228">subjectId</span></span>|<span data-ttu-id="c9124-229">String</span><span class="sxs-lookup"><span data-stu-id="c9124-229">String</span></span>|<span data-ttu-id="c9124-230">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-230">Yes</span></span>|<span data-ttu-id="c9124-231">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c9124-231">\<subjectId\></span></span>|
|<span data-ttu-id="c9124-232">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c9124-232">assignmentState</span></span>|<span data-ttu-id="c9124-233">String</span><span class="sxs-lookup"><span data-stu-id="c9124-233">String</span></span>|<span data-ttu-id="c9124-234">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-234">Yes</span></span>| <span data-ttu-id="c9124-235">Elegíveis / ativo</span><span class="sxs-lookup"><span data-stu-id="c9124-235">Eligible / Active</span></span>|
|<span data-ttu-id="c9124-236">type</span><span class="sxs-lookup"><span data-stu-id="c9124-236">type</span></span>|<span data-ttu-id="c9124-237">String</span><span class="sxs-lookup"><span data-stu-id="c9124-237">String</span></span>|<span data-ttu-id="c9124-238">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-238">Yes</span></span>| <span data-ttu-id="c9124-239">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="c9124-239">AdminAdd</span></span>|
|<span data-ttu-id="c9124-240">motivo</span><span class="sxs-lookup"><span data-stu-id="c9124-240">reason</span></span>|<span data-ttu-id="c9124-241">String</span><span class="sxs-lookup"><span data-stu-id="c9124-241">String</span></span>| <span data-ttu-id="c9124-242">depende de configurações de função</span><span class="sxs-lookup"><span data-stu-id="c9124-242">depends on role Settings</span></span>||
|<span data-ttu-id="c9124-243">agenda</span><span class="sxs-lookup"><span data-stu-id="c9124-243">schedule</span></span>|[<span data-ttu-id="c9124-244">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c9124-244">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="c9124-245">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-245">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="c9124-246">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9124-246">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="c9124-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9124-247">Response</span></span>
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
    "roleAssignmentStartDateTime": "2018-05-12T23:38:34.6007266Z",
    "roleAssignmentEndDateTime": "2018-11-08T23:37:43.356Z",
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

## <a name="example-2"></a><span data-ttu-id="c9124-248">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="c9124-248">Example 2</span></span>
<span data-ttu-id="c9124-249">Neste exemplo, nawu@fimdev.net o usuário ativa a função de leitor de faturamento elegível.</span><span class="sxs-lookup"><span data-stu-id="c9124-249">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="c9124-250">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9124-250">Property</span></span>     | <span data-ttu-id="c9124-251">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9124-251">Type</span></span>    |<span data-ttu-id="c9124-252">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c9124-252">Required</span></span>|  <span data-ttu-id="c9124-253">Valor</span><span class="sxs-lookup"><span data-stu-id="c9124-253">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="c9124-254">resourceId</span><span class="sxs-lookup"><span data-stu-id="c9124-254">resourceId</span></span>|<span data-ttu-id="c9124-255">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9124-255">String</span></span>|<span data-ttu-id="c9124-256">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-256">Yes</span></span>|<span data-ttu-id="c9124-257">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c9124-257">\<resourceId\></span></span>|
|<span data-ttu-id="c9124-258">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c9124-258">roleDefinitionId</span></span>|<span data-ttu-id="c9124-259">String</span><span class="sxs-lookup"><span data-stu-id="c9124-259">String</span></span>|<span data-ttu-id="c9124-260">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-260">Yes</span></span>|<span data-ttu-id="c9124-261">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c9124-261">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="c9124-262">subjectId</span><span class="sxs-lookup"><span data-stu-id="c9124-262">subjectId</span></span>|<span data-ttu-id="c9124-263">String</span><span class="sxs-lookup"><span data-stu-id="c9124-263">String</span></span>|<span data-ttu-id="c9124-264">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-264">Yes</span></span>|<span data-ttu-id="c9124-265">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c9124-265">\<subjectId\></span></span>|
|<span data-ttu-id="c9124-266">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c9124-266">assignmentState</span></span>|<span data-ttu-id="c9124-267">String</span><span class="sxs-lookup"><span data-stu-id="c9124-267">String</span></span>|<span data-ttu-id="c9124-268">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-268">Yes</span></span>| <span data-ttu-id="c9124-269">Ativo</span><span class="sxs-lookup"><span data-stu-id="c9124-269">Active</span></span>|
|<span data-ttu-id="c9124-270">type</span><span class="sxs-lookup"><span data-stu-id="c9124-270">type</span></span>|<span data-ttu-id="c9124-271">String</span><span class="sxs-lookup"><span data-stu-id="c9124-271">String</span></span>|<span data-ttu-id="c9124-272">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-272">Yes</span></span>| <span data-ttu-id="c9124-273">UserAdd</span><span class="sxs-lookup"><span data-stu-id="c9124-273">UserAdd</span></span>|
|<span data-ttu-id="c9124-274">motivo</span><span class="sxs-lookup"><span data-stu-id="c9124-274">reason</span></span>|<span data-ttu-id="c9124-275">String</span><span class="sxs-lookup"><span data-stu-id="c9124-275">String</span></span>| <span data-ttu-id="c9124-276">depende de configurações de função</span><span class="sxs-lookup"><span data-stu-id="c9124-276">depends on role Settings</span></span>||
|<span data-ttu-id="c9124-277">agenda</span><span class="sxs-lookup"><span data-stu-id="c9124-277">schedule</span></span>|[<span data-ttu-id="c9124-278">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c9124-278">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="c9124-279">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-279">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="c9124-280">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9124-280">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="c9124-281">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9124-281">Response</span></span>
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
    "roleAssignmentStartDateTime": "2018-05-12T23:29:29.5123911Z",
    "roleAssignmentEndDateTime": "2018-05-13T08:28:43.537Z",
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

## <a name="example-3"></a><span data-ttu-id="c9124-282">Exemplo 3</span><span class="sxs-lookup"><span data-stu-id="c9124-282">Example 3</span></span>
<span data-ttu-id="c9124-283">Neste exemplo, o nawu@fimdev.net usuário desativa a função de leitor de cobrança ativa.</span><span class="sxs-lookup"><span data-stu-id="c9124-283">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="c9124-284">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9124-284">Property</span></span>     | <span data-ttu-id="c9124-285">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9124-285">Type</span></span>    |<span data-ttu-id="c9124-286">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c9124-286">Required</span></span>|  <span data-ttu-id="c9124-287">Valor</span><span class="sxs-lookup"><span data-stu-id="c9124-287">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="c9124-288">resourceId</span><span class="sxs-lookup"><span data-stu-id="c9124-288">resourceId</span></span>|<span data-ttu-id="c9124-289">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9124-289">String</span></span>|<span data-ttu-id="c9124-290">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-290">Yes</span></span>|<span data-ttu-id="c9124-291">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c9124-291">\<resourceId\></span></span>|
|<span data-ttu-id="c9124-292">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c9124-292">roleDefinitionId</span></span>|<span data-ttu-id="c9124-293">String</span><span class="sxs-lookup"><span data-stu-id="c9124-293">String</span></span>|<span data-ttu-id="c9124-294">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-294">Yes</span></span>|<span data-ttu-id="c9124-295">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c9124-295">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="c9124-296">subjectId</span><span class="sxs-lookup"><span data-stu-id="c9124-296">subjectId</span></span>|<span data-ttu-id="c9124-297">String</span><span class="sxs-lookup"><span data-stu-id="c9124-297">String</span></span>|<span data-ttu-id="c9124-298">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-298">Yes</span></span>|<span data-ttu-id="c9124-299">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c9124-299">\<subjectId\></span></span>|
|<span data-ttu-id="c9124-300">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c9124-300">assignmentState</span></span>|<span data-ttu-id="c9124-301">String</span><span class="sxs-lookup"><span data-stu-id="c9124-301">String</span></span>|<span data-ttu-id="c9124-302">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-302">Yes</span></span>| <span data-ttu-id="c9124-303">Ativo</span><span class="sxs-lookup"><span data-stu-id="c9124-303">Active</span></span>|
|<span data-ttu-id="c9124-304">type</span><span class="sxs-lookup"><span data-stu-id="c9124-304">type</span></span>|<span data-ttu-id="c9124-305">String</span><span class="sxs-lookup"><span data-stu-id="c9124-305">String</span></span>|<span data-ttu-id="c9124-306">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-306">Yes</span></span>| <span data-ttu-id="c9124-307">UserRemove</span><span class="sxs-lookup"><span data-stu-id="c9124-307">UserRemove</span></span>|
|<span data-ttu-id="c9124-308">motivo</span><span class="sxs-lookup"><span data-stu-id="c9124-308">reason</span></span>|<span data-ttu-id="c9124-309">String</span><span class="sxs-lookup"><span data-stu-id="c9124-309">String</span></span>| <span data-ttu-id="c9124-310">Não</span><span class="sxs-lookup"><span data-stu-id="c9124-310">No</span></span>||
|<span data-ttu-id="c9124-311">agenda</span><span class="sxs-lookup"><span data-stu-id="c9124-311">schedule</span></span>|[<span data-ttu-id="c9124-312">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c9124-312">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="c9124-313">Não</span><span class="sxs-lookup"><span data-stu-id="c9124-313">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="c9124-314">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9124-314">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="c9124-315">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9124-315">Response</span></span>
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
    "roleAssignmentStartDateTime": null,
    "roleAssignmentEndDateTime": null,
    "reason": "Evaluate only",
    "schedule": null,
    "status": {
        "status": "Closed",
        "subStatus": "Revoked",
        "statusDetails": []
    }
}
```

### <a name="example-4"></a><span data-ttu-id="c9124-316">Exemplo 4</span><span class="sxs-lookup"><span data-stu-id="c9124-316">Example 4</span></span>
<span data-ttu-id="c9124-317">Neste exemplo, os administradores remover nawu@fimdev.net o usuário da função Leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="c9124-317">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="c9124-318">**Observação:** Além do escopo de permissão, este exemplo requer o solicitante ter pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="c9124-318">**Note:** Besides the permission scope, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="c9124-319">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9124-319">Property</span></span>     | <span data-ttu-id="c9124-320">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9124-320">Type</span></span>    |<span data-ttu-id="c9124-321">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c9124-321">Required</span></span>|  <span data-ttu-id="c9124-322">Valor</span><span class="sxs-lookup"><span data-stu-id="c9124-322">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="c9124-323">resourceId</span><span class="sxs-lookup"><span data-stu-id="c9124-323">resourceId</span></span>|<span data-ttu-id="c9124-324">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9124-324">String</span></span>|<span data-ttu-id="c9124-325">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-325">Yes</span></span>|<span data-ttu-id="c9124-326">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c9124-326">\<resourceId\></span></span>|
|<span data-ttu-id="c9124-327">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c9124-327">roleDefinitionId</span></span>|<span data-ttu-id="c9124-328">String</span><span class="sxs-lookup"><span data-stu-id="c9124-328">String</span></span>|<span data-ttu-id="c9124-329">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-329">Yes</span></span>|<span data-ttu-id="c9124-330">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c9124-330">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="c9124-331">subjectId</span><span class="sxs-lookup"><span data-stu-id="c9124-331">subjectId</span></span>|<span data-ttu-id="c9124-332">String</span><span class="sxs-lookup"><span data-stu-id="c9124-332">String</span></span>|<span data-ttu-id="c9124-333">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-333">Yes</span></span>|<span data-ttu-id="c9124-334">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c9124-334">\<subjectId\></span></span>|
|<span data-ttu-id="c9124-335">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c9124-335">assignmentState</span></span>|<span data-ttu-id="c9124-336">String</span><span class="sxs-lookup"><span data-stu-id="c9124-336">String</span></span>|<span data-ttu-id="c9124-337">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-337">Yes</span></span>| <span data-ttu-id="c9124-338">Elegíveis / ativo</span><span class="sxs-lookup"><span data-stu-id="c9124-338">Eligible / Active</span></span>|
|<span data-ttu-id="c9124-339">type</span><span class="sxs-lookup"><span data-stu-id="c9124-339">type</span></span>|<span data-ttu-id="c9124-340">String</span><span class="sxs-lookup"><span data-stu-id="c9124-340">String</span></span>|<span data-ttu-id="c9124-341">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-341">Yes</span></span>| <span data-ttu-id="c9124-342">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="c9124-342">AdminRemove</span></span>|
|<span data-ttu-id="c9124-343">motivo</span><span class="sxs-lookup"><span data-stu-id="c9124-343">reason</span></span>|<span data-ttu-id="c9124-344">String</span><span class="sxs-lookup"><span data-stu-id="c9124-344">String</span></span>| <span data-ttu-id="c9124-345">Não</span><span class="sxs-lookup"><span data-stu-id="c9124-345">No</span></span>||
|<span data-ttu-id="c9124-346">agenda</span><span class="sxs-lookup"><span data-stu-id="c9124-346">schedule</span></span>|[<span data-ttu-id="c9124-347">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c9124-347">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="c9124-348">Não</span><span class="sxs-lookup"><span data-stu-id="c9124-348">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="c9124-349">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9124-349">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="c9124-350">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9124-350">Response</span></span>
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
  "roleAssignmentStartDateTime":null,
  "roleAssignmentEndDateTime":null,
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```

### <a name="example-5"></a><span data-ttu-id="c9124-351">Exemplo 5</span><span class="sxs-lookup"><span data-stu-id="c9124-351">Example 5</span></span>
<span data-ttu-id="c9124-352">Neste exemplo, os administradores atualizar a atribuição de função para o usuário de nawu@fimdev.net ao proprietário.</span><span class="sxs-lookup"><span data-stu-id="c9124-352">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="c9124-353">**Observação:** Além do escopo de permissão, este exemplo requer o solicitante ter pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="c9124-353">**Note:** Besides the permission scope, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 
| <span data-ttu-id="c9124-354">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9124-354">Property</span></span>     | <span data-ttu-id="c9124-355">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9124-355">Type</span></span>    |<span data-ttu-id="c9124-356">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c9124-356">Required</span></span>|  <span data-ttu-id="c9124-357">Valor</span><span class="sxs-lookup"><span data-stu-id="c9124-357">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="c9124-358">resourceId</span><span class="sxs-lookup"><span data-stu-id="c9124-358">resourceId</span></span>|<span data-ttu-id="c9124-359">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9124-359">String</span></span>|<span data-ttu-id="c9124-360">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-360">Yes</span></span>|<span data-ttu-id="c9124-361">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c9124-361">\<resourceId\></span></span>|
|<span data-ttu-id="c9124-362">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c9124-362">roleDefinitionId</span></span>|<span data-ttu-id="c9124-363">String</span><span class="sxs-lookup"><span data-stu-id="c9124-363">String</span></span>|<span data-ttu-id="c9124-364">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-364">Yes</span></span>|<span data-ttu-id="c9124-365">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c9124-365">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="c9124-366">subjectId</span><span class="sxs-lookup"><span data-stu-id="c9124-366">subjectId</span></span>|<span data-ttu-id="c9124-367">String</span><span class="sxs-lookup"><span data-stu-id="c9124-367">String</span></span>|<span data-ttu-id="c9124-368">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-368">Yes</span></span>|<span data-ttu-id="c9124-369">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c9124-369">\<subjectId\></span></span>|
|<span data-ttu-id="c9124-370">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c9124-370">assignmentState</span></span>|<span data-ttu-id="c9124-371">String</span><span class="sxs-lookup"><span data-stu-id="c9124-371">String</span></span>|<span data-ttu-id="c9124-372">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-372">Yes</span></span>| <span data-ttu-id="c9124-373">Elegíveis / ativo</span><span class="sxs-lookup"><span data-stu-id="c9124-373">Eligible / Active</span></span>|
|<span data-ttu-id="c9124-374">type</span><span class="sxs-lookup"><span data-stu-id="c9124-374">type</span></span>|<span data-ttu-id="c9124-375">String</span><span class="sxs-lookup"><span data-stu-id="c9124-375">String</span></span>|<span data-ttu-id="c9124-376">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-376">Yes</span></span>| <span data-ttu-id="c9124-377">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="c9124-377">AdminUpdate</span></span>|
|<span data-ttu-id="c9124-378">motivo</span><span class="sxs-lookup"><span data-stu-id="c9124-378">reason</span></span>|<span data-ttu-id="c9124-379">String</span><span class="sxs-lookup"><span data-stu-id="c9124-379">String</span></span>| <span data-ttu-id="c9124-380">depende roleSettings</span><span class="sxs-lookup"><span data-stu-id="c9124-380">depends on roleSettings</span></span>||
|<span data-ttu-id="c9124-381">agenda</span><span class="sxs-lookup"><span data-stu-id="c9124-381">schedule</span></span>|[<span data-ttu-id="c9124-382">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c9124-382">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="c9124-383">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-383">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="c9124-384">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9124-384">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="c9124-385">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9124-385">Response</span></span>
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
  "roleAssignmentStartDateTime":"2018-05-12T23:50:03.4755896Z",
  "roleAssignmentEndDateTime":"2018-06-05T05:42:31Z",
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

### <a name="example-6"></a><span data-ttu-id="c9124-386">Exemplo 6</span><span class="sxs-lookup"><span data-stu-id="c9124-386">Example 6</span></span>
<span data-ttu-id="c9124-387">Este exemplo estende a atribuição de função expirar para usuário ANUJCUSER Colaborador do serviço de gerenciamento de API.</span><span class="sxs-lookup"><span data-stu-id="c9124-387">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="c9124-388">**Observação:** Além do escopo de permissão, este exemplo requer o solicitante ter pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="c9124-388">**Note:** Besides the permission scope, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="c9124-389">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9124-389">Property</span></span>     | <span data-ttu-id="c9124-390">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9124-390">Type</span></span>    |<span data-ttu-id="c9124-391">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c9124-391">Required</span></span>|  <span data-ttu-id="c9124-392">Valor</span><span class="sxs-lookup"><span data-stu-id="c9124-392">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="c9124-393">resourceId</span><span class="sxs-lookup"><span data-stu-id="c9124-393">resourceId</span></span>|<span data-ttu-id="c9124-394">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9124-394">String</span></span>|<span data-ttu-id="c9124-395">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-395">Yes</span></span>|<span data-ttu-id="c9124-396">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c9124-396">\<resourceId\></span></span>|
|<span data-ttu-id="c9124-397">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c9124-397">roleDefinitionId</span></span>|<span data-ttu-id="c9124-398">String</span><span class="sxs-lookup"><span data-stu-id="c9124-398">String</span></span>|<span data-ttu-id="c9124-399">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-399">Yes</span></span>|<span data-ttu-id="c9124-400">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c9124-400">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="c9124-401">subjectId</span><span class="sxs-lookup"><span data-stu-id="c9124-401">subjectId</span></span>|<span data-ttu-id="c9124-402">String</span><span class="sxs-lookup"><span data-stu-id="c9124-402">String</span></span>|<span data-ttu-id="c9124-403">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-403">Yes</span></span>|<span data-ttu-id="c9124-404">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c9124-404">\<subjectId\></span></span>|
|<span data-ttu-id="c9124-405">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c9124-405">assignmentState</span></span>|<span data-ttu-id="c9124-406">String</span><span class="sxs-lookup"><span data-stu-id="c9124-406">String</span></span>|<span data-ttu-id="c9124-407">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-407">Yes</span></span>| <span data-ttu-id="c9124-408">Elegíveis / ativo</span><span class="sxs-lookup"><span data-stu-id="c9124-408">Eligible / Active</span></span> |
|<span data-ttu-id="c9124-409">type</span><span class="sxs-lookup"><span data-stu-id="c9124-409">type</span></span>|<span data-ttu-id="c9124-410">String</span><span class="sxs-lookup"><span data-stu-id="c9124-410">String</span></span>|<span data-ttu-id="c9124-411">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-411">Yes</span></span>| <span data-ttu-id="c9124-412">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="c9124-412">AdminExtend</span></span>|
|<span data-ttu-id="c9124-413">motivo</span><span class="sxs-lookup"><span data-stu-id="c9124-413">reason</span></span>|<span data-ttu-id="c9124-414">String</span><span class="sxs-lookup"><span data-stu-id="c9124-414">String</span></span>| <span data-ttu-id="c9124-415">depende roleSettings</span><span class="sxs-lookup"><span data-stu-id="c9124-415">depends on roleSettings</span></span>||
|<span data-ttu-id="c9124-416">agenda</span><span class="sxs-lookup"><span data-stu-id="c9124-416">schedule</span></span>|[<span data-ttu-id="c9124-417">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c9124-417">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="c9124-418">Sim</span><span class="sxs-lookup"><span data-stu-id="c9124-418">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="c9124-419">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9124-419">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="c9124-420">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9124-420">Response</span></span>
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
  "roleAssignmentStartDateTime":"2018-05-12T23:54:09.7221332Z",
  "roleAssignmentEndDateTime":"2018-08-10T23:53:55.327Z",
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
<!-- {
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
