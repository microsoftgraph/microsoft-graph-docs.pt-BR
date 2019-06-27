---
title: Obter alerta
description: Recuperar as propriedades e os relacionamentos de um objeto Alert
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 22ea8d250c7e7b61260e0b2e5503850d251f669a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258566"
---
# <a name="get-alert"></a><span data-ttu-id="c07eb-103">Obter alerta</span><span class="sxs-lookup"><span data-stu-id="c07eb-103">Get alert</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c07eb-104">Recupere as propriedades e os relacionamentos de um objeto [Alert](../resources/alert.md) .</span><span class="sxs-lookup"><span data-stu-id="c07eb-104">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c07eb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c07eb-105">Permissions</span></span>

<span data-ttu-id="c07eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c07eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c07eb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c07eb-108">Permission type</span></span>      | <span data-ttu-id="c07eb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c07eb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c07eb-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c07eb-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c07eb-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c07eb-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="c07eb-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c07eb-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c07eb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c07eb-113">Not supported.</span></span>  |
|<span data-ttu-id="c07eb-114">Application</span><span class="sxs-lookup"><span data-stu-id="c07eb-114">Application</span></span> | <span data-ttu-id="c07eb-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c07eb-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c07eb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c07eb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c07eb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c07eb-117">Request headers</span></span>

| <span data-ttu-id="c07eb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c07eb-118">Name</span></span>      |<span data-ttu-id="c07eb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c07eb-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c07eb-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c07eb-120">Authorization</span></span>  | <span data-ttu-id="c07eb-121">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="c07eb-121">Bearer {code}.</span></span> <span data-ttu-id="c07eb-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c07eb-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c07eb-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c07eb-123">Request body</span></span>

<span data-ttu-id="c07eb-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c07eb-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c07eb-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c07eb-125">Response</span></span>

<span data-ttu-id="c07eb-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **Alert** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c07eb-126">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="c07eb-127">Se um código de status diferente de 2xx ou 404 for retornado de um provedor ou se um provedor expirar, a resposta será um código de status `206 Partial Content` com a resposta do provedor em um cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="c07eb-127">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="c07eb-128">Para obter mais informações, consulte as [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="c07eb-128">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="c07eb-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c07eb-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c07eb-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c07eb-130">Request</span></span>

<span data-ttu-id="c07eb-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c07eb-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts/{id}
```

### <a name="response"></a><span data-ttu-id="c07eb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c07eb-132">Response</span></span>

<span data-ttu-id="c07eb-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c07eb-133">The following is an example of the response.</span></span>
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
  "historyStates": [
    {
      "appId": "appId-value",
      "assignedTo": "assignedTo-value",
      "comments": [
        "comments-value"
      ],
      "feedback": "feedback-value",
      "status": "status-value",
      "updatedDateTime": "datetime-value",
      "user": "user-value"
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
      "protocol": "String",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c07eb-134">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="c07eb-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c07eb-135">C#</span><span class="sxs-lookup"><span data-stu-id="c07eb-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_alert-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c07eb-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="c07eb-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_alert-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c07eb-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c07eb-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_alert-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get glert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/alert-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/alert-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/alert-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
