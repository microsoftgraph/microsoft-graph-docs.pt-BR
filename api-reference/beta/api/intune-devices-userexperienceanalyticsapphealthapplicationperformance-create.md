---
title: Criar userExperienceAnalyticsAppHealthApplicationPerformance
description: Criar um novo objeto userExperienceAnalyticsAppHealthApplicationPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2e2d04f328e25cd44cecbeba4662cc10e6e858c8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49203351"
---
# <a name="create-userexperienceanalyticsapphealthapplicationperformance"></a><span data-ttu-id="fb499-103">Criar userExperienceAnalyticsAppHealthApplicationPerformance</span><span class="sxs-lookup"><span data-stu-id="fb499-103">Create userExperienceAnalyticsAppHealthApplicationPerformance</span></span>

<span data-ttu-id="fb499-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb499-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb499-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fb499-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb499-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb499-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb499-107">Criar um novo objeto [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="fb499-107">Create a new [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb499-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb499-108">Prerequisites</span></span>
<span data-ttu-id="fb499-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb499-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb499-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb499-111">Permission type</span></span>|<span data-ttu-id="fb499-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fb499-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb499-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb499-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb499-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb499-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fb499-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb499-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb499-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb499-116">Not supported.</span></span>|
|<span data-ttu-id="fb499-117">Application</span><span class="sxs-lookup"><span data-stu-id="fb499-117">Application</span></span>|<span data-ttu-id="fb499-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb499-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb499-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb499-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
```

## <a name="request-headers"></a><span data-ttu-id="fb499-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb499-120">Request headers</span></span>
|<span data-ttu-id="fb499-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb499-121">Header</span></span>|<span data-ttu-id="fb499-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fb499-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb499-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb499-123">Authorization</span></span>|<span data-ttu-id="fb499-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb499-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb499-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fb499-125">Accept</span></span>|<span data-ttu-id="fb499-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb499-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb499-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb499-127">Request body</span></span>
<span data-ttu-id="fb499-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsAppHealthApplicationPerformance.</span><span class="sxs-lookup"><span data-stu-id="fb499-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthApplicationPerformance object.</span></span>

<span data-ttu-id="fb499-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsAppHealthApplicationPerformance.</span><span class="sxs-lookup"><span data-stu-id="fb499-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthApplicationPerformance.</span></span>

|<span data-ttu-id="fb499-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb499-130">Property</span></span>|<span data-ttu-id="fb499-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb499-131">Type</span></span>|<span data-ttu-id="fb499-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb499-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb499-133">id</span><span class="sxs-lookup"><span data-stu-id="fb499-133">id</span></span>|<span data-ttu-id="fb499-134">String</span><span class="sxs-lookup"><span data-stu-id="fb499-134">String</span></span>|<span data-ttu-id="fb499-135">O identificador exclusivo do objeto de desempenho do aplicativo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="fb499-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="fb499-136">appHangCount</span><span class="sxs-lookup"><span data-stu-id="fb499-136">appHangCount</span></span>|<span data-ttu-id="fb499-137">Int32</span><span class="sxs-lookup"><span data-stu-id="fb499-137">Int32</span></span>|<span data-ttu-id="fb499-138">O número de suspensões para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb499-138">The number of hangs for the app.</span></span> <span data-ttu-id="fb499-139">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="fb499-139">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="fb499-140">appHealthScore</span><span class="sxs-lookup"><span data-stu-id="fb499-140">appHealthScore</span></span>|<span data-ttu-id="fb499-141">Duplo</span><span class="sxs-lookup"><span data-stu-id="fb499-141">Double</span></span>|<span data-ttu-id="fb499-142">A pontuação de integridade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb499-142">The health score of the app.</span></span> <span data-ttu-id="fb499-143">Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="fb499-143">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="fb499-144">appHealthStatus</span><span class="sxs-lookup"><span data-stu-id="fb499-144">appHealthStatus</span></span>|<span data-ttu-id="fb499-145">String</span><span class="sxs-lookup"><span data-stu-id="fb499-145">String</span></span>|<span data-ttu-id="fb499-146">O status de integridade geral do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb499-146">The overall health status of the app.</span></span>|
|<span data-ttu-id="fb499-147">allOrgsHealthScore</span><span class="sxs-lookup"><span data-stu-id="fb499-147">allOrgsHealthScore</span></span>|<span data-ttu-id="fb499-148">Duplo</span><span class="sxs-lookup"><span data-stu-id="fb499-148">Double</span></span>|<span data-ttu-id="fb499-149">A pontuação de integridade mediana do aplicativo em todas as organizações.</span><span class="sxs-lookup"><span data-stu-id="fb499-149">The median health score of the application across all organizations.</span></span> <span data-ttu-id="fb499-150">Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="fb499-150">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="fb499-151">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fb499-151">activeDeviceCount</span></span>|<span data-ttu-id="fb499-152">Int32</span><span class="sxs-lookup"><span data-stu-id="fb499-152">Int32</span></span>|<span data-ttu-id="fb499-153">O número de dispositivos em que o aplicativo está ativo.</span><span class="sxs-lookup"><span data-stu-id="fb499-153">The number of devices where the app has been active.</span></span> <span data-ttu-id="fb499-154">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="fb499-154">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="fb499-155">appName</span><span class="sxs-lookup"><span data-stu-id="fb499-155">appName</span></span>|<span data-ttu-id="fb499-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb499-156">String</span></span>|<span data-ttu-id="fb499-157">O nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb499-157">The name of the application.</span></span>|
|<span data-ttu-id="fb499-158">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="fb499-158">appDisplayName</span></span>|<span data-ttu-id="fb499-159">String</span><span class="sxs-lookup"><span data-stu-id="fb499-159">String</span></span>|<span data-ttu-id="fb499-160">O nome amigável do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb499-160">The friendly name of the application.</span></span>|
|<span data-ttu-id="fb499-161">appPublisher</span><span class="sxs-lookup"><span data-stu-id="fb499-161">appPublisher</span></span>|<span data-ttu-id="fb499-162">String</span><span class="sxs-lookup"><span data-stu-id="fb499-162">String</span></span>|<span data-ttu-id="fb499-163">O fornecedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb499-163">The publisher of the application.</span></span>|
|<span data-ttu-id="fb499-164">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="fb499-164">appUsageDuration</span></span>|<span data-ttu-id="fb499-165">Int32</span><span class="sxs-lookup"><span data-stu-id="fb499-165">Int32</span></span>|<span data-ttu-id="fb499-166">O tempo total de uso do aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="fb499-166">The total usage time of the application in minutes.</span></span> <span data-ttu-id="fb499-167">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="fb499-167">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="fb499-168">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="fb499-168">appCrashCount</span></span>|<span data-ttu-id="fb499-169">Int32</span><span class="sxs-lookup"><span data-stu-id="fb499-169">Int32</span></span>|<span data-ttu-id="fb499-170">O número de falhas para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb499-170">The number of crashes for the app.</span></span> <span data-ttu-id="fb499-171">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="fb499-171">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="fb499-172">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="fb499-172">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="fb499-173">Int32</span><span class="sxs-lookup"><span data-stu-id="fb499-173">Int32</span></span>|<span data-ttu-id="fb499-174">O tempo médio de falha para o aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="fb499-174">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="fb499-175">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="fb499-175">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="fb499-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb499-176">Response</span></span>
<span data-ttu-id="fb499-177">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb499-177">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb499-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb499-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb499-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb499-179">Request</span></span>
<span data-ttu-id="fb499-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb499-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
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

### <a name="response"></a><span data-ttu-id="fb499-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb499-181">Response</span></span>
<span data-ttu-id="fb499-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb499-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




