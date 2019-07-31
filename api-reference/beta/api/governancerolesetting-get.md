---
title: Obter governanceRoleSetting
description: Recupere as propriedades e os relacionamentos de um governanceRoleSetting.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 8e349ce3930a50a6ddb7863cd7d66a4385e7d46a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954138"
---
# <a name="get-governancerolesetting"></a><span data-ttu-id="6bb20-103">Obter governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="6bb20-103">Get governanceRoleSetting</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bb20-104">Recupere as propriedades e os relacionamentos de um [governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="6bb20-104">Retrieve the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6bb20-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6bb20-105">Permissions</span></span>
<span data-ttu-id="6bb20-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bb20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bb20-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bb20-108">Permission type</span></span>      | <span data-ttu-id="6bb20-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="6bb20-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6bb20-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bb20-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6bb20-111">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="6bb20-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="6bb20-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bb20-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bb20-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bb20-113">Not supported.</span></span>    |
|<span data-ttu-id="6bb20-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bb20-114">Application</span></span> | <span data-ttu-id="6bb20-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bb20-115">Not supported.</span></span> |

<span data-ttu-id="6bb20-116">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso ao qual o [governanceRoleSetting](../resources/governancerolesetting.md) pertence.</span><span class="sxs-lookup"><span data-stu-id="6bb20-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleSetting](../resources/governancerolesetting.md) belongs to.</span></span>
## <a name="http-request"></a><span data-ttu-id="6bb20-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bb20-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6bb20-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6bb20-118">Optional query parameters</span></span>
<span data-ttu-id="6bb20-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6bb20-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6bb20-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bb20-120">Request headers</span></span>
| <span data-ttu-id="6bb20-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6bb20-121">Name</span></span>      |<span data-ttu-id="6bb20-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bb20-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6bb20-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bb20-123">Authorization</span></span>  | <span data-ttu-id="6bb20-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="6bb20-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bb20-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bb20-125">Request body</span></span>
<span data-ttu-id="6bb20-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6bb20-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6bb20-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bb20-127">Response</span></span>
<span data-ttu-id="6bb20-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [governanceRoleSetting](../resources/governancerolesetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bb20-128">If successful, this method returns a `200 OK` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6bb20-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6bb20-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6bb20-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bb20-130">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6bb20-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6bb20-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6bb20-132">C#</span><span class="sxs-lookup"><span data-stu-id="6bb20-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6bb20-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="6bb20-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6bb20-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6bb20-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6bb20-135">Java</span><span class="sxs-lookup"><span data-stu-id="6bb20-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-governancerolesetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6bb20-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bb20-136">Response</span></span>
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
