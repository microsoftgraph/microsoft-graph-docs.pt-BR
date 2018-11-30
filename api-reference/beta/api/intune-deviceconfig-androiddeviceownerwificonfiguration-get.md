---
title: Obter androidDeviceOwnerWiFiConfiguration
description: Leia as propriedades e os relacionamentos do objeto androidDeviceOwnerWiFiConfiguration.
ms.openlocfilehash: df327e42ce57e7026ab1e642ff4b687eb3f15e64
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037265"
---
# <a name="get-androiddeviceownerwificonfiguration"></a><span data-ttu-id="ea0df-103">Obter androidDeviceOwnerWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea0df-103">Get androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="ea0df-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ea0df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea0df-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ea0df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea0df-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ea0df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea0df-107">Leia as propriedades e os relacionamentos do objeto [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ea0df-107">Read properties and relationships of the [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea0df-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ea0df-108">Prerequisites</span></span>
<span data-ttu-id="ea0df-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea0df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea0df-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea0df-111">Permission type</span></span>|<span data-ttu-id="ea0df-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ea0df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea0df-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea0df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea0df-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea0df-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ea0df-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea0df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea0df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea0df-116">Not supported.</span></span>|
|<span data-ttu-id="ea0df-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea0df-117">Application</span></span>|<span data-ttu-id="ea0df-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea0df-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea0df-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea0df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea0df-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ea0df-120">Optional query parameters</span></span>
<span data-ttu-id="ea0df-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ea0df-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ea0df-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea0df-122">Request headers</span></span>
|<span data-ttu-id="ea0df-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ea0df-123">Header</span></span>|<span data-ttu-id="ea0df-124">Valor</span><span class="sxs-lookup"><span data-stu-id="ea0df-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea0df-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea0df-125">Authorization</span></span>|<span data-ttu-id="ea0df-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea0df-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea0df-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ea0df-127">Accept</span></span>|<span data-ttu-id="ea0df-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ea0df-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea0df-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea0df-129">Request body</span></span>
<span data-ttu-id="ea0df-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ea0df-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea0df-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea0df-131">Response</span></span>
<span data-ttu-id="ea0df-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea0df-132">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea0df-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea0df-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea0df-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea0df-134">Request</span></span>
<span data-ttu-id="ea0df-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea0df-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ea0df-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea0df-136">Response</span></span>
<span data-ttu-id="ea0df-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea0df-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 736

{
  "value": {
    "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
    "id": "8d25beba-beba-8d25-babe-258dbabe258d",
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
    "wiFiSecurityType": "wep",
    "preSharedKey": "Pre Shared Key value",
    "preSharedKeyIsSet": true
  }
}
```





