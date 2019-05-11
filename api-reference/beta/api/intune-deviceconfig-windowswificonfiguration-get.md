---
title: Obter windowsWifiConfiguration
description: Leia as propriedades e as relações do objeto windowsWifiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e8390b97804a4481fc6e14e14ba146cf8211a1c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917121"
---
# <a name="get-windowswificonfiguration"></a><span data-ttu-id="cec5a-103">Obter windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="cec5a-103">Get windowsWifiConfiguration</span></span>

> <span data-ttu-id="cec5a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cec5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cec5a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cec5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cec5a-106">Leia as propriedades e as relações do objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="cec5a-106">Read properties and relationships of the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cec5a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cec5a-107">Prerequisites</span></span>
<span data-ttu-id="cec5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cec5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cec5a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cec5a-110">Permission type</span></span>|<span data-ttu-id="cec5a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cec5a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cec5a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cec5a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cec5a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cec5a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cec5a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cec5a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cec5a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cec5a-115">Not supported.</span></span>|
|<span data-ttu-id="cec5a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cec5a-116">Application</span></span>|<span data-ttu-id="cec5a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cec5a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cec5a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cec5a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cec5a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cec5a-119">Optional query parameters</span></span>
<span data-ttu-id="cec5a-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cec5a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cec5a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cec5a-121">Request headers</span></span>
|<span data-ttu-id="cec5a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cec5a-122">Header</span></span>|<span data-ttu-id="cec5a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="cec5a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cec5a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cec5a-124">Authorization</span></span>|<span data-ttu-id="cec5a-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cec5a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cec5a-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cec5a-126">Accept</span></span>|<span data-ttu-id="cec5a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cec5a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cec5a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cec5a-128">Request body</span></span>
<span data-ttu-id="cec5a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cec5a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cec5a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cec5a-130">Response</span></span>
<span data-ttu-id="cec5a-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cec5a-131">If successful, this method returns a `200 OK` response code and [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cec5a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cec5a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cec5a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cec5a-133">Request</span></span>
<span data-ttu-id="cec5a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cec5a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="cec5a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cec5a-135">Response</span></span>
<span data-ttu-id="cec5a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cec5a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1025

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
    "id": "8a9e790f-790f-8a9e-0f79-9e8a0f799e8a",
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
    "forceFIPSCompliance": true
  }
}
```




