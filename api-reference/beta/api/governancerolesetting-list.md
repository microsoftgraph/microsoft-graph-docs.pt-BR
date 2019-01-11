---
title: Lista governanceRoleSettings
description: Recupere uma coleção de governanceRoleSettings em um recurso.
localization_priority: Normal
ms.openlocfilehash: b0b076ed2b63eab8916567f6aef1cb61046dbc91
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853653"
---
# <a name="list-governancerolesettings"></a><span data-ttu-id="33dd0-103">Lista governanceRoleSettings</span><span class="sxs-lookup"><span data-stu-id="33dd0-103">List governanceRoleSettings</span></span>

> <span data-ttu-id="33dd0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="33dd0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33dd0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="33dd0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33dd0-106">Recupere uma coleção de [governanceRoleSettings](../resources/governancerolesetting.md) em um recurso.</span><span class="sxs-lookup"><span data-stu-id="33dd0-106">Retrieve a collection of [governanceRoleSettings](../resources/governancerolesetting.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="33dd0-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="33dd0-107">Permissions</span></span>
<span data-ttu-id="33dd0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33dd0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33dd0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33dd0-110">Permission type</span></span>      | <span data-ttu-id="33dd0-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="33dd0-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33dd0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33dd0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="33dd0-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="33dd0-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="33dd0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33dd0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33dd0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33dd0-115">Not supported.</span></span>    |
|<span data-ttu-id="33dd0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33dd0-116">Application</span></span> | <span data-ttu-id="33dd0-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="33dd0-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="33dd0-118">Além do escopo de permissão, essa API requer o solicitante ter pelo menos uma atribuição no recurso.</span><span class="sxs-lookup"><span data-stu-id="33dd0-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>
## <a name="http-request"></a><span data-ttu-id="33dd0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33dd0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/<resourceId>/roleSettings
GET /privilegedAccess/azureResources/roleSettings?$filter=resourceId+eq+'<resourceId>'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="33dd0-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="33dd0-120">Optional query parameters</span></span>
<span data-ttu-id="33dd0-121">Este método oferece suporte para os [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="33dd0-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33dd0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33dd0-122">Request headers</span></span>
| <span data-ttu-id="33dd0-123">Nome</span><span class="sxs-lookup"><span data-stu-id="33dd0-123">Name</span></span>      |<span data-ttu-id="33dd0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="33dd0-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="33dd0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="33dd0-125">Authorization</span></span>  | <span data-ttu-id="33dd0-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="33dd0-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="33dd0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33dd0-127">Request body</span></span>
<span data-ttu-id="33dd0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="33dd0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33dd0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="33dd0-129">Response</span></span>
<span data-ttu-id="33dd0-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [governanceRoleSetting](../resources/governancerolesetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33dd0-130">If successful, this method returns a `200 OK` response code and collection of [governanceRoleSetting](../resources/governancerolesetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33dd0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33dd0-131">Example</span></span>
<span data-ttu-id="33dd0-132">Este exemplo mostra como um administrador lista as configurações de função para o recurso Wingtip Toys - produção.</span><span class="sxs-lookup"><span data-stu-id="33dd0-132">This example shows how an administrator lists role settings for the resource Wingtip Toys - Prod.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_governancerolesettings"
}-->
##### <a name="request"></a><span data-ttu-id="33dd0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33dd0-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleSettings
```
##### <a name="response"></a><span data-ttu-id="33dd0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="33dd0-134">Response</span></span>
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
        },
        {
            "id": "ac642250-9c22-4ec5-a072-02e06c1ef3a0",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "688de08e-66d4-4efe-b234-1cf476a603b9",
            "isDefault": false,
            "lastUpdatedDateTime": "2017-12-07T18:12:43.417Z",
            "lastUpdatedBy": "Debashis Choudhury",
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
                    "setting": "{\"Enabled\":true,\"Approvers\":[{\"Id\":\"c178dfee-7236-44b5-a363-e15fc63d91f0\",\"Type\":\"User\",\"DisplayName\":\"Debashis Choudhury\",\"Email\":\"debac@fimdev.net\"}],\"BusinessFlowId\":\"fa7d0b98-ed15-47cd-b3e2-aa6bd3e6533a\"}"
                }
            ]
        },
        ...
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List governanceRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
