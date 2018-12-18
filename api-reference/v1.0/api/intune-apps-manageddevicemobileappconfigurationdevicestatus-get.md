---
title: Obter managedDeviceMobileAppConfigurationDeviceStatus
description: Leia as propriedades e os relacionamentos do objeto managedDeviceMobileAppConfigurationDeviceStatus.
author: tfitzmac
ms.openlocfilehash: cc38c226135a7f0660f4d62fe56fb05371cf35f4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342389"
---
# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="63103-103">Obter managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="63103-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="63103-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="63103-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63103-105">Leia as propriedades e os relacionamentos do objeto [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="63103-105">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="63103-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63103-106">Prerequisites</span></span>
<span data-ttu-id="63103-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63103-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63103-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63103-109">Permission type</span></span>|<span data-ttu-id="63103-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63103-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63103-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63103-111">Delegated (work or school account)</span></span>|<span data-ttu-id="63103-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="63103-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="63103-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63103-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63103-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63103-114">Not supported.</span></span>|
|<span data-ttu-id="63103-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63103-115">Application</span></span>|<span data-ttu-id="63103-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63103-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63103-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63103-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="63103-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="63103-118">Optional query parameters</span></span>
<span data-ttu-id="63103-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="63103-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="63103-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63103-120">Request headers</span></span>
|<span data-ttu-id="63103-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63103-121">Header</span></span>|<span data-ttu-id="63103-122">Valor</span><span class="sxs-lookup"><span data-stu-id="63103-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63103-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="63103-123">Authorization</span></span>|<span data-ttu-id="63103-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63103-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63103-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63103-125">Accept</span></span>|<span data-ttu-id="63103-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63103-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63103-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63103-127">Request body</span></span>
<span data-ttu-id="63103-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63103-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63103-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="63103-129">Response</span></span>
<span data-ttu-id="63103-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63103-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63103-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63103-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="63103-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63103-132">Request</span></span>
<span data-ttu-id="63103-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63103-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="63103-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="63103-134">Response</span></span>
<span data-ttu-id="63103-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63103-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 531

{
  "value": {
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
}
```



