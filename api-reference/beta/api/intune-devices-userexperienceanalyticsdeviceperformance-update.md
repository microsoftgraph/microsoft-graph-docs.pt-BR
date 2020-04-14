---
title: Atualizar userExperienceAnalyticsDevicePerformance
description: Atualiza as propriedades de um objeto userExperienceAnalyticsDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75719a81a38e70cfbfc487710358a9f75e866690
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43379641"
---
# <a name="update-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="a1b5c-103">Atualizar userExperienceAnalyticsDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="a1b5c-103">Update userExperienceAnalyticsDevicePerformance</span></span>

<span data-ttu-id="a1b5c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1b5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1b5c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1b5c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1b5c-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="a1b5c-107">Update the properties of a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1b5c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1b5c-108">Prerequisites</span></span>
<span data-ttu-id="a1b5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1b5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1b5c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1b5c-111">Permission type</span></span>|<span data-ttu-id="a1b5c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1b5c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1b5c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1b5c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1b5c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1b5c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a1b5c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1b5c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1b5c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-116">Not supported.</span></span>|
|<span data-ttu-id="a1b5c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1b5c-117">Application</span></span>|<span data-ttu-id="a1b5c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1b5c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1b5c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1b5c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="a1b5c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1b5c-120">Request headers</span></span>
|<span data-ttu-id="a1b5c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1b5c-121">Header</span></span>|<span data-ttu-id="a1b5c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a1b5c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1b5c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1b5c-123">Authorization</span></span>|<span data-ttu-id="a1b5c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1b5c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1b5c-125">Accept</span></span>|<span data-ttu-id="a1b5c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1b5c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1b5c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1b5c-127">Request body</span></span>
<span data-ttu-id="a1b5c-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="a1b5c-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

<span data-ttu-id="a1b5c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span><span class="sxs-lookup"><span data-stu-id="a1b5c-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span></span>

|<span data-ttu-id="a1b5c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1b5c-130">Property</span></span>|<span data-ttu-id="a1b5c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1b5c-131">Type</span></span>|<span data-ttu-id="a1b5c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1b5c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1b5c-133">id</span><span class="sxs-lookup"><span data-stu-id="a1b5c-133">id</span></span>|<span data-ttu-id="a1b5c-134">String</span><span class="sxs-lookup"><span data-stu-id="a1b5c-134">String</span></span>|<span data-ttu-id="a1b5c-135">O identificador exclusivo do dispositivo de desempenho de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-135">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="a1b5c-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="a1b5c-136">deviceName</span></span>|<span data-ttu-id="a1b5c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1b5c-137">String</span></span>|<span data-ttu-id="a1b5c-138">O nome do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="a1b5c-139">modelo</span><span class="sxs-lookup"><span data-stu-id="a1b5c-139">model</span></span>|<span data-ttu-id="a1b5c-140">String</span><span class="sxs-lookup"><span data-stu-id="a1b5c-140">String</span></span>|<span data-ttu-id="a1b5c-141">O modelo de dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="a1b5c-142">fabricante</span><span class="sxs-lookup"><span data-stu-id="a1b5c-142">manufacturer</span></span>|<span data-ttu-id="a1b5c-143">String</span><span class="sxs-lookup"><span data-stu-id="a1b5c-143">String</span></span>|<span data-ttu-id="a1b5c-144">O fabricante do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="a1b5c-145">diskType</span><span class="sxs-lookup"><span data-stu-id="a1b5c-145">diskType</span></span>|[<span data-ttu-id="a1b5c-146">diskType</span><span class="sxs-lookup"><span data-stu-id="a1b5c-146">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="a1b5c-147">O tipo de disco do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-147">The user experience analytics device disk type.</span></span> <span data-ttu-id="a1b5c-148">Os valores possíveis são: `unkown`, `hdd`, `ssd`.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-148">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="a1b5c-149">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="a1b5c-149">operatingSystemVersion</span></span>|<span data-ttu-id="a1b5c-150">String</span><span class="sxs-lookup"><span data-stu-id="a1b5c-150">String</span></span>|<span data-ttu-id="a1b5c-151">A versão do sistema operacional do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-151">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="a1b5c-152">bootScore</span><span class="sxs-lookup"><span data-stu-id="a1b5c-152">bootScore</span></span>|<span data-ttu-id="a1b5c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a1b5c-153">Int32</span></span>|<span data-ttu-id="a1b5c-154">A pontuação de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-154">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="a1b5c-155">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a1b5c-155">coreBootTimeInMs</span></span>|<span data-ttu-id="a1b5c-156">Int32</span><span class="sxs-lookup"><span data-stu-id="a1b5c-156">Int32</span></span>|<span data-ttu-id="a1b5c-157">O tempo de inicialização do núcleo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-157">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="a1b5c-158">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a1b5c-158">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="a1b5c-159">Int32</span><span class="sxs-lookup"><span data-stu-id="a1b5c-159">Int32</span></span>|<span data-ttu-id="a1b5c-160">O tempo de inicialização da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-160">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="a1b5c-161">healthStatus</span><span class="sxs-lookup"><span data-stu-id="a1b5c-161">healthStatus</span></span>|[<span data-ttu-id="a1b5c-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="a1b5c-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="a1b5c-163">O estado de integridade do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-163">The health state of the user experience analytics device.</span></span> <span data-ttu-id="a1b5c-164">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="a1b5c-165">loginScore</span><span class="sxs-lookup"><span data-stu-id="a1b5c-165">loginScore</span></span>|<span data-ttu-id="a1b5c-166">Int32</span><span class="sxs-lookup"><span data-stu-id="a1b5c-166">Int32</span></span>|<span data-ttu-id="a1b5c-167">O placar de logon do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-167">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="a1b5c-168">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a1b5c-168">coreLoginTimeInMs</span></span>|<span data-ttu-id="a1b5c-169">Int32</span><span class="sxs-lookup"><span data-stu-id="a1b5c-169">Int32</span></span>|<span data-ttu-id="a1b5c-170">O tempo de logon do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-170">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="a1b5c-171">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a1b5c-171">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="a1b5c-172">Int32</span><span class="sxs-lookup"><span data-stu-id="a1b5c-172">Int32</span></span>|<span data-ttu-id="a1b5c-173">O tempo de logon da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-173">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="a1b5c-174">deviceCount</span><span class="sxs-lookup"><span data-stu-id="a1b5c-174">deviceCount</span></span>|<span data-ttu-id="a1b5c-175">Int64</span><span class="sxs-lookup"><span data-stu-id="a1b5c-175">Int64</span></span>|<span data-ttu-id="a1b5c-176">Contagem de dispositivos resumida da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-176">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="a1b5c-177">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a1b5c-177">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="a1b5c-178">Int32</span><span class="sxs-lookup"><span data-stu-id="a1b5c-178">Int32</span></span>|<span data-ttu-id="a1b5c-179">O tempo de resposta da análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-179">The user experience analytics responsive desktop time in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="a1b5c-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1b5c-180">Response</span></span>
<span data-ttu-id="a1b5c-181">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-181">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1b5c-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1b5c-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1b5c-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1b5c-183">Request</span></span>
<span data-ttu-id="a1b5c-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
Content-type: application/json
Content-length: 529

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
  "responsiveDesktopTimeInMs": 9
}
```

### <a name="response"></a><span data-ttu-id="a1b5c-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1b5c-185">Response</span></span>
<span data-ttu-id="a1b5c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1b5c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 578

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
  "responsiveDesktopTimeInMs": 9
}
```



