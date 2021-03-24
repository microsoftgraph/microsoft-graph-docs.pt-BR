---
title: Listar androidWorkProfileEnterpriseWiFiConfigurations
description: Listar propriedades e relações dos objetos androidWorkProfileEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3bd5a6f638939fac943332dfaea219cfcd28b0de
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126595"
---
# <a name="list-androidworkprofileenterprisewificonfigurations"></a><span data-ttu-id="473fa-103">Listar androidWorkProfileEnterpriseWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="473fa-103">List androidWorkProfileEnterpriseWiFiConfigurations</span></span>

<span data-ttu-id="473fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="473fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="473fa-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="473fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="473fa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="473fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="473fa-107">Listar propriedades e relações dos objetos [androidWorkProfileEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="473fa-107">List properties and relationships of the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="473fa-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="473fa-108">Prerequisites</span></span>
<span data-ttu-id="473fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="473fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="473fa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="473fa-111">Permission type</span></span>|<span data-ttu-id="473fa-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="473fa-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="473fa-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="473fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="473fa-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="473fa-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="473fa-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="473fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="473fa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="473fa-116">Not supported.</span></span>|
|<span data-ttu-id="473fa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="473fa-117">Application</span></span>|<span data-ttu-id="473fa-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="473fa-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="473fa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="473fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="473fa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="473fa-120">Request headers</span></span>
|<span data-ttu-id="473fa-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="473fa-121">Header</span></span>|<span data-ttu-id="473fa-122">Valor</span><span class="sxs-lookup"><span data-stu-id="473fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="473fa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="473fa-123">Authorization</span></span>|<span data-ttu-id="473fa-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="473fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="473fa-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="473fa-125">Accept</span></span>|<span data-ttu-id="473fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="473fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="473fa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="473fa-127">Request body</span></span>
<span data-ttu-id="473fa-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="473fa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="473fa-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="473fa-129">Response</span></span>
<span data-ttu-id="473fa-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="473fa-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="473fa-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="473fa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="473fa-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="473fa-132">Request</span></span>
<span data-ttu-id="473fa-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="473fa-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="473fa-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="473fa-134">Response</span></span>
<span data-ttu-id="473fa-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="473fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2052

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
      "id": "c48cd726-d726-c48c-26d7-8cc426d78cc4",
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
      "wiFiSecurityType": "wpaEnterprise",
      "eapType": "eapTtls",
      "authenticationMethod": "usernameAndPassword",
      "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
      "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
      "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
      "proxySettings": "manual",
      "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/"
    }
  ]
}
```




