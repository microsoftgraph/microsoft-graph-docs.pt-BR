---
title: Listar userExperienceAnalyticsAppHealthDeviceModelPerformances
description: Listar Propriedades e relações dos objetos userExperienceAnalyticsAppHealthDeviceModelPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f510e195e386ce683ed38070d06cc98b00639ac
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202889"
---
# <a name="list-userexperienceanalyticsapphealthdevicemodelperformances"></a><span data-ttu-id="6ebcc-103">Listar userExperienceAnalyticsAppHealthDeviceModelPerformances</span><span class="sxs-lookup"><span data-stu-id="6ebcc-103">List userExperienceAnalyticsAppHealthDeviceModelPerformances</span></span>

<span data-ttu-id="6ebcc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ebcc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ebcc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ebcc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ebcc-107">Listar Propriedades e relações dos objetos [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="6ebcc-107">List properties and relationships of the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ebcc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6ebcc-108">Prerequisites</span></span>
<span data-ttu-id="6ebcc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ebcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ebcc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ebcc-111">Permission type</span></span>|<span data-ttu-id="6ebcc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6ebcc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ebcc-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ebcc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ebcc-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ebcc-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6ebcc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ebcc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ebcc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-116">Not supported.</span></span>|
|<span data-ttu-id="6ebcc-117">Application</span><span class="sxs-lookup"><span data-stu-id="6ebcc-117">Application</span></span>|<span data-ttu-id="6ebcc-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ebcc-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ebcc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ebcc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance
```

## <a name="request-headers"></a><span data-ttu-id="6ebcc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ebcc-120">Request headers</span></span>
|<span data-ttu-id="6ebcc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ebcc-121">Header</span></span>|<span data-ttu-id="6ebcc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6ebcc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ebcc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ebcc-123">Authorization</span></span>|<span data-ttu-id="6ebcc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ebcc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6ebcc-125">Accept</span></span>|<span data-ttu-id="6ebcc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ebcc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ebcc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ebcc-127">Request body</span></span>
<span data-ttu-id="6ebcc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ebcc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ebcc-129">Response</span></span>
<span data-ttu-id="6ebcc-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ebcc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ebcc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ebcc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ebcc-132">Request</span></span>
<span data-ttu-id="6ebcc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance
```

### <a name="response"></a><span data-ttu-id="6ebcc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ebcc-134">Response</span></span>
<span data-ttu-id="6ebcc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




