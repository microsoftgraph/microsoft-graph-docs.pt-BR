---
title: Listar managedDeviceMobileAppConfigurationDeviceStatuses
description: Listar Propriedades e relações dos objetos managedDeviceMobileAppConfigurationDeviceStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5a1bb26bdf2a69c67259ddcc316f96b419fcb87
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358575"
---
# <a name="list-manageddevicemobileappconfigurationdevicestatuses"></a><span data-ttu-id="e34a4-103">Listar managedDeviceMobileAppConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="e34a4-103">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="e34a4-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e34a4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e34a4-105">Listar Propriedades e relações dos objetos [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="e34a4-105">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e34a4-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e34a4-106">Prerequisites</span></span>
<span data-ttu-id="e34a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e34a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e34a4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e34a4-109">Permission type</span></span>|<span data-ttu-id="e34a4-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e34a4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e34a4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e34a4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e34a4-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e34a4-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e34a4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e34a4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e34a4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e34a4-114">Not supported.</span></span>|
|<span data-ttu-id="e34a4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e34a4-115">Application</span></span>|<span data-ttu-id="e34a4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e34a4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e34a4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e34a4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="e34a4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e34a4-118">Request headers</span></span>
|<span data-ttu-id="e34a4-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e34a4-119">Header</span></span>|<span data-ttu-id="e34a4-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e34a4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e34a4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e34a4-121">Authorization</span></span>|<span data-ttu-id="e34a4-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e34a4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e34a4-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e34a4-123">Accept</span></span>|<span data-ttu-id="e34a4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e34a4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e34a4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e34a4-125">Request body</span></span>
<span data-ttu-id="e34a4-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e34a4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e34a4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e34a4-127">Response</span></span>
<span data-ttu-id="e34a4-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e34a4-128">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e34a4-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e34a4-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e34a4-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e34a4-130">Request</span></span>
<span data-ttu-id="e34a4-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e34a4-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="e34a4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e34a4-132">Response</span></span>
<span data-ttu-id="e34a4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e34a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




