---
title: Listar governançaRoleSettings
description: Recupere uma coleção de governanceRoleSettings em um recurso.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 89241c003ca538da0c368bb75d9ae239ba779b07
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350660"
---
# <a name="list-governancerolesettings"></a><span data-ttu-id="afb54-103">Listar governançaRoleSettings</span><span class="sxs-lookup"><span data-stu-id="afb54-103">List governanceRoleSettings</span></span>

<span data-ttu-id="afb54-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afb54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afb54-105">Recupere uma coleção de [governanceRoleSettings](../resources/governancerolesetting.md) em um recurso.</span><span class="sxs-lookup"><span data-stu-id="afb54-105">Retrieve a collection of [governanceRoleSettings](../resources/governancerolesetting.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="afb54-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="afb54-106">Permissions</span></span>
<span data-ttu-id="afb54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="afb54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="afb54-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="afb54-109">Azure resources</span></span>

| <span data-ttu-id="afb54-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afb54-110">Permission type</span></span> | <span data-ttu-id="afb54-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="afb54-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="afb54-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afb54-112">Delegated (work or school account)</span></span> | <span data-ttu-id="afb54-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="afb54-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="afb54-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afb54-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afb54-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afb54-115">Not supported.</span></span> |
| <span data-ttu-id="afb54-116">Application</span><span class="sxs-lookup"><span data-stu-id="afb54-116">Application</span></span> | <span data-ttu-id="afb54-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="afb54-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="afb54-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="afb54-118">Azure AD</span></span>

| <span data-ttu-id="afb54-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afb54-119">Permission type</span></span> | <span data-ttu-id="afb54-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="afb54-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="afb54-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afb54-121">Delegated (work or school account)</span></span> | <span data-ttu-id="afb54-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="afb54-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="afb54-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afb54-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afb54-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afb54-124">Not supported.</span></span> |
| <span data-ttu-id="afb54-125">Application</span><span class="sxs-lookup"><span data-stu-id="afb54-125">Application</span></span> | <span data-ttu-id="afb54-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="afb54-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="afb54-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="afb54-127">Groups</span></span>

|<span data-ttu-id="afb54-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afb54-128">Permission type</span></span> | <span data-ttu-id="afb54-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="afb54-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="afb54-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afb54-130">Delegated (work or school account)</span></span> | <span data-ttu-id="afb54-131">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="afb54-131">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="afb54-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afb54-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afb54-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afb54-133">Not supported.</span></span> |
| <span data-ttu-id="afb54-134">Application</span><span class="sxs-lookup"><span data-stu-id="afb54-134">Application</span></span> | <span data-ttu-id="afb54-135">PrivilegedAccess.Read.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="afb54-135">PrivilegedAccess.Read.AzureADGroup</span></span> |

<span data-ttu-id="afb54-136">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="afb54-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>
## <a name="http-request"></a><span data-ttu-id="afb54-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afb54-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/<resourceId>/roleSettings
GET /privilegedAccess/azureResources/roleSettings?$filter=resourceId+eq+'<resourceId>'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="afb54-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="afb54-138">Optional query parameters</span></span>
<span data-ttu-id="afb54-139">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="afb54-139">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="afb54-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afb54-140">Request headers</span></span>
| <span data-ttu-id="afb54-141">Nome</span><span class="sxs-lookup"><span data-stu-id="afb54-141">Name</span></span>      |<span data-ttu-id="afb54-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="afb54-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="afb54-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="afb54-143">Authorization</span></span>  | <span data-ttu-id="afb54-144">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="afb54-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="afb54-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afb54-145">Request body</span></span>
<span data-ttu-id="afb54-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="afb54-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afb54-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="afb54-147">Response</span></span>
<span data-ttu-id="afb54-148">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos governanceRoleSetting](../resources/governancerolesetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="afb54-148">If successful, this method returns a `200 OK` response code and collection of [governanceRoleSetting](../resources/governancerolesetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afb54-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="afb54-149">Example</span></span>
<span data-ttu-id="afb54-150">Este exemplo mostra como um administrador lista configurações de função para o recurso Wingtip Toys - Prod.</span><span class="sxs-lookup"><span data-stu-id="afb54-150">This example shows how an administrator lists role settings for the resource Wingtip Toys - Prod.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_governancerolesettings"
}-->
##### <a name="request"></a><span data-ttu-id="afb54-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="afb54-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleSettings
```
##### <a name="response"></a><span data-ttu-id="afb54-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="afb54-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 463

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleSettings",
    "value": [
        {
            "id": "80dc5d6f-8d89-47b3-953f-01dc909ed3f9",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "5b8bea96-e9f6-4c63-a8e9-fb092c79f0a1",
            "isDefault": false,
            "lastUpdatedDateTime": "2018-03-26T21:21:43.113Z",
            "lastUpdatedBy": "Alex Wilber",
            "adminEligibleSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
                }
            ],
            "adminMemberSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":43200}"
                },
                {
                    "ruleIdentifier": "MfaRule",
                    "setting": "{\"mfaRequired\":false}"
                },
                {
                    "ruleIdentifier": "JustificationRule",
                    "setting": "{\"required\":true}"
                }
            ],
            "userEligibleSettings": [],
            "userMemberSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":480}"
                },
                {
                    "ruleIdentifier": "MfaRule",
                    "setting": "{\"mfaRequired\":false}"
                },
                {
                    "ruleIdentifier": "JustificationRule",
                    "setting": "{\"required\":true}"
                },
                {
                    "ruleIdentifier": "ApprovalRule",
                    "setting": "{\"Enabled\":true,\"Approvers\":[{\"Id\":\"20083cf1-b8d8-43be-9d37-96adfb09e619\",\"Type\":\"User\",\"DisplayName\":\"Alex Wilber\",\"Email\":\"AlexW@contoso.com\"},{\"Id\":\"d158e1b0-5080-4088-a1e7-9ca54f39eb53\",\"Type\":\"User\",\"DisplayName\":\"Alex Wilber\",\"Email\":\"AlexW@contoso.com\"}],\"BusinessFlowId\":\"8df9e93a-6ba9-4453-af43-07cb95435032\"}"
                }
            ]
        },
        {
            "id": "ac642250-9c22-4ec5-a072-02e06c1ef3a0",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "688de08e-66d4-4efe-b234-1cf476a603b9",
            "isDefault": false,
            "lastUpdatedDateTime": "2017-12-07T18:12:43.417Z",
            "lastUpdatedBy": "Allan Deyoung",
            "adminEligibleSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
                }
            ],
            "adminMemberSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":43200}"
                },
                {
                    "ruleIdentifier": "MfaRule",
                    "setting": "{\"mfaRequired\":false}"
                },
                {
                    "ruleIdentifier": "JustificationRule",
                    "setting": "{\"required\":true}"
                }
            ],
            "userEligibleSettings": [],
            "userMemberSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":480}"
                },
                {
                    "ruleIdentifier": "MfaRule",
                    "setting": "{\"mfaRequired\":false}"
                },
                {
                    "ruleIdentifier": "JustificationRule",
                    "setting": "{\"required\":true}"
                },
                {
                    "ruleIdentifier": "ApprovalRule",
                    "setting": "{\"Enabled\":true,\"Approvers\":[{\"Id\":\"c178dfee-7236-44b5-a363-e15fc63d91f0\",\"Type\":\"User\",\"DisplayName\":\"Allan Deyoung\",\"Email\":\"AllanD@contoso.com\"}],\"BusinessFlowId\":\"fa7d0b98-ed15-47cd-b3e2-aa6bd3e6533a\"}"
                }
            ]
        },
        ...
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


