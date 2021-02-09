---
title: Criar userExperienceAnalyticsResourcePerformance
description: Crie um novo objeto userExperienceAnalyticsResourcePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b35601c4ad92313d910d4813ac8ace84c4fce9da
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162187"
---
# <a name="create-userexperienceanalyticsresourceperformance"></a><span data-ttu-id="05c4a-103">Criar userExperienceAnalyticsResourcePerformance</span><span class="sxs-lookup"><span data-stu-id="05c4a-103">Create userExperienceAnalyticsResourcePerformance</span></span>

<span data-ttu-id="05c4a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05c4a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05c4a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="05c4a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05c4a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05c4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05c4a-107">Crie um novo [objeto userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)</span><span class="sxs-lookup"><span data-stu-id="05c4a-107">Create a new [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05c4a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05c4a-108">Prerequisites</span></span>
<span data-ttu-id="05c4a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05c4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05c4a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05c4a-111">Permission type</span></span>|<span data-ttu-id="05c4a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05c4a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05c4a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05c4a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05c4a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05c4a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="05c4a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05c4a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05c4a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05c4a-116">Not supported.</span></span>|
|<span data-ttu-id="05c4a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05c4a-117">Application</span></span>|<span data-ttu-id="05c4a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05c4a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05c4a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05c4a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsResourcePerformance
```

## <a name="request-headers"></a><span data-ttu-id="05c4a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05c4a-120">Request headers</span></span>
|<span data-ttu-id="05c4a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05c4a-121">Header</span></span>|<span data-ttu-id="05c4a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="05c4a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05c4a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="05c4a-123">Authorization</span></span>|<span data-ttu-id="05c4a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05c4a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05c4a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="05c4a-125">Accept</span></span>|<span data-ttu-id="05c4a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05c4a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05c4a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05c4a-127">Request body</span></span>
<span data-ttu-id="05c4a-128">No corpo da solicitação, fornece uma representação JSON do objeto userExperienceAnalyticsResourcePerformance.</span><span class="sxs-lookup"><span data-stu-id="05c4a-128">In the request body, supply a JSON representation for the userExperienceAnalyticsResourcePerformance object.</span></span>

<span data-ttu-id="05c4a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsResourcePerformance.</span><span class="sxs-lookup"><span data-stu-id="05c4a-129">The following table shows the properties that are required when you create the userExperienceAnalyticsResourcePerformance.</span></span>

|<span data-ttu-id="05c4a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05c4a-130">Property</span></span>|<span data-ttu-id="05c4a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="05c4a-131">Type</span></span>|<span data-ttu-id="05c4a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="05c4a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05c4a-133">id</span><span class="sxs-lookup"><span data-stu-id="05c4a-133">id</span></span>|<span data-ttu-id="05c4a-134">String</span><span class="sxs-lookup"><span data-stu-id="05c4a-134">String</span></span>|<span data-ttu-id="05c4a-135">O identificador exclusivo da entidade de desempenho do recurso de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="05c4a-135">The unique identifier of the user experience analytics resource performance entity.</span></span>|
|<span data-ttu-id="05c4a-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="05c4a-136">deviceId</span></span>|<span data-ttu-id="05c4a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05c4a-137">String</span></span>|<span data-ttu-id="05c4a-138">A id do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="05c4a-138">The id of the device.</span></span>|
|<span data-ttu-id="05c4a-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="05c4a-139">deviceName</span></span>|<span data-ttu-id="05c4a-140">String</span><span class="sxs-lookup"><span data-stu-id="05c4a-140">String</span></span>|<span data-ttu-id="05c4a-141">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="05c4a-141">The name of the device.</span></span>|
|<span data-ttu-id="05c4a-142">modelo</span><span class="sxs-lookup"><span data-stu-id="05c4a-142">model</span></span>|<span data-ttu-id="05c4a-143">String</span><span class="sxs-lookup"><span data-stu-id="05c4a-143">String</span></span>|<span data-ttu-id="05c4a-144">O modelo de dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="05c4a-144">The user experience analytics device model.</span></span>|
|<span data-ttu-id="05c4a-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="05c4a-145">deviceCount</span></span>|<span data-ttu-id="05c4a-146">Int64</span><span class="sxs-lookup"><span data-stu-id="05c4a-146">Int64</span></span>|<span data-ttu-id="05c4a-147">Contagem resumida de dispositivos da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="05c4a-147">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="05c4a-148">fabricante</span><span class="sxs-lookup"><span data-stu-id="05c4a-148">manufacturer</span></span>|<span data-ttu-id="05c4a-149">String</span><span class="sxs-lookup"><span data-stu-id="05c4a-149">String</span></span>|<span data-ttu-id="05c4a-150">O fabricante do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="05c4a-150">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="05c4a-151">cpuSpikeTimePercentage</span><span class="sxs-lookup"><span data-stu-id="05c4a-151">cpuSpikeTimePercentage</span></span>|<span data-ttu-id="05c4a-152">Duplo</span><span class="sxs-lookup"><span data-stu-id="05c4a-152">Double</span></span>|<span data-ttu-id="05c4a-153">Tempo de pico da CPU em porcentagem.</span><span class="sxs-lookup"><span data-stu-id="05c4a-153">CPU spike time in percentage.</span></span> <span data-ttu-id="05c4a-154">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="05c4a-154">Valid values 0 to 100</span></span>|
|<span data-ttu-id="05c4a-155">ramSpikeTimePercentage</span><span class="sxs-lookup"><span data-stu-id="05c4a-155">ramSpikeTimePercentage</span></span>|<span data-ttu-id="05c4a-156">Duplo</span><span class="sxs-lookup"><span data-stu-id="05c4a-156">Double</span></span>|<span data-ttu-id="05c4a-157">Tempo de pico da RAM em porcentagem.</span><span class="sxs-lookup"><span data-stu-id="05c4a-157">RAM spike time in percentage.</span></span> <span data-ttu-id="05c4a-158">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="05c4a-158">Valid values 0 to 100</span></span>|
|<span data-ttu-id="05c4a-159">cpuSpikeTimeScore</span><span class="sxs-lookup"><span data-stu-id="05c4a-159">cpuSpikeTimeScore</span></span>|<span data-ttu-id="05c4a-160">Int32</span><span class="sxs-lookup"><span data-stu-id="05c4a-160">Int32</span></span>|<span data-ttu-id="05c4a-161">A pontuação de tempo de pico da CPU do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="05c4a-161">The user experience analytics device CPU spike time score.</span></span> <span data-ttu-id="05c4a-162">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="05c4a-162">Valid values 0 to 100</span></span>|
|<span data-ttu-id="05c4a-163">cpuSpikeTimePercentageThreshold</span><span class="sxs-lookup"><span data-stu-id="05c4a-163">cpuSpikeTimePercentageThreshold</span></span>|<span data-ttu-id="05c4a-164">Duplo</span><span class="sxs-lookup"><span data-stu-id="05c4a-164">Double</span></span>|<span data-ttu-id="05c4a-165">Limite de cpuSpikeTimeScore.</span><span class="sxs-lookup"><span data-stu-id="05c4a-165">Threshold of cpuSpikeTimeScore.</span></span> <span data-ttu-id="05c4a-166">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="05c4a-166">Valid values 0 to 100</span></span>|
|<span data-ttu-id="05c4a-167">ramSpikeTimeScore</span><span class="sxs-lookup"><span data-stu-id="05c4a-167">ramSpikeTimeScore</span></span>|<span data-ttu-id="05c4a-168">Int32</span><span class="sxs-lookup"><span data-stu-id="05c4a-168">Int32</span></span>|<span data-ttu-id="05c4a-169">A pontuação de tempo de pico da RAM do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="05c4a-169">The user experience analytics device RAM spike time score.</span></span> <span data-ttu-id="05c4a-170">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="05c4a-170">Valid values 0 to 100</span></span>|
|<span data-ttu-id="05c4a-171">ramSpikeTimePercentageThreshold</span><span class="sxs-lookup"><span data-stu-id="05c4a-171">ramSpikeTimePercentageThreshold</span></span>|<span data-ttu-id="05c4a-172">Duplo</span><span class="sxs-lookup"><span data-stu-id="05c4a-172">Double</span></span>|<span data-ttu-id="05c4a-173">Limite de ramSpikeTimeScore.</span><span class="sxs-lookup"><span data-stu-id="05c4a-173">Threshold of ramSpikeTimeScore.</span></span> <span data-ttu-id="05c4a-174">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="05c4a-174">Valid values 0 to 100</span></span>|
|<span data-ttu-id="05c4a-175">deviceResourcePerformanceScore</span><span class="sxs-lookup"><span data-stu-id="05c4a-175">deviceResourcePerformanceScore</span></span>|<span data-ttu-id="05c4a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="05c4a-176">Int32</span></span>|<span data-ttu-id="05c4a-177">Pontuação de desempenho de recursos de um dispositivo específico.</span><span class="sxs-lookup"><span data-stu-id="05c4a-177">Resource performance score of a specific device.</span></span> <span data-ttu-id="05c4a-178">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="05c4a-178">Valid values 0 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="05c4a-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c4a-179">Response</span></span>
<span data-ttu-id="05c4a-180">Se tiver êxito, este método retornará um código de resposta e um objeto `201 Created` [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05c4a-180">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05c4a-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05c4a-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="05c4a-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05c4a-182">Request</span></span>
<span data-ttu-id="05c4a-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05c4a-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsResourcePerformance
Content-type: application/json
Content-length: 553

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "deviceCount": 11,
  "manufacturer": "Manufacturer value",
  "cpuSpikeTimePercentage": 7.333333333333333,
  "ramSpikeTimePercentage": 7.333333333333333,
  "cpuSpikeTimeScore": 1,
  "cpuSpikeTimePercentageThreshold": 10.333333333333334,
  "ramSpikeTimeScore": 1,
  "ramSpikeTimePercentageThreshold": 10.333333333333334,
  "deviceResourcePerformanceScore": 14
}
```

### <a name="response"></a><span data-ttu-id="05c4a-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c4a-184">Response</span></span>
<span data-ttu-id="05c4a-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05c4a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 602

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
  "id": "d34d78e8-78e8-d34d-e878-4dd3e8784dd3",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "deviceCount": 11,
  "manufacturer": "Manufacturer value",
  "cpuSpikeTimePercentage": 7.333333333333333,
  "ramSpikeTimePercentage": 7.333333333333333,
  "cpuSpikeTimeScore": 1,
  "cpuSpikeTimePercentageThreshold": 10.333333333333334,
  "ramSpikeTimeScore": 1,
  "ramSpikeTimePercentageThreshold": 10.333333333333334,
  "deviceResourcePerformanceScore": 14
}
```




