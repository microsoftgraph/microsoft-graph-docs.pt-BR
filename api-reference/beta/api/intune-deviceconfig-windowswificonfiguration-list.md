---
title: Lista windowsWifiConfigurations
description: Lista as propriedades e os relacionamentos dos objetos windowsWifiConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c09af90d530a1f871b9aec8b015a0f640a6a3ece
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416738"
---
# <a name="list-windowswificonfigurations"></a><span data-ttu-id="32f35-103">Lista windowsWifiConfigurations</span><span class="sxs-lookup"><span data-stu-id="32f35-103">List windowsWifiConfigurations</span></span>

> <span data-ttu-id="32f35-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="32f35-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="32f35-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="32f35-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32f35-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="32f35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32f35-107">Lista as propriedades e os relacionamentos dos objetos [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="32f35-107">List properties and relationships of the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32f35-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32f35-108">Prerequisites</span></span>
<span data-ttu-id="32f35-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="32f35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="32f35-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32f35-111">Permission type</span></span>|<span data-ttu-id="32f35-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="32f35-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32f35-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32f35-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32f35-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="32f35-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="32f35-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32f35-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32f35-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32f35-116">Not supported.</span></span>|
|<span data-ttu-id="32f35-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32f35-117">Application</span></span>|<span data-ttu-id="32f35-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32f35-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32f35-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32f35-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="32f35-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32f35-120">Request headers</span></span>
|<span data-ttu-id="32f35-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32f35-121">Header</span></span>|<span data-ttu-id="32f35-122">Valor</span><span class="sxs-lookup"><span data-stu-id="32f35-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32f35-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="32f35-123">Authorization</span></span>|<span data-ttu-id="32f35-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32f35-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32f35-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="32f35-125">Accept</span></span>|<span data-ttu-id="32f35-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32f35-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32f35-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32f35-127">Request body</span></span>
<span data-ttu-id="32f35-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32f35-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32f35-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="32f35-129">Response</span></span>
<span data-ttu-id="32f35-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32f35-130">If successful, this method returns a `200 OK` response code and a collection of [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32f35-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32f35-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="32f35-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32f35-132">Request</span></span>
<span data-ttu-id="32f35-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32f35-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="32f35-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="32f35-134">Response</span></span>
<span data-ttu-id="32f35-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32f35-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1087

{
  "value": [
    {
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
  ]
}
```




