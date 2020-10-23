---
title: Criar userExperienceAnalyticsAppHealthDevicePerformanceDetails
description: Criar um novo objeto userExperienceAnalyticsAppHealthDevicePerformanceDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7b84784636ff3fe6d4efe5f4644e929c06dfe82f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693175"
---
# <a name="create-userexperienceanalyticsapphealthdeviceperformancedetails"></a><span data-ttu-id="78782-103">Criar userExperienceAnalyticsAppHealthDevicePerformanceDetails</span><span class="sxs-lookup"><span data-stu-id="78782-103">Create userExperienceAnalyticsAppHealthDevicePerformanceDetails</span></span>

<span data-ttu-id="78782-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78782-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78782-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="78782-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78782-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78782-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78782-107">Criar um novo objeto [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .</span><span class="sxs-lookup"><span data-stu-id="78782-107">Create a new [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78782-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="78782-108">Prerequisites</span></span>
<span data-ttu-id="78782-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78782-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78782-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78782-111">Permission type</span></span>|<span data-ttu-id="78782-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="78782-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78782-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78782-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78782-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78782-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="78782-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78782-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78782-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78782-116">Not supported.</span></span>|
|<span data-ttu-id="78782-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78782-117">Application</span></span>|<span data-ttu-id="78782-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78782-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78782-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78782-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
```

## <a name="request-headers"></a><span data-ttu-id="78782-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78782-120">Request headers</span></span>
|<span data-ttu-id="78782-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78782-121">Header</span></span>|<span data-ttu-id="78782-122">Valor</span><span class="sxs-lookup"><span data-stu-id="78782-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78782-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="78782-123">Authorization</span></span>|<span data-ttu-id="78782-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78782-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78782-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="78782-125">Accept</span></span>|<span data-ttu-id="78782-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78782-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78782-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78782-127">Request body</span></span>
<span data-ttu-id="78782-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsAppHealthDevicePerformanceDetails.</span><span class="sxs-lookup"><span data-stu-id="78782-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthDevicePerformanceDetails object.</span></span>

<span data-ttu-id="78782-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsAppHealthDevicePerformanceDetails.</span><span class="sxs-lookup"><span data-stu-id="78782-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthDevicePerformanceDetails.</span></span>

|<span data-ttu-id="78782-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78782-130">Property</span></span>|<span data-ttu-id="78782-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="78782-131">Type</span></span>|<span data-ttu-id="78782-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="78782-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78782-133">id</span><span class="sxs-lookup"><span data-stu-id="78782-133">id</span></span>|<span data-ttu-id="78782-134">String</span><span class="sxs-lookup"><span data-stu-id="78782-134">String</span></span>|<span data-ttu-id="78782-135">O identificador exclusivo do objeto de desempenho do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="78782-135">The unique identifier of the user experience analytics device performance object.</span></span>|
|<span data-ttu-id="78782-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="78782-136">eventDateTime</span></span>|<span data-ttu-id="78782-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78782-137">DateTimeOffset</span></span>|<span data-ttu-id="78782-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="78782-138">The time the event occurred.</span></span>|
|<span data-ttu-id="78782-139">eventType</span><span class="sxs-lookup"><span data-stu-id="78782-139">eventType</span></span>|<span data-ttu-id="78782-140">String</span><span class="sxs-lookup"><span data-stu-id="78782-140">String</span></span>|<span data-ttu-id="78782-141">O tipo do evento.</span><span class="sxs-lookup"><span data-stu-id="78782-141">The type of the event.</span></span>|
|<span data-ttu-id="78782-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="78782-142">appDisplayName</span></span>|<span data-ttu-id="78782-143">String</span><span class="sxs-lookup"><span data-stu-id="78782-143">String</span></span>|<span data-ttu-id="78782-144">O nome amigável do aplicativo para o qual o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="78782-144">The friendly name of the application for which the event occurred.</span></span>|
|<span data-ttu-id="78782-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="78782-145">deviceId</span></span>|<span data-ttu-id="78782-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78782-146">String</span></span>|<span data-ttu-id="78782-147">A ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="78782-147">The id of the device.</span></span>|
|<span data-ttu-id="78782-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="78782-148">deviceDisplayName</span></span>|<span data-ttu-id="78782-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78782-149">String</span></span>|<span data-ttu-id="78782-150">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="78782-150">The name of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="78782-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="78782-151">Response</span></span>
<span data-ttu-id="78782-152">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78782-152">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78782-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78782-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="78782-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78782-154">Request</span></span>
<span data-ttu-id="78782-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78782-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
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

### <a name="response"></a><span data-ttu-id="78782-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="78782-156">Response</span></span>
<span data-ttu-id="78782-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78782-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





