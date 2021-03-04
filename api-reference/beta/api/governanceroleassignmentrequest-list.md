---
title: Listar governançaRoleAssignmentRequests
description: 'Recupere uma coleção de governanceRoleAssignmentRequests. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a084967a7d0daa20a71992dad102c6a0d46b302e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435865"
---
# <a name="list-governanceroleassignmentrequests"></a><span data-ttu-id="a0d02-103">Listar governançaRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="a0d02-103">List governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="a0d02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0d02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0d02-105">Recupere uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="a0d02-105">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a0d02-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0d02-106">Permissions</span></span>
<span data-ttu-id="a0d02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="a0d02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="a0d02-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="a0d02-109">Azure resources</span></span>

| <span data-ttu-id="a0d02-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0d02-110">Permission type</span></span> | <span data-ttu-id="a0d02-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0d02-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="a0d02-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0d02-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a0d02-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a0d02-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="a0d02-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0d02-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0d02-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0d02-115">Not supported.</span></span> |
| <span data-ttu-id="a0d02-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0d02-116">Application</span></span> | <span data-ttu-id="a0d02-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a0d02-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="a0d02-118">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a0d02-118">Azure AD</span></span>

| <span data-ttu-id="a0d02-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0d02-119">Permission type</span></span> | <span data-ttu-id="a0d02-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0d02-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="a0d02-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0d02-121">Delegated (work or school account)</span></span> | <span data-ttu-id="a0d02-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="a0d02-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="a0d02-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0d02-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0d02-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0d02-124">Not supported.</span></span> |
| <span data-ttu-id="a0d02-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0d02-125">Application</span></span> | <span data-ttu-id="a0d02-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="a0d02-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="a0d02-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="a0d02-127">Groups</span></span>

|<span data-ttu-id="a0d02-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0d02-128">Permission type</span></span> | <span data-ttu-id="a0d02-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0d02-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="a0d02-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0d02-130">Delegated (work or school account)</span></span> | <span data-ttu-id="a0d02-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="a0d02-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="a0d02-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0d02-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0d02-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0d02-133">Not supported.</span></span> |
| <span data-ttu-id="a0d02-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0d02-134">Application</span></span> | <span data-ttu-id="a0d02-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="a0d02-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0d02-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0d02-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a0d02-137">Listar uma coleção [de governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) em um recurso.</span><span class="sxs-lookup"><span data-stu-id="a0d02-137">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource.</span></span>
    
><span data-ttu-id="a0d02-138">**Observação:** Além do escopo de permissão, a solicitação exige que o solicitante tenha pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="a0d02-138">**Note:** Besides the permission scope, the request requires the requestor to have at least one role assignment on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignmentRequests
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="a0d02-139">Listar uma coleção [de governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) minha.</span><span class="sxs-lookup"><span data-stu-id="a0d02-139">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=subjectId+eq+'{myId}'
```

<span data-ttu-id="a0d02-140">Listar uma coleção [de governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) que estão pendentes de decisões de administrador.</span><span class="sxs-lookup"><span data-stu-id="a0d02-140">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are pending administrator decisions.</span></span>
    
><span data-ttu-id="a0d02-141">**Observação:** Além do escopo de permissão, essa solicitação exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` ( ou ) no `owner` `user access administrator` recurso.</span><span class="sxs-lookup"><span data-stu-id="a0d02-141">**Note:** Besides the permission scope, this request requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=status/subStatus+eq+'PendingAdminDecision'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0d02-142">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a0d02-142">Optional query parameters</span></span>
<span data-ttu-id="a0d02-143">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a0d02-143">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0d02-144">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0d02-144">Request headers</span></span>
| <span data-ttu-id="a0d02-145">Nome</span><span class="sxs-lookup"><span data-stu-id="a0d02-145">Name</span></span>      |<span data-ttu-id="a0d02-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0d02-146">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a0d02-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0d02-147">Authorization</span></span>  | <span data-ttu-id="a0d02-148">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a0d02-148">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0d02-149">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0d02-149">Request body</span></span>
<span data-ttu-id="a0d02-150">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0d02-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0d02-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0d02-151">Response</span></span>
<span data-ttu-id="a0d02-152">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0d02-152">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0d02-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0d02-153">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequests"
}-->
<span data-ttu-id="a0d02-154">Os administradores consultam solicitações pendentes de atribuição de função para a assinatura Wingtip Toys - Prod.</span><span class="sxs-lookup"><span data-stu-id="a0d02-154">Administrators query pending role assignment requests for subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="a0d02-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0d02-155">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="a0d02-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0d02-156">Response</span></span>
<span data-ttu-id="a0d02-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0d02-157">Here is an example of the response.</span></span> 

><span data-ttu-id="a0d02-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0d02-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


