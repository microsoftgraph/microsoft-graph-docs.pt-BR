---
title: Atualizar userExperienceAnalyticsAppHealthDeviceModelPerformance
description: Atualize as propriedades de um objeto userExperienceAnalyticsAppHealthDeviceModelPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26667c68a45158a29c991dc91be28bce0cf13fd9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136157"
---
# <a name="update-userexperienceanalyticsapphealthdevicemodelperformance"></a><span data-ttu-id="9010c-103">Atualizar userExperienceAnalyticsAppHealthDeviceModelPerformance</span><span class="sxs-lookup"><span data-stu-id="9010c-103">Update userExperienceAnalyticsAppHealthDeviceModelPerformance</span></span>

<span data-ttu-id="9010c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9010c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9010c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9010c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9010c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9010c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9010c-107">Atualize as propriedades de [um objeto userExperienceAnalyticsAppHealthDeviceModelPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)</span><span class="sxs-lookup"><span data-stu-id="9010c-107">Update the properties of a [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9010c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9010c-108">Prerequisites</span></span>
<span data-ttu-id="9010c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9010c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9010c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9010c-111">Permission type</span></span>|<span data-ttu-id="9010c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9010c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9010c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9010c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9010c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9010c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9010c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9010c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9010c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9010c-116">Not supported.</span></span>|
|<span data-ttu-id="9010c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9010c-117">Application</span></span>|<span data-ttu-id="9010c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9010c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9010c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9010c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="9010c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9010c-120">Request headers</span></span>
|<span data-ttu-id="9010c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9010c-121">Header</span></span>|<span data-ttu-id="9010c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9010c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9010c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9010c-123">Authorization</span></span>|<span data-ttu-id="9010c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9010c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9010c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9010c-125">Accept</span></span>|<span data-ttu-id="9010c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9010c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9010c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9010c-127">Request body</span></span>
<span data-ttu-id="9010c-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsAppHealthDeviceModelPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)</span><span class="sxs-lookup"><span data-stu-id="9010c-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object.</span></span>

<span data-ttu-id="9010c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o usuárioExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md).</span><span class="sxs-lookup"><span data-stu-id="9010c-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md).</span></span>

|<span data-ttu-id="9010c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9010c-130">Property</span></span>|<span data-ttu-id="9010c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9010c-131">Type</span></span>|<span data-ttu-id="9010c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9010c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9010c-133">id</span><span class="sxs-lookup"><span data-stu-id="9010c-133">id</span></span>|<span data-ttu-id="9010c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9010c-134">String</span></span>|<span data-ttu-id="9010c-135">O identificador exclusivo do objeto de desempenho do modelo de dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9010c-135">The unique identifier of the user experience analytics device model performance object.</span></span>|
|<span data-ttu-id="9010c-136">deviceModel</span><span class="sxs-lookup"><span data-stu-id="9010c-136">deviceModel</span></span>|<span data-ttu-id="9010c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9010c-137">String</span></span>|<span data-ttu-id="9010c-138">O nome do modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9010c-138">The model name of the device.</span></span>|
|<span data-ttu-id="9010c-139">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="9010c-139">deviceManufacturer</span></span>|<span data-ttu-id="9010c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9010c-140">String</span></span>|<span data-ttu-id="9010c-141">O nome do fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9010c-141">The manufacturer name of the device.</span></span>|
|<span data-ttu-id="9010c-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9010c-142">activeDeviceCount</span></span>|<span data-ttu-id="9010c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9010c-143">Int32</span></span>|<span data-ttu-id="9010c-144">O número de dispositivos ativos para o modelo.</span><span class="sxs-lookup"><span data-stu-id="9010c-144">The number of active devices for the model.</span></span> <span data-ttu-id="9010c-145">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="9010c-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="9010c-146">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="9010c-146">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="9010c-147">Int32</span><span class="sxs-lookup"><span data-stu-id="9010c-147">Int32</span></span>|<span data-ttu-id="9010c-148">O tempo de falha média para o dispositivo modelo em minutos.</span><span class="sxs-lookup"><span data-stu-id="9010c-148">The mean time to failure for the model device in minutes.</span></span> <span data-ttu-id="9010c-149">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="9010c-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="9010c-150">modelAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="9010c-150">modelAppHealthScore</span></span>|<span data-ttu-id="9010c-151">Duplo</span><span class="sxs-lookup"><span data-stu-id="9010c-151">Double</span></span>|<span data-ttu-id="9010c-152">A pontuação de saúde do aplicativo do modelo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9010c-152">The app health score of the device model.</span></span> <span data-ttu-id="9010c-153">Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="9010c-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="9010c-154">modelAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="9010c-154">modelAppHealthStatus</span></span>|<span data-ttu-id="9010c-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9010c-155">String</span></span>|<span data-ttu-id="9010c-156">O status geral da saúde do aplicativo do modelo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9010c-156">The overall app health status of the device model.</span></span>|



## <a name="response"></a><span data-ttu-id="9010c-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="9010c-157">Response</span></span>
<span data-ttu-id="9010c-158">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9010c-158">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9010c-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9010c-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="9010c-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9010c-160">Request</span></span>
<span data-ttu-id="9010c-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9010c-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9010c-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="9010c-162">Response</span></span>
<span data-ttu-id="9010c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9010c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




