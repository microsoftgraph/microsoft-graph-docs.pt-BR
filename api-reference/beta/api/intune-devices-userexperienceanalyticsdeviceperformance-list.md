---
title: Listar userExperienceAnalyticsDevicePerformances
description: Listar Propriedades e relações dos objetos userExperienceAnalyticsDevicePerformance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26102ca70a26d69edfe44674ef1d160e15140cc1
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37529232"
---
# <a name="list-userexperienceanalyticsdeviceperformances"></a><span data-ttu-id="26166-103">Listar userExperienceAnalyticsDevicePerformances</span><span class="sxs-lookup"><span data-stu-id="26166-103">List userExperienceAnalyticsDevicePerformances</span></span>

> <span data-ttu-id="26166-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26166-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26166-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26166-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26166-106">Listar Propriedades e relações dos objetos [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="26166-106">List properties and relationships of the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26166-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26166-107">Prerequisites</span></span>
<span data-ttu-id="26166-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26166-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26166-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26166-110">Permission type</span></span>|<span data-ttu-id="26166-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="26166-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26166-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26166-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26166-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="26166-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="26166-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26166-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26166-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26166-115">Not supported.</span></span>|
|<span data-ttu-id="26166-116">Application</span><span class="sxs-lookup"><span data-stu-id="26166-116">Application</span></span>|<span data-ttu-id="26166-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="26166-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26166-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26166-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicePerformance
```

## <a name="request-headers"></a><span data-ttu-id="26166-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26166-119">Request headers</span></span>
|<span data-ttu-id="26166-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26166-120">Header</span></span>|<span data-ttu-id="26166-121">Valor</span><span class="sxs-lookup"><span data-stu-id="26166-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26166-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="26166-122">Authorization</span></span>|<span data-ttu-id="26166-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26166-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26166-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26166-124">Accept</span></span>|<span data-ttu-id="26166-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26166-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26166-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26166-126">Request body</span></span>
<span data-ttu-id="26166-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="26166-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26166-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="26166-128">Response</span></span>
<span data-ttu-id="26166-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26166-129">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26166-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26166-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="26166-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26166-131">Request</span></span>
<span data-ttu-id="26166-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26166-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance
```

### <a name="response"></a><span data-ttu-id="26166-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="26166-133">Response</span></span>
<span data-ttu-id="26166-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26166-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 636

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
      "deviceCount": 11
    }
  ]
}
```






