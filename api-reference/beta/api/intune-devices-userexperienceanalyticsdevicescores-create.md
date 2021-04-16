---
title: Criar userExperienceAnalyticsDeviceScores
description: Crie um novo objeto userExperienceAnalyticsDeviceScores.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 60b7474deb9a9f845f7d90e419e1c5c813dce483
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868351"
---
# <a name="create-userexperienceanalyticsdevicescores"></a><span data-ttu-id="d602d-103">Criar userExperienceAnalyticsDeviceScores</span><span class="sxs-lookup"><span data-stu-id="d602d-103">Create userExperienceAnalyticsDeviceScores</span></span>

<span data-ttu-id="d602d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d602d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d602d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d602d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d602d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d602d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d602d-107">Crie um novo [objeto userExperienceAnalyticsDeviceScores.](../resources/intune-devices-userexperienceanalyticsdevicescores.md)</span><span class="sxs-lookup"><span data-stu-id="d602d-107">Create a new [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d602d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d602d-108">Prerequisites</span></span>
<span data-ttu-id="d602d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d602d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d602d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d602d-111">Permission type</span></span>|<span data-ttu-id="d602d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d602d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d602d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d602d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d602d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d602d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d602d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d602d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d602d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d602d-116">Not supported.</span></span>|
|<span data-ttu-id="d602d-117">Application</span><span class="sxs-lookup"><span data-stu-id="d602d-117">Application</span></span>|<span data-ttu-id="d602d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d602d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d602d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d602d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceScores
```

## <a name="request-headers"></a><span data-ttu-id="d602d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d602d-120">Request headers</span></span>
|<span data-ttu-id="d602d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d602d-121">Header</span></span>|<span data-ttu-id="d602d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d602d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d602d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d602d-123">Authorization</span></span>|<span data-ttu-id="d602d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d602d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d602d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d602d-125">Accept</span></span>|<span data-ttu-id="d602d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d602d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d602d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d602d-127">Request body</span></span>
<span data-ttu-id="d602d-128">No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsDeviceScores.</span><span class="sxs-lookup"><span data-stu-id="d602d-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceScores object.</span></span>

<span data-ttu-id="d602d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsDeviceScores.</span><span class="sxs-lookup"><span data-stu-id="d602d-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceScores.</span></span>

|<span data-ttu-id="d602d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d602d-130">Property</span></span>|<span data-ttu-id="d602d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d602d-131">Type</span></span>|<span data-ttu-id="d602d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d602d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d602d-133">id</span><span class="sxs-lookup"><span data-stu-id="d602d-133">id</span></span>|<span data-ttu-id="d602d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d602d-134">String</span></span>|<span data-ttu-id="d602d-135">O identificador exclusivo do dispositivo de pontuação do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="d602d-135">The unique identifier of the user experience analytics device scores device.</span></span>|
|<span data-ttu-id="d602d-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="d602d-136">deviceName</span></span>|<span data-ttu-id="d602d-137">String</span><span class="sxs-lookup"><span data-stu-id="d602d-137">String</span></span>|<span data-ttu-id="d602d-138">O nome do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="d602d-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="d602d-139">modelo</span><span class="sxs-lookup"><span data-stu-id="d602d-139">model</span></span>|<span data-ttu-id="d602d-140">String</span><span class="sxs-lookup"><span data-stu-id="d602d-140">String</span></span>|<span data-ttu-id="d602d-141">O modelo de dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="d602d-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="d602d-142">fabricante</span><span class="sxs-lookup"><span data-stu-id="d602d-142">manufacturer</span></span>|<span data-ttu-id="d602d-143">String</span><span class="sxs-lookup"><span data-stu-id="d602d-143">String</span></span>|<span data-ttu-id="d602d-144">O fabricante do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="d602d-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="d602d-145">endpointAnalyticsScore</span><span class="sxs-lookup"><span data-stu-id="d602d-145">endpointAnalyticsScore</span></span>|<span data-ttu-id="d602d-146">Duplo</span><span class="sxs-lookup"><span data-stu-id="d602d-146">Double</span></span>|<span data-ttu-id="d602d-147">A pontuação do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="d602d-147">The user experience analytics device score.</span></span> <span data-ttu-id="d602d-148">Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="d602d-148">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="d602d-149">startupPerformanceScore</span><span class="sxs-lookup"><span data-stu-id="d602d-149">startupPerformanceScore</span></span>|<span data-ttu-id="d602d-150">Duplo</span><span class="sxs-lookup"><span data-stu-id="d602d-150">Double</span></span>|<span data-ttu-id="d602d-151">A pontuação de desempenho de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="d602d-151">The user experience analytics device startup performance score.</span></span> <span data-ttu-id="d602d-152">Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="d602d-152">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="d602d-153">appReliabilityScore</span><span class="sxs-lookup"><span data-stu-id="d602d-153">appReliabilityScore</span></span>|<span data-ttu-id="d602d-154">Duplo</span><span class="sxs-lookup"><span data-stu-id="d602d-154">Double</span></span>|<span data-ttu-id="d602d-155">A pontuação de confiabilidade do aplicativo de dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="d602d-155">The user experience analytics device app reliability score.</span></span> <span data-ttu-id="d602d-156">Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="d602d-156">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="d602d-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="d602d-157">Response</span></span>
<span data-ttu-id="d602d-158">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d602d-158">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d602d-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d602d-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="d602d-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d602d-160">Request</span></span>
<span data-ttu-id="d602d-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d602d-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceScores
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "endpointAnalyticsScore": 7.333333333333333,
  "startupPerformanceScore": 7.666666666666667,
  "appReliabilityScore": 6.333333333333333
}
```

### <a name="response"></a><span data-ttu-id="d602d-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="d602d-162">Response</span></span>
<span data-ttu-id="d602d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d602d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 374

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
  "id": "0dd9f6cf-f6cf-0dd9-cff6-d90dcff6d90d",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "endpointAnalyticsScore": 7.333333333333333,
  "startupPerformanceScore": 7.666666666666667,
  "appReliabilityScore": 6.333333333333333
}
```




