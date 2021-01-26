---
title: Obter governanceRoleSetting
description: Recupere as propriedades e os relacionamentos de uma governanceRoleSetting.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 26fcb5363118f74665a7bf319f8ab65a4df10c50
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983367"
---
# <a name="get-governancerolesetting"></a><span data-ttu-id="41a32-103">Obter governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="41a32-103">Get governanceRoleSetting</span></span>

<span data-ttu-id="41a32-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41a32-104">Namespace: microsoft.graph</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41a32-105">Recupere as propriedades e os relacionamentos de uma [governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="41a32-105">Retrieve the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="41a32-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="41a32-106">Permissions</span></span>
<span data-ttu-id="41a32-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="41a32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="41a32-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="41a32-109">Azure resources</span></span>

| <span data-ttu-id="41a32-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41a32-110">Permission type</span></span> | <span data-ttu-id="41a32-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="41a32-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="41a32-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41a32-112">Delegated (work or school account)</span></span> | <span data-ttu-id="41a32-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="41a32-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="41a32-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41a32-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41a32-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41a32-115">Not supported.</span></span> |
| <span data-ttu-id="41a32-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41a32-116">Application</span></span> | <span data-ttu-id="41a32-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="41a32-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="41a32-118">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="41a32-118">Azure AD</span></span>

| <span data-ttu-id="41a32-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41a32-119">Permission type</span></span> | <span data-ttu-id="41a32-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="41a32-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="41a32-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41a32-121">Delegated (work or school account)</span></span> | <span data-ttu-id="41a32-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="41a32-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="41a32-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41a32-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41a32-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41a32-124">Not supported.</span></span> |
| <span data-ttu-id="41a32-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41a32-125">Application</span></span> | <span data-ttu-id="41a32-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="41a32-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="41a32-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="41a32-127">Groups</span></span>

|<span data-ttu-id="41a32-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41a32-128">Permission type</span></span> | <span data-ttu-id="41a32-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="41a32-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="41a32-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41a32-130">Delegated (work or school account)</span></span> | <span data-ttu-id="41a32-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="41a32-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="41a32-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41a32-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41a32-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41a32-133">Not supported.</span></span> |
| <span data-ttu-id="41a32-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41a32-134">Application</span></span> | <span data-ttu-id="41a32-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="41a32-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="41a32-136">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso, à qual a [governanceRoleSetting](../resources/governancerolesetting.md) pertence.</span><span class="sxs-lookup"><span data-stu-id="41a32-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleSetting](../resources/governancerolesetting.md) belongs to.</span></span>
## <a name="http-request"></a><span data-ttu-id="41a32-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41a32-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="41a32-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="41a32-138">Optional query parameters</span></span>
<span data-ttu-id="41a32-139">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="41a32-139">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41a32-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41a32-140">Request headers</span></span>
| <span data-ttu-id="41a32-141">Nome</span><span class="sxs-lookup"><span data-stu-id="41a32-141">Name</span></span>      |<span data-ttu-id="41a32-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="41a32-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="41a32-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="41a32-143">Authorization</span></span>  | <span data-ttu-id="41a32-144">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="41a32-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="41a32-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41a32-145">Request body</span></span>
<span data-ttu-id="41a32-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41a32-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="41a32-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="41a32-147">Response</span></span>
<span data-ttu-id="41a32-148">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [governanceRoleSetting](../resources/governancerolesetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41a32-148">If successful, this method returns a `200 OK` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="41a32-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41a32-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41a32-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41a32-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="41a32-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="41a32-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9
```
# <a name="c"></a>[<span data-ttu-id="41a32-152">C#</span><span class="sxs-lookup"><span data-stu-id="41a32-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41a32-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41a32-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41a32-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41a32-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41a32-155">Java</span><span class="sxs-lookup"><span data-stu-id="41a32-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-governancerolesetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="41a32-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="41a32-156">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 370

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleSettings/$entity",
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
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


