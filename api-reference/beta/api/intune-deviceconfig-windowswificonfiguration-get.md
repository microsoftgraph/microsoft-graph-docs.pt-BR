---
title: Obter windowsWifiConfiguration
description: Leia as propriedades e os relacionamentos do objeto windowsWifiConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e5e5e4d1f916350f2b9e7ce97d001d65142b9f63
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397572"
---
# <a name="get-windowswificonfiguration"></a><span data-ttu-id="0d9d7-103">Obter windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="0d9d7-103">Get windowsWifiConfiguration</span></span>

> <span data-ttu-id="0d9d7-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="0d9d7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0d9d7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0d9d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d9d7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0d9d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d9d7-107">Leia as propriedades e os relacionamentos do objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0d9d7-107">Read properties and relationships of the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d9d7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0d9d7-108">Prerequisites</span></span>
<span data-ttu-id="0d9d7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0d9d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0d9d7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d9d7-111">Permission type</span></span>|<span data-ttu-id="0d9d7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0d9d7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d9d7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d9d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d9d7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d9d7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0d9d7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d9d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d9d7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d9d7-116">Not supported.</span></span>|
|<span data-ttu-id="0d9d7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d9d7-117">Application</span></span>|<span data-ttu-id="0d9d7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d9d7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d9d7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d9d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0d9d7-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0d9d7-120">Optional query parameters</span></span>
<span data-ttu-id="0d9d7-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0d9d7-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d9d7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d9d7-122">Request headers</span></span>
|<span data-ttu-id="0d9d7-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0d9d7-123">Header</span></span>|<span data-ttu-id="0d9d7-124">Valor</span><span class="sxs-lookup"><span data-stu-id="0d9d7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d9d7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d9d7-125">Authorization</span></span>|<span data-ttu-id="0d9d7-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d9d7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d9d7-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0d9d7-127">Accept</span></span>|<span data-ttu-id="0d9d7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0d9d7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d9d7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d9d7-129">Request body</span></span>
<span data-ttu-id="0d9d7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d9d7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d9d7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d9d7-131">Response</span></span>
<span data-ttu-id="0d9d7-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d9d7-132">If successful, this method returns a `200 OK` response code and [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d9d7-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d9d7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d9d7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d9d7-134">Request</span></span>
<span data-ttu-id="0d9d7-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d9d7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="0d9d7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d9d7-136">Response</span></span>
<span data-ttu-id="0d9d7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d9d7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




