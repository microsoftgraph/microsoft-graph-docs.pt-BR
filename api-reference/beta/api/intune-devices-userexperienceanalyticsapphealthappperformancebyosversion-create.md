---
title: Criar userExperienceAnalyticsAppHealthAppPerformanceByOSVersion
description: Crie um novo objeto userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4e90ced56c6831005d9d878bcec6ab613e8060c8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158028"
---
# <a name="create-userexperienceanalyticsapphealthappperformancebyosversion"></a><span data-ttu-id="b69cb-103">Criar userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span><span class="sxs-lookup"><span data-stu-id="b69cb-103">Create userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span></span>

<span data-ttu-id="b69cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b69cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b69cb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b69cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b69cb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b69cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b69cb-107">Crie um novo [objeto userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)</span><span class="sxs-lookup"><span data-stu-id="b69cb-107">Create a new [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b69cb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b69cb-108">Prerequisites</span></span>
<span data-ttu-id="b69cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b69cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b69cb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b69cb-111">Permission type</span></span>|<span data-ttu-id="b69cb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b69cb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b69cb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b69cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b69cb-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b69cb-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b69cb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b69cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b69cb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b69cb-116">Not supported.</span></span>|
|<span data-ttu-id="b69cb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b69cb-117">Application</span></span>|<span data-ttu-id="b69cb-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b69cb-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b69cb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b69cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion
```

## <a name="request-headers"></a><span data-ttu-id="b69cb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b69cb-120">Request headers</span></span>
|<span data-ttu-id="b69cb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b69cb-121">Header</span></span>|<span data-ttu-id="b69cb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b69cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b69cb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b69cb-123">Authorization</span></span>|<span data-ttu-id="b69cb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b69cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b69cb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b69cb-125">Accept</span></span>|<span data-ttu-id="b69cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b69cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b69cb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b69cb-127">Request body</span></span>
<span data-ttu-id="b69cb-128">No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.</span><span class="sxs-lookup"><span data-stu-id="b69cb-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthAppPerformanceByOSVersion object.</span></span>

<span data-ttu-id="b69cb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.</span><span class="sxs-lookup"><span data-stu-id="b69cb-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.</span></span>

|<span data-ttu-id="b69cb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b69cb-130">Property</span></span>|<span data-ttu-id="b69cb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b69cb-131">Type</span></span>|<span data-ttu-id="b69cb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b69cb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b69cb-133">id</span><span class="sxs-lookup"><span data-stu-id="b69cb-133">id</span></span>|<span data-ttu-id="b69cb-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b69cb-134">String</span></span>|<span data-ttu-id="b69cb-135">O identificador exclusivo do objeto de desempenho de versão do aplicativo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="b69cb-135">The unique identifier of the user experience analytics app version performance object.</span></span>|
|<span data-ttu-id="b69cb-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="b69cb-136">osVersion</span></span>|<span data-ttu-id="b69cb-137">String</span><span class="sxs-lookup"><span data-stu-id="b69cb-137">String</span></span>|<span data-ttu-id="b69cb-138">A versão do sistema operacional do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b69cb-138">The os version of the application.</span></span>|
|<span data-ttu-id="b69cb-139">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="b69cb-139">osBuildNumber</span></span>|<span data-ttu-id="b69cb-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b69cb-140">String</span></span>|<span data-ttu-id="b69cb-141">O número de com build do sistema operacional do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b69cb-141">The os build number of the application.</span></span>|
|<span data-ttu-id="b69cb-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b69cb-142">activeDeviceCount</span></span>|<span data-ttu-id="b69cb-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b69cb-143">Int32</span></span>|<span data-ttu-id="b69cb-144">O número de dispositivos em que o aplicativo está ativo.</span><span class="sxs-lookup"><span data-stu-id="b69cb-144">The number of devices where the app has been active.</span></span> <span data-ttu-id="b69cb-145">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="b69cb-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="b69cb-146">appName</span><span class="sxs-lookup"><span data-stu-id="b69cb-146">appName</span></span>|<span data-ttu-id="b69cb-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b69cb-147">String</span></span>|<span data-ttu-id="b69cb-148">O nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b69cb-148">The name of the application.</span></span>|
|<span data-ttu-id="b69cb-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="b69cb-149">appDisplayName</span></span>|<span data-ttu-id="b69cb-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b69cb-150">String</span></span>|<span data-ttu-id="b69cb-151">O nome amigável do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b69cb-151">The friendly name of the application.</span></span>|
|<span data-ttu-id="b69cb-152">appPublisher</span><span class="sxs-lookup"><span data-stu-id="b69cb-152">appPublisher</span></span>|<span data-ttu-id="b69cb-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b69cb-153">String</span></span>|<span data-ttu-id="b69cb-154">O editor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b69cb-154">The publisher of the application.</span></span>|
|<span data-ttu-id="b69cb-155">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="b69cb-155">appUsageDuration</span></span>|<span data-ttu-id="b69cb-156">Int32</span><span class="sxs-lookup"><span data-stu-id="b69cb-156">Int32</span></span>|<span data-ttu-id="b69cb-157">O tempo total de uso do aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="b69cb-157">The total usage time of the application in minutes.</span></span> <span data-ttu-id="b69cb-158">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="b69cb-158">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="b69cb-159">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="b69cb-159">appCrashCount</span></span>|<span data-ttu-id="b69cb-160">Int32</span><span class="sxs-lookup"><span data-stu-id="b69cb-160">Int32</span></span>|<span data-ttu-id="b69cb-161">O número de falhas para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b69cb-161">The number of crashes for the app.</span></span> <span data-ttu-id="b69cb-162">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="b69cb-162">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="b69cb-163">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="b69cb-163">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="b69cb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b69cb-164">Int32</span></span>|<span data-ttu-id="b69cb-165">O tempo de falha média do aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="b69cb-165">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="b69cb-166">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="b69cb-166">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="b69cb-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="b69cb-167">Response</span></span>
<span data-ttu-id="b69cb-168">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b69cb-168">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b69cb-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b69cb-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="b69cb-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b69cb-170">Request</span></span>
<span data-ttu-id="b69cb-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b69cb-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion
Content-type: application/json
Content-length: 415

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByOSVersion",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```

### <a name="response"></a><span data-ttu-id="b69cb-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="b69cb-172">Response</span></span>
<span data-ttu-id="b69cb-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b69cb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 464

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByOSVersion",
  "id": "65f9bde9-bde9-65f9-e9bd-f965e9bdf965",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```




