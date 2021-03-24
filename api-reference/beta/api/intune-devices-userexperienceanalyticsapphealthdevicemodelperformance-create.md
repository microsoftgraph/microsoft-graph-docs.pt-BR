---
title: Criar userExperienceAnalyticsAppHealthDeviceModelPerformance
description: Crie um novo objeto userExperienceAnalyticsAppHealthDeviceModelPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5592d2acc10279b4a9af869443acf9b961ab0e9b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136199"
---
# <a name="create-userexperienceanalyticsapphealthdevicemodelperformance"></a><span data-ttu-id="f7bb4-103">Criar userExperienceAnalyticsAppHealthDeviceModelPerformance</span><span class="sxs-lookup"><span data-stu-id="f7bb4-103">Create userExperienceAnalyticsAppHealthDeviceModelPerformance</span></span>

<span data-ttu-id="f7bb4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7bb4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7bb4-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f7bb4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7bb4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f7bb4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7bb4-107">Crie um novo [objeto userExperienceAnalyticsAppHealthDeviceModelPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)</span><span class="sxs-lookup"><span data-stu-id="f7bb4-107">Create a new [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7bb4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f7bb4-108">Prerequisites</span></span>
<span data-ttu-id="f7bb4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7bb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7bb4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7bb4-111">Permission type</span></span>|<span data-ttu-id="f7bb4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7bb4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7bb4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7bb4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7bb4-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7bb4-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f7bb4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7bb4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7bb4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7bb4-116">Not supported.</span></span>|
|<span data-ttu-id="f7bb4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7bb4-117">Application</span></span>|<span data-ttu-id="f7bb4-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7bb4-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7bb4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7bb4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance
```

## <a name="request-headers"></a><span data-ttu-id="f7bb4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7bb4-120">Request headers</span></span>
|<span data-ttu-id="f7bb4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7bb4-121">Header</span></span>|<span data-ttu-id="f7bb4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f7bb4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7bb4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7bb4-123">Authorization</span></span>|<span data-ttu-id="f7bb4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7bb4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7bb4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f7bb4-125">Accept</span></span>|<span data-ttu-id="f7bb4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7bb4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7bb4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7bb4-127">Request body</span></span>
<span data-ttu-id="f7bb4-128">No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsAppHealthDeviceModelPerformance.</span><span class="sxs-lookup"><span data-stu-id="f7bb4-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthDeviceModelPerformance object.</span></span>

<span data-ttu-id="f7bb4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsAppHealthDeviceModelPerformance.</span><span class="sxs-lookup"><span data-stu-id="f7bb4-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthDeviceModelPerformance.</span></span>

|<span data-ttu-id="f7bb4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7bb4-130">Property</span></span>|<span data-ttu-id="f7bb4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7bb4-131">Type</span></span>|<span data-ttu-id="f7bb4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7bb4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7bb4-133">id</span><span class="sxs-lookup"><span data-stu-id="f7bb4-133">id</span></span>|<span data-ttu-id="f7bb4-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7bb4-134">String</span></span>|<span data-ttu-id="f7bb4-135">O identificador exclusivo do objeto de desempenho do modelo de dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="f7bb4-135">The unique identifier of the user experience analytics device model performance object.</span></span>|
|<span data-ttu-id="f7bb4-136">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f7bb4-136">deviceModel</span></span>|<span data-ttu-id="f7bb4-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7bb4-137">String</span></span>|<span data-ttu-id="f7bb4-138">O nome do modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f7bb4-138">The model name of the device.</span></span>|
|<span data-ttu-id="f7bb4-139">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="f7bb4-139">deviceManufacturer</span></span>|<span data-ttu-id="f7bb4-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7bb4-140">String</span></span>|<span data-ttu-id="f7bb4-141">O nome do fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f7bb4-141">The manufacturer name of the device.</span></span>|
|<span data-ttu-id="f7bb4-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7bb4-142">activeDeviceCount</span></span>|<span data-ttu-id="f7bb4-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f7bb4-143">Int32</span></span>|<span data-ttu-id="f7bb4-144">O número de dispositivos ativos para o modelo.</span><span class="sxs-lookup"><span data-stu-id="f7bb4-144">The number of active devices for the model.</span></span> <span data-ttu-id="f7bb4-145">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="f7bb4-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="f7bb4-146">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="f7bb4-146">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="f7bb4-147">Int32</span><span class="sxs-lookup"><span data-stu-id="f7bb4-147">Int32</span></span>|<span data-ttu-id="f7bb4-148">O tempo de falha média para o dispositivo modelo em minutos.</span><span class="sxs-lookup"><span data-stu-id="f7bb4-148">The mean time to failure for the model device in minutes.</span></span> <span data-ttu-id="f7bb4-149">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="f7bb4-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="f7bb4-150">modelAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="f7bb4-150">modelAppHealthScore</span></span>|<span data-ttu-id="f7bb4-151">Duplo</span><span class="sxs-lookup"><span data-stu-id="f7bb4-151">Double</span></span>|<span data-ttu-id="f7bb4-152">A pontuação de saúde do aplicativo do modelo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f7bb4-152">The app health score of the device model.</span></span> <span data-ttu-id="f7bb4-153">Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="f7bb4-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="f7bb4-154">modelAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="f7bb4-154">modelAppHealthStatus</span></span>|<span data-ttu-id="f7bb4-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7bb4-155">String</span></span>|<span data-ttu-id="f7bb4-156">O status geral da saúde do aplicativo do modelo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f7bb4-156">The overall app health status of the device model.</span></span>|



## <a name="response"></a><span data-ttu-id="f7bb4-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7bb4-157">Response</span></span>
<span data-ttu-id="f7bb4-158">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7bb4-158">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7bb4-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7bb4-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7bb4-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7bb4-160">Request</span></span>
<span data-ttu-id="f7bb4-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7bb4-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance
Content-type: application/json
Content-length: 359

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "modelAppHealthScore": 6.333333333333333,
  "modelAppHealthStatus": "Model App Health Status value"
}
```

### <a name="response"></a><span data-ttu-id="f7bb4-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7bb4-162">Response</span></span>
<span data-ttu-id="f7bb4-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7bb4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 408

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance",
  "id": "4daddc60-dc60-4dad-60dc-ad4d60dcad4d",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "modelAppHealthScore": 6.333333333333333,
  "modelAppHealthStatus": "Model App Health Status value"
}
```




