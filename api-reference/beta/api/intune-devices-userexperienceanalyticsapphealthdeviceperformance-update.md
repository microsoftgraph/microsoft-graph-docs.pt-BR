---
title: Atualizar userExperienceAnalyticsAppHealthDevicePerformance
description: Atualiza as propriedades de um objeto userExperienceAnalyticsAppHealthDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c14e2b4b2955dc028ab45aab5db87710e6780acc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202813"
---
# <a name="update-userexperienceanalyticsapphealthdeviceperformance"></a><span data-ttu-id="1108d-103">Atualizar userExperienceAnalyticsAppHealthDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="1108d-103">Update userExperienceAnalyticsAppHealthDevicePerformance</span></span>

<span data-ttu-id="1108d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1108d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1108d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1108d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1108d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1108d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1108d-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="1108d-107">Update the properties of a [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1108d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1108d-108">Prerequisites</span></span>
<span data-ttu-id="1108d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1108d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1108d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1108d-111">Permission type</span></span>|<span data-ttu-id="1108d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1108d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1108d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1108d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1108d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1108d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1108d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1108d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1108d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1108d-116">Not supported.</span></span>|
|<span data-ttu-id="1108d-117">Application</span><span class="sxs-lookup"><span data-stu-id="1108d-117">Application</span></span>|<span data-ttu-id="1108d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1108d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1108d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1108d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance/{userExperienceAnalyticsAppHealthDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="1108d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1108d-120">Request headers</span></span>
|<span data-ttu-id="1108d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1108d-121">Header</span></span>|<span data-ttu-id="1108d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1108d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1108d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1108d-123">Authorization</span></span>|<span data-ttu-id="1108d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1108d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1108d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1108d-125">Accept</span></span>|<span data-ttu-id="1108d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1108d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1108d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1108d-127">Request body</span></span>
<span data-ttu-id="1108d-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="1108d-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object.</span></span>

<span data-ttu-id="1108d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md).</span><span class="sxs-lookup"><span data-stu-id="1108d-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md).</span></span>

|<span data-ttu-id="1108d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1108d-130">Property</span></span>|<span data-ttu-id="1108d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1108d-131">Type</span></span>|<span data-ttu-id="1108d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1108d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1108d-133">id</span><span class="sxs-lookup"><span data-stu-id="1108d-133">id</span></span>|<span data-ttu-id="1108d-134">String</span><span class="sxs-lookup"><span data-stu-id="1108d-134">String</span></span>|<span data-ttu-id="1108d-135">O identificador exclusivo do objeto de desempenho do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="1108d-135">The unique identifier of the user experience analytics device performance object.</span></span>|
|<span data-ttu-id="1108d-136">deviceModel</span><span class="sxs-lookup"><span data-stu-id="1108d-136">deviceModel</span></span>|<span data-ttu-id="1108d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1108d-137">String</span></span>|<span data-ttu-id="1108d-138">O nome do modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1108d-138">The model name of the device.</span></span>|
|<span data-ttu-id="1108d-139">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="1108d-139">deviceManufacturer</span></span>|<span data-ttu-id="1108d-140">String</span><span class="sxs-lookup"><span data-stu-id="1108d-140">String</span></span>|<span data-ttu-id="1108d-141">O nome do fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1108d-141">The manufacturer name of the device.</span></span>|
|<span data-ttu-id="1108d-142">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="1108d-142">appCrashCount</span></span>|<span data-ttu-id="1108d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1108d-143">Int32</span></span>|<span data-ttu-id="1108d-144">O número de falhas do aplicativo para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1108d-144">The number of app crashes for the device.</span></span> <span data-ttu-id="1108d-145">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="1108d-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="1108d-146">crashedAppCount</span><span class="sxs-lookup"><span data-stu-id="1108d-146">crashedAppCount</span></span>|<span data-ttu-id="1108d-147">Int32</span><span class="sxs-lookup"><span data-stu-id="1108d-147">Int32</span></span>|<span data-ttu-id="1108d-148">O número de falhas de aplicativos distintos para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1108d-148">The number of distinct app crashes for the device.</span></span> <span data-ttu-id="1108d-149">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="1108d-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="1108d-150">appHangCount</span><span class="sxs-lookup"><span data-stu-id="1108d-150">appHangCount</span></span>|<span data-ttu-id="1108d-151">Int32</span><span class="sxs-lookup"><span data-stu-id="1108d-151">Int32</span></span>|<span data-ttu-id="1108d-152">O número de bloqueios de aplicativo para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1108d-152">The number of app hangs for the device.</span></span> <span data-ttu-id="1108d-153">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="1108d-153">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="1108d-154">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="1108d-154">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="1108d-155">Int32</span><span class="sxs-lookup"><span data-stu-id="1108d-155">Int32</span></span>|<span data-ttu-id="1108d-156">O tempo médio de falha para o dispositivo em minutos.</span><span class="sxs-lookup"><span data-stu-id="1108d-156">The mean time to failure for the device in minutes.</span></span> <span data-ttu-id="1108d-157">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="1108d-157">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="1108d-158">deviceAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="1108d-158">deviceAppHealthScore</span></span>|<span data-ttu-id="1108d-159">Duplo</span><span class="sxs-lookup"><span data-stu-id="1108d-159">Double</span></span>|<span data-ttu-id="1108d-160">A pontuação de integridade do aplicativo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1108d-160">The app health score of the device.</span></span> <span data-ttu-id="1108d-161">Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="1108d-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="1108d-162">deviceAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="1108d-162">deviceAppHealthStatus</span></span>|<span data-ttu-id="1108d-163">String</span><span class="sxs-lookup"><span data-stu-id="1108d-163">String</span></span>|<span data-ttu-id="1108d-164">O status de integridade geral do aplicativo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1108d-164">The overall app health status of the device.</span></span>|
|<span data-ttu-id="1108d-165">deviceId</span><span class="sxs-lookup"><span data-stu-id="1108d-165">deviceId</span></span>|<span data-ttu-id="1108d-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1108d-166">String</span></span>|<span data-ttu-id="1108d-167">A ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1108d-167">The id of the device.</span></span>|
|<span data-ttu-id="1108d-168">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="1108d-168">deviceDisplayName</span></span>|<span data-ttu-id="1108d-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1108d-169">String</span></span>|<span data-ttu-id="1108d-170">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1108d-170">The name of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="1108d-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="1108d-171">Response</span></span>
<span data-ttu-id="1108d-172">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1108d-172">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1108d-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1108d-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="1108d-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1108d-174">Request</span></span>
<span data-ttu-id="1108d-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1108d-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance/{userExperienceAnalyticsAppHealthDevicePerformanceId}
Content-type: application/json
Content-length: 490

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "appCrashCount": 13,
  "crashedAppCount": 15,
  "appHangCount": 12,
  "meanTimeToFailureInMinutes": 10,
  "deviceAppHealthScore": 6.666666666666667,
  "deviceAppHealthStatus": "Device App Health Status value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="1108d-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="1108d-176">Response</span></span>
<span data-ttu-id="1108d-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1108d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "id": "2c651499-1499-2c65-9914-652c9914652c",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "appCrashCount": 13,
  "crashedAppCount": 15,
  "appHangCount": 12,
  "meanTimeToFailureInMinutes": 10,
  "deviceAppHealthScore": 6.666666666666667,
  "deviceAppHealthStatus": "Device App Health Status value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```




