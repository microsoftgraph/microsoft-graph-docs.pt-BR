---
title: Lista managedDeviceMobileAppConfigurationDeviceStatuses
description: Lista as propriedades e os relacionamentos dos objetos managedDeviceMobileAppConfigurationDeviceStatus.
ms.openlocfilehash: 0bdbc59ce4aaa32054a8ee8e25535e6dfc03d5eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005582"
---
# <a name="list-manageddevicemobileappconfigurationdevicestatuses"></a><span data-ttu-id="1afe7-103">Lista managedDeviceMobileAppConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="1afe7-103">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="1afe7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1afe7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1afe7-105">Lista as propriedades e os relacionamentos dos objetos [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="1afe7-105">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1afe7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1afe7-106">Prerequisites</span></span>
<span data-ttu-id="1afe7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1afe7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1afe7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1afe7-109">Permission type</span></span>|<span data-ttu-id="1afe7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1afe7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1afe7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1afe7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1afe7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1afe7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1afe7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1afe7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1afe7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1afe7-114">Not supported.</span></span>|
|<span data-ttu-id="1afe7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1afe7-115">Application</span></span>|<span data-ttu-id="1afe7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1afe7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1afe7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1afe7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="1afe7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1afe7-118">Request headers</span></span>
|<span data-ttu-id="1afe7-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1afe7-119">Header</span></span>|<span data-ttu-id="1afe7-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1afe7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1afe7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1afe7-121">Authorization</span></span>|<span data-ttu-id="1afe7-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1afe7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1afe7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1afe7-123">Accept</span></span>|<span data-ttu-id="1afe7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1afe7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1afe7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1afe7-125">Request body</span></span>
<span data-ttu-id="1afe7-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1afe7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1afe7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1afe7-127">Response</span></span>
<span data-ttu-id="1afe7-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1afe7-128">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1afe7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1afe7-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="1afe7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1afe7-130">Request</span></span>
<span data-ttu-id="1afe7-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1afe7-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="1afe7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1afe7-132">Response</span></span>
<span data-ttu-id="1afe7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1afe7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 563

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
      "id": "477d3651-3651-477d-5136-7d4751367d47",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



