---
title: Atualizar userExperienceAnalyticsAppHealthApplicationPerformance
description: Atualize as propriedades de um objeto userExperienceAnalyticsAppHealthApplicationPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 99ffe6141c124e8de8ecd1a6a7fdf362b9cf6ff9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158098"
---
# <a name="update-userexperienceanalyticsapphealthapplicationperformance"></a><span data-ttu-id="c7d00-103">Atualizar userExperienceAnalyticsAppHealthApplicationPerformance</span><span class="sxs-lookup"><span data-stu-id="c7d00-103">Update userExperienceAnalyticsAppHealthApplicationPerformance</span></span>

<span data-ttu-id="c7d00-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7d00-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7d00-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7d00-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7d00-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7d00-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7d00-107">Atualize as propriedades de [um objeto userExperienceAnalyticsAppHealthApplicationPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)</span><span class="sxs-lookup"><span data-stu-id="c7d00-107">Update the properties of a [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7d00-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7d00-108">Prerequisites</span></span>
<span data-ttu-id="c7d00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7d00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7d00-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7d00-111">Permission type</span></span>|<span data-ttu-id="c7d00-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7d00-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7d00-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7d00-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7d00-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7d00-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c7d00-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7d00-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7d00-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7d00-116">Not supported.</span></span>|
|<span data-ttu-id="c7d00-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7d00-117">Application</span></span>|<span data-ttu-id="c7d00-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7d00-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7d00-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7d00-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="c7d00-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d00-120">Request headers</span></span>
|<span data-ttu-id="c7d00-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7d00-121">Header</span></span>|<span data-ttu-id="c7d00-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c7d00-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7d00-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7d00-123">Authorization</span></span>|<span data-ttu-id="c7d00-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7d00-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7d00-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7d00-125">Accept</span></span>|<span data-ttu-id="c7d00-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7d00-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7d00-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d00-127">Request body</span></span>
<span data-ttu-id="c7d00-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsAppHealthApplicationPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)</span><span class="sxs-lookup"><span data-stu-id="c7d00-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

<span data-ttu-id="c7d00-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).</span><span class="sxs-lookup"><span data-stu-id="c7d00-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).</span></span>

