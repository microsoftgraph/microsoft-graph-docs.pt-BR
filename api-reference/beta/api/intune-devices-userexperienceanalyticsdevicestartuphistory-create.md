---
title: Criar userExperienceAnalyticsDeviceStartupHistory
description: Criar um novo objeto userExperienceAnalyticsDeviceStartupHistory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07905b1aaae394c8b366949bc657cb15679ae7fb
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944467"
---
# <a name="create-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="fe8c6-103">Criar userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="fe8c6-103">Create userExperienceAnalyticsDeviceStartupHistory</span></span>

> <span data-ttu-id="fe8c6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe8c6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe8c6-106">Criar um novo objeto [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .</span><span class="sxs-lookup"><span data-stu-id="fe8c6-106">Create a new [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe8c6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fe8c6-107">Prerequisites</span></span>
<span data-ttu-id="fe8c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe8c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe8c6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe8c6-110">Permission type</span></span>|<span data-ttu-id="fe8c6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fe8c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe8c6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe8c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe8c6-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8c6-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fe8c6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe8c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe8c6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-115">Not supported.</span></span>|
|<span data-ttu-id="fe8c6-116">Application</span><span class="sxs-lookup"><span data-stu-id="fe8c6-116">Application</span></span>|<span data-ttu-id="fe8c6-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8c6-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe8c6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe8c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a><span data-ttu-id="fe8c6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe8c6-119">Request headers</span></span>
|<span data-ttu-id="fe8c6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe8c6-120">Header</span></span>|<span data-ttu-id="fe8c6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fe8c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe8c6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe8c6-122">Authorization</span></span>|<span data-ttu-id="fe8c6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe8c6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fe8c6-124">Accept</span></span>|<span data-ttu-id="fe8c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fe8c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe8c6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe8c6-126">Request body</span></span>
<span data-ttu-id="fe8c6-127">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsDeviceStartupHistory.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-127">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupHistory object.</span></span>

<span data-ttu-id="fe8c6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsDeviceStartupHistory.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-128">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupHistory.</span></span>

|<span data-ttu-id="fe8c6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe8c6-129">Property</span></span>|<span data-ttu-id="fe8c6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe8c6-130">Type</span></span>|<span data-ttu-id="fe8c6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe8c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe8c6-132">id</span><span class="sxs-lookup"><span data-stu-id="fe8c6-132">id</span></span>|<span data-ttu-id="fe8c6-133">String</span><span class="sxs-lookup"><span data-stu-id="fe8c6-133">String</span></span>|<span data-ttu-id="fe8c6-134">O identificador exclusivo do histórico de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-134">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="fe8c6-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="fe8c6-135">deviceId</span></span>|<span data-ttu-id="fe8c6-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe8c6-136">String</span></span>|<span data-ttu-id="fe8c6-137">A ID do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-137">The user experience analytics device id.</span></span>|
|<span data-ttu-id="fe8c6-138">startTime</span><span class="sxs-lookup"><span data-stu-id="fe8c6-138">startTime</span></span>|<span data-ttu-id="fe8c6-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe8c6-139">DateTimeOffset</span></span>|<span data-ttu-id="fe8c6-140">A hora de início do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-140">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="fe8c6-141">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fe8c6-141">coreBootTimeInMs</span></span>|<span data-ttu-id="fe8c6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="fe8c6-142">Int32</span></span>|<span data-ttu-id="fe8c6-143">O tempo de inicialização do núcleo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-143">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="fe8c6-144">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fe8c6-144">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="fe8c6-145">Int32</span><span class="sxs-lookup"><span data-stu-id="fe8c6-145">Int32</span></span>|<span data-ttu-id="fe8c6-146">O tempo de inicialização da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-146">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="fe8c6-147">featureUpdateBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fe8c6-147">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="fe8c6-148">Int32</span><span class="sxs-lookup"><span data-stu-id="fe8c6-148">Int32</span></span>|<span data-ttu-id="fe8c6-149">O tempo de atualização de recursos do dispositivo de análise de experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-149">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="fe8c6-150">totalBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fe8c6-150">totalBootTimeInMs</span></span>|<span data-ttu-id="fe8c6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="fe8c6-151">Int32</span></span>|<span data-ttu-id="fe8c6-152">O tempo de inicialização total do dispositivo de análise da experiência do usuário, em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-152">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="fe8c6-153">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fe8c6-153">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="fe8c6-154">Int32</span><span class="sxs-lookup"><span data-stu-id="fe8c6-154">Int32</span></span>|<span data-ttu-id="fe8c6-155">O tempo de logon da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-155">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="fe8c6-156">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fe8c6-156">coreLoginTimeInMs</span></span>|<span data-ttu-id="fe8c6-157">Int32</span><span class="sxs-lookup"><span data-stu-id="fe8c6-157">Int32</span></span>|<span data-ttu-id="fe8c6-158">O tempo de logon do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-158">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="fe8c6-159">totalLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fe8c6-159">totalLoginTimeInMs</span></span>|<span data-ttu-id="fe8c6-160">Int32</span><span class="sxs-lookup"><span data-stu-id="fe8c6-160">Int32</span></span>|<span data-ttu-id="fe8c6-161">O tempo total de logon do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-161">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="fe8c6-162">isFirstLogin</span><span class="sxs-lookup"><span data-stu-id="fe8c6-162">isFirstLogin</span></span>|<span data-ttu-id="fe8c6-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe8c6-163">Boolean</span></span>|<span data-ttu-id="fe8c6-164">O dispositivo de análise de experiência do usuário primeiro logon.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-164">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="fe8c6-165">isFeatureUpdate</span><span class="sxs-lookup"><span data-stu-id="fe8c6-165">isFeatureUpdate</span></span>|<span data-ttu-id="fe8c6-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe8c6-166">Boolean</span></span>|<span data-ttu-id="fe8c6-167">O registro de inicialização do dispositivo de análise da experiência do usuário é uma atualização de recurso.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-167">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="fe8c6-168">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="fe8c6-168">operatingSystemVersion</span></span>|<span data-ttu-id="fe8c6-169">String</span><span class="sxs-lookup"><span data-stu-id="fe8c6-169">String</span></span>|<span data-ttu-id="fe8c6-170">A versão do sistema operacional do registro de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-170">The user experience analytics device boot record's operating system version.</span></span>|



## <a name="response"></a><span data-ttu-id="fe8c6-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe8c6-171">Response</span></span>
<span data-ttu-id="fe8c6-172">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-172">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe8c6-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe8c6-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe8c6-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe8c6-174">Request</span></span>
<span data-ttu-id="fe8c6-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
Content-type: application/json
Content-length: 498

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
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value"
}
```

### <a name="response"></a><span data-ttu-id="fe8c6-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe8c6-176">Response</span></span>
<span data-ttu-id="fe8c6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe8c6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 547

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
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value"
}
```





