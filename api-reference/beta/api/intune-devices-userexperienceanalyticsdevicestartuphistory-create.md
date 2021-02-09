---
title: Criar userExperienceAnalyticsDeviceStartupHistory
description: Crie um novo objeto userExperienceAnalyticsDeviceStartupHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2bfbe3272018304da8e959ea9663ccd38119c0fe
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159672"
---
# <a name="create-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="5411f-103">Criar userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="5411f-103">Create userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="5411f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5411f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5411f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5411f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5411f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5411f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5411f-107">Crie um novo [objeto userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)</span><span class="sxs-lookup"><span data-stu-id="5411f-107">Create a new [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5411f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5411f-108">Prerequisites</span></span>
<span data-ttu-id="5411f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5411f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5411f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5411f-111">Permission type</span></span>|<span data-ttu-id="5411f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5411f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5411f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5411f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5411f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5411f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5411f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5411f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5411f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5411f-116">Not supported.</span></span>|
|<span data-ttu-id="5411f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5411f-117">Application</span></span>|<span data-ttu-id="5411f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5411f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5411f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5411f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a><span data-ttu-id="5411f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5411f-120">Request headers</span></span>
|<span data-ttu-id="5411f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5411f-121">Header</span></span>|<span data-ttu-id="5411f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5411f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5411f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5411f-123">Authorization</span></span>|<span data-ttu-id="5411f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5411f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5411f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5411f-125">Accept</span></span>|<span data-ttu-id="5411f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5411f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5411f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5411f-127">Request body</span></span>
<span data-ttu-id="5411f-128">No corpo da solicitação, fornece uma representação JSON do objeto userExperienceAnalyticsDeviceStartupHistory.</span><span class="sxs-lookup"><span data-stu-id="5411f-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupHistory object.</span></span>

<span data-ttu-id="5411f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsDeviceStartupHistory.</span><span class="sxs-lookup"><span data-stu-id="5411f-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupHistory.</span></span>

