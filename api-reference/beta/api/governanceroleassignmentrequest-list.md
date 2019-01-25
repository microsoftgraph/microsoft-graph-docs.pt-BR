---
title: Lista governanceRoleAssignmentRequests
description: 'Recupere uma coleção de governanceRoleAssignmentRequests. '
localization_priority: Normal
ms.openlocfilehash: 5ad26ef352eae93e9c804cfb62f5d00df12e32ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515458"
---
# <a name="list-governanceroleassignmentrequests"></a><span data-ttu-id="f8722-103">Lista governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="f8722-103">List governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8722-104">Recupere uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="f8722-104">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="f8722-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8722-105">Permissions</span></span>
<span data-ttu-id="f8722-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8722-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8722-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8722-108">Permission type</span></span>      | <span data-ttu-id="f8722-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8722-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8722-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8722-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f8722-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f8722-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f8722-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8722-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8722-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8722-113">Not supported.</span></span>    |
|<span data-ttu-id="f8722-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8722-114">Application</span></span> | <span data-ttu-id="f8722-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f8722-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8722-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8722-116">HTTP request</span></span>
<span data-ttu-id="f8722-117"><!-- { "blockType": "ignored" } -->Uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) em um recurso de lista.</span><span class="sxs-lookup"><span data-stu-id="f8722-117"><!-- { "blockType": "ignored" } --> List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource.</span></span>
    
><span data-ttu-id="f8722-118">**Observação:** Além do escopo de permissão, a solicitação exige o solicitante ter pelo menos uma atribuição no recurso.</span><span class="sxs-lookup"><span data-stu-id="f8722-118">**Note:** Besides the permission scope, the request requires the requestor to have at least one role assignment on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignmentRequests
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="f8722-119">Uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) dos meus de lista.</span><span class="sxs-lookup"><span data-stu-id="f8722-119">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=subjectId+eq+'{myId}'
```

<span data-ttu-id="f8722-120">Uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) que são as decisões de administrador pendentes de lista.</span><span class="sxs-lookup"><span data-stu-id="f8722-120">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are pending administrator decisions.</span></span>
    
><span data-ttu-id="f8722-121">**Observação:** Além do escopo de permissão, esta solicitação requer o solicitante ter pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="f8722-121">**Note:** Besides the permission scope, this request requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=status/subStatus+eq+'PendingAdminDecision'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8722-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f8722-122">Optional query parameters</span></span>
<span data-ttu-id="f8722-123">Este método oferece suporte para os [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f8722-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8722-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8722-124">Request headers</span></span>
| <span data-ttu-id="f8722-125">Nome</span><span class="sxs-lookup"><span data-stu-id="f8722-125">Name</span></span>      |<span data-ttu-id="f8722-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8722-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f8722-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8722-127">Authorization</span></span>  | <span data-ttu-id="f8722-128">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f8722-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8722-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8722-129">Request body</span></span>
<span data-ttu-id="f8722-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8722-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8722-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8722-131">Response</span></span>
<span data-ttu-id="f8722-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8722-132">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8722-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8722-133">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequests"
}-->
<span data-ttu-id="f8722-134">Os administradores de solicitações de atribuição de função pendente para assinatura Wingtip Toys - produção de consulta.</span><span class="sxs-lookup"><span data-stu-id="f8722-134">Administrators query pending role assignment requests for subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="f8722-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8722-135">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="f8722-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8722-136">Response</span></span>
<span data-ttu-id="f8722-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8722-137">Here is an example of the response.</span></span> 

><span data-ttu-id="f8722-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8722-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests",
    "value": [
        {
            "id": "d75c65d8-9e66-44ff-b1cd-1ab0947fde1d",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": "",
            "type": "UserRemove",
            "assignmentState": "Active",
            "requestedDateTime": "2018-01-09T23:41:34.367Z",
            "reason": "Deactivation request",
            "schedule": null,
            "status": {
                "status": "Closed",
                "subStatus": "Revoked",
                "statusDetails": []
            }
        },
        {
            "id": "38f42071-3e81-4191-8c0b-11450fb6b547",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": "",
            "type": "UserAdd",
            "assignmentState": "Active",
            "requestedDateTime": "2018-01-10T20:58:09.163Z",
            "reason": "test activations",
            "status": {
                "status": "Closed",
                "subStatus": "Provisioned",
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
                "startDateTime": "2018-01-10T20:58:11.363914Z",
                "endDateTime": "0001-01-01T00:00:00Z",
                "duration": "PT5H"
            }
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
  "description": "List governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
