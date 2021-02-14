---
title: 'synchronizationJob: provisionOnDemand'
description: Selecione um usuário e provisione a conta sob demanda.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 3e1007dfd7bce9ff64f54651104de943348c10dc
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240560"
---
# <a name="synchronizationjob-provisionondemand"></a><span data-ttu-id="3d72e-103">synchronizationJob: provisionOnDemand</span><span class="sxs-lookup"><span data-stu-id="3d72e-103">synchronizationJob: provisionOnDemand</span></span>

<span data-ttu-id="3d72e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d72e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3d72e-105">Selecione um usuário e provisione a conta sob demanda.</span><span class="sxs-lookup"><span data-stu-id="3d72e-105">Select a user and provision the account on-demand.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d72e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d72e-106">Permissions</span></span>
<span data-ttu-id="3d72e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d72e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d72e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d72e-109">Permission type</span></span>                        | <span data-ttu-id="3d72e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d72e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d72e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d72e-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="3d72e-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d72e-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3d72e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d72e-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3d72e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d72e-114">Not supported.</span></span> |
|<span data-ttu-id="3d72e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d72e-115">Application</span></span>                            |<span data-ttu-id="3d72e-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d72e-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d72e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d72e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /servicePrincipals/{servicePrincipalsId}/synchronization/jobs/{synchronizationJobId}/provisionOnDemand
```

## <a name="request-headers"></a><span data-ttu-id="3d72e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d72e-118">Request headers</span></span>
|<span data-ttu-id="3d72e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3d72e-119">Name</span></span>|<span data-ttu-id="3d72e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d72e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3d72e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d72e-121">Authorization</span></span>|<span data-ttu-id="3d72e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d72e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3d72e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3d72e-124">Content-Type</span></span>|<span data-ttu-id="3d72e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d72e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d72e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d72e-127">Request body</span></span>
<span data-ttu-id="3d72e-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3d72e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3d72e-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3d72e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3d72e-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3d72e-130">Parameter</span></span>|<span data-ttu-id="3d72e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d72e-131">Type</span></span>|<span data-ttu-id="3d72e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d72e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d72e-133">parameters</span><span class="sxs-lookup"><span data-stu-id="3d72e-133">parameters</span></span>|<span data-ttu-id="3d72e-134">[Coleção synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md)</span><span class="sxs-lookup"><span data-stu-id="3d72e-134">[synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md) collection</span></span>|<span data-ttu-id="3d72e-135">Representa os objetos que serão provisionados e as regras de sincronização executadas.</span><span class="sxs-lookup"><span data-stu-id="3d72e-135">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="3d72e-136">O recurso é usado principalmente para provisionamento sob demanda.</span><span class="sxs-lookup"><span data-stu-id="3d72e-136">The resource is primarily used for on-demand provisioning.</span></span> |



## <a name="response"></a><span data-ttu-id="3d72e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d72e-137">Response</span></span>

<span data-ttu-id="3d72e-138">Se bem-sucedido, este método retorna `200 OK` um código de resposta e uma cadeia de caracteresKeyStringValuePair.</span><span class="sxs-lookup"><span data-stu-id="3d72e-138">If successful, this method returns a `200 OK` response code and a stringKeyStringValuePair.</span></span>

## <a name="examples"></a><span data-ttu-id="3d72e-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3d72e-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3d72e-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d72e-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3d72e-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d72e-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_provisionondemand"
}
-->
``` http
POST https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalsId}/synchronization/jobs/{synchronizationJobId}/provisionOnDemand
Content-Type: application/json
Content-length: 122

{
    "parameters": [{
      "subjects": [{
          "objectId": "9bb0f679-a883-4a6f-8260-35b491b8b8c8",
          "objectTypeName": "User"
      }],
      "ruleId": "ea807875-5618-4f0a-9125-0b46a05298ca"
    }]
  }
