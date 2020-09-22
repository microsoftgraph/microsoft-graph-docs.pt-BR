---
title: Obter governanceRoleSetting
description: Recupere as propriedades e os relacionamentos de um governanceRoleSetting.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 619bc7e17d8f1d6501191a8d7f7fe4d50a60166e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991023"
---
# <a name="get-governancerolesetting"></a><span data-ttu-id="6b6a9-103">Obter governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="6b6a9-103">Get governanceRoleSetting</span></span>

<span data-ttu-id="6b6a9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b6a9-104">Namespace: microsoft.graph</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b6a9-105">Recupere as propriedades e os relacionamentos de um [governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="6b6a9-105">Retrieve the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6b6a9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b6a9-106">Permissions</span></span>
<span data-ttu-id="6b6a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b6a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b6a9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b6a9-109">Permission type</span></span>      | <span data-ttu-id="6b6a9-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b6a9-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b6a9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b6a9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b6a9-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6b6a9-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="6b6a9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b6a9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b6a9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b6a9-114">Not supported.</span></span>    |
|<span data-ttu-id="6b6a9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b6a9-115">Application</span></span> | <span data-ttu-id="6b6a9-116">PrivilegedAccess. Read. AzureResources</span><span class="sxs-lookup"><span data-stu-id="6b6a9-116">PrivilegedAccess.Read.AzureResources</span></span> |

<span data-ttu-id="6b6a9-117">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso ao qual o [governanceRoleSetting](../resources/governancerolesetting.md) pertence.</span><span class="sxs-lookup"><span data-stu-id="6b6a9-117">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleSetting](../resources/governancerolesetting.md) belongs to.</span></span>
## <a name="http-request"></a><span data-ttu-id="6b6a9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b6a9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6b6a9-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6b6a9-119">Optional query parameters</span></span>
<span data-ttu-id="6b6a9-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6b6a9-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b6a9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b6a9-121">Request headers</span></span>
| <span data-ttu-id="6b6a9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6b6a9-122">Name</span></span>      |<span data-ttu-id="6b6a9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b6a9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6b6a9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b6a9-124">Authorization</span></span>  | <span data-ttu-id="6b6a9-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="6b6a9-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b6a9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b6a9-126">Request body</span></span>
<span data-ttu-id="6b6a9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6b6a9-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6b6a9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b6a9-128">Response</span></span>
<span data-ttu-id="6b6a9-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [governanceRoleSetting](../resources/governancerolesetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b6a9-129">If successful, this method returns a `200 OK` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b6a9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b6a9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b6a9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b6a9-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6b6a9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b6a9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9
```
# <a name="c"></a>[<span data-ttu-id="6b6a9-133">C#</span><span class="sxs-lookup"><span data-stu-id="6b6a9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b6a9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b6a9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b6a9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b6a9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b6a9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b6a9-136">Response</span></span>
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
    "lastUpdatedBy": "Vishal Seri",
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
            "setting": "{\"Enabled\":true,\"Approvers\":[{\"Id\":\"20083cf1-b8d8-43be-9d37-96adfb09e619\",\"Type\":\"User\",\"DisplayName\":\"Vishal Seri\",\"Email\":\"viseri@fimdev.net\"},{\"Id\":\"d158e1b0-5080-4088-a1e7-9ca54f39eb53\",\"Type\":\"User\",\"DisplayName\":\"viseri\",\"Email\":\"viseri@microsoft.com\"}],\"BusinessFlowId\":\"8df9e93a-6ba9-4453-af43-07cb95435032\"}"
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


