---
title: Listar provisioningObjectSummary
description: Obter todos os eventos de provisionamento que ocorreram em seu locatário.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 9e907b5fd55d6022fde87816179c89a7689be41b
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231370"
---
# <a name="list-provisioningobjectsummary"></a><span data-ttu-id="0602d-103">Listar provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="0602d-103">List provisioningObjectSummary</span></span>

<span data-ttu-id="0602d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0602d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0602d-105">Obter todos os eventos de provisionamento que ocorreram em seu locatário, como a exclusão de um grupo em um aplicativo de destino ou a criação de um usuário ao provisionar contas de usuário do seu sistema de RH.</span><span class="sxs-lookup"><span data-stu-id="0602d-105">Get all provisioning events that occurred in your tenant, such as the deletion of a group in a target application or the creation of a user when provisioning user accounts from your HR system.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0602d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0602d-106">Permissions</span></span>

<span data-ttu-id="0602d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0602d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0602d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0602d-109">Permission type</span></span> | <span data-ttu-id="0602d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0602d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0602d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0602d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0602d-112">AuditLog.Read.All e Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0602d-112">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="0602d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0602d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0602d-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0602d-114">Not supported</span></span>   |
|<span data-ttu-id="0602d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0602d-115">Application</span></span> | <span data-ttu-id="0602d-116">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="0602d-116">AuditLog.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0602d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0602d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /auditLogs/provisioning
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0602d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0602d-118">Optional query parameters</span></span>

<span data-ttu-id="0602d-119">Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0602d-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="0602d-120">Observe que os filtros são todos sensíveis a minúsculas, exceto para status.</span><span class="sxs-lookup"><span data-stu-id="0602d-120">Note that the filters are all case sensitive except for status.</span></span> 

