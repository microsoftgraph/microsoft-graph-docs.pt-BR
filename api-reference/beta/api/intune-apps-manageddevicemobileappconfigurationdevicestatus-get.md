---
title: Obter managedDeviceMobileAppConfigurationDeviceStatus
description: Leia as propriedades e as relações do objeto managedDeviceMobileAppConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f763b0a917550127a5cafea2d2362940a6bea356
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43405860"
---
# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="aaedc-103">Obter managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="aaedc-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

<span data-ttu-id="aaedc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaedc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aaedc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aaedc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aaedc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aaedc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaedc-107">Leia as propriedades e as relações do objeto [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="aaedc-107">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aaedc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aaedc-108">Prerequisites</span></span>
<span data-ttu-id="aaedc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaedc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaedc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aaedc-111">Permission type</span></span>|<span data-ttu-id="aaedc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aaedc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaedc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aaedc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aaedc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aaedc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="aaedc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aaedc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaedc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aaedc-116">Not supported.</span></span>|
|<span data-ttu-id="aaedc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aaedc-117">Application</span></span>|<span data-ttu-id="aaedc-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aaedc-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaedc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aaedc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aaedc-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aaedc-120">Optional query parameters</span></span>
<span data-ttu-id="aaedc-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aaedc-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aaedc-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aaedc-122">Request headers</span></span>
|<span data-ttu-id="aaedc-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aaedc-123">Header</span></span>|<span data-ttu-id="aaedc-124">Valor</span><span class="sxs-lookup"><span data-stu-id="aaedc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaedc-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="aaedc-125">Authorization</span></span>|<span data-ttu-id="aaedc-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aaedc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaedc-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aaedc-127">Accept</span></span>|<span data-ttu-id="aaedc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="aaedc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaedc-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aaedc-129">Request body</span></span>
<span data-ttu-id="aaedc-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aaedc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aaedc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaedc-131">Response</span></span>
<span data-ttu-id="aaedc-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aaedc-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaedc-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aaedc-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="aaedc-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aaedc-134">Request</span></span>
<span data-ttu-id="aaedc-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aaedc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="aaedc-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaedc-136">Response</span></span>
<span data-ttu-id="aaedc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aaedc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 551

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
    "id": "477d3651-3651-477d-5136-7d4751367d47",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "platform": 8,
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



