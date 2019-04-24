---
title: Listar windowsWifiEnterpriseEAPConfigurations
description: Listar Propriedades e relações dos objetos windowsWifiEnterpriseEAPConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b3e1e99d3c42fc961926a2daffefb3ee1c3b7889
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32510861"
---
# <a name="list-windowswifienterpriseeapconfigurations"></a><span data-ttu-id="83102-103">Listar windowsWifiEnterpriseEAPConfigurations</span><span class="sxs-lookup"><span data-stu-id="83102-103">List windowsWifiEnterpriseEAPConfigurations</span></span>

> <span data-ttu-id="83102-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83102-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83102-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83102-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83102-106">Listar Propriedades e relações dos objetos [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="83102-106">List properties and relationships of the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83102-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="83102-107">Prerequisites</span></span>
<span data-ttu-id="83102-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83102-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83102-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83102-110">Permission type</span></span>|<span data-ttu-id="83102-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="83102-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83102-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83102-112">Delegated (work or school account)</span></span>|<span data-ttu-id="83102-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="83102-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="83102-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83102-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83102-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83102-115">Not supported.</span></span>|
|<span data-ttu-id="83102-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83102-116">Application</span></span>|<span data-ttu-id="83102-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83102-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83102-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83102-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="83102-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83102-119">Request headers</span></span>
|<span data-ttu-id="83102-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83102-120">Header</span></span>|<span data-ttu-id="83102-121">Valor</span><span class="sxs-lookup"><span data-stu-id="83102-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83102-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="83102-122">Authorization</span></span>|<span data-ttu-id="83102-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83102-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83102-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="83102-124">Accept</span></span>|<span data-ttu-id="83102-125">application/json</span><span class="sxs-lookup"><span data-stu-id="83102-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83102-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83102-126">Request body</span></span>
<span data-ttu-id="83102-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83102-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83102-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="83102-128">Response</span></span>
<span data-ttu-id="83102-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83102-129">If successful, this method returns a `200 OK` response code and a collection of [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83102-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83102-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="83102-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83102-131">Request</span></span>
<span data-ttu-id="83102-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83102-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="83102-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="83102-133">Response</span></span>
<span data-ttu-id="83102-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83102-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1865

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
      "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "preSharedKey": "Pre Shared Key value",
      "wifiSecurityType": "wpaPersonal",
      "meteredConnectionLimit": "fixed",
      "ssid": "Ssid value",
      "networkName": "Network Name value",
      "connectAutomatically": true,
      "connectToPreferredNetwork": true,
      "connectWhenNetworkNameIsHidden": true,
      "proxySetting": "manual",
      "proxyManualAddress": "Proxy Manual Address value",
      "proxyManualPort": 15,
      "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
      "forceFIPSCompliance": true,
      "networkSingleSignOn": "prelogon",
      "maximumAuthenticationTimeoutInSeconds": 5,
      "promptForAdditionalAuthenticationCredentials": true,
      "enablePairwiseMasterKeyCaching": true,
      "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
      "maximumNumberOfPairwiseMasterKeysInCache": 8,
      "enablePreAuthentication": true,
      "maximumPreAuthenticationAttempts": 0,
      "eapType": "leap",
      "trustedServerCertificateNames": [
        "Trusted Server Certificate Names value"
      ],
      "authenticationMethod": "usernameAndPassword",
      "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
      "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
    }
  ]
}
```





