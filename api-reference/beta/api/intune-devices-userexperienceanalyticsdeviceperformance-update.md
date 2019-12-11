---
title: Atualizar userExperienceAnalyticsDevicePerformance
description: Atualiza as propriedades de um objeto userExperienceAnalyticsDevicePerformance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f125ce0beeb76bd8d3a6ef098b8a70e280c6b1a9
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944474"
---
# <a name="update-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="e1788-103">Atualizar userExperienceAnalyticsDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="e1788-103">Update userExperienceAnalyticsDevicePerformance</span></span>

> <span data-ttu-id="e1788-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1788-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1788-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1788-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1788-106">Atualiza as propriedades de um objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="e1788-106">Update the properties of a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1788-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1788-107">Prerequisites</span></span>
<span data-ttu-id="e1788-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1788-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1788-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1788-110">Permission type</span></span>|<span data-ttu-id="e1788-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1788-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1788-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1788-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1788-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1788-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e1788-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1788-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1788-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1788-115">Not supported.</span></span>|
|<span data-ttu-id="e1788-116">Application</span><span class="sxs-lookup"><span data-stu-id="e1788-116">Application</span></span>|<span data-ttu-id="e1788-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1788-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1788-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1788-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="e1788-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1788-119">Request headers</span></span>
|<span data-ttu-id="e1788-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1788-120">Header</span></span>|<span data-ttu-id="e1788-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e1788-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1788-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1788-122">Authorization</span></span>|<span data-ttu-id="e1788-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1788-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1788-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1788-124">Accept</span></span>|<span data-ttu-id="e1788-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e1788-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1788-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1788-126">Request body</span></span>
<span data-ttu-id="e1788-127">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="e1788-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

<span data-ttu-id="e1788-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span><span class="sxs-lookup"><span data-stu-id="e1788-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span></span>

|<span data-ttu-id="e1788-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1788-129">Property</span></span>|<span data-ttu-id="e1788-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1788-130">Type</span></span>|<span data-ttu-id="e1788-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1788-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1788-132">id</span><span class="sxs-lookup"><span data-stu-id="e1788-132">id</span></span>|<span data-ttu-id="e1788-133">String</span><span class="sxs-lookup"><span data-stu-id="e1788-133">String</span></span>|<span data-ttu-id="e1788-134">O identificador exclusivo do dispositivo de desempenho de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1788-134">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="e1788-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="e1788-135">deviceName</span></span>|<span data-ttu-id="e1788-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1788-136">String</span></span>|<span data-ttu-id="e1788-137">O nome do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1788-137">The user experience analytics device name.</span></span>|
|<span data-ttu-id="e1788-138">modelo</span><span class="sxs-lookup"><span data-stu-id="e1788-138">model</span></span>|<span data-ttu-id="e1788-139">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e1788-139">String</span></span>|<span data-ttu-id="e1788-140">O modelo de dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1788-140">The user experience analytics device model.</span></span>|
|<span data-ttu-id="e1788-141">fabricante</span><span class="sxs-lookup"><span data-stu-id="e1788-141">manufacturer</span></span>|<span data-ttu-id="e1788-142">String</span><span class="sxs-lookup"><span data-stu-id="e1788-142">String</span></span>|<span data-ttu-id="e1788-143">O fabricante do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1788-143">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="e1788-144">diskType</span><span class="sxs-lookup"><span data-stu-id="e1788-144">diskType</span></span>|[<span data-ttu-id="e1788-145">diskType</span><span class="sxs-lookup"><span data-stu-id="e1788-145">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="e1788-146">O tipo de disco do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1788-146">The user experience analytics device disk type.</span></span> <span data-ttu-id="e1788-147">Os valores possíveis são: `unkown`, `hdd`, `ssd`.</span><span class="sxs-lookup"><span data-stu-id="e1788-147">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="e1788-148">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="e1788-148">operatingSystemVersion</span></span>|<span data-ttu-id="e1788-149">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e1788-149">String</span></span>|<span data-ttu-id="e1788-150">A versão do sistema operacional do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1788-150">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="e1788-151">bootScore</span><span class="sxs-lookup"><span data-stu-id="e1788-151">bootScore</span></span>|<span data-ttu-id="e1788-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e1788-152">Int32</span></span>|<span data-ttu-id="e1788-153">A pontuação de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1788-153">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="e1788-154">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="e1788-154">coreBootTimeInMs</span></span>|<span data-ttu-id="e1788-155">Int32</span><span class="sxs-lookup"><span data-stu-id="e1788-155">Int32</span></span>|<span data-ttu-id="e1788-156">O tempo de inicialização do núcleo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="e1788-156">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="e1788-157">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="e1788-157">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="e1788-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e1788-158">Int32</span></span>|<span data-ttu-id="e1788-159">O tempo de inicialização da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="e1788-159">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="e1788-160">healthStatus</span><span class="sxs-lookup"><span data-stu-id="e1788-160">healthStatus</span></span>|[<span data-ttu-id="e1788-161">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="e1788-161">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="e1788-162">O estado de integridade do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1788-162">The health state of the user experience analytics device.</span></span> <span data-ttu-id="e1788-163">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="e1788-163">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="e1788-164">loginScore</span><span class="sxs-lookup"><span data-stu-id="e1788-164">loginScore</span></span>|<span data-ttu-id="e1788-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e1788-165">Int32</span></span>|<span data-ttu-id="e1788-166">O placar de logon do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1788-166">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="e1788-167">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="e1788-167">coreLoginTimeInMs</span></span>|<span data-ttu-id="e1788-168">Int32</span><span class="sxs-lookup"><span data-stu-id="e1788-168">Int32</span></span>|<span data-ttu-id="e1788-169">O tempo de logon do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="e1788-169">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="e1788-170">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="e1788-170">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="e1788-171">Int32</span><span class="sxs-lookup"><span data-stu-id="e1788-171">Int32</span></span>|<span data-ttu-id="e1788-172">O tempo de logon da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="e1788-172">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="e1788-173">deviceCount</span><span class="sxs-lookup"><span data-stu-id="e1788-173">deviceCount</span></span>|<span data-ttu-id="e1788-174">Int64</span><span class="sxs-lookup"><span data-stu-id="e1788-174">Int64</span></span>|<span data-ttu-id="e1788-175">Contagem de dispositivos resumida da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1788-175">User experience analytics summarized device count.</span></span>|



## <a name="response"></a><span data-ttu-id="e1788-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1788-176">Response</span></span>
<span data-ttu-id="e1788-177">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1788-177">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1788-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1788-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1788-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1788-179">Request</span></span>
<span data-ttu-id="e1788-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1788-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
Content-type: application/json
Content-length: 494

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
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="e1788-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1788-181">Response</span></span>
<span data-ttu-id="e1788-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1788-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

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
```





