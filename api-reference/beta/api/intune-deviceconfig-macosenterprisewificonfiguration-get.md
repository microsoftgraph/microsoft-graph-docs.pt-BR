---
title: Obter macOSEnterpriseWiFiConfiguration
description: Leia propriedades e relações do objeto macOSEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9390198ec333e8d956d73b771c9dd5b244f3593f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131285"
---
# <a name="get-macosenterprisewificonfiguration"></a><span data-ttu-id="e9092-103">Obter macOSEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9092-103">Get macOSEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="e9092-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9092-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9092-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e9092-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9092-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9092-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9092-107">Leia propriedades e relações do [objeto macOSEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e9092-107">Read properties and relationships of the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9092-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9092-108">Prerequisites</span></span>
<span data-ttu-id="e9092-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9092-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9092-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9092-111">Permission type</span></span>|<span data-ttu-id="e9092-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9092-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9092-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9092-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9092-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9092-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e9092-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9092-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9092-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9092-116">Not supported.</span></span>|
|<span data-ttu-id="e9092-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9092-117">Application</span></span>|<span data-ttu-id="e9092-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9092-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9092-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9092-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9092-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9092-120">Optional query parameters</span></span>
<span data-ttu-id="e9092-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9092-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9092-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9092-122">Request headers</span></span>
|<span data-ttu-id="e9092-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9092-123">Header</span></span>|<span data-ttu-id="e9092-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e9092-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9092-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9092-125">Authorization</span></span>|<span data-ttu-id="e9092-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9092-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9092-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9092-127">Accept</span></span>|<span data-ttu-id="e9092-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e9092-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9092-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9092-129">Request body</span></span>
<span data-ttu-id="e9092-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9092-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9092-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9092-131">Response</span></span>
<span data-ttu-id="e9092-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9092-132">If successful, this method returns a `200 OK` response code and [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9092-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9092-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9092-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9092-134">Request</span></span>
<span data-ttu-id="e9092-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9092-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e9092-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9092-136">Response</span></span>
<span data-ttu-id="e9092-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9092-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2149

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
    "id": "7a6f9a2e-9a2e-7a6f-2e9a-6f7a2e9a6f7a",
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
    "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
  }
}
```




