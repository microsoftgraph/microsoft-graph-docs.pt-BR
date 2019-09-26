---
title: Listar iosEnterpriseWiFiConfigurations
description: Listar Propriedades e relações dos objetos iosEnterpriseWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ce31a89d9e35975c4f03751d44f0e7f535240209
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37167652"
---
# <a name="list-iosenterprisewificonfigurations"></a><span data-ttu-id="79c3f-103">Listar iosEnterpriseWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="79c3f-103">List iosEnterpriseWiFiConfigurations</span></span>

> <span data-ttu-id="79c3f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79c3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79c3f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79c3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79c3f-106">Listar Propriedades e relações dos objetos [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="79c3f-106">List properties and relationships of the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79c3f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79c3f-107">Prerequisites</span></span>
<span data-ttu-id="79c3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79c3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79c3f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79c3f-110">Permission type</span></span>|<span data-ttu-id="79c3f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="79c3f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79c3f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79c3f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79c3f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79c3f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="79c3f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79c3f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79c3f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79c3f-115">Not supported.</span></span>|
|<span data-ttu-id="79c3f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79c3f-116">Application</span></span>|<span data-ttu-id="79c3f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79c3f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79c3f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79c3f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="79c3f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79c3f-119">Request headers</span></span>
|<span data-ttu-id="79c3f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79c3f-120">Header</span></span>|<span data-ttu-id="79c3f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="79c3f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79c3f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="79c3f-122">Authorization</span></span>|<span data-ttu-id="79c3f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79c3f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79c3f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79c3f-124">Accept</span></span>|<span data-ttu-id="79c3f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="79c3f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79c3f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79c3f-126">Request body</span></span>
<span data-ttu-id="79c3f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79c3f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79c3f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="79c3f-128">Response</span></span>
<span data-ttu-id="79c3f-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79c3f-129">If successful, this method returns a `200 OK` response code and a collection of [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79c3f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79c3f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="79c3f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79c3f-131">Request</span></span>
<span data-ttu-id="79c3f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79c3f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="79c3f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="79c3f-133">Response</span></span>
<span data-ttu-id="79c3f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79c3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2387

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
      "id": "7593f7ba-f7ba-7593-baf7-9375baf79375",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "windows10EnterpriseN"
        ],
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "sModeConfiguration",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "networkName": "Network Name value",
      "ssid": "Ssid value",
      "connectAutomatically": true,
      "connectWhenNetworkNameIsHidden": true,
      "wiFiSecurityType": "wpaPersonal",
      "proxySettings": "manual",
      "proxyManualAddress": "Proxy Manual Address value",
      "proxyManualPort": 15,
      "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
      "preSharedKey": "Pre Shared Key value",
      "eapType": "leap",
      "eapFastConfiguration": "useProtectedAccessCredential",
      "trustedServerCertificateNames": [
        "Trusted Server Certificate Names value"
      ],
      "authenticationMethod": "usernameAndPassword",
      "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
      "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
      "usernameFormatString": "Username Format String value",
      "passwordFormatString": "Password Format String value"
    }
  ]
}
```




