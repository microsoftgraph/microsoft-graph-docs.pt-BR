---
title: Atualizar userExperienceAnalyticsAppHealthDevicePerformanceDetails
description: Atualize as propriedades de um objeto userExperienceAnalyticsAppHealthDevicePerformanceDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d4a922aa2d6101667024dff7fa458f43fb82f25
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136010"
---
# <a name="update-userexperienceanalyticsapphealthdeviceperformancedetails"></a><span data-ttu-id="77664-103">Atualizar userExperienceAnalyticsAppHealthDevicePerformanceDetails</span><span class="sxs-lookup"><span data-stu-id="77664-103">Update userExperienceAnalyticsAppHealthDevicePerformanceDetails</span></span>

<span data-ttu-id="77664-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77664-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77664-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="77664-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77664-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77664-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77664-107">Atualize as propriedades de [um objeto userExperienceAnalyticsAppHealthDevicePerformanceDetails.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)</span><span class="sxs-lookup"><span data-stu-id="77664-107">Update the properties of a [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77664-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="77664-108">Prerequisites</span></span>
<span data-ttu-id="77664-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77664-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77664-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77664-111">Permission type</span></span>|<span data-ttu-id="77664-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77664-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77664-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77664-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77664-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77664-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="77664-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77664-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77664-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77664-116">Not supported.</span></span>|
|<span data-ttu-id="77664-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77664-117">Application</span></span>|<span data-ttu-id="77664-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77664-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77664-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77664-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails/{userExperienceAnalyticsAppHealthDevicePerformanceDetailsId}
```

## <a name="request-headers"></a><span data-ttu-id="77664-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77664-120">Request headers</span></span>
|<span data-ttu-id="77664-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77664-121">Header</span></span>|<span data-ttu-id="77664-122">Valor</span><span class="sxs-lookup"><span data-stu-id="77664-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77664-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="77664-123">Authorization</span></span>|<span data-ttu-id="77664-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77664-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77664-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="77664-125">Accept</span></span>|<span data-ttu-id="77664-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77664-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77664-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77664-127">Request body</span></span>
<span data-ttu-id="77664-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsAppHealthDevicePerformanceDetails.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)</span><span class="sxs-lookup"><span data-stu-id="77664-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) object.</span></span>

<span data-ttu-id="77664-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md).</span><span class="sxs-lookup"><span data-stu-id="77664-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md).</span></span>

|<span data-ttu-id="77664-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77664-130">Property</span></span>|<span data-ttu-id="77664-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="77664-131">Type</span></span>|<span data-ttu-id="77664-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="77664-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77664-133">id</span><span class="sxs-lookup"><span data-stu-id="77664-133">id</span></span>|<span data-ttu-id="77664-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77664-134">String</span></span>|<span data-ttu-id="77664-135">O identificador exclusivo do objeto de desempenho do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="77664-135">The unique identifier of the user experience analytics device performance object.</span></span>|
|<span data-ttu-id="77664-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="77664-136">eventDateTime</span></span>|<span data-ttu-id="77664-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77664-137">DateTimeOffset</span></span>|<span data-ttu-id="77664-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="77664-138">The time the event occurred.</span></span>|
|<span data-ttu-id="77664-139">eventType</span><span class="sxs-lookup"><span data-stu-id="77664-139">eventType</span></span>|<span data-ttu-id="77664-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77664-140">String</span></span>|<span data-ttu-id="77664-141">O tipo do evento.</span><span class="sxs-lookup"><span data-stu-id="77664-141">The type of the event.</span></span>|
|<span data-ttu-id="77664-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="77664-142">appDisplayName</span></span>|<span data-ttu-id="77664-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77664-143">String</span></span>|<span data-ttu-id="77664-144">O nome amigável do aplicativo para o qual o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="77664-144">The friendly name of the application for which the event occurred.</span></span>|
|<span data-ttu-id="77664-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="77664-145">deviceId</span></span>|<span data-ttu-id="77664-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77664-146">String</span></span>|<span data-ttu-id="77664-147">A id do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="77664-147">The id of the device.</span></span>|
|<span data-ttu-id="77664-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="77664-148">deviceDisplayName</span></span>|<span data-ttu-id="77664-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77664-149">String</span></span>|<span data-ttu-id="77664-150">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="77664-150">The name of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="77664-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="77664-151">Response</span></span>
<span data-ttu-id="77664-152">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77664-152">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77664-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77664-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="77664-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77664-154">Request</span></span>
<span data-ttu-id="77664-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77664-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails/{userExperienceAnalyticsAppHealthDevicePerformanceDetailsId}
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "eventType": "Event Type value",
  "appDisplayName": "App Display Name value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="77664-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="77664-156">Response</span></span>
<span data-ttu-id="77664-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77664-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "id": "bc8c5273-5273-bc8c-7352-8cbc73528cbc",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "eventType": "Event Type value",
  "appDisplayName": "App Display Name value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```




