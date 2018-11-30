---
title: Obter alerta
description: " Recupere as propriedades e relacionamentos de um objeto de alerta."
ms.openlocfilehash: b5e85fe33f4896714c4100c22a26417091d154ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006516"
---
# <a name="get-alert"></a><span data-ttu-id="a0886-103">Obter alerta</span><span class="sxs-lookup"><span data-stu-id="a0886-103">Get alert</span></span>

 <span data-ttu-id="a0886-104">Recupere as propriedades e relacionamentos de um objeto de [alerta](../resources/alert.md) .</span><span class="sxs-lookup"><span data-stu-id="a0886-104">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0886-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="a0886-105">Permissions</span></span>

<span data-ttu-id="a0886-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0886-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0886-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0886-108">Permission type</span></span>      | <span data-ttu-id="a0886-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0886-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0886-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0886-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a0886-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0886-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="a0886-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0886-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a0886-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0886-113">Not supported.</span></span>  |
|<span data-ttu-id="a0886-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0886-114">Application</span></span> | <span data-ttu-id="a0886-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0886-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0886-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0886-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="a0886-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0886-117">Request headers</span></span>

| <span data-ttu-id="a0886-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a0886-118">Name</span></span>      |<span data-ttu-id="a0886-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0886-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a0886-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0886-120">Authorization</span></span>  | <span data-ttu-id="a0886-p102">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0886-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0886-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0886-123">Request body</span></span>

<span data-ttu-id="a0886-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0886-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0886-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0886-125">Response</span></span>

<span data-ttu-id="a0886-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de **alerta** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0886-126">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="a0886-127">Se um código de status diferente 2xx ou 404 é retornado por um provedor ou se um provedor de tempo limite, a resposta será um `206 Partial Content` código de status com a resposta de provedores em um cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="a0886-127">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the providers response in a warning header.</span></span> <span data-ttu-id="a0886-128">Para obter mais informações, consulte [respostas de erros de API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="a0886-128">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="a0886-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0886-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0886-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0886-130">Request</span></span>

<span data-ttu-id="a0886-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0886-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
```

### <a name="response"></a><span data-ttu-id="a0886-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0886-132">Response</span></span>

<span data-ttu-id="a0886-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a0886-133">The following is an example of the response.</span></span>
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
  "tocPath": ""
}-->
