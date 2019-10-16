---
title: Criar userExperienceAnalyticsDeviceStartupHistory
description: Criar um novo objeto userExperienceAnalyticsDeviceStartupHistory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d36442808380f408998b8dedaf5d89d45acb0982
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37529197"
---
# <a name="create-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="23b73-103">Criar userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="23b73-103">Create userExperienceAnalyticsDeviceStartupHistory</span></span>

> <span data-ttu-id="23b73-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="23b73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23b73-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23b73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23b73-106">Criar um novo objeto [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .</span><span class="sxs-lookup"><span data-stu-id="23b73-106">Create a new [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23b73-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="23b73-107">Prerequisites</span></span>
<span data-ttu-id="23b73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23b73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23b73-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23b73-110">Permission type</span></span>|<span data-ttu-id="23b73-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="23b73-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23b73-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23b73-112">Delegated (work or school account)</span></span>|<span data-ttu-id="23b73-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23b73-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="23b73-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23b73-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23b73-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23b73-115">Not supported.</span></span>|
|<span data-ttu-id="23b73-116">Application</span><span class="sxs-lookup"><span data-stu-id="23b73-116">Application</span></span>|<span data-ttu-id="23b73-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23b73-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23b73-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23b73-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a><span data-ttu-id="23b73-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23b73-119">Request headers</span></span>
|<span data-ttu-id="23b73-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23b73-120">Header</span></span>|<span data-ttu-id="23b73-121">Valor</span><span class="sxs-lookup"><span data-stu-id="23b73-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23b73-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="23b73-122">Authorization</span></span>|<span data-ttu-id="23b73-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23b73-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23b73-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="23b73-124">Accept</span></span>|<span data-ttu-id="23b73-125">application/json</span><span class="sxs-lookup"><span data-stu-id="23b73-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23b73-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23b73-126">Request body</span></span>
<span data-ttu-id="23b73-127">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsDeviceStartupHistory.</span><span class="sxs-lookup"><span data-stu-id="23b73-127">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupHistory object.</span></span>

<span data-ttu-id="23b73-128">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsDeviceStartupHistory.</span><span class="sxs-lookup"><span data-stu-id="23b73-128">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupHistory.</span></span>

|<span data-ttu-id="23b73-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23b73-129">Property</span></span>|<span data-ttu-id="23b73-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="23b73-130">Type</span></span>|<span data-ttu-id="23b73-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="23b73-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23b73-132">id</span><span class="sxs-lookup"><span data-stu-id="23b73-132">id</span></span>|<span data-ttu-id="23b73-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23b73-133">String</span></span>|<span data-ttu-id="23b73-134">O identificador exclusivo do histórico de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="23b73-134">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="23b73-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="23b73-135">deviceId</span></span>|<span data-ttu-id="23b73-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23b73-136">String</span></span>|<span data-ttu-id="23b73-137">A ID do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="23b73-137">The user experience analytics device id.</span></span>|
|<span data-ttu-id="23b73-138">startTime</span><span class="sxs-lookup"><span data-stu-id="23b73-138">startTime</span></span>|<span data-ttu-id="23b73-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23b73-139">DateTimeOffset</span></span>|<span data-ttu-id="23b73-140">A hora de início do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="23b73-140">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="23b73-141">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="23b73-141">coreBootTimeInMs</span></span>|<span data-ttu-id="23b73-142">Int32</span><span class="sxs-lookup"><span data-stu-id="23b73-142">Int32</span></span>|<span data-ttu-id="23b73-143">O tempo de inicialização do núcleo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="23b73-143">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="23b73-144">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="23b73-144">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="23b73-145">Int32</span><span class="sxs-lookup"><span data-stu-id="23b73-145">Int32</span></span>|<span data-ttu-id="23b73-146">O tempo de inicialização da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="23b73-146">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="23b73-147">featureUpdateBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="23b73-147">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="23b73-148">Int32</span><span class="sxs-lookup"><span data-stu-id="23b73-148">Int32</span></span>|<span data-ttu-id="23b73-149">O tempo de atualização de recursos do dispositivo de análise de experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="23b73-149">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="23b73-150">totalBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="23b73-150">totalBootTimeInMs</span></span>|<span data-ttu-id="23b73-151">Int32</span><span class="sxs-lookup"><span data-stu-id="23b73-151">Int32</span></span>|<span data-ttu-id="23b73-152">O tempo de inicialização total do dispositivo de análise da experiência do usuário, em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="23b73-152">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="23b73-153">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="23b73-153">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="23b73-154">Int32</span><span class="sxs-lookup"><span data-stu-id="23b73-154">Int32</span></span>|<span data-ttu-id="23b73-155">O tempo de logon da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="23b73-155">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="23b73-156">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="23b73-156">coreLoginTimeInMs</span></span>|<span data-ttu-id="23b73-157">Int32</span><span class="sxs-lookup"><span data-stu-id="23b73-157">Int32</span></span>|<span data-ttu-id="23b73-158">O tempo de logon do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="23b73-158">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="23b73-159">totalLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="23b73-159">totalLoginTimeInMs</span></span>|<span data-ttu-id="23b73-160">Int32</span><span class="sxs-lookup"><span data-stu-id="23b73-160">Int32</span></span>|<span data-ttu-id="23b73-161">O tempo total de logon do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="23b73-161">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="23b73-162">isFirstLogin</span><span class="sxs-lookup"><span data-stu-id="23b73-162">isFirstLogin</span></span>|<span data-ttu-id="23b73-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="23b73-163">Boolean</span></span>|<span data-ttu-id="23b73-164">O dispositivo de análise de experiência do usuário primeiro logon.</span><span class="sxs-lookup"><span data-stu-id="23b73-164">The user experience analytics device first login.</span></span>|



## <a name="response"></a><span data-ttu-id="23b73-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="23b73-165">Response</span></span>
<span data-ttu-id="23b73-166">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23b73-166">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23b73-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23b73-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="23b73-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23b73-168">Request</span></span>
<span data-ttu-id="23b73-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23b73-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
Content-type: application/json
Content-length: 407

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
  "isFirstLogin": true
}
```

### <a name="response"></a><span data-ttu-id="23b73-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="23b73-170">Response</span></span>
<span data-ttu-id="23b73-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23b73-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 456

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
  "isFirstLogin": true
}
```






