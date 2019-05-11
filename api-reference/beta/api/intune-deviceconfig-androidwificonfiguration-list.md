---
title: Listar androidWiFiConfigurations
description: Listar Propriedades e relações dos objetos androidWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f51b6f00272d8e5faccef58a63b1911a2a9cb6d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928733"
---
# <a name="list-androidwificonfigurations"></a><span data-ttu-id="69289-103">Listar androidWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="69289-103">List androidWiFiConfigurations</span></span>

> <span data-ttu-id="69289-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69289-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69289-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69289-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69289-106">Listar Propriedades e relações dos objetos [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="69289-106">List properties and relationships of the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69289-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="69289-107">Prerequisites</span></span>
<span data-ttu-id="69289-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69289-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69289-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69289-110">Permission type</span></span>|<span data-ttu-id="69289-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="69289-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69289-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69289-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69289-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69289-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="69289-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69289-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69289-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69289-115">Not supported.</span></span>|
|<span data-ttu-id="69289-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69289-116">Application</span></span>|<span data-ttu-id="69289-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69289-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69289-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69289-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="69289-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69289-119">Request headers</span></span>
|<span data-ttu-id="69289-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="69289-120">Header</span></span>|<span data-ttu-id="69289-121">Valor</span><span class="sxs-lookup"><span data-stu-id="69289-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69289-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="69289-122">Authorization</span></span>|<span data-ttu-id="69289-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69289-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69289-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="69289-124">Accept</span></span>|<span data-ttu-id="69289-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69289-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69289-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69289-126">Request body</span></span>
<span data-ttu-id="69289-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="69289-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69289-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="69289-128">Response</span></span>
<span data-ttu-id="69289-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69289-129">If successful, this method returns a `200 OK` response code and a collection of [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69289-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69289-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="69289-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69289-131">Request</span></span>
<span data-ttu-id="69289-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69289-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="69289-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="69289-133">Response</span></span>
<span data-ttu-id="69289-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69289-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 704

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
      "id": "51cfd26f-d26f-51cf-6fd2-cf516fd2cf51",
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
      "wiFiSecurityType": "wpaEnterprise"
    }
  ]
}
```




