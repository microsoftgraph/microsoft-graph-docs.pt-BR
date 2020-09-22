---
title: Atualizar userExperienceAnalyticsAppHealthDeviceModelPerformance
description: Atualiza as propriedades de um objeto userExperienceAnalyticsAppHealthDeviceModelPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5cf04fafbea00ca2a3f45c659d1996b399ddba7d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992516"
---
# <a name="update-userexperienceanalyticsapphealthdevicemodelperformance"></a><span data-ttu-id="c6483-103">Atualizar userExperienceAnalyticsAppHealthDeviceModelPerformance</span><span class="sxs-lookup"><span data-stu-id="c6483-103">Update userExperienceAnalyticsAppHealthDeviceModelPerformance</span></span>

<span data-ttu-id="c6483-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6483-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6483-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c6483-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6483-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c6483-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6483-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="c6483-107">Update the properties of a [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6483-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c6483-108">Prerequisites</span></span>
<span data-ttu-id="c6483-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6483-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6483-111">Permission type</span></span>|<span data-ttu-id="c6483-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c6483-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6483-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6483-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6483-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6483-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c6483-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6483-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6483-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6483-116">Not supported.</span></span>|
|<span data-ttu-id="c6483-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6483-117">Application</span></span>|<span data-ttu-id="c6483-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6483-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6483-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6483-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="c6483-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6483-120">Request headers</span></span>
|<span data-ttu-id="c6483-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6483-121">Header</span></span>|<span data-ttu-id="c6483-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c6483-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6483-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6483-123">Authorization</span></span>|<span data-ttu-id="c6483-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6483-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6483-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c6483-125">Accept</span></span>|<span data-ttu-id="c6483-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6483-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6483-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6483-127">Request body</span></span>
<span data-ttu-id="c6483-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="c6483-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object.</span></span>

<span data-ttu-id="c6483-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md).</span><span class="sxs-lookup"><span data-stu-id="c6483-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md).</span></span>

|<span data-ttu-id="c6483-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6483-130">Property</span></span>|<span data-ttu-id="c6483-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6483-131">Type</span></span>|<span data-ttu-id="c6483-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6483-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6483-133">id</span><span class="sxs-lookup"><span data-stu-id="c6483-133">id</span></span>|<span data-ttu-id="c6483-134">String</span><span class="sxs-lookup"><span data-stu-id="c6483-134">String</span></span>|<span data-ttu-id="c6483-135">O identificador exclusivo do objeto de desempenho da experiência do usuário do Analytics Device Model.</span><span class="sxs-lookup"><span data-stu-id="c6483-135">The unique identifier of the user experience analytics device model performance object.</span></span>|
|<span data-ttu-id="c6483-136">deviceModel</span><span class="sxs-lookup"><span data-stu-id="c6483-136">deviceModel</span></span>|<span data-ttu-id="c6483-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6483-137">String</span></span>|<span data-ttu-id="c6483-138">O nome do modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c6483-138">The model name of the device.</span></span>|
|<span data-ttu-id="c6483-139">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="c6483-139">deviceManufacturer</span></span>|<span data-ttu-id="c6483-140">String</span><span class="sxs-lookup"><span data-stu-id="c6483-140">String</span></span>|<span data-ttu-id="c6483-141">O nome do fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c6483-141">The manufacturer name of the device.</span></span>|
|<span data-ttu-id="c6483-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c6483-142">activeDeviceCount</span></span>|<span data-ttu-id="c6483-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c6483-143">Int32</span></span>|<span data-ttu-id="c6483-144">O número de dispositivos ativos para o modelo.</span><span class="sxs-lookup"><span data-stu-id="c6483-144">The number of active devices for the model.</span></span> <span data-ttu-id="c6483-145">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="c6483-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="c6483-146">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="c6483-146">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="c6483-147">Int32</span><span class="sxs-lookup"><span data-stu-id="c6483-147">Int32</span></span>|<span data-ttu-id="c6483-148">O tempo médio de falha para o dispositivo de modelo em minutos.</span><span class="sxs-lookup"><span data-stu-id="c6483-148">The mean time to failure for the model device in minutes.</span></span> <span data-ttu-id="c6483-149">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="c6483-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="c6483-150">modelAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="c6483-150">modelAppHealthScore</span></span>|<span data-ttu-id="c6483-151">Duplo</span><span class="sxs-lookup"><span data-stu-id="c6483-151">Double</span></span>|<span data-ttu-id="c6483-152">A pontuação de integridade do aplicativo do modelo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c6483-152">The app health score of the device model.</span></span> <span data-ttu-id="c6483-153">Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="c6483-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="c6483-154">modelAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="c6483-154">modelAppHealthStatus</span></span>|<span data-ttu-id="c6483-155">String</span><span class="sxs-lookup"><span data-stu-id="c6483-155">String</span></span>|<span data-ttu-id="c6483-156">O status de integridade do aplicativo geral do modelo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c6483-156">The overall app health status of the device model.</span></span>|



## <a name="response"></a><span data-ttu-id="c6483-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6483-157">Response</span></span>
<span data-ttu-id="c6483-158">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6483-158">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6483-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6483-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6483-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6483-160">Request</span></span>
<span data-ttu-id="c6483-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6483-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
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

### <a name="response"></a><span data-ttu-id="c6483-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6483-162">Response</span></span>
<span data-ttu-id="c6483-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6483-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






