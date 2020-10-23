---
title: Listar userExperienceAnalyticsAppHealthDevicePerformanceDetailses
description: Listar Propriedades e relações dos objetos userExperienceAnalyticsAppHealthDevicePerformanceDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d66f1e3bcba448d669d54684451aa0f1d043ebb8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735915"
---
# <a name="list-userexperienceanalyticsapphealthdeviceperformancedetailses"></a><span data-ttu-id="88632-103">Listar userExperienceAnalyticsAppHealthDevicePerformanceDetailses</span><span class="sxs-lookup"><span data-stu-id="88632-103">List userExperienceAnalyticsAppHealthDevicePerformanceDetailses</span></span>

<span data-ttu-id="88632-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88632-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88632-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88632-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88632-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88632-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88632-107">Listar Propriedades e relações dos objetos [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .</span><span class="sxs-lookup"><span data-stu-id="88632-107">List properties and relationships of the [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88632-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88632-108">Prerequisites</span></span>
<span data-ttu-id="88632-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88632-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88632-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88632-111">Permission type</span></span>|<span data-ttu-id="88632-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="88632-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88632-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88632-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88632-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="88632-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="88632-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88632-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88632-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88632-116">Not supported.</span></span>|
|<span data-ttu-id="88632-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88632-117">Application</span></span>|<span data-ttu-id="88632-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="88632-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88632-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88632-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
```

## <a name="request-headers"></a><span data-ttu-id="88632-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88632-120">Request headers</span></span>
|<span data-ttu-id="88632-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88632-121">Header</span></span>|<span data-ttu-id="88632-122">Valor</span><span class="sxs-lookup"><span data-stu-id="88632-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88632-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="88632-123">Authorization</span></span>|<span data-ttu-id="88632-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88632-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88632-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88632-125">Accept</span></span>|<span data-ttu-id="88632-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88632-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88632-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88632-127">Request body</span></span>
<span data-ttu-id="88632-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88632-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88632-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="88632-129">Response</span></span>
<span data-ttu-id="88632-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88632-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88632-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88632-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="88632-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88632-132">Request</span></span>
<span data-ttu-id="88632-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88632-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
```

### <a name="response"></a><span data-ttu-id="88632-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="88632-134">Response</span></span>
<span data-ttu-id="88632-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88632-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 435

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
      "id": "bc8c5273-5273-bc8c-7352-8cbc73528cbc",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "eventType": "Event Type value",
      "appDisplayName": "App Display Name value",
      "deviceId": "Device Id value",
      "deviceDisplayName": "Device Display Name value"
    }
  ]
}
```





