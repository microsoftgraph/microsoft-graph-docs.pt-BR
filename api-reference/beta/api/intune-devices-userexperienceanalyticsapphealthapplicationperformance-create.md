---
title: Criar userExperienceAnalyticsAppHealthApplicationPerformance
description: Criar um novo objeto userExperienceAnalyticsAppHealthApplicationPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3cf8c7485bca42f5d2a776033c70232a87e9411f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703171"
---
# <a name="create-userexperienceanalyticsapphealthapplicationperformance"></a><span data-ttu-id="f26cc-103">Criar userExperienceAnalyticsAppHealthApplicationPerformance</span><span class="sxs-lookup"><span data-stu-id="f26cc-103">Create userExperienceAnalyticsAppHealthApplicationPerformance</span></span>

<span data-ttu-id="f26cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f26cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f26cc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f26cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f26cc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f26cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f26cc-107">Criar um novo objeto [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="f26cc-107">Create a new [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f26cc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f26cc-108">Prerequisites</span></span>
<span data-ttu-id="f26cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f26cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f26cc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f26cc-111">Permission type</span></span>|<span data-ttu-id="f26cc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f26cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f26cc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f26cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f26cc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f26cc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f26cc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f26cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f26cc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f26cc-116">Not supported.</span></span>|
|<span data-ttu-id="f26cc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f26cc-117">Application</span></span>|<span data-ttu-id="f26cc-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f26cc-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f26cc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f26cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
```

## <a name="request-headers"></a><span data-ttu-id="f26cc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f26cc-120">Request headers</span></span>
|<span data-ttu-id="f26cc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f26cc-121">Header</span></span>|<span data-ttu-id="f26cc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f26cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f26cc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f26cc-123">Authorization</span></span>|<span data-ttu-id="f26cc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f26cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f26cc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f26cc-125">Accept</span></span>|<span data-ttu-id="f26cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f26cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f26cc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f26cc-127">Request body</span></span>
<span data-ttu-id="f26cc-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsAppHealthApplicationPerformance.</span><span class="sxs-lookup"><span data-stu-id="f26cc-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthApplicationPerformance object.</span></span>

<span data-ttu-id="f26cc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsAppHealthApplicationPerformance.</span><span class="sxs-lookup"><span data-stu-id="f26cc-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthApplicationPerformance.</span></span>

|<span data-ttu-id="f26cc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f26cc-130">Property</span></span>|<span data-ttu-id="f26cc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f26cc-131">Type</span></span>|<span data-ttu-id="f26cc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f26cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f26cc-133">id</span><span class="sxs-lookup"><span data-stu-id="f26cc-133">id</span></span>|<span data-ttu-id="f26cc-134">String</span><span class="sxs-lookup"><span data-stu-id="f26cc-134">String</span></span>|<span data-ttu-id="f26cc-135">O identificador exclusivo do objeto de desempenho do aplicativo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="f26cc-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="f26cc-136">appHangCount</span><span class="sxs-lookup"><span data-stu-id="f26cc-136">appHangCount</span></span>|<span data-ttu-id="f26cc-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f26cc-137">Int32</span></span>|<span data-ttu-id="f26cc-138">O número de suspensões para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f26cc-138">The number of hangs for the app.</span></span> <span data-ttu-id="f26cc-139">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="f26cc-139">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="f26cc-140">appHealthScore</span><span class="sxs-lookup"><span data-stu-id="f26cc-140">appHealthScore</span></span>|<span data-ttu-id="f26cc-141">Duplo</span><span class="sxs-lookup"><span data-stu-id="f26cc-141">Double</span></span>|<span data-ttu-id="f26cc-142">A pontuação de integridade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f26cc-142">The health score of the app.</span></span> <span data-ttu-id="f26cc-143">Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="f26cc-143">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="f26cc-144">appHealthStatus</span><span class="sxs-lookup"><span data-stu-id="f26cc-144">appHealthStatus</span></span>|<span data-ttu-id="f26cc-145">String</span><span class="sxs-lookup"><span data-stu-id="f26cc-145">String</span></span>|<span data-ttu-id="f26cc-146">O status de integridade geral do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f26cc-146">The overall health status of the app.</span></span>|
|<span data-ttu-id="f26cc-147">allOrgsHealthScore</span><span class="sxs-lookup"><span data-stu-id="f26cc-147">allOrgsHealthScore</span></span>|<span data-ttu-id="f26cc-148">Duplo</span><span class="sxs-lookup"><span data-stu-id="f26cc-148">Double</span></span>|<span data-ttu-id="f26cc-149">A pontuação de integridade mediana do aplicativo em todas as organizações.</span><span class="sxs-lookup"><span data-stu-id="f26cc-149">The median health score of the application across all organizations.</span></span> <span data-ttu-id="f26cc-150">Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="f26cc-150">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="f26cc-151">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f26cc-151">activeDeviceCount</span></span>|<span data-ttu-id="f26cc-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f26cc-152">Int32</span></span>|<span data-ttu-id="f26cc-153">O número de dispositivos em que o aplicativo está ativo.</span><span class="sxs-lookup"><span data-stu-id="f26cc-153">The number of devices where the app has been active.</span></span> <span data-ttu-id="f26cc-154">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="f26cc-154">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="f26cc-155">appName</span><span class="sxs-lookup"><span data-stu-id="f26cc-155">appName</span></span>|<span data-ttu-id="f26cc-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f26cc-156">String</span></span>|<span data-ttu-id="f26cc-157">O nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f26cc-157">The name of the application.</span></span>|
|<span data-ttu-id="f26cc-158">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="f26cc-158">appDisplayName</span></span>|<span data-ttu-id="f26cc-159">String</span><span class="sxs-lookup"><span data-stu-id="f26cc-159">String</span></span>|<span data-ttu-id="f26cc-160">O nome amigável do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f26cc-160">The friendly name of the application.</span></span>|
|<span data-ttu-id="f26cc-161">appPublisher</span><span class="sxs-lookup"><span data-stu-id="f26cc-161">appPublisher</span></span>|<span data-ttu-id="f26cc-162">String</span><span class="sxs-lookup"><span data-stu-id="f26cc-162">String</span></span>|<span data-ttu-id="f26cc-163">O fornecedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f26cc-163">The publisher of the application.</span></span>|
|<span data-ttu-id="f26cc-164">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="f26cc-164">appUsageDuration</span></span>|<span data-ttu-id="f26cc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f26cc-165">Int32</span></span>|<span data-ttu-id="f26cc-166">O tempo total de uso do aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="f26cc-166">The total usage time of the application in minutes.</span></span> <span data-ttu-id="f26cc-167">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="f26cc-167">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="f26cc-168">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="f26cc-168">appCrashCount</span></span>|<span data-ttu-id="f26cc-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f26cc-169">Int32</span></span>|<span data-ttu-id="f26cc-170">O número de falhas para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f26cc-170">The number of crashes for the app.</span></span> <span data-ttu-id="f26cc-171">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="f26cc-171">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="f26cc-172">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="f26cc-172">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="f26cc-173">Int32</span><span class="sxs-lookup"><span data-stu-id="f26cc-173">Int32</span></span>|<span data-ttu-id="f26cc-174">O tempo médio de falha para o aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="f26cc-174">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="f26cc-175">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="f26cc-175">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="f26cc-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="f26cc-176">Response</span></span>
<span data-ttu-id="f26cc-177">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f26cc-177">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f26cc-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f26cc-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="f26cc-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f26cc-179">Request</span></span>
<span data-ttu-id="f26cc-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f26cc-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f26cc-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="f26cc-181">Response</span></span>
<span data-ttu-id="f26cc-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f26cc-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