|<span data-ttu-id="5411f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5411f-130">Property</span></span>|<span data-ttu-id="5411f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5411f-131">Type</span></span>|<span data-ttu-id="5411f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5411f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5411f-133">id</span><span class="sxs-lookup"><span data-stu-id="5411f-133">id</span></span>|<span data-ttu-id="5411f-134">String</span><span class="sxs-lookup"><span data-stu-id="5411f-134">String</span></span>|<span data-ttu-id="5411f-135">O identificador exclusivo do histórico de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="5411f-135">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="5411f-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="5411f-136">deviceId</span></span>|<span data-ttu-id="5411f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5411f-137">String</span></span>|<span data-ttu-id="5411f-138">A ID do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="5411f-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="5411f-139">startTime</span><span class="sxs-lookup"><span data-stu-id="5411f-139">startTime</span></span>|<span data-ttu-id="5411f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5411f-140">DateTimeOffset</span></span>|<span data-ttu-id="5411f-141">A hora de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="5411f-141">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="5411f-142">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="5411f-142">coreBootTimeInMs</span></span>|<span data-ttu-id="5411f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5411f-143">Int32</span></span>|<span data-ttu-id="5411f-144">O tempo de inicialização principal do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="5411f-144">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="5411f-145">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="5411f-145">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="5411f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="5411f-146">Int32</span></span>|<span data-ttu-id="5411f-147">A análise da experiência do usuário Tempo de inicialização da política de grupo do dispositivo em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="5411f-147">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="5411f-148">featureUpdateBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="5411f-148">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="5411f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="5411f-149">Int32</span></span>|<span data-ttu-id="5411f-150">O tempo de atualização de recursos do dispositivo de análise de experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="5411f-150">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="5411f-151">totalBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="5411f-151">totalBootTimeInMs</span></span>|<span data-ttu-id="5411f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5411f-152">Int32</span></span>|<span data-ttu-id="5411f-153">O tempo total de inicialização do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="5411f-153">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="5411f-154">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="5411f-154">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="5411f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="5411f-155">Int32</span></span>|<span data-ttu-id="5411f-156">O tempo de logon da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="5411f-156">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="5411f-157">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="5411f-157">coreLoginTimeInMs</span></span>|<span data-ttu-id="5411f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="5411f-158">Int32</span></span>|<span data-ttu-id="5411f-159">O tempo de logon principal do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="5411f-159">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="5411f-160">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="5411f-160">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="5411f-161">Int32</span><span class="sxs-lookup"><span data-stu-id="5411f-161">Int32</span></span>|<span data-ttu-id="5411f-162">O tempo da área de trabalho responsivo da análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="5411f-162">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="5411f-163">totalLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="5411f-163">totalLoginTimeInMs</span></span>|<span data-ttu-id="5411f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5411f-164">Int32</span></span>|<span data-ttu-id="5411f-165">O tempo total de logon do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="5411f-165">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="5411f-166">isFirstLogin</span><span class="sxs-lookup"><span data-stu-id="5411f-166">isFirstLogin</span></span>|<span data-ttu-id="5411f-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="5411f-167">Boolean</span></span>|<span data-ttu-id="5411f-168">O primeiro logon do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="5411f-168">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="5411f-169">isFeatureUpdate</span><span class="sxs-lookup"><span data-stu-id="5411f-169">isFeatureUpdate</span></span>|<span data-ttu-id="5411f-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="5411f-170">Boolean</span></span>|<span data-ttu-id="5411f-171">O registro de inicialização do dispositivo de análise de experiência do usuário é uma atualização de recurso.</span><span class="sxs-lookup"><span data-stu-id="5411f-171">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="5411f-172">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="5411f-172">operatingSystemVersion</span></span>|<span data-ttu-id="5411f-173">String</span><span class="sxs-lookup"><span data-stu-id="5411f-173">String</span></span>|<span data-ttu-id="5411f-174">A versão do sistema operacional do registro de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="5411f-174">The user experience analytics device boot record's operating system version.</span></span>|
|<span data-ttu-id="5411f-175">restartCategory</span><span class="sxs-lookup"><span data-stu-id="5411f-175">restartCategory</span></span>|[<span data-ttu-id="5411f-176">userExperienceAnalyticsOperatingSystemRestartCategory</span><span class="sxs-lookup"><span data-stu-id="5411f-176">userExperienceAnalyticsOperatingSystemRestartCategory</span></span>](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|<span data-ttu-id="5411f-177">Categoria de reinicialização do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="5411f-177">OS restart category.</span></span> <span data-ttu-id="5411f-178">Os valores possíveis são: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.</span><span class="sxs-lookup"><span data-stu-id="5411f-178">Possible values are: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.</span></span>|
|<span data-ttu-id="5411f-179">restartStopCode</span><span class="sxs-lookup"><span data-stu-id="5411f-179">restartStopCode</span></span>|<span data-ttu-id="5411f-180">String</span><span class="sxs-lookup"><span data-stu-id="5411f-180">String</span></span>|<span data-ttu-id="5411f-181">Código de parada de reinicialização do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="5411f-181">OS restart stop code.</span></span> <span data-ttu-id="5411f-182">Isso mostra o código de verificação de bugs que pode ser usado para procurar o motivo da tela azul.</span><span class="sxs-lookup"><span data-stu-id="5411f-182">This shows the bug check code which can be used to look up the blue screen reason.</span></span>|
|<span data-ttu-id="5411f-183">restartFaultBucket</span><span class="sxs-lookup"><span data-stu-id="5411f-183">restartFaultBucket</span></span>|<span data-ttu-id="5411f-184">String</span><span class="sxs-lookup"><span data-stu-id="5411f-184">String</span></span>|<span data-ttu-id="5411f-185">Sistema operacional reinicia o bucket de falha.</span><span class="sxs-lookup"><span data-stu-id="5411f-185">OS restart fault bucket.</span></span> <span data-ttu-id="5411f-186">O bucket de falha é usado para encontrar informações adicionais sobre uma falha do sistema.</span><span class="sxs-lookup"><span data-stu-id="5411f-186">The fault bucket is used to find additional information about a system crash.</span></span>|



## <a name="response"></a><span data-ttu-id="5411f-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="5411f-187">Response</span></span>
<span data-ttu-id="5411f-188">Se tiver êxito, este método retornará um código de resposta e um objeto `201 Created` [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5411f-188">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5411f-189">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5411f-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="5411f-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5411f-190">Request</span></span>
<span data-ttu-id="5411f-191">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5411f-191">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
Content-type: application/json
Content-length: 680

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:03:29.2730865-08:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "responsiveDesktopTimeInMs": 9,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value",
  "restartCategory": "restartWithUpdate",
  "restartStopCode": "Restart Stop Code value",
  "restartFaultBucket": "Restart Fault Bucket value"
}
```

### <a name="response"></a><span data-ttu-id="5411f-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="5411f-192">Response</span></span>
<span data-ttu-id="5411f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5411f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 729

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "id": "13357123-7123-1335-2371-351323713513",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:03:29.2730865-08:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "responsiveDesktopTimeInMs": 9,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value",
  "restartCategory": "restartWithUpdate",
  "restartStopCode": "Restart Stop Code value",
  "restartFaultBucket": "Restart Fault Bucket value"
}
```




