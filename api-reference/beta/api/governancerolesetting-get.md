---
title: Obter governanceRoleSetting
description: Recupere as propriedades e os relacionamentos de um governanceRoleSetting.
localization_priority: Normal
ms.openlocfilehash: 2c432c0f680acd2411d57ab6e4b4a7af21f3350a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503076"
---
# <a name="get-governancerolesetting"></a><span data-ttu-id="f7fca-103">Obter governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="f7fca-103">Get governanceRoleSetting</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7fca-104">Recupere as propriedades e os relacionamentos de um [governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="f7fca-104">Retrieve the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f7fca-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7fca-105">Permissions</span></span>
<span data-ttu-id="f7fca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7fca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7fca-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7fca-108">Permission type</span></span>      | <span data-ttu-id="f7fca-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7fca-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7fca-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7fca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7fca-111">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="f7fca-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f7fca-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7fca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7fca-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7fca-113">Not supported.</span></span>    |
|<span data-ttu-id="f7fca-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7fca-114">Application</span></span> | <span data-ttu-id="f7fca-115">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="f7fca-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="f7fca-116">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso ao qual o [governanceRoleSetting](../resources/governancerolesetting.md) pertence.</span><span class="sxs-lookup"><span data-stu-id="f7fca-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleSetting](../resources/governancerolesetting.md) belongs to.</span></span>
## <a name="http-request"></a><span data-ttu-id="f7fca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7fca-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f7fca-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f7fca-118">Optional query parameters</span></span>
<span data-ttu-id="f7fca-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f7fca-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7fca-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7fca-120">Request headers</span></span>
| <span data-ttu-id="f7fca-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f7fca-121">Name</span></span>      |<span data-ttu-id="f7fca-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7fca-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f7fca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7fca-123">Authorization</span></span>  | <span data-ttu-id="f7fca-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f7fca-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7fca-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7fca-125">Request body</span></span>
<span data-ttu-id="f7fca-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7fca-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f7fca-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7fca-127">Response</span></span>
<span data-ttu-id="f7fca-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [governanceRoleSetting](../resources/governancerolesetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7fca-128">If successful, this method returns a `200 OK` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f7fca-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7fca-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7fca-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7fca-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9
```
##### <a name="response"></a><span data-ttu-id="f7fca-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7fca-131">Response</span></span>
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
    "Error: /api-reference/beta/api/governancerolesetting-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
