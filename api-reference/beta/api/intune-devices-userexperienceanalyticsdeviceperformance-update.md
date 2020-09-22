---
title: Atualizar userExperienceAnalyticsDevicePerformance
description: Atualiza as propriedades de um objeto userExperienceAnalyticsDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aecb06c539644770d2478533e6c66c46324ee09c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050567"
---
# <a name="update-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="9dd5d-103">Atualizar userExperienceAnalyticsDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="9dd5d-103">Update userExperienceAnalyticsDevicePerformance</span></span>

<span data-ttu-id="9dd5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9dd5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9dd5d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9dd5d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dd5d-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="9dd5d-107">Update the properties of a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9dd5d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9dd5d-108">Prerequisites</span></span>
<span data-ttu-id="9dd5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dd5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dd5d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9dd5d-111">Permission type</span></span>|<span data-ttu-id="9dd5d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9dd5d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9dd5d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9dd5d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9dd5d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dd5d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9dd5d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9dd5d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9dd5d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-116">Not supported.</span></span>|
|<span data-ttu-id="9dd5d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9dd5d-117">Application</span></span>|<span data-ttu-id="9dd5d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dd5d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9dd5d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9dd5d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="9dd5d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9dd5d-120">Request headers</span></span>
|<span data-ttu-id="9dd5d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9dd5d-121">Header</span></span>|<span data-ttu-id="9dd5d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9dd5d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9dd5d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9dd5d-123">Authorization</span></span>|<span data-ttu-id="9dd5d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9dd5d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9dd5d-125">Accept</span></span>|<span data-ttu-id="9dd5d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9dd5d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dd5d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9dd5d-127">Request body</span></span>
<span data-ttu-id="9dd5d-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="9dd5d-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

<span data-ttu-id="9dd5d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span><span class="sxs-lookup"><span data-stu-id="9dd5d-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span></span>

