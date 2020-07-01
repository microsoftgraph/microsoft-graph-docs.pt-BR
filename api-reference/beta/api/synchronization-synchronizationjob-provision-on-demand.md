---
title: 'synchronizationJob: provisionOnDemand'
description: Selecione um usuário e provisione a conta sob demanda.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6b333350b335e431808caa74f65dc1f61601cddb
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007138"
---
# <a name="synchronizationjob-provisionondemand"></a><span data-ttu-id="676f0-103">synchronizationJob: provisionOnDemand</span><span class="sxs-lookup"><span data-stu-id="676f0-103">synchronizationJob: provisionOnDemand</span></span>

<span data-ttu-id="676f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="676f0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="676f0-105">Selecione um usuário e provisione a conta sob demanda.</span><span class="sxs-lookup"><span data-stu-id="676f0-105">Select a user and provision the account on-demand.</span></span>

## <a name="permissions"></a><span data-ttu-id="676f0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="676f0-106">Permissions</span></span>
<span data-ttu-id="676f0-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="676f0-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="676f0-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="676f0-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="676f0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="676f0-109">Permission type</span></span>                        | <span data-ttu-id="676f0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="676f0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="676f0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="676f0-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="676f0-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="676f0-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="676f0-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="676f0-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="676f0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="676f0-114">Not supported.</span></span> |
|<span data-ttu-id="676f0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="676f0-115">Application</span></span>                            |<span data-ttu-id="676f0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="676f0-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="676f0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="676f0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /servicePrincipals/{servicePrincipalsId}/synchronization/jobs/{synchronizationJobId}/provisionOnDemand
```

## <a name="request-headers"></a><span data-ttu-id="676f0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="676f0-118">Request headers</span></span>
|<span data-ttu-id="676f0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="676f0-119">Name</span></span>|<span data-ttu-id="676f0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="676f0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="676f0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="676f0-121">Authorization</span></span>|<span data-ttu-id="676f0-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="676f0-122">Bearer {token}.</span></span> <span data-ttu-id="676f0-123">Required.</span><span class="sxs-lookup"><span data-stu-id="676f0-123">Required.</span></span>|
|<span data-ttu-id="676f0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="676f0-124">Content-Type</span></span>|<span data-ttu-id="676f0-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="676f0-125">application/json.</span></span> <span data-ttu-id="676f0-126">Required.</span><span class="sxs-lookup"><span data-stu-id="676f0-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="676f0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="676f0-127">Request body</span></span>
<span data-ttu-id="676f0-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="676f0-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="676f0-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="676f0-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="676f0-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="676f0-130">Parameter</span></span>|<span data-ttu-id="676f0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="676f0-131">Type</span></span>|<span data-ttu-id="676f0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="676f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="676f0-133">parameters</span><span class="sxs-lookup"><span data-stu-id="676f0-133">parameters</span></span>|<span data-ttu-id="676f0-134">coleção [synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md)</span><span class="sxs-lookup"><span data-stu-id="676f0-134">[synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md) collection</span></span>|<span data-ttu-id="676f0-135">Representa os objetos que serão provisionados e as regras de sincronização executadas.</span><span class="sxs-lookup"><span data-stu-id="676f0-135">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="676f0-136">O recurso é usado principalmente para provisionamento sob demanda.</span><span class="sxs-lookup"><span data-stu-id="676f0-136">The resource is primarily used for on-demand provisioning.</span></span> |



## <a name="response"></a><span data-ttu-id="676f0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="676f0-137">Response</span></span>

<span data-ttu-id="676f0-138">Se tiver êxito, este método retornará um `200 OK` código de resposta e um stringKeyStringValuePair.</span><span class="sxs-lookup"><span data-stu-id="676f0-138">If successful, this method returns a `200 OK` response code and a stringKeyStringValuePair.</span></span>

## <a name="examples"></a><span data-ttu-id="676f0-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="676f0-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="676f0-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="676f0-140">Request</span></span>
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
    "parameters" [{
      "subjects": [{
          "objectId": "9bb0f679-a883-4a6f-8260-35b491b8b8c8",
          "objectType": "User"
      }],
      "ruleId": "ea807875-5618-4f0a-9125-0b46a05298ca"
    }]
  }
```


### <a name="response"></a><span data-ttu-id="676f0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="676f0-141">Response</span></span>
<span data-ttu-id="676f0-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="676f0-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
