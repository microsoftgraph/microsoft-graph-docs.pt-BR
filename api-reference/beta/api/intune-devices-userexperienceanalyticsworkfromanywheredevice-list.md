---
title: Listar userExperienceAnalyticsWorkFromAnywhereDevices
description: Listar propriedades e relações dos objetos userExperienceAnalyticsWorkFromAnywhereDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 33b0659d3ca6c86b3c57c10fb17625bcdb91bf09
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868332"
---
# <a name="list-userexperienceanalyticsworkfromanywheredevices"></a><span data-ttu-id="19b89-103">Listar userExperienceAnalyticsWorkFromAnywhereDevices</span><span class="sxs-lookup"><span data-stu-id="19b89-103">List userExperienceAnalyticsWorkFromAnywhereDevices</span></span>

<span data-ttu-id="19b89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19b89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19b89-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="19b89-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19b89-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="19b89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19b89-107">Listar propriedades e relações dos [objetos userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)</span><span class="sxs-lookup"><span data-stu-id="19b89-107">List properties and relationships of the [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19b89-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="19b89-108">Prerequisites</span></span>
<span data-ttu-id="19b89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19b89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19b89-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19b89-111">Permission type</span></span>|<span data-ttu-id="19b89-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19b89-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19b89-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19b89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19b89-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19b89-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="19b89-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19b89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19b89-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19b89-116">Not supported.</span></span>|
|<span data-ttu-id="19b89-117">Application</span><span class="sxs-lookup"><span data-stu-id="19b89-117">Application</span></span>|<span data-ttu-id="19b89-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19b89-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19b89-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19b89-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
```

## <a name="request-headers"></a><span data-ttu-id="19b89-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19b89-120">Request headers</span></span>
|<span data-ttu-id="19b89-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19b89-121">Header</span></span>|<span data-ttu-id="19b89-122">Valor</span><span class="sxs-lookup"><span data-stu-id="19b89-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19b89-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="19b89-123">Authorization</span></span>|<span data-ttu-id="19b89-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19b89-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19b89-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="19b89-125">Accept</span></span>|<span data-ttu-id="19b89-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19b89-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19b89-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19b89-127">Request body</span></span>
<span data-ttu-id="19b89-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="19b89-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19b89-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="19b89-129">Response</span></span>
<span data-ttu-id="19b89-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19b89-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19b89-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19b89-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="19b89-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19b89-132">Request</span></span>
<span data-ttu-id="19b89-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19b89-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
```

### <a name="response"></a><span data-ttu-id="19b89-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="19b89-134">Response</span></span>
<span data-ttu-id="19b89-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19b89-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 639

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
      "azureAdJoinType": "Azure Ad Join Type value"
    }
  ]
}
```




