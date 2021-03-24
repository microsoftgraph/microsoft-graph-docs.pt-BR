---
title: Listar managedDeviceMobileAppConfigurationDeviceStatuses
description: Listar propriedades e relações dos objetos managedDeviceMobileAppConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 328ec70f5ec0bc480ce7678ed3c951401a9ee465
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140144"
---
# <a name="list-manageddevicemobileappconfigurationdevicestatuses"></a><span data-ttu-id="c4997-103">Listar managedDeviceMobileAppConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c4997-103">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>

<span data-ttu-id="c4997-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4997-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4997-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4997-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4997-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4997-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4997-107">Listar propriedades e relações dos [objetos managedDeviceMobileAppConfigurationDeviceStatus.](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="c4997-107">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4997-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4997-108">Prerequisites</span></span>
<span data-ttu-id="c4997-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4997-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4997-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4997-111">Permission type</span></span>|<span data-ttu-id="c4997-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4997-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4997-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4997-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4997-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4997-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c4997-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4997-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4997-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4997-116">Not supported.</span></span>|
|<span data-ttu-id="c4997-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4997-117">Application</span></span>|<span data-ttu-id="c4997-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4997-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4997-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4997-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c4997-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4997-120">Request headers</span></span>
|<span data-ttu-id="c4997-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4997-121">Header</span></span>|<span data-ttu-id="c4997-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c4997-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4997-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4997-123">Authorization</span></span>|<span data-ttu-id="c4997-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4997-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4997-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4997-125">Accept</span></span>|<span data-ttu-id="c4997-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4997-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4997-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4997-127">Request body</span></span>
<span data-ttu-id="c4997-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4997-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4997-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4997-129">Response</span></span>
<span data-ttu-id="c4997-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4997-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4997-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4997-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4997-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4997-132">Request</span></span>
<span data-ttu-id="c4997-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4997-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="c4997-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4997-134">Response</span></span>
<span data-ttu-id="c4997-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4997-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 585

{
  "value": [
    {
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
  ]
}
```