|<span data-ttu-id="c7d00-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7d00-130">Property</span></span>|<span data-ttu-id="c7d00-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7d00-131">Type</span></span>|<span data-ttu-id="c7d00-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7d00-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7d00-133">id</span><span class="sxs-lookup"><span data-stu-id="c7d00-133">id</span></span>|<span data-ttu-id="c7d00-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7d00-134">String</span></span>|<span data-ttu-id="c7d00-135">O identificador exclusivo do objeto de desempenho do aplicativo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="c7d00-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="c7d00-136">appHangCount</span><span class="sxs-lookup"><span data-stu-id="c7d00-136">appHangCount</span></span>|<span data-ttu-id="c7d00-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d00-137">Int32</span></span>|<span data-ttu-id="c7d00-138">O número de travas para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c7d00-138">The number of hangs for the app.</span></span> <span data-ttu-id="c7d00-139">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="c7d00-139">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="c7d00-140">appHealthScore</span><span class="sxs-lookup"><span data-stu-id="c7d00-140">appHealthScore</span></span>|<span data-ttu-id="c7d00-141">Duplo</span><span class="sxs-lookup"><span data-stu-id="c7d00-141">Double</span></span>|<span data-ttu-id="c7d00-142">A pontuação de saúde do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c7d00-142">The health score of the app.</span></span> <span data-ttu-id="c7d00-143">Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="c7d00-143">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="c7d00-144">appHealthStatus</span><span class="sxs-lookup"><span data-stu-id="c7d00-144">appHealthStatus</span></span>|<span data-ttu-id="c7d00-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7d00-145">String</span></span>|<span data-ttu-id="c7d00-146">O status de saúde geral do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c7d00-146">The overall health status of the app.</span></span>|
|<span data-ttu-id="c7d00-147">allOrgsHealthScore</span><span class="sxs-lookup"><span data-stu-id="c7d00-147">allOrgsHealthScore</span></span>|<span data-ttu-id="c7d00-148">Duplo</span><span class="sxs-lookup"><span data-stu-id="c7d00-148">Double</span></span>|<span data-ttu-id="c7d00-149">A pontuação de saúde mediana do aplicativo em todas as organizações.</span><span class="sxs-lookup"><span data-stu-id="c7d00-149">The median health score of the application across all organizations.</span></span> <span data-ttu-id="c7d00-150">Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="c7d00-150">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="c7d00-151">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7d00-151">activeDeviceCount</span></span>|<span data-ttu-id="c7d00-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d00-152">Int32</span></span>|<span data-ttu-id="c7d00-153">O número de dispositivos em que o aplicativo está ativo.</span><span class="sxs-lookup"><span data-stu-id="c7d00-153">The number of devices where the app has been active.</span></span> <span data-ttu-id="c7d00-154">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="c7d00-154">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="c7d00-155">appName</span><span class="sxs-lookup"><span data-stu-id="c7d00-155">appName</span></span>|<span data-ttu-id="c7d00-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7d00-156">String</span></span>|<span data-ttu-id="c7d00-157">O nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c7d00-157">The name of the application.</span></span>|
|<span data-ttu-id="c7d00-158">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="c7d00-158">appDisplayName</span></span>|<span data-ttu-id="c7d00-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7d00-159">String</span></span>|<span data-ttu-id="c7d00-160">O nome amigável do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c7d00-160">The friendly name of the application.</span></span>|
|<span data-ttu-id="c7d00-161">appPublisher</span><span class="sxs-lookup"><span data-stu-id="c7d00-161">appPublisher</span></span>|<span data-ttu-id="c7d00-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7d00-162">String</span></span>|<span data-ttu-id="c7d00-163">O editor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c7d00-163">The publisher of the application.</span></span>|
|<span data-ttu-id="c7d00-164">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="c7d00-164">appUsageDuration</span></span>|<span data-ttu-id="c7d00-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d00-165">Int32</span></span>|<span data-ttu-id="c7d00-166">O tempo total de uso do aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="c7d00-166">The total usage time of the application in minutes.</span></span> <span data-ttu-id="c7d00-167">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="c7d00-167">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="c7d00-168">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="c7d00-168">appCrashCount</span></span>|<span data-ttu-id="c7d00-169">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d00-169">Int32</span></span>|<span data-ttu-id="c7d00-170">O número de falhas para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c7d00-170">The number of crashes for the app.</span></span> <span data-ttu-id="c7d00-171">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="c7d00-171">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="c7d00-172">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="c7d00-172">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="c7d00-173">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d00-173">Int32</span></span>|<span data-ttu-id="c7d00-174">O tempo de falha média do aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="c7d00-174">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="c7d00-175">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="c7d00-175">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="c7d00-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7d00-176">Response</span></span>
<span data-ttu-id="c7d00-177">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7d00-177">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7d00-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7d00-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7d00-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d00-179">Request</span></span>
<span data-ttu-id="c7d00-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7d00-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
Content-type: application/json
Content-length: 473

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "appHangCount": 12,
  "appHealthScore": 4.666666666666667,
  "appHealthStatus": "App Health Status value",
  "allOrgsHealthScore": 6.0,
  "activeDeviceCount": 1,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```

### <a name="response"></a><span data-ttu-id="c7d00-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7d00-181">Response</span></span>
<span data-ttu-id="c7d00-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7d00-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 522

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "id": "c7962a87-2a87-c796-872a-96c7872a96c7",
  "appHangCount": 12,
  "appHealthScore": 4.666666666666667,
  "appHealthStatus": "App Health Status value",
  "allOrgsHealthScore": 6.0,
  "activeDeviceCount": 1,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```




