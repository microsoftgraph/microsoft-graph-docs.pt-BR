---
title: Obter alerta
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: b8e3acbabab70c04f2dfa479b39f458950dfb6b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820241"
---
# <a name="get-alert"></a><span data-ttu-id="48436-104">Obter alerta</span><span class="sxs-lookup"><span data-stu-id="48436-104">Get alert</span></span>

 > <span data-ttu-id="48436-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="48436-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48436-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="48436-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48436-107">Recupere as propriedades e relacionamentos de um objeto de [alerta](../resources/alert.md) .</span><span class="sxs-lookup"><span data-stu-id="48436-107">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="48436-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="48436-108">Permissions</span></span>

<span data-ttu-id="48436-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48436-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48436-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48436-111">Permission type</span></span>      | <span data-ttu-id="48436-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48436-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48436-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48436-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="48436-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48436-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="48436-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48436-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="48436-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48436-116">Not supported.</span></span>  |
|<span data-ttu-id="48436-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48436-117">Application</span></span> | <span data-ttu-id="48436-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48436-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48436-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48436-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="48436-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48436-120">Request headers</span></span>

| <span data-ttu-id="48436-121">Nome</span><span class="sxs-lookup"><span data-stu-id="48436-121">Name</span></span>      |<span data-ttu-id="48436-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="48436-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="48436-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="48436-123">Authorization</span></span>  | <span data-ttu-id="48436-p104">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48436-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="48436-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48436-126">Request body</span></span>

<span data-ttu-id="48436-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="48436-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48436-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="48436-128">Response</span></span>

<span data-ttu-id="48436-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de **alerta** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48436-129">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="48436-130">Se um código de status diferente 2xx ou 404 é retornado por um provedor ou se um provedor de tempo limite, a resposta será um `206 Partial Content` código de status com a resposta do provedor em um cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="48436-130">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="48436-131">Para obter mais informações, consulte [respostas de erros de API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="48436-131">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="48436-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48436-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="48436-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48436-133">Request</span></span>

<span data-ttu-id="48436-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="48436-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts/{id}
```

### <a name="response"></a><span data-ttu-id="48436-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="48436-135">Response</span></span>

<span data-ttu-id="48436-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="48436-136">The following is an example of the response.</span></span>
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
