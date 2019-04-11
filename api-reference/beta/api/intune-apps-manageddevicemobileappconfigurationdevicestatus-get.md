---
title: Obter managedDeviceMobileAppConfigurationDeviceStatus
description: Leia as propriedades e as relações do objeto managedDeviceMobileAppConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9cfc8994eac177b1c2e2ac17f9ec8ec24407243
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792220"
---
# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="12d08-103">Obter managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="12d08-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="12d08-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12d08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12d08-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12d08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12d08-106">Leia as propriedades e as relações do objeto [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="12d08-106">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12d08-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12d08-107">Prerequisites</span></span>
<span data-ttu-id="12d08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12d08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12d08-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12d08-110">Permission type</span></span>|<span data-ttu-id="12d08-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="12d08-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12d08-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12d08-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12d08-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="12d08-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="12d08-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12d08-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12d08-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12d08-115">Not supported.</span></span>|
|<span data-ttu-id="12d08-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12d08-116">Application</span></span>|<span data-ttu-id="12d08-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12d08-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12d08-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12d08-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12d08-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="12d08-119">Optional query parameters</span></span>
<span data-ttu-id="12d08-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="12d08-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12d08-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12d08-121">Request headers</span></span>
|<span data-ttu-id="12d08-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12d08-122">Header</span></span>|<span data-ttu-id="12d08-123">Valor</span><span class="sxs-lookup"><span data-stu-id="12d08-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12d08-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="12d08-124">Authorization</span></span>|<span data-ttu-id="12d08-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12d08-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12d08-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12d08-126">Accept</span></span>|<span data-ttu-id="12d08-127">application/json</span><span class="sxs-lookup"><span data-stu-id="12d08-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12d08-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12d08-128">Request body</span></span>
<span data-ttu-id="12d08-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12d08-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12d08-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="12d08-130">Response</span></span>
<span data-ttu-id="12d08-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12d08-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12d08-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12d08-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="12d08-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12d08-133">Request</span></span>
<span data-ttu-id="12d08-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12d08-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="12d08-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="12d08-135">Response</span></span>
<span data-ttu-id="12d08-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12d08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