|<span data-ttu-id="0602d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0602d-121">Name</span></span>     |<span data-ttu-id="0602d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0602d-122">Description</span></span>                            |<span data-ttu-id="0602d-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0602d-123">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="0602d-124">$filter</span><span class="sxs-lookup"><span data-stu-id="0602d-124">$filter</span></span>](/graph/query-parameters#filter-parameter)|<span data-ttu-id="0602d-125">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="0602d-125">Filters results (rows).</span></span> |/`auditLogs/provisioning?$filter=id eq '74c3b0ae-9cc5-850e-e0a5-7r6a4231de87'`
|[<span data-ttu-id="0602d-126">$top</span><span class="sxs-lookup"><span data-stu-id="0602d-126">$top</span></span>](/graph/query-parameters#top-parameter)|<span data-ttu-id="0602d-127">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="0602d-127">Sets the page size of results.</span></span>|`/auditLogs/provisioning?$top=20`|
|[<span data-ttu-id="0602d-128">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="0602d-128">$skiptoken</span></span>](/graph/query-parameters#skiptoken-parameter)|<span data-ttu-id="0602d-129">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas.</span><span class="sxs-lookup"><span data-stu-id="0602d-129">Retrieves the next page of results from result sets that span multiple pages.</span></span> <span data-ttu-id="0602d-130">Você deve passar o filtro superior na consulta para gerar o token.</span><span class="sxs-lookup"><span data-stu-id="0602d-130">You must pass the top filter in the query to generate the token.</span></span> <span data-ttu-id="0602d-131">Não é possível especificar o número de resultados a serem ignorados.</span><span class="sxs-lookup"><span data-stu-id="0602d-131">You cannot specify the number of results to be skipped.</span></span>|`/auditLogs/provisioning?$top=20&$skiptoken=g822a72df43b19c8ce94b71d153981b680a08800bc3e35f239dffb378ff72c25"`|

<span data-ttu-id="0602d-132">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="0602d-132">For general information, see [OData query parameters](/graph/query_parameters).</span></span>

### <a name="attributes-supported-by-the-filter-parameter"></a><span data-ttu-id="0602d-133">Atributos suportados pelo parâmetro $filter</span><span class="sxs-lookup"><span data-stu-id="0602d-133">Attributes supported by the $filter parameter</span></span>

|<span data-ttu-id="0602d-134">Nome do atributo</span><span class="sxs-lookup"><span data-stu-id="0602d-134">Attribute name</span></span> |<span data-ttu-id="0602d-135">Operadores com suporte</span><span class="sxs-lookup"><span data-stu-id="0602d-135">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="0602d-136">id</span><span class="sxs-lookup"><span data-stu-id="0602d-136">id</span></span>| <span data-ttu-id="0602d-137">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-137">eq, contains</span></span>|
|<span data-ttu-id="0602d-138">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="0602d-138">activityDateTime</span></span>| <span data-ttu-id="0602d-139">eq</span><span class="sxs-lookup"><span data-stu-id="0602d-139">eq</span></span>|
|<span data-ttu-id="0602d-140">tenantid</span><span class="sxs-lookup"><span data-stu-id="0602d-140">tenantid</span></span>|<span data-ttu-id="0602d-141">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-141">eq, contains</span></span>|
|<span data-ttu-id="0602d-142">jobid</span><span class="sxs-lookup"><span data-stu-id="0602d-142">jobid</span></span>|<span data-ttu-id="0602d-143">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-143">eq, contains</span></span>|
|<span data-ttu-id="0602d-144">changeid</span><span class="sxs-lookup"><span data-stu-id="0602d-144">changeid</span></span>|<span data-ttu-id="0602d-145">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-145">eq, contains</span></span>|
|<span data-ttu-id="0602d-146">cycleid</span><span class="sxs-lookup"><span data-stu-id="0602d-146">cycleid</span></span>|<span data-ttu-id="0602d-147">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-147">eq, contains</span></span>|
|<span data-ttu-id="0602d-148">ação</span><span class="sxs-lookup"><span data-stu-id="0602d-148">action</span></span>|<span data-ttu-id="0602d-149">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-149">eq, contains</span></span>|
|<span data-ttu-id="0602d-150">provisioningAction</span><span class="sxs-lookup"><span data-stu-id="0602d-150">provisioningAction</span></span>|<span data-ttu-id="0602d-151">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-151">eq, contains</span></span>|
|<span data-ttu-id="0602d-152">durationInMilliseconds</span><span class="sxs-lookup"><span data-stu-id="0602d-152">durationInMilliseconds</span></span>|<span data-ttu-id="0602d-153">eq, gt, lt</span><span class="sxs-lookup"><span data-stu-id="0602d-153">eq, gt, lt</span></span>|
|<span data-ttu-id="0602d-154">provisioningStatusInfo/status</span><span class="sxs-lookup"><span data-stu-id="0602d-154">provisioningStatusInfo/status</span></span>|<span data-ttu-id="0602d-155">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-155">eq, contains</span></span>|
|<span data-ttu-id="0602d-156">statusInfo/status</span><span class="sxs-lookup"><span data-stu-id="0602d-156">statusInfo/status</span></span>|<span data-ttu-id="0602d-157">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-157">eq, contains</span></span>|
|<span data-ttu-id="0602d-158">sourceSystem/displayName</span><span class="sxs-lookup"><span data-stu-id="0602d-158">sourceSystem/displayName</span></span>|<span data-ttu-id="0602d-159">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-159">eq, contains</span></span>|
|<span data-ttu-id="0602d-160">targetSystem/displayName</span><span class="sxs-lookup"><span data-stu-id="0602d-160">targetSystem/displayName</span></span>|<span data-ttu-id="0602d-161">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-161">eq, contains</span></span>|
|<span data-ttu-id="0602d-162">sourceIdentity/identityType</span><span class="sxs-lookup"><span data-stu-id="0602d-162">sourceIdentity/identityType</span></span>|<span data-ttu-id="0602d-163">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-163">eq, contains</span></span>|
|<span data-ttu-id="0602d-164">targetIdentity/identityType</span><span class="sxs-lookup"><span data-stu-id="0602d-164">targetIdentity/identityType</span></span>|<span data-ttu-id="0602d-165">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-165">eq, contains</span></span>|
|<span data-ttu-id="0602d-166">sourceIdentity/id</span><span class="sxs-lookup"><span data-stu-id="0602d-166">sourceIdentity/id</span></span>|<span data-ttu-id="0602d-167">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-167">eq, contains</span></span>|
|<span data-ttu-id="0602d-168">servicePrincipal/id</span><span class="sxs-lookup"><span data-stu-id="0602d-168">servicePrincipal/id</span></span>|<span data-ttu-id="0602d-169">eq</span><span class="sxs-lookup"><span data-stu-id="0602d-169">eq</span></span>|
|<span data-ttu-id="0602d-170">servicePrincipal/name</span><span class="sxs-lookup"><span data-stu-id="0602d-170">servicePrincipal/name</span></span>|<span data-ttu-id="0602d-171">eq</span><span class="sxs-lookup"><span data-stu-id="0602d-171">eq</span></span>|
|<span data-ttu-id="0602d-172">targetIdentity/id</span><span class="sxs-lookup"><span data-stu-id="0602d-172">targetIdentity/id</span></span>|<span data-ttu-id="0602d-173">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-173">eq, contains</span></span>|
|<span data-ttu-id="0602d-174">sourceIdentity/displayName</span><span class="sxs-lookup"><span data-stu-id="0602d-174">sourceIdentity/displayName</span></span>|<span data-ttu-id="0602d-175">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-175">eq, contains</span></span>|
|<span data-ttu-id="0602d-176">targetIdentity/displayName</span><span class="sxs-lookup"><span data-stu-id="0602d-176">targetIdentity/displayName</span></span>|<span data-ttu-id="0602d-177">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-177">eq, contains</span></span>|
|<span data-ttu-id="0602d-178">initiatedBy/displayName</span><span class="sxs-lookup"><span data-stu-id="0602d-178">initiatedBy/displayName</span></span>|<span data-ttu-id="0602d-179">eq, contém</span><span class="sxs-lookup"><span data-stu-id="0602d-179">eq, contains</span></span>|

## <a name="request-headers"></a><span data-ttu-id="0602d-180">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0602d-180">Request headers</span></span>

| <span data-ttu-id="0602d-181">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0602d-181">Header</span></span>        | <span data-ttu-id="0602d-182">Valor</span><span class="sxs-lookup"><span data-stu-id="0602d-182">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="0602d-183">Autorização</span><span class="sxs-lookup"><span data-stu-id="0602d-183">Authorization</span></span> | <span data-ttu-id="0602d-184">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="0602d-184">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0602d-185">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0602d-185">Request body</span></span>

<span data-ttu-id="0602d-186">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0602d-186">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0602d-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="0602d-187">Response</span></span>

<span data-ttu-id="0602d-188">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [provisioningObjectSummary](../resources/provisioningobjectsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0602d-188">If successful, this method returns a `200 OK` response code and a collection of [provisioningObjectSummary](../resources/provisioningobjectsummary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0602d-189">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0602d-189">Examples</span></span>

### <a name="example-1-successful-request"></a><span data-ttu-id="0602d-190">Exemplo 1: Solicitação bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="0602d-190">Example 1: Successful request</span></span>

### <a name="request"></a><span data-ttu-id="0602d-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0602d-191">Request</span></span>

<span data-ttu-id="0602d-192">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0602d-192">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0602d-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="0602d-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/provisioning
```
# <a name="c"></a>[<span data-ttu-id="0602d-194">C#</span><span class="sxs-lookup"><span data-stu-id="0602d-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-provisioningobjectsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0602d-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0602d-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-provisioningobjectsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0602d-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0602d-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-provisioningobjectsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0602d-197">Java</span><span class="sxs-lookup"><span data-stu-id="0602d-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-provisioningobjectsummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0602d-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="0602d-198">Response</span></span>

<span data-ttu-id="0602d-199">A seguir, um exemplo da resposta para um evento bem-sucedido.</span><span class="sxs-lookup"><span data-stu-id="0602d-199">The following is an example of the response for a successful event.</span></span>

><span data-ttu-id="0602d-200">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0602d-200">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "name": "list_provisioningobjectsummary"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/provisioning",
    "value": [
         {
            "id": "75b5b0ae-9fc5-8d0e-e0a9-7y6a4728de56",
            "activityDateTime": "2019-05-04T03:00:54Z",
            "tenantId": "74beb175-3b80-7b63-b9d5-6f0b76082b16",
            "jobId": "aws.74beb1753b704b63b8d56f0b76082b16.10a7a801-7101-4c69-ae00-ce9f75f8460a",
            "cycleId": "b6502552-018d-79bd-8869-j47194dc65c1",
            "changeId": "b6502552-018d-89bd-9969-b49194dc65c1",
            "action": "Create",
            "provisioningAction": "create",
            "durationInMilliseconds": 3236,
            "statusInfo": {
                "status": "success"
            },
            "provisioningStatusInfo": {
                "status": "success",
                "errorInformation" : null
            },
            "provisioningSteps": [
                {
                    "name": "EntryImport",
                    "provisioningStepType": "Import",
                    "status": "success",
                    "description": "Retrieved RolesCompound '10a7a801-7101-4c69-ae00-ce9f75f8460a' from Contoso",
                    "details": {}
                },
                {
                    "name": "EntryExportUpdate",
                    "provisioningStepType": "Export",
                    "status": "success",
                    "description": "RolesCompound '60a7a801-7101-4c69-ae00-ce9f75f8460a' was updated in Azure Active Directory",
                    "details": {
                        "ReportableIdentifier": "60a7a801-7101-4c69-ae00-ce9f75f8460a"
                    }
                }
            ],
            "modifiedProperties": [
                {
                    "displayName": "appId",
                    "oldValue": null,
                    "newValue": "60a7a801-7101-4c69-ae00-ce9f75f8460a"
                },
                {
                    "displayName": "Roles",
                    "oldValue": null,
                    "newValue": "jaws-prod-role2,jaws-prod-saml2, jayaws-role,jayaws-saml, TestRole,super-saml"
                },
                {
                    "displayName": "objectId",
                    "oldValue": null,
                    "newValue": "6nn37b93-185a-4485-a519-50c09549f3ad"
                },
                {
                    "displayName": "displayName",
                    "oldValue": null,
                    "newValue": "Contoso"
                },
                {
                    "displayName": "homepage",
                    "oldValue": null,
                    "newValue": "https://signin.contoso.com/saml?metadata=contoso|ISV9.1|primary|z"
                },
            ],
            "servicePrincipal": {
                "id": "6cc35b93-185a-4485-a519-50c09549g3ad",
                "displayName": "Contoso"
            },
            "sourceSystem": {
                "id": "d1e090e1-f2f4-4678-be44-6442ffff0621",
                "displayName": "Contoso",
                "details": {}
            },
            "targetSystem": {
                "id": "e69d4bd2-2da2-483e-bc49-aad4080b91b3",
                "displayName": "Azure Active Directory",
                "details": {
                    "ApplicationId": "bcf4d658-ac9f-408d-bf04-e86dc10328fb",
                    "ServicePrincipalId": "6nn35b93-185a-4485-a519-50c09549f3ad",
                    "ServicePrincipalDisplayName": "Contoso"
                }
            },
            "initiatedBy": {
                "initiatingType": "system",
                "id": "",
                "displayName": "Azure AD Provisioning Service"
            },
            "sourceIdentity": {
                "identityType": "RolesCompound",
                "id": "60a7a801-7101-4c69-ae00-ce9f75f8460a",
                "displayName": "",
                "details": {}
            },
            "targetIdentity": {
                "identityType": "ServicePrincipal",
                "id": "6nn35b93-185a-4485-a519-50c09549f3ad",
                "displayName": "",
                "details": {}
            }
          }
    ]
}

```
### <a name="example-2-error-reponse"></a><span data-ttu-id="0602d-201">Exemplo 2: Reponse de erro</span><span class="sxs-lookup"><span data-stu-id="0602d-201">Example 2: Error reponse</span></span>

### <a name="request"></a><span data-ttu-id="0602d-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0602d-202">Request</span></span>

<span data-ttu-id="0602d-203">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0602d-203">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0602d-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="0602d-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary_error"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/provisioning
```
# <a name="c"></a>[<span data-ttu-id="0602d-205">C#</span><span class="sxs-lookup"><span data-stu-id="0602d-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-provisioningobjectsummary-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0602d-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0602d-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-provisioningobjectsummary-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0602d-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0602d-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-provisioningobjectsummary-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0602d-208">Java</span><span class="sxs-lookup"><span data-stu-id="0602d-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-provisioningobjectsummary-error-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0602d-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="0602d-209">Response</span></span>

<span data-ttu-id="0602d-210">A seguir, um exemplo da resposta para um evento de provisionamento com falha.</span><span class="sxs-lookup"><span data-stu-id="0602d-210">The following is an example of the response for a failed provisioning event.</span></span>

><span data-ttu-id="0602d-211">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0602d-211">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "name": "list_provisioningobjectsummary_error"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/provisioning",
    "value": [
        {
            "id": "gc532ff9-r265-ec76-861e-42e2970a8218",
            "activityDateTime": "2019-06-24T20:53:08Z",
            "tenantId": "7928d5b5-7442-4a97-ne2d-66f9j9972ecn",
            "jobId": "ContosoOutDelta.7928d5b574424a97ne2d66f9j9972ecn",
            "cycleId": "44576n58-v14b-70fj-8404-3d22tt46ed93",
            "changeId": "eaad2f8b-e6e3-409b-83bd-e4e2e57177d5",
            "action": "Create",
            "durationInMilliseconds": 2785,
            "sourceSystem": {
                "id": "0404601d-a9c0-4ec7-bbcd-02660120d8c9",
                "displayName": "Azure Active Directory",
                "details": {}
            },
            "targetSystem": {
                "id": "cd22f60b-5f2d-1adg-adb4-76ef31db996b",
                "displayName": "Contoso",
                "details": {
                    "ApplicationId": "f2764360-e0ec-5676-711e-cd6fc0d4dd61",
                    "ServicePrincipalId": "chc46a42-966b-47d7-9774-576b1c8bd0b8",
                    "ServicePrincipalDisplayName": "Contoso"
                }
            },
            "initiatedBy": {
                "id": "",
                "displayName": "Azure AD Provisioning Service",
                "initiatorType": "system"
            },
            "servicePrincipal": {
                "id": "chc46a42-966b-47d7-9774-576b1c8bd0b8",
                "displayName": "Contoso"
            },
            "sourceIdentity": {
                "id": "5e6c9rae-ab4d-5239-8ad0-174391d110eb",
                "displayName": "Self-service Pilot",
                "identityType": "Group",
                "details": {}
            },
            "targetIdentity": {
                "id": "",
                "displayName": "",
                "identityType": "Group",
                "details": {}
            },
            "statusInfo": {
                "@odata.type": "#microsoft.graph.statusDetails",
                "status": "failure",
                "errorCode": "ContosoEntryConflict",
                "reason": "Message: Contoso returned an error response with the HTTP status code 409.  This response indicates that a user or a group already exisits with the same name. This can be avoided by identifying and removing the conflicting user from Contoso via the Contoso administrative user interface, or removing the current user from the scope of provisioning either by removing their assignment to the Contoso application in Azure Active Directory or adding a scoping filter to exclude the user.",
                "additionalDetails": null,
                "errorCategory": "nonServiceFailure",
                "recommendedAction": null
            },
            "provisioningStatusInfo": {                
                "status": "failure",
                "errorInformation" : {
                    "errorCode": "ContosoEntryConflict",
                    "reason": "Message: Contoso returned an error response with the HTTP status code 409.  This response indicates that a user or a group already exisits with the same name. This can be avoided by identifying and removing the conflicting user from Contoso via the Contoso administrative user interface, or removing the current user from the scope of provisioning either by removing their assignment to the Contoso application in Azure Active Directory or adding a scoping filter to exclude the user.",
                    "additionalDetails": null,
                    "errorCategory": "nonServiceFailure",
                    "recommendedAction": null
                }
            },
            "provisioningSteps": [
                {
                    "name": "EntryImportAdd",
                    "provisioningStepType": "import",
                    "status": "success",
                    "description": "Received Group 'Self-service Pilot' change of type (Add) from Azure Active Directory",
                    "details": {}
                },
                {
                    "name": "EntrySynchronizationAdd",
                    "provisioningStepType": "matching",
                    "status": "success",
                    "description": "Group 'Self-service Pilot' will be created in Contoso (Group is active and assigned in Azure Active Directory, but no matching Group was found in Contoso)",
                    "details": {}
                },
                {
                    "name": "EntryExportAdd",
                    "provisioningStepType": "export",
                    "status": "failure",
                    "description": "Failed to create Group 'Self-service Pilot' in Contoso",
                    "details": {
                        "ReportableIdentifier": "Self-service Pilot"
                    }
                }
            ],
            "modifiedProperties": [
                {
                    "displayName": "objectId",
                    "oldValue": null,
                    "newValue": "5e0c9eae-ad3d-4139-5ad0-174391d110eb"
                },
                {
                    "displayName": "displayName",
                    "oldValue": null,
                    "newValue": "Self-service Pilot"
                },
                {
                    "displayName": "mailEnabled",
                    "oldValue": null,
                    "newValue": "False"
                },
                {
                    "displayName": "mailNickname",
                    "oldValue": null,
                    "newValue": "5ce25n9a-4c5f-45c9-8362-ef3da29c66c5"
                },
                {
                    "displayName": "securityEnabled",
                    "oldValue": null,
                    "newValue": "True"
                },
                {
                    "displayName": "Name",
                    "oldValue": null,
                    "newValue": "Self-service Pilot"
                }
            ]
       }
    ]
}

```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get provisioningObjectSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