|<span data-ttu-id="9dd5d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9dd5d-130">Property</span></span>|<span data-ttu-id="9dd5d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9dd5d-131">Type</span></span>|<span data-ttu-id="9dd5d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9dd5d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dd5d-133">id</span><span class="sxs-lookup"><span data-stu-id="9dd5d-133">id</span></span>|<span data-ttu-id="9dd5d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9dd5d-134">String</span></span>|<span data-ttu-id="9dd5d-135">O identificador exclusivo do dispositivo de desempenho de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-135">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="9dd5d-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="9dd5d-136">deviceName</span></span>|<span data-ttu-id="9dd5d-137">String</span><span class="sxs-lookup"><span data-stu-id="9dd5d-137">String</span></span>|<span data-ttu-id="9dd5d-138">O nome do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="9dd5d-139">modelo</span><span class="sxs-lookup"><span data-stu-id="9dd5d-139">model</span></span>|<span data-ttu-id="9dd5d-140">String</span><span class="sxs-lookup"><span data-stu-id="9dd5d-140">String</span></span>|<span data-ttu-id="9dd5d-141">O modelo de dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="9dd5d-142">fabricante</span><span class="sxs-lookup"><span data-stu-id="9dd5d-142">manufacturer</span></span>|<span data-ttu-id="9dd5d-143">String</span><span class="sxs-lookup"><span data-stu-id="9dd5d-143">String</span></span>|<span data-ttu-id="9dd5d-144">O fabricante do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="9dd5d-145">diskType</span><span class="sxs-lookup"><span data-stu-id="9dd5d-145">diskType</span></span>|[<span data-ttu-id="9dd5d-146">diskType</span><span class="sxs-lookup"><span data-stu-id="9dd5d-146">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="9dd5d-147">O tipo de disco do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-147">The user experience analytics device disk type.</span></span> <span data-ttu-id="9dd5d-148">Os valores possíveis são: `unkown`, `hdd`, `ssd`.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-148">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="9dd5d-149">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="9dd5d-149">operatingSystemVersion</span></span>|<span data-ttu-id="9dd5d-150">String</span><span class="sxs-lookup"><span data-stu-id="9dd5d-150">String</span></span>|<span data-ttu-id="9dd5d-151">A versão do sistema operacional do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-151">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="9dd5d-152">bootScore</span><span class="sxs-lookup"><span data-stu-id="9dd5d-152">bootScore</span></span>|<span data-ttu-id="9dd5d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="9dd5d-153">Int32</span></span>|<span data-ttu-id="9dd5d-154">A pontuação de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-154">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="9dd5d-155">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9dd5d-155">coreBootTimeInMs</span></span>|<span data-ttu-id="9dd5d-156">Int32</span><span class="sxs-lookup"><span data-stu-id="9dd5d-156">Int32</span></span>|<span data-ttu-id="9dd5d-157">O tempo de inicialização do núcleo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-157">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="9dd5d-158">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9dd5d-158">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="9dd5d-159">Int32</span><span class="sxs-lookup"><span data-stu-id="9dd5d-159">Int32</span></span>|<span data-ttu-id="9dd5d-160">O tempo de inicialização da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-160">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="9dd5d-161">healthStatus</span><span class="sxs-lookup"><span data-stu-id="9dd5d-161">healthStatus</span></span>|[<span data-ttu-id="9dd5d-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="9dd5d-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="9dd5d-163">O estado de integridade do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-163">The health state of the user experience analytics device.</span></span> <span data-ttu-id="9dd5d-164">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="9dd5d-165">loginScore</span><span class="sxs-lookup"><span data-stu-id="9dd5d-165">loginScore</span></span>|<span data-ttu-id="9dd5d-166">Int32</span><span class="sxs-lookup"><span data-stu-id="9dd5d-166">Int32</span></span>|<span data-ttu-id="9dd5d-167">O placar de logon do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-167">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="9dd5d-168">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9dd5d-168">coreLoginTimeInMs</span></span>|<span data-ttu-id="9dd5d-169">Int32</span><span class="sxs-lookup"><span data-stu-id="9dd5d-169">Int32</span></span>|<span data-ttu-id="9dd5d-170">O tempo de logon do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-170">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="9dd5d-171">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9dd5d-171">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="9dd5d-172">Int32</span><span class="sxs-lookup"><span data-stu-id="9dd5d-172">Int32</span></span>|<span data-ttu-id="9dd5d-173">O tempo de logon da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-173">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="9dd5d-174">deviceCount</span><span class="sxs-lookup"><span data-stu-id="9dd5d-174">deviceCount</span></span>|<span data-ttu-id="9dd5d-175">Int64</span><span class="sxs-lookup"><span data-stu-id="9dd5d-175">Int64</span></span>|<span data-ttu-id="9dd5d-176">Contagem de dispositivos resumida da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-176">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="9dd5d-177">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9dd5d-177">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="9dd5d-178">Int32</span><span class="sxs-lookup"><span data-stu-id="9dd5d-178">Int32</span></span>|<span data-ttu-id="9dd5d-179">O tempo de resposta da análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-179">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="9dd5d-180">blueScreenCount</span><span class="sxs-lookup"><span data-stu-id="9dd5d-180">blueScreenCount</span></span>|<span data-ttu-id="9dd5d-181">Int32</span><span class="sxs-lookup"><span data-stu-id="9dd5d-181">Int32</span></span>|<span data-ttu-id="9dd5d-182">Número de telas azuis nos últimos 14 dias.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-182">Number of Blue Screens in the last 14 days.</span></span> <span data-ttu-id="9dd5d-183">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="9dd5d-183">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="9dd5d-184">restartCount</span><span class="sxs-lookup"><span data-stu-id="9dd5d-184">restartCount</span></span>|<span data-ttu-id="9dd5d-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9dd5d-185">Int32</span></span>|<span data-ttu-id="9dd5d-186">Número de reinicializações nos últimos 14 dias.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-186">Number of Restarts in the last 14 days.</span></span> <span data-ttu-id="9dd5d-187">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="9dd5d-187">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="9dd5d-188">averageBlueScreens</span><span class="sxs-lookup"><span data-stu-id="9dd5d-188">averageBlueScreens</span></span>|<span data-ttu-id="9dd5d-189">Duplo</span><span class="sxs-lookup"><span data-stu-id="9dd5d-189">Double</span></span>|<span data-ttu-id="9dd5d-190">Média (média) número de telas azuis por dispositivo nos últimos 14 dias.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-190">Average (mean) number of Blue Screens per device in the last 14 days.</span></span> <span data-ttu-id="9dd5d-191">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="9dd5d-191">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="9dd5d-192">averageRestarts</span><span class="sxs-lookup"><span data-stu-id="9dd5d-192">averageRestarts</span></span>|<span data-ttu-id="9dd5d-193">Duplo</span><span class="sxs-lookup"><span data-stu-id="9dd5d-193">Double</span></span>|<span data-ttu-id="9dd5d-194">Média (média) número de reinicializações por dispositivo nos últimos 14 dias.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-194">Average (mean) number of Restarts per device in the last 14 days.</span></span> <span data-ttu-id="9dd5d-195">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="9dd5d-195">Valid values 0 to 9999999</span></span>|



## <a name="response"></a><span data-ttu-id="9dd5d-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="9dd5d-196">Response</span></span>
<span data-ttu-id="9dd5d-197">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-197">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dd5d-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9dd5d-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="9dd5d-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9dd5d-199">Request</span></span>
<span data-ttu-id="9dd5d-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
Content-type: application/json
Content-length: 635

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
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
```

### <a name="response"></a><span data-ttu-id="9dd5d-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="9dd5d-201">Response</span></span>
<span data-ttu-id="9dd5d-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9dd5d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 684

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
```






