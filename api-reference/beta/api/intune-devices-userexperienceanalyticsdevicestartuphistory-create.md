---
title: Criar userExperienceAnalyticsDeviceStartupHistory
description: Criar um novo objeto userExperienceAnalyticsDeviceStartupHistory.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f5b91043417fb0e33dd7f7781c82503525b5d185
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791348"
---
# <a name="create-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="52d4b-103">Criar userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="52d4b-103">Create userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="52d4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52d4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52d4b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52d4b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52d4b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52d4b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52d4b-107">Criar um novo objeto [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .</span><span class="sxs-lookup"><span data-stu-id="52d4b-107">Create a new [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52d4b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52d4b-108">Prerequisites</span></span>
<span data-ttu-id="52d4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52d4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52d4b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52d4b-111">Permission type</span></span>|<span data-ttu-id="52d4b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="52d4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52d4b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52d4b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52d4b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52d4b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="52d4b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52d4b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52d4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52d4b-116">Not supported.</span></span>|
|<span data-ttu-id="52d4b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52d4b-117">Application</span></span>|<span data-ttu-id="52d4b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52d4b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52d4b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52d4b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a><span data-ttu-id="52d4b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52d4b-120">Request headers</span></span>
|<span data-ttu-id="52d4b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52d4b-121">Header</span></span>|<span data-ttu-id="52d4b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="52d4b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52d4b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="52d4b-123">Authorization</span></span>|<span data-ttu-id="52d4b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52d4b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52d4b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52d4b-125">Accept</span></span>|<span data-ttu-id="52d4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52d4b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52d4b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52d4b-127">Request body</span></span>
<span data-ttu-id="52d4b-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsDeviceStartupHistory.</span><span class="sxs-lookup"><span data-stu-id="52d4b-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupHistory object.</span></span>

<span data-ttu-id="52d4b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsDeviceStartupHistory.</span><span class="sxs-lookup"><span data-stu-id="52d4b-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupHistory.</span></span>

