---
title: Listar provisioningObjectSummary
description: Obter todos os eventos de provisionamento que ocorreram em seu locatário.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: abae4feb7f68097b828ac4989561c168c81b3491
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349335"
---
# <a name="list-provisioningobjectsummary"></a><span data-ttu-id="db42b-103">Listar provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="db42b-103">List provisioningObjectSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db42b-104">Obter todos os eventos de provisionamento que ocorreram em seu locatário, como a exclusão de um grupo em um aplicativo de destino ou a criação de um usuário ao provisionar contas de usuário do seu sistema de RH.</span><span class="sxs-lookup"><span data-stu-id="db42b-104">Get all provisioning events that occurred in your tenant, such as the deletion of a group in a target application or the creation of a user when provisioning user accounts from your HR system.</span></span> 

## <a name="permissions"></a><span data-ttu-id="db42b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="db42b-105">Permissions</span></span>

<span data-ttu-id="db42b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db42b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db42b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db42b-108">Permission type</span></span>      | <span data-ttu-id="db42b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db42b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db42b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db42b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db42b-111">AuditLog. Read. All e Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="db42b-111">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="db42b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db42b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db42b-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="db42b-113">Not supported</span></span>   |
|<span data-ttu-id="db42b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db42b-114">Application</span></span> | <span data-ttu-id="db42b-115">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="db42b-115">AuditLog.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db42b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db42b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /auditLogs/directoryProvisioning
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db42b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="db42b-117">Optional query parameters</span></span>

<span data-ttu-id="db42b-118">Este método dá suporte ao seguinte parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="db42b-118">This method supports the following OData query parameter to help customize the response.</span></span> <span data-ttu-id="db42b-119">Observe que os filtros são diferenciados entre maiúsculas e minúsculas, exceto o status.</span><span class="sxs-lookup"><span data-stu-id="db42b-119">Note that the filters are all case sensitive except for status.</span></span> 

