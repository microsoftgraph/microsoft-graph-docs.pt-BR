---
title: Criar userExperienceAnalyticsAppHealthDevicePerformance
description: Crie um novo objeto userExperienceAnalyticsAppHealthDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b10beeca6d79b8dc596cfa509a5a1a817af9a346
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136129"
---
# <a name="create-userexperienceanalyticsapphealthdeviceperformance"></a><span data-ttu-id="5e87f-103">Criar userExperienceAnalyticsAppHealthDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="5e87f-103">Create userExperienceAnalyticsAppHealthDevicePerformance</span></span>

<span data-ttu-id="5e87f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e87f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e87f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5e87f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e87f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e87f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e87f-107">Crie um novo [objeto userExperienceAnalyticsAppHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="5e87f-107">Create a new [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e87f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e87f-108">Prerequisites</span></span>
<span data-ttu-id="5e87f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e87f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e87f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e87f-111">Permission type</span></span>|<span data-ttu-id="5e87f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e87f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e87f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e87f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e87f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e87f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5e87f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e87f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e87f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e87f-116">Not supported.</span></span>|
|<span data-ttu-id="5e87f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e87f-117">Application</span></span>|<span data-ttu-id="5e87f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e87f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e87f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e87f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
```

## <a name="request-headers"></a><span data-ttu-id="5e87f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e87f-120">Request headers</span></span>
|<span data-ttu-id="5e87f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e87f-121">Header</span></span>|<span data-ttu-id="5e87f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5e87f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e87f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e87f-123">Authorization</span></span>|<span data-ttu-id="5e87f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e87f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e87f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5e87f-125">Accept</span></span>|<span data-ttu-id="5e87f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e87f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e87f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e87f-127">Request body</span></span>
<span data-ttu-id="5e87f-128">No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsAppHealthDevicePerformance.</span><span class="sxs-lookup"><span data-stu-id="5e87f-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthDevicePerformance object.</span></span>

<span data-ttu-id="5e87f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsAppHealthDevicePerformance.</span><span class="sxs-lookup"><span data-stu-id="5e87f-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthDevicePerformance.</span></span>

|<span data-ttu-id="5e87f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e87f-130">Property</span></span>|<span data-ttu-id="5e87f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e87f-131">Type</span></span>|<span data-ttu-id="5e87f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e87f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e87f-133">id</span><span class="sxs-lookup"><span data-stu-id="5e87f-133">id</span></span>|<span data-ttu-id="5e87f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e87f-134">String</span></span>|<span data-ttu-id="5e87f-135">O identificador exclusivo do objeto de desempenho do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="5e87f-135">The unique identifier of the user experience analytics device performance object.</span></span>|
|<span data-ttu-id="5e87f-136">deviceModel</span><span class="sxs-lookup"><span data-stu-id="5e87f-136">deviceModel</span></span>|<span data-ttu-id="5e87f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e87f-137">String</span></span>|<span data-ttu-id="5e87f-138">O nome do modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e87f-138">The model name of the device.</span></span>|
|<span data-ttu-id="5e87f-139">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="5e87f-139">deviceManufacturer</span></span>|<span data-ttu-id="5e87f-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e87f-140">String</span></span>|<span data-ttu-id="5e87f-141">O nome do fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e87f-141">The manufacturer name of the device.</span></span>|
|<span data-ttu-id="5e87f-142">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="5e87f-142">appCrashCount</span></span>|<span data-ttu-id="5e87f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5e87f-143">Int32</span></span>|<span data-ttu-id="5e87f-144">O número de falhas de aplicativo para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e87f-144">The number of app crashes for the device.</span></span> <span data-ttu-id="5e87f-145">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="5e87f-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="5e87f-146">crashedAppCount</span><span class="sxs-lookup"><span data-stu-id="5e87f-146">crashedAppCount</span></span>|<span data-ttu-id="5e87f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="5e87f-147">Int32</span></span>|<span data-ttu-id="5e87f-148">O número de falhas distintas do aplicativo para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e87f-148">The number of distinct app crashes for the device.</span></span> <span data-ttu-id="5e87f-149">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="5e87f-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="5e87f-150">appHangCount</span><span class="sxs-lookup"><span data-stu-id="5e87f-150">appHangCount</span></span>|<span data-ttu-id="5e87f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="5e87f-151">Int32</span></span>|<span data-ttu-id="5e87f-152">O número de travas de aplicativo para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e87f-152">The number of app hangs for the device.</span></span> <span data-ttu-id="5e87f-153">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="5e87f-153">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="5e87f-154">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="5e87f-154">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="5e87f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="5e87f-155">Int32</span></span>|<span data-ttu-id="5e87f-156">O tempo de falha média do dispositivo em minutos.</span><span class="sxs-lookup"><span data-stu-id="5e87f-156">The mean time to failure for the device in minutes.</span></span> <span data-ttu-id="5e87f-157">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="5e87f-157">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="5e87f-158">deviceAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="5e87f-158">deviceAppHealthScore</span></span>|<span data-ttu-id="5e87f-159">Duplo</span><span class="sxs-lookup"><span data-stu-id="5e87f-159">Double</span></span>|<span data-ttu-id="5e87f-160">A pontuação de saúde do aplicativo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e87f-160">The app health score of the device.</span></span> <span data-ttu-id="5e87f-161">Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="5e87f-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="5e87f-162">deviceAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="5e87f-162">deviceAppHealthStatus</span></span>|<span data-ttu-id="5e87f-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e87f-163">String</span></span>|<span data-ttu-id="5e87f-164">O status geral da saúde do aplicativo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e87f-164">The overall app health status of the device.</span></span>|
|<span data-ttu-id="5e87f-165">deviceId</span><span class="sxs-lookup"><span data-stu-id="5e87f-165">deviceId</span></span>|<span data-ttu-id="5e87f-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e87f-166">String</span></span>|<span data-ttu-id="5e87f-167">A id do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e87f-167">The id of the device.</span></span>|
|<span data-ttu-id="5e87f-168">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="5e87f-168">deviceDisplayName</span></span>|<span data-ttu-id="5e87f-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e87f-169">String</span></span>|<span data-ttu-id="5e87f-170">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e87f-170">The name of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="5e87f-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e87f-171">Response</span></span>
<span data-ttu-id="5e87f-172">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e87f-172">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e87f-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e87f-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e87f-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e87f-174">Request</span></span>
<span data-ttu-id="5e87f-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e87f-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
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

### <a name="response"></a><span data-ttu-id="5e87f-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e87f-176">Response</span></span>
<span data-ttu-id="5e87f-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e87f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




