---
title: Atualizar userExperienceAnalyticsDevicePerformance
description: Atualiza as propriedades de um objeto userExperienceAnalyticsDevicePerformance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3d116950d788c57c19ce153605d1dd88909e5be9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468387"
---
# <a name="update-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="a3d2e-103">Atualizar userExperienceAnalyticsDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="a3d2e-103">Update userExperienceAnalyticsDevicePerformance</span></span>

<span data-ttu-id="a3d2e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a3d2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3d2e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3d2e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3d2e-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="a3d2e-107">Update the properties of a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3d2e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a3d2e-108">Prerequisites</span></span>
<span data-ttu-id="a3d2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3d2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3d2e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3d2e-111">Permission type</span></span>|<span data-ttu-id="a3d2e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a3d2e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3d2e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3d2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3d2e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3d2e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a3d2e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3d2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3d2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-116">Not supported.</span></span>|
|<span data-ttu-id="a3d2e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3d2e-117">Application</span></span>|<span data-ttu-id="a3d2e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3d2e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3d2e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3d2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="a3d2e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3d2e-120">Request headers</span></span>
|<span data-ttu-id="a3d2e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3d2e-121">Header</span></span>|<span data-ttu-id="a3d2e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a3d2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3d2e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3d2e-123">Authorization</span></span>|<span data-ttu-id="a3d2e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3d2e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a3d2e-125">Accept</span></span>|<span data-ttu-id="a3d2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3d2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3d2e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3d2e-127">Request body</span></span>
<span data-ttu-id="a3d2e-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="a3d2e-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

<span data-ttu-id="a3d2e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span><span class="sxs-lookup"><span data-stu-id="a3d2e-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span></span>

|<span data-ttu-id="a3d2e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3d2e-130">Property</span></span>|<span data-ttu-id="a3d2e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3d2e-131">Type</span></span>|<span data-ttu-id="a3d2e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3d2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3d2e-133">id</span><span class="sxs-lookup"><span data-stu-id="a3d2e-133">id</span></span>|<span data-ttu-id="a3d2e-134">String</span><span class="sxs-lookup"><span data-stu-id="a3d2e-134">String</span></span>|<span data-ttu-id="a3d2e-135">O identificador exclusivo do dispositivo de desempenho de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-135">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="a3d2e-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="a3d2e-136">deviceName</span></span>|<span data-ttu-id="a3d2e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3d2e-137">String</span></span>|<span data-ttu-id="a3d2e-138">O nome do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="a3d2e-139">modelo</span><span class="sxs-lookup"><span data-stu-id="a3d2e-139">model</span></span>|<span data-ttu-id="a3d2e-140">String</span><span class="sxs-lookup"><span data-stu-id="a3d2e-140">String</span></span>|<span data-ttu-id="a3d2e-141">O modelo de dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="a3d2e-142">fabricante</span><span class="sxs-lookup"><span data-stu-id="a3d2e-142">manufacturer</span></span>|<span data-ttu-id="a3d2e-143">String</span><span class="sxs-lookup"><span data-stu-id="a3d2e-143">String</span></span>|<span data-ttu-id="a3d2e-144">O fabricante do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="a3d2e-145">diskType</span><span class="sxs-lookup"><span data-stu-id="a3d2e-145">diskType</span></span>|[<span data-ttu-id="a3d2e-146">diskType</span><span class="sxs-lookup"><span data-stu-id="a3d2e-146">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="a3d2e-147">O tipo de disco do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-147">The user experience analytics device disk type.</span></span> <span data-ttu-id="a3d2e-148">Os valores possíveis são: `unkown`, `hdd`, `ssd`.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-148">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="a3d2e-149">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="a3d2e-149">operatingSystemVersion</span></span>|<span data-ttu-id="a3d2e-150">String</span><span class="sxs-lookup"><span data-stu-id="a3d2e-150">String</span></span>|<span data-ttu-id="a3d2e-151">A versão do sistema operacional do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-151">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="a3d2e-152">bootScore</span><span class="sxs-lookup"><span data-stu-id="a3d2e-152">bootScore</span></span>|<span data-ttu-id="a3d2e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a3d2e-153">Int32</span></span>|<span data-ttu-id="a3d2e-154">A pontuação de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-154">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="a3d2e-155">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a3d2e-155">coreBootTimeInMs</span></span>|<span data-ttu-id="a3d2e-156">Int32</span><span class="sxs-lookup"><span data-stu-id="a3d2e-156">Int32</span></span>|<span data-ttu-id="a3d2e-157">O tempo de inicialização do núcleo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-157">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="a3d2e-158">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a3d2e-158">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="a3d2e-159">Int32</span><span class="sxs-lookup"><span data-stu-id="a3d2e-159">Int32</span></span>|<span data-ttu-id="a3d2e-160">O tempo de inicialização da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-160">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="a3d2e-161">healthStatus</span><span class="sxs-lookup"><span data-stu-id="a3d2e-161">healthStatus</span></span>|[<span data-ttu-id="a3d2e-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="a3d2e-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="a3d2e-163">O estado de integridade do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-163">The health state of the user experience analytics device.</span></span> <span data-ttu-id="a3d2e-164">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="a3d2e-165">loginScore</span><span class="sxs-lookup"><span data-stu-id="a3d2e-165">loginScore</span></span>|<span data-ttu-id="a3d2e-166">Int32</span><span class="sxs-lookup"><span data-stu-id="a3d2e-166">Int32</span></span>|<span data-ttu-id="a3d2e-167">O placar de logon do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-167">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="a3d2e-168">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a3d2e-168">coreLoginTimeInMs</span></span>|<span data-ttu-id="a3d2e-169">Int32</span><span class="sxs-lookup"><span data-stu-id="a3d2e-169">Int32</span></span>|<span data-ttu-id="a3d2e-170">O tempo de logon do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-170">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="a3d2e-171">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a3d2e-171">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="a3d2e-172">Int32</span><span class="sxs-lookup"><span data-stu-id="a3d2e-172">Int32</span></span>|<span data-ttu-id="a3d2e-173">O tempo de logon da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-173">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="a3d2e-174">deviceCount</span><span class="sxs-lookup"><span data-stu-id="a3d2e-174">deviceCount</span></span>|<span data-ttu-id="a3d2e-175">Int64</span><span class="sxs-lookup"><span data-stu-id="a3d2e-175">Int64</span></span>|<span data-ttu-id="a3d2e-176">Contagem de dispositivos resumida da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-176">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="a3d2e-177">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a3d2e-177">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="a3d2e-178">Int32</span><span class="sxs-lookup"><span data-stu-id="a3d2e-178">Int32</span></span>|<span data-ttu-id="a3d2e-179">O tempo de resposta da análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-179">The user experience analytics responsive desktop time in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="a3d2e-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3d2e-180">Response</span></span>
<span data-ttu-id="a3d2e-181">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-181">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3d2e-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3d2e-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3d2e-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3d2e-183">Request</span></span>
<span data-ttu-id="a3d2e-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a3d2e-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3d2e-185">Response</span></span>
<span data-ttu-id="a3d2e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3d2e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





