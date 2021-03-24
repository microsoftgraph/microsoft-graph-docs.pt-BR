---
title: Atualizar userExperienceAnalyticsDeviceStartupHistory
description: Atualize as propriedades de um objeto userExperienceAnalyticsDeviceStartupHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 17eccd604ae452bb169fe4d7eb82f97ed1bc51ab
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146227"
---
# <a name="update-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="9e432-103">Atualizar userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="9e432-103">Update userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="9e432-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e432-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e432-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9e432-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e432-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e432-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e432-107">Atualize as propriedades de [um objeto userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)</span><span class="sxs-lookup"><span data-stu-id="9e432-107">Update the properties of a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e432-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e432-108">Prerequisites</span></span>
<span data-ttu-id="9e432-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e432-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e432-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e432-111">Permission type</span></span>|<span data-ttu-id="9e432-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e432-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e432-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e432-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e432-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e432-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9e432-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e432-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e432-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e432-116">Not supported.</span></span>|
|<span data-ttu-id="9e432-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e432-117">Application</span></span>|<span data-ttu-id="9e432-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e432-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e432-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e432-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="9e432-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e432-120">Request headers</span></span>
|<span data-ttu-id="9e432-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e432-121">Header</span></span>|<span data-ttu-id="9e432-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9e432-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e432-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e432-123">Authorization</span></span>|<span data-ttu-id="9e432-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e432-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e432-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9e432-125">Accept</span></span>|<span data-ttu-id="9e432-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e432-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e432-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e432-127">Request body</span></span>
<span data-ttu-id="9e432-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)</span><span class="sxs-lookup"><span data-stu-id="9e432-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

<span data-ttu-id="9e432-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).</span><span class="sxs-lookup"><span data-stu-id="9e432-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).</span></span>

