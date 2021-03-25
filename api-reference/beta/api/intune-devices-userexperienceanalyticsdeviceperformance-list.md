---
title: Listar userExperienceAnalyticsDevicePerformances
description: Listar propriedades e relações dos objetos userExperienceAnalyticsDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4cd55b528cce2ac46cf5eb6f54d2974445b14540
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154165"
---
# <a name="list-userexperienceanalyticsdeviceperformances"></a><span data-ttu-id="a9184-103">Listar userExperienceAnalyticsDevicePerformances</span><span class="sxs-lookup"><span data-stu-id="a9184-103">List userExperienceAnalyticsDevicePerformances</span></span>

<span data-ttu-id="a9184-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9184-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9184-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9184-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9184-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9184-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9184-107">Listar propriedades e relações dos [objetos userExperienceAnalyticsDevicePerformance.](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="a9184-107">List properties and relationships of the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9184-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9184-108">Prerequisites</span></span>
<span data-ttu-id="a9184-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9184-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9184-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9184-111">Permission type</span></span>|<span data-ttu-id="a9184-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9184-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9184-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9184-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9184-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9184-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a9184-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9184-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9184-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9184-116">Not supported.</span></span>|
|<span data-ttu-id="a9184-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9184-117">Application</span></span>|<span data-ttu-id="a9184-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9184-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9184-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9184-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicePerformance
```

## <a name="request-headers"></a><span data-ttu-id="a9184-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9184-120">Request headers</span></span>
|<span data-ttu-id="a9184-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9184-121">Header</span></span>|<span data-ttu-id="a9184-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a9184-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9184-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9184-123">Authorization</span></span>|<span data-ttu-id="a9184-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9184-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9184-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a9184-125">Accept</span></span>|<span data-ttu-id="a9184-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9184-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9184-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9184-127">Request body</span></span>
<span data-ttu-id="a9184-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9184-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9184-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9184-129">Response</span></span>
<span data-ttu-id="a9184-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9184-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9184-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9184-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9184-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9184-132">Request</span></span>
<span data-ttu-id="a9184-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9184-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance
```

### <a name="response"></a><span data-ttu-id="a9184-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9184-134">Response</span></span>
<span data-ttu-id="a9184-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9184-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 797

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
      "id": "852ae826-e826-852a-26e8-2a8526e82a85",
      "deviceName": "Device Name value",
      "model": "Model value",
      "manufacturer": "Manufacturer value",
      "diskType": "hdd",
      "operatingSystemVersion": "Operating System Version value",
      "bootScore": 9,
      "coreBootTimeInMs": 0,
      "groupPolicyBootTimeInMs": 7,
      "healthStatus": "insufficientData",
      "loginScore": 10,
      "coreLoginTimeInMs": 1,
      "groupPolicyLoginTimeInMs": 8,
      "deviceCount": 11,
      "responsiveDesktopTimeInMs": 9,
      "blueScreenCount": 15,
      "restartCount": 12,
      "averageBlueScreens": 6.0,
      "averageRestarts": 5.0
    }
  ]
}
```




