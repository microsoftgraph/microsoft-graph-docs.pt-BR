---
title: Obter governanceRoleSetting
description: Recupere as propriedades e relacionamentos de um governanceRoleSetting.
ms.openlocfilehash: 2b0a54fc31ec18816e32bfa2377ddcc0974ac09d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038046"
---
# <a name="get-governancerolesetting"></a><span data-ttu-id="49288-103">Obter governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="49288-103">Get governanceRoleSetting</span></span>


> <span data-ttu-id="49288-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="49288-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49288-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="49288-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49288-106">Recupere as propriedades e relacionamentos de um [governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="49288-106">Retrieve the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="49288-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="49288-107">Permissions</span></span>
<span data-ttu-id="49288-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49288-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49288-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49288-110">Permission type</span></span>      | <span data-ttu-id="49288-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="49288-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49288-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49288-112">Delegated (work or school account)</span></span> | <span data-ttu-id="49288-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="49288-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="49288-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49288-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49288-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49288-115">Not supported.</span></span>    |
|<span data-ttu-id="49288-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49288-116">Application</span></span> | <span data-ttu-id="49288-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="49288-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="49288-118">Além do escopo de permissão, essa API requer o solicitante ter pelo menos uma atribuição do recurso, que pertence a [governanceRoleSetting](../resources/governancerolesetting.md) .</span><span class="sxs-lookup"><span data-stu-id="49288-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleSetting](../resources/governancerolesetting.md) belongs to.</span></span>
## <a name="http-request"></a><span data-ttu-id="49288-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49288-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="49288-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="49288-120">Optional query parameters</span></span>
<span data-ttu-id="49288-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="49288-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49288-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49288-122">Request headers</span></span>
| <span data-ttu-id="49288-123">Nome</span><span class="sxs-lookup"><span data-stu-id="49288-123">Name</span></span>      |<span data-ttu-id="49288-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="49288-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49288-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="49288-125">Authorization</span></span>  | <span data-ttu-id="49288-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="49288-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="49288-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49288-127">Request body</span></span>
<span data-ttu-id="49288-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="49288-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="49288-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="49288-129">Response</span></span>
<span data-ttu-id="49288-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [governanceRoleSetting](../resources/governancerolesetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49288-130">If successful, this method returns a `200 OK` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="49288-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49288-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49288-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49288-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9
```
##### <a name="response"></a><span data-ttu-id="49288-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="49288-133">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
