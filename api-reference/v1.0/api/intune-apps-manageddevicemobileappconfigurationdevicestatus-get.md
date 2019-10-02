---
title: Obter managedDeviceMobileAppConfigurationDeviceStatus
description: Leia as propriedades e as relações do objeto managedDeviceMobileAppConfigurationDeviceStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 699359cd7bdafeba6b1d721743af72d0452647cd
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355383"
---
# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="0da0f-103">Obter managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="0da0f-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="0da0f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0da0f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0da0f-105">Leia as propriedades e as relações do objeto [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="0da0f-105">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0da0f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0da0f-106">Prerequisites</span></span>
<span data-ttu-id="0da0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0da0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0da0f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0da0f-109">Permission type</span></span>|<span data-ttu-id="0da0f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0da0f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0da0f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0da0f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0da0f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0da0f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0da0f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0da0f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0da0f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0da0f-114">Not supported.</span></span>|
|<span data-ttu-id="0da0f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0da0f-115">Application</span></span>|<span data-ttu-id="0da0f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0da0f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0da0f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0da0f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0da0f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0da0f-118">Optional query parameters</span></span>
<span data-ttu-id="0da0f-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0da0f-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0da0f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0da0f-120">Request headers</span></span>
|<span data-ttu-id="0da0f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0da0f-121">Header</span></span>|<span data-ttu-id="0da0f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0da0f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0da0f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0da0f-123">Authorization</span></span>|<span data-ttu-id="0da0f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0da0f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0da0f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0da0f-125">Accept</span></span>|<span data-ttu-id="0da0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0da0f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0da0f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0da0f-127">Request body</span></span>
<span data-ttu-id="0da0f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0da0f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0da0f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0da0f-129">Response</span></span>
<span data-ttu-id="0da0f-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0da0f-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0da0f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0da0f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0da0f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0da0f-132">Request</span></span>
<span data-ttu-id="0da0f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0da0f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="0da0f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0da0f-134">Response</span></span>
<span data-ttu-id="0da0f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0da0f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




