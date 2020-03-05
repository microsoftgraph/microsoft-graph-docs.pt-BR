---
title: Criar userExperienceAnalyticsDevicePerformance
description: Criar um novo objeto userExperienceAnalyticsDevicePerformance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 061f42f824f05eb9012aeee9641d5d545a9b87cd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468436"
---
# <a name="create-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="6d924-103">Criar userExperienceAnalyticsDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="6d924-103">Create userExperienceAnalyticsDevicePerformance</span></span>

<span data-ttu-id="6d924-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6d924-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d924-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d924-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d924-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d924-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d924-107">Criar um novo objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="6d924-107">Create a new [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d924-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6d924-108">Prerequisites</span></span>
<span data-ttu-id="6d924-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d924-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d924-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d924-111">Permission type</span></span>|<span data-ttu-id="6d924-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6d924-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d924-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d924-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d924-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d924-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6d924-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d924-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d924-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d924-116">Not supported.</span></span>|
|<span data-ttu-id="6d924-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d924-117">Application</span></span>|<span data-ttu-id="6d924-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d924-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d924-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d924-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDevicePerformance
```

## <a name="request-headers"></a><span data-ttu-id="6d924-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d924-120">Request headers</span></span>
|<span data-ttu-id="6d924-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d924-121">Header</span></span>|<span data-ttu-id="6d924-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6d924-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d924-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d924-123">Authorization</span></span>|<span data-ttu-id="6d924-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d924-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d924-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d924-125">Accept</span></span>|<span data-ttu-id="6d924-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d924-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d924-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d924-127">Request body</span></span>
<span data-ttu-id="6d924-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsDevicePerformance.</span><span class="sxs-lookup"><span data-stu-id="6d924-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDevicePerformance object.</span></span>

<span data-ttu-id="6d924-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsDevicePerformance.</span><span class="sxs-lookup"><span data-stu-id="6d924-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDevicePerformance.</span></span>

|<span data-ttu-id="6d924-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d924-130">Property</span></span>|<span data-ttu-id="6d924-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d924-131">Type</span></span>|<span data-ttu-id="6d924-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d924-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d924-133">id</span><span class="sxs-lookup"><span data-stu-id="6d924-133">id</span></span>|<span data-ttu-id="6d924-134">String</span><span class="sxs-lookup"><span data-stu-id="6d924-134">String</span></span>|<span data-ttu-id="6d924-135">O identificador exclusivo do dispositivo de desempenho de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="6d924-135">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="6d924-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="6d924-136">deviceName</span></span>|<span data-ttu-id="6d924-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d924-137">String</span></span>|<span data-ttu-id="6d924-138">O nome do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="6d924-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="6d924-139">modelo</span><span class="sxs-lookup"><span data-stu-id="6d924-139">model</span></span>|<span data-ttu-id="6d924-140">String</span><span class="sxs-lookup"><span data-stu-id="6d924-140">String</span></span>|<span data-ttu-id="6d924-141">O modelo de dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="6d924-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="6d924-142">fabricante</span><span class="sxs-lookup"><span data-stu-id="6d924-142">manufacturer</span></span>|<span data-ttu-id="6d924-143">String</span><span class="sxs-lookup"><span data-stu-id="6d924-143">String</span></span>|<span data-ttu-id="6d924-144">O fabricante do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="6d924-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="6d924-145">diskType</span><span class="sxs-lookup"><span data-stu-id="6d924-145">diskType</span></span>|[<span data-ttu-id="6d924-146">diskType</span><span class="sxs-lookup"><span data-stu-id="6d924-146">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="6d924-147">O tipo de disco do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="6d924-147">The user experience analytics device disk type.</span></span> <span data-ttu-id="6d924-148">Os valores possíveis são: `unkown`, `hdd`, `ssd`.</span><span class="sxs-lookup"><span data-stu-id="6d924-148">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="6d924-149">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="6d924-149">operatingSystemVersion</span></span>|<span data-ttu-id="6d924-150">String</span><span class="sxs-lookup"><span data-stu-id="6d924-150">String</span></span>|<span data-ttu-id="6d924-151">A versão do sistema operacional do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="6d924-151">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="6d924-152">bootScore</span><span class="sxs-lookup"><span data-stu-id="6d924-152">bootScore</span></span>|<span data-ttu-id="6d924-153">Int32</span><span class="sxs-lookup"><span data-stu-id="6d924-153">Int32</span></span>|<span data-ttu-id="6d924-154">A pontuação de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="6d924-154">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="6d924-155">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="6d924-155">coreBootTimeInMs</span></span>|<span data-ttu-id="6d924-156">Int32</span><span class="sxs-lookup"><span data-stu-id="6d924-156">Int32</span></span>|<span data-ttu-id="6d924-157">O tempo de inicialização do núcleo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="6d924-157">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="6d924-158">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="6d924-158">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="6d924-159">Int32</span><span class="sxs-lookup"><span data-stu-id="6d924-159">Int32</span></span>|<span data-ttu-id="6d924-160">O tempo de inicialização da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="6d924-160">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="6d924-161">healthStatus</span><span class="sxs-lookup"><span data-stu-id="6d924-161">healthStatus</span></span>|[<span data-ttu-id="6d924-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="6d924-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="6d924-163">O estado de integridade do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="6d924-163">The health state of the user experience analytics device.</span></span> <span data-ttu-id="6d924-164">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="6d924-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="6d924-165">loginScore</span><span class="sxs-lookup"><span data-stu-id="6d924-165">loginScore</span></span>|<span data-ttu-id="6d924-166">Int32</span><span class="sxs-lookup"><span data-stu-id="6d924-166">Int32</span></span>|<span data-ttu-id="6d924-167">O placar de logon do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="6d924-167">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="6d924-168">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="6d924-168">coreLoginTimeInMs</span></span>|<span data-ttu-id="6d924-169">Int32</span><span class="sxs-lookup"><span data-stu-id="6d924-169">Int32</span></span>|<span data-ttu-id="6d924-170">O tempo de logon do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="6d924-170">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="6d924-171">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="6d924-171">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="6d924-172">Int32</span><span class="sxs-lookup"><span data-stu-id="6d924-172">Int32</span></span>|<span data-ttu-id="6d924-173">O tempo de logon da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="6d924-173">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="6d924-174">deviceCount</span><span class="sxs-lookup"><span data-stu-id="6d924-174">deviceCount</span></span>|<span data-ttu-id="6d924-175">Int64</span><span class="sxs-lookup"><span data-stu-id="6d924-175">Int64</span></span>|<span data-ttu-id="6d924-176">Contagem de dispositivos resumida da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="6d924-176">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="6d924-177">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="6d924-177">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="6d924-178">Int32</span><span class="sxs-lookup"><span data-stu-id="6d924-178">Int32</span></span>|<span data-ttu-id="6d924-179">O tempo de resposta da análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="6d924-179">The user experience analytics responsive desktop time in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="6d924-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d924-180">Response</span></span>
<span data-ttu-id="6d924-181">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d924-181">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d924-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d924-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d924-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d924-183">Request</span></span>
<span data-ttu-id="6d924-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d924-184">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance
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

### <a name="response"></a><span data-ttu-id="6d924-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d924-185">Response</span></span>
<span data-ttu-id="6d924-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d924-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