|<span data-ttu-id="db42b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="db42b-120">Name</span></span>     |<span data-ttu-id="db42b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="db42b-121">Description</span></span>                            |<span data-ttu-id="db42b-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db42b-122">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="db42b-123">$filter</span><span class="sxs-lookup"><span data-stu-id="db42b-123">$filter</span></span>](/graph/query-parameters#filter-parameter)|<span data-ttu-id="db42b-124">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="db42b-124">Filters results (rows).</span></span> |/`auditLogs/directoryProvisioning?$filter=id eq '74c3b0ae-9cc5-850e-e0a5-7r6a4231de87'`

<span data-ttu-id="db42b-125">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="db42b-125">For general information, see [OData query parameters](/graph/query_parameters).</span></span>

### <a name="attributes-supported-by-the-filter-parameter"></a><span data-ttu-id="db42b-126">Atributos com suporte do parâmetro $filter</span><span class="sxs-lookup"><span data-stu-id="db42b-126">Attributes supported by the $filter parameter</span></span>

|<span data-ttu-id="db42b-127">Nome do atributo</span><span class="sxs-lookup"><span data-stu-id="db42b-127">Attribute name</span></span> |<span data-ttu-id="db42b-128">Operadores com suporte</span><span class="sxs-lookup"><span data-stu-id="db42b-128">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="db42b-129">id</span><span class="sxs-lookup"><span data-stu-id="db42b-129">id</span></span>| <span data-ttu-id="db42b-130">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-130">eq, contains</span></span>|
|<span data-ttu-id="db42b-131">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="db42b-131">activityDateTime</span></span>| <span data-ttu-id="db42b-132">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-132">eq, contains</span></span>|
|<span data-ttu-id="db42b-133">tenantid</span><span class="sxs-lookup"><span data-stu-id="db42b-133">tenantid</span></span>|<span data-ttu-id="db42b-134">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-134">eq, contains</span></span>|
|<span data-ttu-id="db42b-135">ID</span><span class="sxs-lookup"><span data-stu-id="db42b-135">jobid</span></span>|<span data-ttu-id="db42b-136">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-136">eq, contains</span></span>|
|<span data-ttu-id="db42b-137">ChangeId</span><span class="sxs-lookup"><span data-stu-id="db42b-137">changeid</span></span>|<span data-ttu-id="db42b-138">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-138">eq, contains</span></span>|
|<span data-ttu-id="db42b-139">cycleid</span><span class="sxs-lookup"><span data-stu-id="db42b-139">cycleid</span></span>|<span data-ttu-id="db42b-140">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-140">eq, contains</span></span>|
|<span data-ttu-id="db42b-141">ação</span><span class="sxs-lookup"><span data-stu-id="db42b-141">action</span></span>|<span data-ttu-id="db42b-142">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-142">eq, contains</span></span>|
|<span data-ttu-id="db42b-143">modifiedproperty/DisplayName</span><span class="sxs-lookup"><span data-stu-id="db42b-143">modifiedproperty/DisplayName</span></span>| <span data-ttu-id="db42b-144">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-144">eq, contains</span></span>|
|<span data-ttu-id="db42b-145">modifiedproperty/oldValue</span><span class="sxs-lookup"><span data-stu-id="db42b-145">modifiedproperty/oldValue</span></span>| <span data-ttu-id="db42b-146">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-146">eq, contains</span></span>|
|<span data-ttu-id="db42b-147">modifiedproperty/newValue</span><span class="sxs-lookup"><span data-stu-id="db42b-147">modifiedproperty/newValue</span></span>| <span data-ttu-id="db42b-148">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-148">eq, contains</span></span>|
|<span data-ttu-id="db42b-149">statusInfo/status</span><span class="sxs-lookup"><span data-stu-id="db42b-149">statusInfo/status</span></span>|<span data-ttu-id="db42b-150">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-150">eq, contains</span></span>|
|<span data-ttu-id="db42b-151">sourceSystem/displayName</span><span class="sxs-lookup"><span data-stu-id="db42b-151">sourceSystem/displayName</span></span>|<span data-ttu-id="db42b-152">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-152">eq, contains</span></span>|
|<span data-ttu-id="db42b-153">targetSystem/displayName</span><span class="sxs-lookup"><span data-stu-id="db42b-153">targetSystem/displayName</span></span>|<span data-ttu-id="db42b-154">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-154">eq, contains</span></span>|
|<span data-ttu-id="db42b-155">sourceIdentity/IdentityType</span><span class="sxs-lookup"><span data-stu-id="db42b-155">sourceIdentity/identityType</span></span>|<span data-ttu-id="db42b-156">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-156">eq, contains</span></span>|
|<span data-ttu-id="db42b-157">targetIdentity/IdentityType</span><span class="sxs-lookup"><span data-stu-id="db42b-157">targetIdentity/identityType</span></span>|<span data-ttu-id="db42b-158">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-158">eq, contains</span></span>|
|<span data-ttu-id="db42b-159">sourceIdentity/ID</span><span class="sxs-lookup"><span data-stu-id="db42b-159">sourceIdentity/id</span></span>|<span data-ttu-id="db42b-160">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-160">eq, contains</span></span>|
|<span data-ttu-id="db42b-161">targetIdentity/ID</span><span class="sxs-lookup"><span data-stu-id="db42b-161">targetIdentity/id</span></span>|<span data-ttu-id="db42b-162">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-162">eq, contains</span></span>|
|<span data-ttu-id="db42b-163">sourceIdentity/displayName</span><span class="sxs-lookup"><span data-stu-id="db42b-163">sourceIdentity/displayName</span></span>|<span data-ttu-id="db42b-164">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-164">eq, contains</span></span>|
|<span data-ttu-id="db42b-165">targetIdentity/displayName</span><span class="sxs-lookup"><span data-stu-id="db42b-165">targetIdentity/displayName</span></span>|<span data-ttu-id="db42b-166">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-166">eq, contains</span></span>|
|<span data-ttu-id="db42b-167">initiatedBy/displayName</span><span class="sxs-lookup"><span data-stu-id="db42b-167">initiatedBy/displayName</span></span>|<span data-ttu-id="db42b-168">EQ, contém</span><span class="sxs-lookup"><span data-stu-id="db42b-168">eq, contains</span></span>|

## <a name="request-headers"></a><span data-ttu-id="db42b-169">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db42b-169">Request headers</span></span>

| <span data-ttu-id="db42b-170">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db42b-170">Header</span></span>        | <span data-ttu-id="db42b-171">Valor</span><span class="sxs-lookup"><span data-stu-id="db42b-171">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="db42b-172">Autorização</span><span class="sxs-lookup"><span data-stu-id="db42b-172">Authorization</span></span> | <span data-ttu-id="db42b-173">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="db42b-173">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="db42b-174">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db42b-174">Request body</span></span>

<span data-ttu-id="db42b-175">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="db42b-175">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db42b-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="db42b-176">Response</span></span>

<span data-ttu-id="db42b-177">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [provisioningObjectSummary](../resources/provisioningobjectsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db42b-177">If successful, this method returns a `200 OK` response code and a collection of [provisioningObjectSummary](../resources/provisioningobjectsummary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db42b-178">Exemplos</span><span class="sxs-lookup"><span data-stu-id="db42b-178">Examples</span></span>

### <a name="example-1-successful-request"></a><span data-ttu-id="db42b-179">Exemplo 1: solicitação bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="db42b-179">Example 1: Successful request</span></span>

### <a name="request"></a><span data-ttu-id="db42b-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db42b-180">Request</span></span>

<span data-ttu-id="db42b-181">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db42b-181">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary"
} -->

```http
GET https://graph.microsoft.com/beta/auditLogs/directoryProvisioning
```

### <a name="response"></a><span data-ttu-id="db42b-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="db42b-182">Response</span></span>

<span data-ttu-id="db42b-183">Veja a seguir um exemplo da resposta para um evento bem-sucedido.</span><span class="sxs-lookup"><span data-stu-id="db42b-183">The following is an example of the response for a successful event.</span></span>

><span data-ttu-id="db42b-184">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="db42b-184">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="db42b-185">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db42b-185">All the properties will be returned from an actual call.</span></span>

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
    
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/directoryProvisioning",
    "value": [
         {
            "id": "75b5b0ae-9fc5-8d0e-e0a9-7y6a4728de56",
            "activityDateTime": "2019-05-04T03:00:54Z",
            "tenantId": "74beb175-3b80-7b63-b9d5-6f0b76082b16",
            "jobId": "aws.74beb1753b704b63b8d56f0b76082b16.10a7a801-7101-4c69-ae00-ce9f75f8460a",
            "cycleId": "b6502552-018d-79bd-8869-j47194dc65c1",
            "changeId": "b6502552-018d-89bd-9969-b49194dc65c1",
            "action": "EntryExportUpdate",
            "durationInMilliseconds": 3236,
            "statusInfo": {
                "status": "success"
            },
            "provisioningSteps": [
                {
                    "name": "EntryImport",
                    "provisioningStepType": "Import",
                    "status": "success",
                    "description": "Retrieved RolesCompound '10a7a801-7101-4c69-ae00-ce9f75f8460a' from Amazon Web Services",
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
                    "newValue": "Amazon Web Services (AWS)"
                },
                {
                    "displayName": "homepage",
                    "oldValue": null,
                    "newValue": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z"
                },
            ],
            "sourceSystem": {
                "id": "d1e090e1-f2f4-4678-be44-6442ffff0621",
                "displayName": "Amazon Web Services",
                "details": {}
            },
            "targetSystem": {
                "id": "e69d4bd2-2da2-483e-bc49-aad4080b91b3",
                "displayName": "Azure Active Directory",
                "details": {
                    "ApplicationId": "bcf4d658-ac9f-408d-bf04-e86dc10328fb",
                    "ServicePrincipalId": "6nn35b93-185a-4485-a519-50c09549f3ad",
                    "ServicePrincipalDisplayName": "Amazon Web Services (AWS)"
                }
            },
            "initiatedBy": {
                "initiatingType": "System",
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
### <a name="example-2-error-reponse"></a><span data-ttu-id="db42b-186">Exemplo 2: resposta de erro</span><span class="sxs-lookup"><span data-stu-id="db42b-186">Example 2: Error reponse</span></span>

### <a name="request"></a><span data-ttu-id="db42b-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db42b-187">Request</span></span>

<span data-ttu-id="db42b-188">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db42b-188">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary_error"
} -->

```http
GET https://graph.microsoft.com/beta/auditLogs/directoryProvisioning
```

### <a name="response"></a><span data-ttu-id="db42b-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="db42b-189">Response</span></span>

<span data-ttu-id="db42b-190">Veja a seguir um exemplo da resposta de um evento de provisionamento com falha.</span><span class="sxs-lookup"><span data-stu-id="db42b-190">The following is an example of the response for a failed provisioning event.</span></span>

><span data-ttu-id="db42b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db42b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/directoryProvisioning",
    "value": [
        {
            "id": "gc532ff9-r265-ec76-861e-42e2970a8218",
            "activityDateTime": "2019-06-24T20:53:08Z",
            "tenantId": "7928d5b5-7442-4a97-ne2d-66f9j9972ecn",
            "jobId": "BoxOutDelta.7928d5b574424a97ne2d66f9j9972ecn",
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
                "displayName": "Box",
                "details": {
                    "ApplicationId": "f2764360-e0ec-5676-711e-cd6fc0d4dd61",
                    "ServicePrincipalId": "chc46a42-966b-47d7-9774-576b1c8bd0b8",
                    "ServicePrincipalDisplayName": "Box"
                }
            },
            "initiatedBy": {
                "id": "",
                "displayName": "Azure AD Provisioning Service",
                "initiatorType": "system"
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
                "errorCode": "BoxEntryConflict",
                "reason": "Message: Box returned an error response with the HTTP status code 409.  This response indicates that a user or a group already exisits with the same name. This can be avoided by identifying and removing the conflicting user from Box via the Box administrative user interface, or removing the current user from the scope of provisioning either by removing their assignment to the Box application in Azure Active Directory or adding a scoping filter to exclude the user.",
                "additionalDetails": null,
                "errorCategory": "NonServiceFailure",
                "recommendedAction": null
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
                    "description": "Group 'Self-service Pilot' will be created in Box (Group is active and assigned in Azure Active Directory, but no matching Group was found in Box)",
                    "details": {}
                },
                {
                    "name": "EntryExportAdd",
                    "provisioningStepType": "export",
                    "status": "failure",
                    "description": "Failed to create Group 'Self-service Pilot' in Box",
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
