---
title: Listar userExperienceAnalyticsAppHealthDeviceModelPerformances
description: Listar Propriedades e relações dos objetos userExperienceAnalyticsAppHealthDeviceModelPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0aa74e3458e7a94db445f7eb221792032ae8d802
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992517"
---
# <a name="list-userexperienceanalyticsapphealthdevicemodelperformances"></a><span data-ttu-id="0e319-103">Listar userExperienceAnalyticsAppHealthDeviceModelPerformances</span><span class="sxs-lookup"><span data-stu-id="0e319-103">List userExperienceAnalyticsAppHealthDeviceModelPerformances</span></span>

<span data-ttu-id="0e319-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e319-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e319-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e319-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e319-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e319-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e319-107">Listar Propriedades e relações dos objetos [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="0e319-107">List properties and relationships of the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e319-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0e319-108">Prerequisites</span></span>
<span data-ttu-id="0e319-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e319-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e319-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e319-111">Permission type</span></span>|<span data-ttu-id="0e319-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0e319-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e319-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e319-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e319-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e319-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0e319-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e319-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e319-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e319-116">Not supported.</span></span>|
|<span data-ttu-id="0e319-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e319-117">Application</span></span>|<span data-ttu-id="0e319-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e319-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e319-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e319-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance
```

## <a name="request-headers"></a><span data-ttu-id="0e319-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e319-120">Request headers</span></span>
|<span data-ttu-id="0e319-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e319-121">Header</span></span>|<span data-ttu-id="0e319-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0e319-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e319-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e319-123">Authorization</span></span>|<span data-ttu-id="0e319-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e319-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e319-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0e319-125">Accept</span></span>|<span data-ttu-id="0e319-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e319-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e319-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e319-127">Request body</span></span>
<span data-ttu-id="0e319-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e319-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e319-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e319-129">Response</span></span>
<span data-ttu-id="0e319-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e319-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e319-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e319-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e319-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e319-132">Request</span></span>
<span data-ttu-id="0e319-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e319-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance
```

### <a name="response"></a><span data-ttu-id="0e319-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e319-134">Response</span></span>
<span data-ttu-id="0e319-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e319-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 473

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance",
      "id": "4daddc60-dc60-4dad-60dc-ad4d60dcad4d",
      "deviceModel": "Device Model value",
      "deviceManufacturer": "Device Manufacturer value",
      "activeDeviceCount": 1,
      "meanTimeToFailureInMinutes": 10,
      "modelAppHealthScore": 6.333333333333333,
      "modelAppHealthStatus": "Model App Health Status value"
    }
  ]
}
```






