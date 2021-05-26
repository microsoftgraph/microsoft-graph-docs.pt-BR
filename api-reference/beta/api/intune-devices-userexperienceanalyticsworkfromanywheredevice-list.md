---
title: Listar userExperienceAnalyticsWorkFromAnywhereDevices
description: Listar propriedades e relações dos objetos userExperienceAnalyticsWorkFromAnywhereDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fa16bf6df1f912004cb7dd57422ea8d4bfb807ad
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665032"
---
# <a name="list-userexperienceanalyticsworkfromanywheredevices"></a><span data-ttu-id="8b9c1-103">Listar userExperienceAnalyticsWorkFromAnywhereDevices</span><span class="sxs-lookup"><span data-stu-id="8b9c1-103">List userExperienceAnalyticsWorkFromAnywhereDevices</span></span>

<span data-ttu-id="8b9c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b9c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b9c1-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8b9c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b9c1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8b9c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b9c1-107">Listar propriedades e relações dos [objetos userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)</span><span class="sxs-lookup"><span data-stu-id="8b9c1-107">List properties and relationships of the [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b9c1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8b9c1-108">Prerequisites</span></span>
<span data-ttu-id="8b9c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b9c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b9c1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b9c1-111">Permission type</span></span>|<span data-ttu-id="8b9c1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b9c1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b9c1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b9c1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8b9c1-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b9c1-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8b9c1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b9c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b9c1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b9c1-116">Not supported.</span></span>|
|<span data-ttu-id="8b9c1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b9c1-117">Application</span></span>|<span data-ttu-id="8b9c1-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b9c1-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b9c1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b9c1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
```

## <a name="request-headers"></a><span data-ttu-id="8b9c1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b9c1-120">Request headers</span></span>
|<span data-ttu-id="8b9c1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8b9c1-121">Header</span></span>|<span data-ttu-id="8b9c1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8b9c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b9c1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b9c1-123">Authorization</span></span>|<span data-ttu-id="8b9c1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b9c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b9c1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8b9c1-125">Accept</span></span>|<span data-ttu-id="8b9c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b9c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b9c1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b9c1-127">Request body</span></span>
<span data-ttu-id="8b9c1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8b9c1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b9c1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b9c1-129">Response</span></span>
<span data-ttu-id="8b9c1-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b9c1-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b9c1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b9c1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b9c1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b9c1-132">Request</span></span>
<span data-ttu-id="8b9c1-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b9c1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
```

### <a name="response"></a><span data-ttu-id="8b9c1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b9c1-134">Response</span></span>
<span data-ttu-id="8b9c1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8b9c1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 727

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
      "id": "83d5adfc-adfc-83d5-fcad-d583fcadd583",
      "deviceName": "Device Name value",
      "serialNumber": "Serial Number value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "ownership": "Ownership value",
      "managedBy": "Managed By value",
      "autoPilotRegistered": true,
      "autoPilotProfileAssigned": true,
      "azureAdRegistered": true,
      "azureAdDeviceId": "Azure Ad Device Id value",
      "azureAdJoinType": "Azure Ad Join Type value",
      "osDescription": "Os Description value",
      "osVersion": "Os Version value"
    }
  ]
}
```




