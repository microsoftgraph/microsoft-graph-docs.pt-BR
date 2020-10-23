---
title: Obter managedDeviceMobileAppConfigurationDeviceStatus
description: Leia as propriedades e as relações do objeto managedDeviceMobileAppConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2d589552bd2621ea954f65addb81346d7ea04396
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699419"
---
# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="2f819-103">Obter managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="2f819-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

<span data-ttu-id="2f819-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f819-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f819-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f819-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f819-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f819-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f819-107">Leia as propriedades e as relações do objeto [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="2f819-107">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f819-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f819-108">Prerequisites</span></span>
<span data-ttu-id="2f819-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f819-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f819-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f819-111">Permission type</span></span>|<span data-ttu-id="2f819-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f819-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f819-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f819-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f819-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f819-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2f819-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f819-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f819-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f819-116">Not supported.</span></span>|
|<span data-ttu-id="2f819-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f819-117">Application</span></span>|<span data-ttu-id="2f819-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f819-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f819-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f819-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f819-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2f819-120">Optional query parameters</span></span>
<span data-ttu-id="2f819-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2f819-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f819-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f819-122">Request headers</span></span>
|<span data-ttu-id="2f819-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f819-123">Header</span></span>|<span data-ttu-id="2f819-124">Valor</span><span class="sxs-lookup"><span data-stu-id="2f819-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f819-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f819-125">Authorization</span></span>|<span data-ttu-id="2f819-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f819-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f819-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f819-127">Accept</span></span>|<span data-ttu-id="2f819-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2f819-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f819-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f819-129">Request body</span></span>
<span data-ttu-id="2f819-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f819-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f819-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f819-131">Response</span></span>
<span data-ttu-id="2f819-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f819-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f819-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f819-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f819-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f819-134">Request</span></span>
<span data-ttu-id="2f819-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f819-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="2f819-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f819-136">Response</span></span>
<span data-ttu-id="2f819-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f819-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





