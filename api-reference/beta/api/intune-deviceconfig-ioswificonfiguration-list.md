---
title: Lista iosWiFiConfigurations
description: Lista as propriedades e os relacionamentos dos objetos iosWiFiConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7d7ad169613f022b656c248dd64aeefb6c12d40b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419965"
---
# <a name="list-ioswificonfigurations"></a><span data-ttu-id="935f3-103">Lista iosWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="935f3-103">List iosWiFiConfigurations</span></span>

> <span data-ttu-id="935f3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="935f3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="935f3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="935f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="935f3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="935f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="935f3-107">Lista as propriedades e os relacionamentos dos objetos [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="935f3-107">List properties and relationships of the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="935f3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="935f3-108">Prerequisites</span></span>
<span data-ttu-id="935f3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="935f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="935f3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="935f3-111">Permission type</span></span>|<span data-ttu-id="935f3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="935f3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="935f3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="935f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="935f3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="935f3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="935f3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="935f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="935f3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="935f3-116">Not supported.</span></span>|
|<span data-ttu-id="935f3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="935f3-117">Application</span></span>|<span data-ttu-id="935f3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="935f3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="935f3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="935f3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="935f3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="935f3-120">Request headers</span></span>
|<span data-ttu-id="935f3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="935f3-121">Header</span></span>|<span data-ttu-id="935f3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="935f3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="935f3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="935f3-123">Authorization</span></span>|<span data-ttu-id="935f3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="935f3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="935f3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="935f3-125">Accept</span></span>|<span data-ttu-id="935f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="935f3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="935f3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="935f3-127">Request body</span></span>
<span data-ttu-id="935f3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="935f3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="935f3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="935f3-129">Response</span></span>
<span data-ttu-id="935f3-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="935f3-130">If successful, this method returns a `200 OK` response code and a collection of [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="935f3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="935f3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="935f3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="935f3-132">Request</span></span>
<span data-ttu-id="935f3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="935f3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="935f3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="935f3-134">Response</span></span>
<span data-ttu-id="935f3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="935f3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