```
# <a name="javascript"></a>[<span data-ttu-id="3d72e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d72e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-provisionondemand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="3d72e-143">C#</span><span class="sxs-lookup"><span data-stu-id="3d72e-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-provisionondemand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d72e-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d72e-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-provisionondemand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3d72e-145">Java</span><span class="sxs-lookup"><span data-stu-id="3d72e-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-provisionondemand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3d72e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d72e-146">Response</span></span>
<span data-ttu-id="3d72e-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3d72e-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
}
-->
```
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.stringKeyStringValuePair",
    "key": "{\"result\":\"Skipped\",\"details\":{\"errorCode\":\"RedundantExport\",\"errorMessage\":\"The state of the user in both the source and target systems already match.\"}}",
    "value": "{\"action\":\"Other\",\"changeId\":\"g8ba3be8-1d7f-4a60-ae31-a8980da0a389\",\"endTime\":\"2020-06-26T13:58:24.7682084Z\",\"modifiedProperties\":[{\"displayName\":\"objectId\",\"oldValue\":null,\"newValue\":\"52cf7b7a-52be-4a9b-9c69-e4d4a4a14f76\"},{\"displayName\":\"accountEnabled\",\"oldValue\":null,\"newValue\":\"True\"},{\"displayName\":\"displayName\",\"oldValue\":null,\"newValue\":\"Bill Bob\"},{\"displayName\":\"mailNickname\",\"oldValue\":null,\"newValue\":\"Bill\"},{\"displayName\":\"userPrincipalName\",\"oldValue\":null,\"newValue\":\"BillBob@scimreftest.onmicrosoft.com\"},{\"displayName\":\"IsSoftDeleted\",\"oldValue\":null,\"newValue\":\"False\"},{\"displayName\":\"appRoleAssignments\",\"oldValue\":null,\"newValue\":\"User\"}],\"provisioningSteps\":[{\"name\":\"EntryImport\",\"type\":\"Import\",\"status\":\"Success\",\"description\":\"Retrieved User 'BillBob@scimreftest.onmicrosoft.com' from Azure Active Directory\",\"timestamp\":\"2020-06-26T13:58:24.5494971Z\",\"details\":{\"objectId\":\"52cf7b7a-52be-4a9b-9c69-e4d4a4a14f76\",\"accountEnabled\":\"True\",\"displayName\":\"Fill Bob\",\"mailNickname\":\"Bill\",\"userPrincipalName\":\"BillBob@scimreftest.onmicrosoft.com\",\"IsSoftDeleted\":\"False\",\"appRoleAssignments\":\"User\"}},{\"name\":\"EntryImport\",\"type\":\"Matching\",\"status\":\"Success\",\"description\":\"Retrieved  'BillBob@scimreftest.onmicrosoft.com' from customappsso\",\"timestamp\":\"2020-06-26T13:58:24.7214072Z\",\"details\":{\"active\":\"True\",\"displayName\":\"Bill Bob\",\"externalId\":\"Bill\",\"id\":\"52507a19-96ec-4e73-9250-3e65ffd2d926\",\"userName\":\"BillBob@scimreftest.onmicrosoft.com\"}},{\"name\":\"EntrySynchronizationScoping\",\"type\":\"Scoping\",\"status\":\"Success\",\"description\":\"Determine if User in scope by evaluating against each scoping filter\",\"timestamp\":\"2020-06-26T13:58:24.7526181Z\",\"details\":{\"IsActive\":\"True\",\"Assigned\":\"True\",\"IsEffectivelyEntitledForProvisioning\":\"True\",\"IsInProvisioningScopeDisplayName\":\"True\",\"ScopeEvaluationResult\":\"{}\"}},{\"name\":\"EntrySynchronizationSkip\",\"type\":\"Export\",\"status\":\"Skipped\",\"description\":\"The state of the user in both the source and target systems already match. No change to the User 'BillBob@scimreftest.onmicrosoft.com' currently needs to be made.\",\"timestamp\":\"2020-06-26T13:58:24.7682084Z\",\"details\":{\"SkipReason\":\"RedundantExport\"}}],\"reportableIdentifier\":\"BillBob@scimreftest.onmicrosoft.com\",\"startTime\":\"2020-06-26T13:58:24.5494971Z\",\"statusInfo\":{\"status\":\"Skipped\",\"errorCode\":null,\"reason\":null,\"additionalDetails\":null,\"errorCategory\":null,\"recommendedAction\":null},\"sourceIdentity\":{\"id\":\"62cf7b7a-52be-4a9b-9c69-e5d4a4a14f67\",\"type\":\"User\",\"displayName\":null,\"details\":null},\"sourceSystem\":{\"id\":null,\"name\":\"Azure Active Directory\",\"details\":null},\"targetIdentity\":{\"id\":\"52507a19-96ec-4e73-9250-3e65ffd2d926\",\"type\":\"urn:ietf:params:scim:schemas:extension:enterprise:2.0:User\",\"displayName\":null,\"details\":null},\"targetSystem\":{\"id\":null,\"name\":\"customappsso\",\"details\":null}}"
}
```
