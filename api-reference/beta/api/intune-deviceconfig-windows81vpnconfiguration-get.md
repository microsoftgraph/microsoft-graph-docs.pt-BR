---
title: Obter windows81VpnConfiguration
description: Leia as propriedades e as relações do objeto windows81VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cfad9f681880a967131c069d9e13bf707ab63ac4
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37186999"
---
# <a name="get-windows81vpnconfiguration"></a><span data-ttu-id="3740a-103">Obter windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3740a-103">Get windows81VpnConfiguration</span></span>

> <span data-ttu-id="3740a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3740a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3740a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3740a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3740a-106">Leia as propriedades e as relações do objeto [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3740a-106">Read properties and relationships of the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3740a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3740a-107">Prerequisites</span></span>
<span data-ttu-id="3740a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3740a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3740a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3740a-110">Permission type</span></span>|<span data-ttu-id="3740a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3740a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3740a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3740a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3740a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3740a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3740a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3740a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3740a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3740a-115">Not supported.</span></span>|
|<span data-ttu-id="3740a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3740a-116">Application</span></span>|<span data-ttu-id="3740a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3740a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3740a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3740a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3740a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3740a-119">Optional query parameters</span></span>
<span data-ttu-id="3740a-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3740a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3740a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3740a-121">Request headers</span></span>
|<span data-ttu-id="3740a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3740a-122">Header</span></span>|<span data-ttu-id="3740a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3740a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3740a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3740a-124">Authorization</span></span>|<span data-ttu-id="3740a-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3740a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3740a-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3740a-126">Accept</span></span>|<span data-ttu-id="3740a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3740a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3740a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3740a-128">Request body</span></span>
<span data-ttu-id="3740a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3740a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3740a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3740a-130">Response</span></span>
<span data-ttu-id="3740a-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3740a-131">If successful, this method returns a `200 OK` response code and [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3740a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3740a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3740a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3740a-133">Request</span></span>
<span data-ttu-id="3740a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3740a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3740a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3740a-135">Response</span></span>
<span data-ttu-id="3740a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3740a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2087

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
    "id": "6aa07da3-7da3-6aa0-a37d-a06aa37da06a",
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
    "connectionName": "Connection Name value",
    "servers": [
      {
        "@odata.type": "microsoft.graph.vpnServer",
        "description": "Description value",
        "address": "Address value",
        "isDefaultServer": true
      }
    ],
    "customXml": "Y3VzdG9tWG1s",
    "applyOnlyToWindows81": true,
    "connectionType": "f5EdgeClient",
    "loginGroupOrDomain": "Login Group Or Domain value",
    "enableSplitTunneling": true,
    "proxyServer": {
      "@odata.type": "microsoft.graph.windows81VpnProxyServer",
      "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
      "address": "Address value",
      "port": 4,
      "automaticallyDetectProxySettings": true,
      "bypassProxyServerForLocalAddress": true
    }
  }
}
```




