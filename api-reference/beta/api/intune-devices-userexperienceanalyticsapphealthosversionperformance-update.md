---
title: Atualizar userExperienceAnalyticsAppHealthOSVersionPerformance
description: Atualize as propriedades de um objeto userExperienceAnalyticsAppHealthOSVersionPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 67fc4fbe6128842db99fb70a2198da21bfd30714
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157944"
---
# <a name="update-userexperienceanalyticsapphealthosversionperformance"></a><span data-ttu-id="3a4b7-103">Atualizar userExperienceAnalyticsAppHealthOSVersionPerformance</span><span class="sxs-lookup"><span data-stu-id="3a4b7-103">Update userExperienceAnalyticsAppHealthOSVersionPerformance</span></span>

<span data-ttu-id="3a4b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a4b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a4b7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3a4b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a4b7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a4b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a4b7-107">Atualize as propriedades de [um objeto userExperienceAnalyticsAppHealthOSVersionPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)</span><span class="sxs-lookup"><span data-stu-id="3a4b7-107">Update the properties of a [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a4b7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3a4b7-108">Prerequisites</span></span>
<span data-ttu-id="3a4b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a4b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a4b7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a4b7-111">Permission type</span></span>|<span data-ttu-id="3a4b7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a4b7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a4b7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a4b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a4b7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a4b7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3a4b7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a4b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a4b7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a4b7-116">Not supported.</span></span>|
|<span data-ttu-id="3a4b7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a4b7-117">Application</span></span>|<span data-ttu-id="3a4b7-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a4b7-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a4b7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a4b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance/{userExperienceAnalyticsAppHealthOSVersionPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="3a4b7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a4b7-120">Request headers</span></span>
|<span data-ttu-id="3a4b7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a4b7-121">Header</span></span>|<span data-ttu-id="3a4b7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3a4b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a4b7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a4b7-123">Authorization</span></span>|<span data-ttu-id="3a4b7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a4b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a4b7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3a4b7-125">Accept</span></span>|<span data-ttu-id="3a4b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a4b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a4b7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a4b7-127">Request body</span></span>
<span data-ttu-id="3a4b7-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsAppHealthOSVersionPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)</span><span class="sxs-lookup"><span data-stu-id="3a4b7-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object.</span></span>

<span data-ttu-id="3a4b7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md).</span><span class="sxs-lookup"><span data-stu-id="3a4b7-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md).</span></span>

|<span data-ttu-id="3a4b7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a4b7-130">Property</span></span>|<span data-ttu-id="3a4b7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a4b7-131">Type</span></span>|<span data-ttu-id="3a4b7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a4b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a4b7-133">id</span><span class="sxs-lookup"><span data-stu-id="3a4b7-133">id</span></span>|<span data-ttu-id="3a4b7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a4b7-134">String</span></span>|<span data-ttu-id="3a4b7-135">O identificador exclusivo do objeto de desempenho de versão do sistema operacional de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="3a4b7-135">The unique identifier of the user experience analytics OS version performance object.</span></span>|
|<span data-ttu-id="3a4b7-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="3a4b7-136">osVersion</span></span>|<span data-ttu-id="3a4b7-137">String</span><span class="sxs-lookup"><span data-stu-id="3a4b7-137">String</span></span>|<span data-ttu-id="3a4b7-138">A versão do sistema operacional instalada no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3a4b7-138">The OS version installed on the device.</span></span>|
|<span data-ttu-id="3a4b7-139">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="3a4b7-139">osBuildNumber</span></span>|<span data-ttu-id="3a4b7-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a4b7-140">String</span></span>|<span data-ttu-id="3a4b7-141">O número de com build do sistema operacional instalado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3a4b7-141">The OS build number installed on the device.</span></span>|
|<span data-ttu-id="3a4b7-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3a4b7-142">activeDeviceCount</span></span>|<span data-ttu-id="3a4b7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3a4b7-143">Int32</span></span>|<span data-ttu-id="3a4b7-144">O número de dispositivos ativos para a versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="3a4b7-144">The number of active devices for the OS version.</span></span> <span data-ttu-id="3a4b7-145">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="3a4b7-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="3a4b7-146">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="3a4b7-146">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="3a4b7-147">Int32</span><span class="sxs-lookup"><span data-stu-id="3a4b7-147">Int32</span></span>|<span data-ttu-id="3a4b7-148">O tempo de falha média para a versão do sistema operacional em minutos.</span><span class="sxs-lookup"><span data-stu-id="3a4b7-148">The mean time to failure for the OS version in minutes.</span></span> <span data-ttu-id="3a4b7-149">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="3a4b7-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="3a4b7-150">osVersionAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="3a4b7-150">osVersionAppHealthScore</span></span>|<span data-ttu-id="3a4b7-151">Duplo</span><span class="sxs-lookup"><span data-stu-id="3a4b7-151">Double</span></span>|<span data-ttu-id="3a4b7-152">A pontuação de saúde do aplicativo da versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="3a4b7-152">The app health score of the OS version.</span></span> <span data-ttu-id="3a4b7-153">Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="3a4b7-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="3a4b7-154">osVersionAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="3a4b7-154">osVersionAppHealthStatus</span></span>|<span data-ttu-id="3a4b7-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a4b7-155">String</span></span>|<span data-ttu-id="3a4b7-156">O status geral da saúde do aplicativo da versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="3a4b7-156">The overall app health status of the OS version.</span></span>|



## <a name="response"></a><span data-ttu-id="3a4b7-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a4b7-157">Response</span></span>
<span data-ttu-id="3a4b7-158">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a4b7-158">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a4b7-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a4b7-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a4b7-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a4b7-160">Request</span></span>
<span data-ttu-id="3a4b7-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a4b7-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance/{userExperienceAnalyticsAppHealthOSVersionPerformanceId}
Content-type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "osVersionAppHealthScore": 7.666666666666667,
  "osVersionAppHealthStatus": "Os Version App Health Status value"
}
```

### <a name="response"></a><span data-ttu-id="3a4b7-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a4b7-162">Response</span></span>
<span data-ttu-id="3a4b7-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a4b7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 406

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
  "id": "7c28e16b-e16b-7c28-6be1-287c6be1287c",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "osVersionAppHealthScore": 7.666666666666667,
  "osVersionAppHealthStatus": "Os Version App Health Status value"
}
```




