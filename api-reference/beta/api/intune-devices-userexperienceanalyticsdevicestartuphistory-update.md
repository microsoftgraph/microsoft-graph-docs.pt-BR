---
title: Atualizar userExperienceAnalyticsDeviceStartupHistory
description: Atualiza as propriedades de um objeto userExperienceAnalyticsDeviceStartupHistory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c4e4ea779fd9d11d243a4afbb35ba9c626b79e92
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468366"
---
# <a name="update-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="6f348-103">Atualizar userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="6f348-103">Update userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="6f348-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6f348-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f348-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6f348-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f348-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f348-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f348-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .</span><span class="sxs-lookup"><span data-stu-id="6f348-107">Update the properties of a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f348-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6f348-108">Prerequisites</span></span>
<span data-ttu-id="6f348-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f348-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f348-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f348-111">Permission type</span></span>|<span data-ttu-id="6f348-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6f348-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f348-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f348-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f348-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f348-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6f348-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f348-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f348-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f348-116">Not supported.</span></span>|
|<span data-ttu-id="6f348-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f348-117">Application</span></span>|<span data-ttu-id="6f348-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f348-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f348-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f348-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="6f348-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f348-120">Request headers</span></span>
|<span data-ttu-id="6f348-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f348-121">Header</span></span>|<span data-ttu-id="6f348-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6f348-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f348-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f348-123">Authorization</span></span>|<span data-ttu-id="6f348-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f348-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f348-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6f348-125">Accept</span></span>|<span data-ttu-id="6f348-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f348-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f348-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f348-127">Request body</span></span>
<span data-ttu-id="6f348-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .</span><span class="sxs-lookup"><span data-stu-id="6f348-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

<span data-ttu-id="6f348-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).</span><span class="sxs-lookup"><span data-stu-id="6f348-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).</span></span>

|<span data-ttu-id="6f348-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f348-130">Property</span></span>|<span data-ttu-id="6f348-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f348-131">Type</span></span>|<span data-ttu-id="6f348-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f348-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f348-133">id</span><span class="sxs-lookup"><span data-stu-id="6f348-133">id</span></span>|<span data-ttu-id="6f348-134">String</span><span class="sxs-lookup"><span data-stu-id="6f348-134">String</span></span>|<span data-ttu-id="6f348-135">O identificador exclusivo do histórico de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="6f348-135">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="6f348-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="6f348-136">deviceId</span></span>|<span data-ttu-id="6f348-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f348-137">String</span></span>|<span data-ttu-id="6f348-138">A ID do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="6f348-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="6f348-139">startTime</span><span class="sxs-lookup"><span data-stu-id="6f348-139">startTime</span></span>|<span data-ttu-id="6f348-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f348-140">DateTimeOffset</span></span>|<span data-ttu-id="6f348-141">A hora de início do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="6f348-141">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="6f348-142">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="6f348-142">coreBootTimeInMs</span></span>|<span data-ttu-id="6f348-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6f348-143">Int32</span></span>|<span data-ttu-id="6f348-144">O tempo de inicialização do núcleo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="6f348-144">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="6f348-145">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="6f348-145">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="6f348-146">Int32</span><span class="sxs-lookup"><span data-stu-id="6f348-146">Int32</span></span>|<span data-ttu-id="6f348-147">O tempo de inicialização da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="6f348-147">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="6f348-148">featureUpdateBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="6f348-148">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="6f348-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6f348-149">Int32</span></span>|<span data-ttu-id="6f348-150">O tempo de atualização de recursos do dispositivo de análise de experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="6f348-150">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="6f348-151">totalBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="6f348-151">totalBootTimeInMs</span></span>|<span data-ttu-id="6f348-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6f348-152">Int32</span></span>|<span data-ttu-id="6f348-153">O tempo de inicialização total do dispositivo de análise da experiência do usuário, em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="6f348-153">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="6f348-154">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="6f348-154">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="6f348-155">Int32</span><span class="sxs-lookup"><span data-stu-id="6f348-155">Int32</span></span>|<span data-ttu-id="6f348-156">O tempo de logon da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="6f348-156">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="6f348-157">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="6f348-157">coreLoginTimeInMs</span></span>|<span data-ttu-id="6f348-158">Int32</span><span class="sxs-lookup"><span data-stu-id="6f348-158">Int32</span></span>|<span data-ttu-id="6f348-159">O tempo de logon do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="6f348-159">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="6f348-160">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="6f348-160">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="6f348-161">Int32</span><span class="sxs-lookup"><span data-stu-id="6f348-161">Int32</span></span>|<span data-ttu-id="6f348-162">O tempo de resposta da análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="6f348-162">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="6f348-163">totalLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="6f348-163">totalLoginTimeInMs</span></span>|<span data-ttu-id="6f348-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6f348-164">Int32</span></span>|<span data-ttu-id="6f348-165">O tempo total de logon do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="6f348-165">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="6f348-166">isFirstLogin</span><span class="sxs-lookup"><span data-stu-id="6f348-166">isFirstLogin</span></span>|<span data-ttu-id="6f348-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f348-167">Boolean</span></span>|<span data-ttu-id="6f348-168">O dispositivo de análise de experiência do usuário primeiro logon.</span><span class="sxs-lookup"><span data-stu-id="6f348-168">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="6f348-169">isFeatureUpdate</span><span class="sxs-lookup"><span data-stu-id="6f348-169">isFeatureUpdate</span></span>|<span data-ttu-id="6f348-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f348-170">Boolean</span></span>|<span data-ttu-id="6f348-171">O registro de inicialização do dispositivo de análise da experiência do usuário é uma atualização de recurso.</span><span class="sxs-lookup"><span data-stu-id="6f348-171">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="6f348-172">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="6f348-172">operatingSystemVersion</span></span>|<span data-ttu-id="6f348-173">String</span><span class="sxs-lookup"><span data-stu-id="6f348-173">String</span></span>|<span data-ttu-id="6f348-174">A versão do sistema operacional do registro de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="6f348-174">The user experience analytics device boot record's operating system version.</span></span>|



## <a name="response"></a><span data-ttu-id="6f348-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f348-175">Response</span></span>
<span data-ttu-id="6f348-176">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f348-176">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f348-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f348-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f348-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f348-178">Request</span></span>
<span data-ttu-id="6f348-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f348-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
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

### <a name="response"></a><span data-ttu-id="6f348-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f348-180">Response</span></span>
<span data-ttu-id="6f348-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f348-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