|<span data-ttu-id="52d4b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52d4b-130">Property</span></span>|<span data-ttu-id="52d4b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="52d4b-131">Type</span></span>|<span data-ttu-id="52d4b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="52d4b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52d4b-133">id</span><span class="sxs-lookup"><span data-stu-id="52d4b-133">id</span></span>|<span data-ttu-id="52d4b-134">String</span><span class="sxs-lookup"><span data-stu-id="52d4b-134">String</span></span>|<span data-ttu-id="52d4b-135">O identificador exclusivo do histórico de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="52d4b-135">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="52d4b-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="52d4b-136">deviceId</span></span>|<span data-ttu-id="52d4b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52d4b-137">String</span></span>|<span data-ttu-id="52d4b-138">A ID do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="52d4b-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="52d4b-139">startTime</span><span class="sxs-lookup"><span data-stu-id="52d4b-139">startTime</span></span>|<span data-ttu-id="52d4b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52d4b-140">DateTimeOffset</span></span>|<span data-ttu-id="52d4b-141">A hora de início do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="52d4b-141">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="52d4b-142">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="52d4b-142">coreBootTimeInMs</span></span>|<span data-ttu-id="52d4b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="52d4b-143">Int32</span></span>|<span data-ttu-id="52d4b-144">O tempo de inicialização do núcleo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="52d4b-144">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="52d4b-145">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="52d4b-145">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="52d4b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="52d4b-146">Int32</span></span>|<span data-ttu-id="52d4b-147">O tempo de inicialização da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="52d4b-147">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="52d4b-148">featureUpdateBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="52d4b-148">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="52d4b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="52d4b-149">Int32</span></span>|<span data-ttu-id="52d4b-150">O tempo de atualização de recursos do dispositivo de análise de experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="52d4b-150">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="52d4b-151">totalBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="52d4b-151">totalBootTimeInMs</span></span>|<span data-ttu-id="52d4b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="52d4b-152">Int32</span></span>|<span data-ttu-id="52d4b-153">O tempo de inicialização total do dispositivo de análise da experiência do usuário, em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="52d4b-153">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="52d4b-154">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="52d4b-154">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="52d4b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="52d4b-155">Int32</span></span>|<span data-ttu-id="52d4b-156">O tempo de logon da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="52d4b-156">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="52d4b-157">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="52d4b-157">coreLoginTimeInMs</span></span>|<span data-ttu-id="52d4b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="52d4b-158">Int32</span></span>|<span data-ttu-id="52d4b-159">O tempo de logon do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="52d4b-159">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="52d4b-160">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="52d4b-160">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="52d4b-161">Int32</span><span class="sxs-lookup"><span data-stu-id="52d4b-161">Int32</span></span>|<span data-ttu-id="52d4b-162">O tempo de resposta da análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="52d4b-162">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="52d4b-163">totalLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="52d4b-163">totalLoginTimeInMs</span></span>|<span data-ttu-id="52d4b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="52d4b-164">Int32</span></span>|<span data-ttu-id="52d4b-165">O tempo total de logon do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="52d4b-165">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="52d4b-166">isFirstLogin</span><span class="sxs-lookup"><span data-stu-id="52d4b-166">isFirstLogin</span></span>|<span data-ttu-id="52d4b-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="52d4b-167">Boolean</span></span>|<span data-ttu-id="52d4b-168">O dispositivo de análise de experiência do usuário primeiro logon.</span><span class="sxs-lookup"><span data-stu-id="52d4b-168">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="52d4b-169">isFeatureUpdate</span><span class="sxs-lookup"><span data-stu-id="52d4b-169">isFeatureUpdate</span></span>|<span data-ttu-id="52d4b-170">Booliano</span><span class="sxs-lookup"><span data-stu-id="52d4b-170">Boolean</span></span>|<span data-ttu-id="52d4b-171">O registro de inicialização do dispositivo de análise da experiência do usuário é uma atualização de recurso.</span><span class="sxs-lookup"><span data-stu-id="52d4b-171">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="52d4b-172">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="52d4b-172">operatingSystemVersion</span></span>|<span data-ttu-id="52d4b-173">String</span><span class="sxs-lookup"><span data-stu-id="52d4b-173">String</span></span>|<span data-ttu-id="52d4b-174">A versão do sistema operacional do registro de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="52d4b-174">The user experience analytics device boot record's operating system version.</span></span>|
|<span data-ttu-id="52d4b-175">restartCategory</span><span class="sxs-lookup"><span data-stu-id="52d4b-175">restartCategory</span></span>|[<span data-ttu-id="52d4b-176">userExperienceAnalyticsOperatingSystemRestartCategory</span><span class="sxs-lookup"><span data-stu-id="52d4b-176">userExperienceAnalyticsOperatingSystemRestartCategory</span></span>](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|<span data-ttu-id="52d4b-177">Categoria de reinício de so.</span><span class="sxs-lookup"><span data-stu-id="52d4b-177">OS restart category.</span></span> <span data-ttu-id="52d4b-178">Os possíveis valores são: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`.</span><span class="sxs-lookup"><span data-stu-id="52d4b-178">Possible values are: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`.</span></span>|



## <a name="response"></a><span data-ttu-id="52d4b-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="52d4b-179">Response</span></span>
<span data-ttu-id="52d4b-180">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52d4b-180">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52d4b-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52d4b-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="52d4b-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52d4b-182">Request</span></span>
<span data-ttu-id="52d4b-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52d4b-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
Content-type: application/json
Content-length: 576

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
  "restartCategory": "restartWithUpdate"
}
```

### <a name="response"></a><span data-ttu-id="52d4b-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="52d4b-184">Response</span></span>
<span data-ttu-id="52d4b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52d4b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 625

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
  "restartCategory": "restartWithUpdate"
}
```



