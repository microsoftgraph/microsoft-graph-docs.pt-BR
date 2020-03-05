---
title: Criar userExperienceAnalyticsDeviceStartupHistory
description: Criar um novo objeto userExperienceAnalyticsDeviceStartupHistory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d2fe97a2567bcde086f8cbc8febbedff3829658b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468359"
---
# <a name="create-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="f1c6d-103">Criar userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="f1c6d-103">Create userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="f1c6d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f1c6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1c6d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1c6d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1c6d-107">Criar um novo objeto [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .</span><span class="sxs-lookup"><span data-stu-id="f1c6d-107">Create a new [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1c6d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1c6d-108">Prerequisites</span></span>
<span data-ttu-id="f1c6d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1c6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1c6d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1c6d-111">Permission type</span></span>|<span data-ttu-id="f1c6d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1c6d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1c6d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1c6d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1c6d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1c6d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f1c6d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1c6d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1c6d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-116">Not supported.</span></span>|
|<span data-ttu-id="f1c6d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1c6d-117">Application</span></span>|<span data-ttu-id="f1c6d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1c6d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1c6d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1c6d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a><span data-ttu-id="f1c6d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1c6d-120">Request headers</span></span>
|<span data-ttu-id="f1c6d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1c6d-121">Header</span></span>|<span data-ttu-id="f1c6d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f1c6d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1c6d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1c6d-123">Authorization</span></span>|<span data-ttu-id="f1c6d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1c6d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1c6d-125">Accept</span></span>|<span data-ttu-id="f1c6d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1c6d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1c6d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1c6d-127">Request body</span></span>
<span data-ttu-id="f1c6d-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsDeviceStartupHistory.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupHistory object.</span></span>

<span data-ttu-id="f1c6d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsDeviceStartupHistory.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupHistory.</span></span>

|<span data-ttu-id="f1c6d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1c6d-130">Property</span></span>|<span data-ttu-id="f1c6d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1c6d-131">Type</span></span>|<span data-ttu-id="f1c6d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1c6d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1c6d-133">id</span><span class="sxs-lookup"><span data-stu-id="f1c6d-133">id</span></span>|<span data-ttu-id="f1c6d-134">String</span><span class="sxs-lookup"><span data-stu-id="f1c6d-134">String</span></span>|<span data-ttu-id="f1c6d-135">O identificador exclusivo do histórico de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-135">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="f1c6d-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="f1c6d-136">deviceId</span></span>|<span data-ttu-id="f1c6d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1c6d-137">String</span></span>|<span data-ttu-id="f1c6d-138">A ID do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="f1c6d-139">startTime</span><span class="sxs-lookup"><span data-stu-id="f1c6d-139">startTime</span></span>|<span data-ttu-id="f1c6d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1c6d-140">DateTimeOffset</span></span>|<span data-ttu-id="f1c6d-141">A hora de início do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-141">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="f1c6d-142">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f1c6d-142">coreBootTimeInMs</span></span>|<span data-ttu-id="f1c6d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f1c6d-143">Int32</span></span>|<span data-ttu-id="f1c6d-144">O tempo de inicialização do núcleo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-144">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="f1c6d-145">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f1c6d-145">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="f1c6d-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f1c6d-146">Int32</span></span>|<span data-ttu-id="f1c6d-147">O tempo de inicialização da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-147">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="f1c6d-148">featureUpdateBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f1c6d-148">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="f1c6d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f1c6d-149">Int32</span></span>|<span data-ttu-id="f1c6d-150">O tempo de atualização de recursos do dispositivo de análise de experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-150">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="f1c6d-151">totalBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f1c6d-151">totalBootTimeInMs</span></span>|<span data-ttu-id="f1c6d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f1c6d-152">Int32</span></span>|<span data-ttu-id="f1c6d-153">O tempo de inicialização total do dispositivo de análise da experiência do usuário, em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-153">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="f1c6d-154">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f1c6d-154">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="f1c6d-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f1c6d-155">Int32</span></span>|<span data-ttu-id="f1c6d-156">O tempo de logon da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-156">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="f1c6d-157">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f1c6d-157">coreLoginTimeInMs</span></span>|<span data-ttu-id="f1c6d-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f1c6d-158">Int32</span></span>|<span data-ttu-id="f1c6d-159">O tempo de logon do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-159">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="f1c6d-160">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f1c6d-160">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="f1c6d-161">Int32</span><span class="sxs-lookup"><span data-stu-id="f1c6d-161">Int32</span></span>|<span data-ttu-id="f1c6d-162">O tempo de resposta da análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-162">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="f1c6d-163">totalLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f1c6d-163">totalLoginTimeInMs</span></span>|<span data-ttu-id="f1c6d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f1c6d-164">Int32</span></span>|<span data-ttu-id="f1c6d-165">O tempo total de logon do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-165">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="f1c6d-166">isFirstLogin</span><span class="sxs-lookup"><span data-stu-id="f1c6d-166">isFirstLogin</span></span>|<span data-ttu-id="f1c6d-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1c6d-167">Boolean</span></span>|<span data-ttu-id="f1c6d-168">O dispositivo de análise de experiência do usuário primeiro logon.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-168">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="f1c6d-169">isFeatureUpdate</span><span class="sxs-lookup"><span data-stu-id="f1c6d-169">isFeatureUpdate</span></span>|<span data-ttu-id="f1c6d-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1c6d-170">Boolean</span></span>|<span data-ttu-id="f1c6d-171">O registro de inicialização do dispositivo de análise da experiência do usuário é uma atualização de recurso.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-171">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="f1c6d-172">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="f1c6d-172">operatingSystemVersion</span></span>|<span data-ttu-id="f1c6d-173">String</span><span class="sxs-lookup"><span data-stu-id="f1c6d-173">String</span></span>|<span data-ttu-id="f1c6d-174">A versão do sistema operacional do registro de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-174">The user experience analytics device boot record's operating system version.</span></span>|



## <a name="response"></a><span data-ttu-id="f1c6d-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1c6d-175">Response</span></span>
<span data-ttu-id="f1c6d-176">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-176">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1c6d-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1c6d-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1c6d-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1c6d-178">Request</span></span>
<span data-ttu-id="f1c6d-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
Content-type: application/json
Content-length: 533

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
  "operatingSystemVersion": "Operating System Version value"
}
```

### <a name="response"></a><span data-ttu-id="f1c6d-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1c6d-180">Response</span></span>
<span data-ttu-id="f1c6d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1c6d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 582

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
  "operatingSystemVersion": "Operating System Version value"
}
```





