---
title: Listar governanceRoleAssignmentRequests
description: 'Recupere uma coleção de governanceRoleAssignmentRequests. '
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identitiy-platform
ms.openlocfilehash: 5d69c81fcd9de1d69be69500c2b654351d68897a
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639811"
---
# <a name="list-governanceroleassignmentrequests"></a><span data-ttu-id="8c67c-103">Listar governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="8c67c-103">List governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="8c67c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c67c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c67c-105">Recupere uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="8c67c-105">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="8c67c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c67c-106">Permissions</span></span>
<span data-ttu-id="8c67c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c67c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c67c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c67c-109">Permission type</span></span>      | <span data-ttu-id="8c67c-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c67c-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c67c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c67c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8c67c-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8c67c-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="8c67c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c67c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c67c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c67c-114">Not supported.</span></span>    |
|<span data-ttu-id="8c67c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c67c-115">Application</span></span> | <span data-ttu-id="8c67c-116">PrivilegedAccess. Read. AzureResources</span><span class="sxs-lookup"><span data-stu-id="8c67c-116">PrivilegedAccess.Read.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c67c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c67c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="8c67c-118">Lista uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) em um recurso.</span><span class="sxs-lookup"><span data-stu-id="8c67c-118">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource.</span></span>
    
><span data-ttu-id="8c67c-119">**Observação:** Além do escopo de permissão, a solicitação exige que o solicitante tenha pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="8c67c-119">**Note:** Besides the permission scope, the request requires the requestor to have at least one role assignment on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignmentRequests
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="8c67c-120">Liste uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) de meus.</span><span class="sxs-lookup"><span data-stu-id="8c67c-120">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=subjectId+eq+'{myId}'
```

<span data-ttu-id="8c67c-121">Liste uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) que estão com decisões de administrador pendentes.</span><span class="sxs-lookup"><span data-stu-id="8c67c-121">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are pending administrator decisions.</span></span>
    
><span data-ttu-id="8c67c-122">**Observação:** Além do escopo de permissão, essa solicitação exige que o solicitante tenha pelo menos `Active` uma atribuição de função`owner` de `user access administrator`administrador (ou) no recurso.</span><span class="sxs-lookup"><span data-stu-id="8c67c-122">**Note:** Besides the permission scope, this request requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=status/subStatus+eq+'PendingAdminDecision'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c67c-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8c67c-123">Optional query parameters</span></span>
<span data-ttu-id="8c67c-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8c67c-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c67c-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c67c-125">Request headers</span></span>
| <span data-ttu-id="8c67c-126">Nome</span><span class="sxs-lookup"><span data-stu-id="8c67c-126">Name</span></span>      |<span data-ttu-id="8c67c-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c67c-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c67c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c67c-128">Authorization</span></span>  | <span data-ttu-id="8c67c-129">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="8c67c-129">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c67c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c67c-130">Request body</span></span>
<span data-ttu-id="8c67c-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8c67c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c67c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c67c-132">Response</span></span>
<span data-ttu-id="8c67c-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c67c-133">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c67c-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c67c-134">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequests"
}-->
<span data-ttu-id="8c67c-135">Administradores consultam solicitações pendentes de atribuição de função para a assinatura Wingtip Toys-prod.</span><span class="sxs-lookup"><span data-stu-id="8c67c-135">Administrators query pending role assignment requests for subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="8c67c-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c67c-136">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="8c67c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c67c-137">Response</span></span>
<span data-ttu-id="8c67c-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c67c-138">Here is an example of the response.</span></span> 

><span data-ttu-id="8c67c-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c67c-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