|<span data-ttu-id="9e432-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e432-130">Property</span></span>|<span data-ttu-id="9e432-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e432-131">Type</span></span>|<span data-ttu-id="9e432-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e432-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e432-133">id</span><span class="sxs-lookup"><span data-stu-id="9e432-133">id</span></span>|<span data-ttu-id="9e432-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e432-134">String</span></span>|<span data-ttu-id="9e432-135">O identificador exclusivo do histórico de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9e432-135">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="9e432-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="9e432-136">deviceId</span></span>|<span data-ttu-id="9e432-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e432-137">String</span></span>|<span data-ttu-id="9e432-138">A ID do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9e432-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="9e432-139">startTime</span><span class="sxs-lookup"><span data-stu-id="9e432-139">startTime</span></span>|<span data-ttu-id="9e432-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e432-140">DateTimeOffset</span></span>|<span data-ttu-id="9e432-141">A hora de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9e432-141">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="9e432-142">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9e432-142">coreBootTimeInMs</span></span>|<span data-ttu-id="9e432-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9e432-143">Int32</span></span>|<span data-ttu-id="9e432-144">O tempo de inicialização principal do dispositivo de análise de experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="9e432-144">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="9e432-145">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9e432-145">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="9e432-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9e432-146">Int32</span></span>|<span data-ttu-id="9e432-147">Análise de experiência do usuário Tempo de inicialização da política de grupo do dispositivo em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="9e432-147">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="9e432-148">featureUpdateBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9e432-148">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="9e432-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9e432-149">Int32</span></span>|<span data-ttu-id="9e432-150">O tempo de atualização de recursos do dispositivo de análise de experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="9e432-150">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="9e432-151">totalBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9e432-151">totalBootTimeInMs</span></span>|<span data-ttu-id="9e432-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9e432-152">Int32</span></span>|<span data-ttu-id="9e432-153">O tempo total de inicialização do dispositivo de análise de experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="9e432-153">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="9e432-154">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9e432-154">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="9e432-155">Int32</span><span class="sxs-lookup"><span data-stu-id="9e432-155">Int32</span></span>|<span data-ttu-id="9e432-156">Análise de experiência do usuário Tempo de logon da política de grupo do dispositivo em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="9e432-156">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="9e432-157">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9e432-157">coreLoginTimeInMs</span></span>|<span data-ttu-id="9e432-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9e432-158">Int32</span></span>|<span data-ttu-id="9e432-159">O tempo de logon principal do dispositivo de análise de experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="9e432-159">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="9e432-160">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9e432-160">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="9e432-161">Int32</span><span class="sxs-lookup"><span data-stu-id="9e432-161">Int32</span></span>|<span data-ttu-id="9e432-162">A análise da experiência do usuário responde ao tempo da área de trabalho em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="9e432-162">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="9e432-163">totalLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9e432-163">totalLoginTimeInMs</span></span>|<span data-ttu-id="9e432-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9e432-164">Int32</span></span>|<span data-ttu-id="9e432-165">O tempo total de logon do dispositivo de análise de experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="9e432-165">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="9e432-166">isFirstLogin</span><span class="sxs-lookup"><span data-stu-id="9e432-166">isFirstLogin</span></span>|<span data-ttu-id="9e432-167">Booleano</span><span class="sxs-lookup"><span data-stu-id="9e432-167">Boolean</span></span>|<span data-ttu-id="9e432-168">O primeiro logon do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9e432-168">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="9e432-169">isFeatureUpdate</span><span class="sxs-lookup"><span data-stu-id="9e432-169">isFeatureUpdate</span></span>|<span data-ttu-id="9e432-170">Booleano</span><span class="sxs-lookup"><span data-stu-id="9e432-170">Boolean</span></span>|<span data-ttu-id="9e432-171">O registro de inicialização do dispositivo de análise de experiência do usuário é uma atualização de recurso.</span><span class="sxs-lookup"><span data-stu-id="9e432-171">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="9e432-172">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="9e432-172">operatingSystemVersion</span></span>|<span data-ttu-id="9e432-173">String</span><span class="sxs-lookup"><span data-stu-id="9e432-173">String</span></span>|<span data-ttu-id="9e432-174">A versão do sistema operacional do registro de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9e432-174">The user experience analytics device boot record's operating system version.</span></span>|
|<span data-ttu-id="9e432-175">restartCategory</span><span class="sxs-lookup"><span data-stu-id="9e432-175">restartCategory</span></span>|[<span data-ttu-id="9e432-176">userExperienceAnalyticsOperatingSystemRestartCategory</span><span class="sxs-lookup"><span data-stu-id="9e432-176">userExperienceAnalyticsOperatingSystemRestartCategory</span></span>](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|<span data-ttu-id="9e432-177">Categoria de reinicialização do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="9e432-177">OS restart category.</span></span> <span data-ttu-id="9e432-178">Os valores possíveis são: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.</span><span class="sxs-lookup"><span data-stu-id="9e432-178">Possible values are: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.</span></span>|
|<span data-ttu-id="9e432-179">restartStopCode</span><span class="sxs-lookup"><span data-stu-id="9e432-179">restartStopCode</span></span>|<span data-ttu-id="9e432-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e432-180">String</span></span>|<span data-ttu-id="9e432-181">Código de parada de reinicialização do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="9e432-181">OS restart stop code.</span></span> <span data-ttu-id="9e432-182">Isso mostra o código de verificação de bugs que pode ser usado para procurar o motivo da tela azul.</span><span class="sxs-lookup"><span data-stu-id="9e432-182">This shows the bug check code which can be used to look up the blue screen reason.</span></span>|
|<span data-ttu-id="9e432-183">restartFaultBucket</span><span class="sxs-lookup"><span data-stu-id="9e432-183">restartFaultBucket</span></span>|<span data-ttu-id="9e432-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e432-184">String</span></span>|<span data-ttu-id="9e432-185">Bucket de falha de reinicialização do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="9e432-185">OS restart fault bucket.</span></span> <span data-ttu-id="9e432-186">O bucket de falhas é usado para encontrar informações adicionais sobre uma falha no sistema.</span><span class="sxs-lookup"><span data-stu-id="9e432-186">The fault bucket is used to find additional information about a system crash.</span></span>|



## <a name="response"></a><span data-ttu-id="9e432-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e432-187">Response</span></span>
<span data-ttu-id="9e432-188">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e432-188">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e432-189">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e432-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e432-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e432-190">Request</span></span>
<span data-ttu-id="9e432-191">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e432-191">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
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

### <a name="response"></a><span data-ttu-id="9e432-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e432-192">Response</span></span>
<span data-ttu-id="9e432-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e432-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




