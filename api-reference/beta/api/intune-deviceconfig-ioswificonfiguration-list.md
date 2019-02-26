---
title: Listar iosWiFiConfigurations
description: Listar Propriedades e relações dos objetos iosWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e08dae472cc12da19f35fa97dcb32d4d5fef3b3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170025"
---
# <a name="list-ioswificonfigurations"></a><span data-ttu-id="6cdf5-103">Listar iosWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="6cdf5-103">List iosWiFiConfigurations</span></span>

> <span data-ttu-id="6cdf5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6cdf5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cdf5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6cdf5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cdf5-106">Listar Propriedades e relações dos objetos [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6cdf5-106">List properties and relationships of the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cdf5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6cdf5-107">Prerequisites</span></span>
<span data-ttu-id="6cdf5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6cdf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6cdf5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cdf5-110">Permission type</span></span>|<span data-ttu-id="6cdf5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6cdf5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cdf5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cdf5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6cdf5-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cdf5-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6cdf5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cdf5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cdf5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cdf5-115">Not supported.</span></span>|
|<span data-ttu-id="6cdf5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cdf5-116">Application</span></span>|<span data-ttu-id="6cdf5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cdf5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cdf5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cdf5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6cdf5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cdf5-119">Request headers</span></span>
|<span data-ttu-id="6cdf5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6cdf5-120">Header</span></span>|<span data-ttu-id="6cdf5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6cdf5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cdf5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cdf5-122">Authorization</span></span>|<span data-ttu-id="6cdf5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cdf5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cdf5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6cdf5-124">Accept</span></span>|<span data-ttu-id="6cdf5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6cdf5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cdf5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cdf5-126">Request body</span></span>
<span data-ttu-id="6cdf5-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6cdf5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cdf5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cdf5-128">Response</span></span>
<span data-ttu-id="6cdf5-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cdf5-129">If successful, this method returns a `200 OK` response code and a collection of [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cdf5-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cdf5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cdf5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cdf5-131">Request</span></span>
<span data-ttu-id="6cdf5-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cdf5-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="6cdf5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cdf5-133">Response</span></span>
<span data-ttu-id="6cdf5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6cdf5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 964

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
      "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
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
      "preSharedKey": "Pre Shared Key value"
    }
  ]
}
```




