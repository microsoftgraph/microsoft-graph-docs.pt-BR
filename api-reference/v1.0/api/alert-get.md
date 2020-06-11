---
title: Obter alerta
description: " Recupere as propriedades e os relacionamentos de um objeto Alert."
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: fe9a0a6c8f4ad3549e51b3a8d534014d4f9d0c69
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44680574"
---
# <a name="get-alert"></a><span data-ttu-id="e1005-103">Obter alerta</span><span class="sxs-lookup"><span data-stu-id="e1005-103">Get alert</span></span>

<span data-ttu-id="e1005-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1005-104">Namespace: microsoft.graph</span></span>

 <span data-ttu-id="e1005-105">Recupere as propriedades e os relacionamentos de um objeto [Alert](../resources/alert.md) .</span><span class="sxs-lookup"><span data-stu-id="e1005-105">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1005-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1005-106">Permissions</span></span>

<span data-ttu-id="e1005-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1005-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1005-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1005-109">Permission type</span></span>      | <span data-ttu-id="e1005-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1005-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1005-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1005-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="e1005-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1005-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="e1005-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1005-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e1005-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1005-114">Not supported.</span></span>  |
|<span data-ttu-id="e1005-115">Application</span><span class="sxs-lookup"><span data-stu-id="e1005-115">Application</span></span> | <span data-ttu-id="e1005-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1005-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1005-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1005-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="e1005-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1005-118">Request headers</span></span>

| <span data-ttu-id="e1005-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e1005-119">Name</span></span>      |<span data-ttu-id="e1005-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1005-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e1005-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1005-121">Authorization</span></span>  | <span data-ttu-id="e1005-122">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="e1005-122">Bearer {code}.</span></span> <span data-ttu-id="e1005-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1005-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1005-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1005-124">Request body</span></span>

<span data-ttu-id="e1005-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1005-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1005-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1005-126">Response</span></span>

<span data-ttu-id="e1005-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **Alert** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1005-127">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="e1005-128">Se um código de status diferente de 2xx ou 404 for retornado de um provedor ou se um provedor expirar, a resposta será um código de status `206 Partial Content` com a resposta do provedor em um cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="e1005-128">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="e1005-129">Para obter mais informações, consulte as [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="e1005-129">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="e1005-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1005-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1005-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1005-131">Request</span></span>

<span data-ttu-id="e1005-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1005-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1005-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1005-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
```
# <a name="c"></a>[<span data-ttu-id="e1005-134">C#</span><span class="sxs-lookup"><span data-stu-id="e1005-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1005-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1005-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1005-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1005-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1005-137">Java</span><span class="sxs-lookup"><span data-stu-id="e1005-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-alert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e1005-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1005-138">Response</span></span>

<span data-ttu-id="e1005-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e1005-139">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "String",
  "assignedTo": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "category": "String",
  "closedDateTime": "String (timestamp)",
  "cloudAppStates": [
    {
      "destinationServiceIp": "String",
      "destinationServiceName": "String",
      "riskScore": "String"
    }
  ],
  "comments": ["String"],
  "confidence": 1024,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "detectionIds": ["String"],
  "eventDateTime": "String (timestamp)",
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "fileStates": [
    {
      "fileHash": {
        "hashType": "@odata.type: microsoft.graph.fileHashType",
        "hashValue": "String"
      },
      "name": "String",
      "path": "String",
      "riskScore": "String"
    }
  ],
  "hostStates": [
    {
      "fqdn": "String",
      "isAzureAadJoined": true,
      "isAzureAadRegistered": true,
      "isHybridAzureDomainJoined": true,
      "netBiosName": "String",
      "os": "String",
      "privateIpAddress": "String",
      "publicIpAddress": "String",
      "riskScore": "String"
    }
  ],
  "id": "String (identifier)",
  "incidentIds": ["String"],
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [
    {
      "category": "String",
      "family": "String",
      "name": "String",
      "severity": "String",
      "wasRunning": true
    }
  ],
  "networkConnections": [
    {
      "applicationName": "String",
      "destinationAddress": "String",
      "destinationDomain": "String",
      "destinationLocation": "String",
      "destinationPort": "String",
      "destinationUrl": "String",
      "direction": "@odata.type: microsoft.graph.connectionDirection",
      "domainRegisteredDateTime": "String (timestamp)",
      "localDnsName": "String",
      "natDestinationAddress": "String",
      "natDestinationPort": "String",
      "natSourceAddress": "String",
      "natSourcePort": "String",
      "protocol": "@odata.type: microsoft.graph.securityNetworkProtocol",
      "riskScore": "String",
      "sourceAddress": "String",
      "sourceLocation": "String",
      "sourcePort": "String",
      "status": "@odata.type: microsoft.graph.connectionStatus",
      "urlParameters": "String"
    }
  ],
  "processes": [
    {
      "accountName": "String",
      "commandLine": "String",
      "createdDateTime": "String (timestamp)",
      "fileHash": {
        "hashType": "@odata.type: microsoft.graph.fileHashType",
        "hashValue": "String"
      },
      "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
      "isElevated": true,
      "name": "String",
      "parentProcessCreatedDateTime": "String (timestamp)",
      "parentProcessId": 1024,
      "parentProcessName": "String",
      "path": "String",
      "processId": 1024
    }
  ],
  "recommendedActions": ["String"],
  "registryKeyStates": [
    {
      "hive": "@odata.type: microsoft.graph.registryHive",
      "key": "String",
      "oldKey": "String",
      "oldValueData": "String",
      "oldValueName": "String",
      "operation": "@odata.type: microsoft.graph.registryOperation",
      "processId": 1024,
      "valueData": "String",
      "valueName": "String",
      "valueType": "@odata.type: microsoft.graph.registryValueType"
    }
  ],
   "securityResources": [
    {
      "resource": "String",
      "resourceType": "@odata.type: microsoft.graph.securityResourceType"
    }
   ],
  "severity": "@odata.type: microsoft.graph.alertSeverity",
  "sourceMaterials": ["String"],
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "title": "String",
  "triggers": [
    {
      "name": "String",
      "type": "String",
      "value": "String"
    }
  ],
  "userStates": [
    {
      "aadUserId": "String",
      "accountName": "String",
      "domainName": "String",
      "emailRole": "@odata.type: microsoft.graph.emailRole",
      "isVpn": true,
      "logonDateTime": "String (timestamp)",
      "logonId": "String",
      "logonIp": "String",
      "logonLocation": "String",
      "logonType": "@odata.type: microsoft.graph.logonType",
      "onPremisesSecurityIdentifier": "String",
      "riskScore": "String",
      "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
      "userPrincipalName": "String"
    }
  ],
  "vendorInformation": {
    "provider": "String",
    "providerVersion": "String",
    "subProvider": "String",
    "vendor": "String"
  },
  "vulnerabilityStates": [
    {
      "cve": "String",
      "severity": "String",
      "wasRunning": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get glert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
