---
title: Criar userExperienceAnalyticsAppHealthAppPerformanceByOSVersion
description: Criar um novo objeto userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b1c3ac5f96c506e01492c11aaf6c0fef2ea75686
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49203141"
---
# <a name="create-userexperienceanalyticsapphealthappperformancebyosversion"></a><span data-ttu-id="681bd-103">Criar userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span><span class="sxs-lookup"><span data-stu-id="681bd-103">Create userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span></span>

<span data-ttu-id="681bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="681bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="681bd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="681bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="681bd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="681bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="681bd-107">Criar um novo objeto [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) .</span><span class="sxs-lookup"><span data-stu-id="681bd-107">Create a new [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="681bd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="681bd-108">Prerequisites</span></span>
<span data-ttu-id="681bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="681bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="681bd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="681bd-111">Permission type</span></span>|<span data-ttu-id="681bd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="681bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="681bd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="681bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="681bd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="681bd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="681bd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="681bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="681bd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="681bd-116">Not supported.</span></span>|
|<span data-ttu-id="681bd-117">Application</span><span class="sxs-lookup"><span data-stu-id="681bd-117">Application</span></span>|<span data-ttu-id="681bd-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="681bd-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="681bd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="681bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion
```

## <a name="request-headers"></a><span data-ttu-id="681bd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="681bd-120">Request headers</span></span>
|<span data-ttu-id="681bd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="681bd-121">Header</span></span>|<span data-ttu-id="681bd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="681bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="681bd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="681bd-123">Authorization</span></span>|<span data-ttu-id="681bd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="681bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="681bd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="681bd-125">Accept</span></span>|<span data-ttu-id="681bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="681bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="681bd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="681bd-127">Request body</span></span>
<span data-ttu-id="681bd-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.</span><span class="sxs-lookup"><span data-stu-id="681bd-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthAppPerformanceByOSVersion object.</span></span>

<span data-ttu-id="681bd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.</span><span class="sxs-lookup"><span data-stu-id="681bd-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.</span></span>

|<span data-ttu-id="681bd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="681bd-130">Property</span></span>|<span data-ttu-id="681bd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="681bd-131">Type</span></span>|<span data-ttu-id="681bd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="681bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="681bd-133">id</span><span class="sxs-lookup"><span data-stu-id="681bd-133">id</span></span>|<span data-ttu-id="681bd-134">String</span><span class="sxs-lookup"><span data-stu-id="681bd-134">String</span></span>|<span data-ttu-id="681bd-135">O identificador exclusivo do objeto de desempenho da versão do aplicativo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="681bd-135">The unique identifier of the user experience analytics app version performance object.</span></span>|
|<span data-ttu-id="681bd-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="681bd-136">osVersion</span></span>|<span data-ttu-id="681bd-137">String</span><span class="sxs-lookup"><span data-stu-id="681bd-137">String</span></span>|<span data-ttu-id="681bd-138">A versão do sistema operacional do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="681bd-138">The os version of the application.</span></span>|
|<span data-ttu-id="681bd-139">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="681bd-139">osBuildNumber</span></span>|<span data-ttu-id="681bd-140">String</span><span class="sxs-lookup"><span data-stu-id="681bd-140">String</span></span>|<span data-ttu-id="681bd-141">O número de compilação do sistema operacional do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="681bd-141">The os build number of the application.</span></span>|
|<span data-ttu-id="681bd-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="681bd-142">activeDeviceCount</span></span>|<span data-ttu-id="681bd-143">Int32</span><span class="sxs-lookup"><span data-stu-id="681bd-143">Int32</span></span>|<span data-ttu-id="681bd-144">O número de dispositivos em que o aplicativo está ativo.</span><span class="sxs-lookup"><span data-stu-id="681bd-144">The number of devices where the app has been active.</span></span> <span data-ttu-id="681bd-145">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="681bd-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="681bd-146">appName</span><span class="sxs-lookup"><span data-stu-id="681bd-146">appName</span></span>|<span data-ttu-id="681bd-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="681bd-147">String</span></span>|<span data-ttu-id="681bd-148">O nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="681bd-148">The name of the application.</span></span>|
|<span data-ttu-id="681bd-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="681bd-149">appDisplayName</span></span>|<span data-ttu-id="681bd-150">String</span><span class="sxs-lookup"><span data-stu-id="681bd-150">String</span></span>|<span data-ttu-id="681bd-151">O nome amigável do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="681bd-151">The friendly name of the application.</span></span>|
|<span data-ttu-id="681bd-152">appPublisher</span><span class="sxs-lookup"><span data-stu-id="681bd-152">appPublisher</span></span>|<span data-ttu-id="681bd-153">String</span><span class="sxs-lookup"><span data-stu-id="681bd-153">String</span></span>|<span data-ttu-id="681bd-154">O fornecedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="681bd-154">The publisher of the application.</span></span>|
|<span data-ttu-id="681bd-155">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="681bd-155">appUsageDuration</span></span>|<span data-ttu-id="681bd-156">Int32</span><span class="sxs-lookup"><span data-stu-id="681bd-156">Int32</span></span>|<span data-ttu-id="681bd-157">O tempo total de uso do aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="681bd-157">The total usage time of the application in minutes.</span></span> <span data-ttu-id="681bd-158">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="681bd-158">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="681bd-159">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="681bd-159">appCrashCount</span></span>|<span data-ttu-id="681bd-160">Int32</span><span class="sxs-lookup"><span data-stu-id="681bd-160">Int32</span></span>|<span data-ttu-id="681bd-161">O número de falhas para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="681bd-161">The number of crashes for the app.</span></span> <span data-ttu-id="681bd-162">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="681bd-162">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="681bd-163">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="681bd-163">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="681bd-164">Int32</span><span class="sxs-lookup"><span data-stu-id="681bd-164">Int32</span></span>|<span data-ttu-id="681bd-165">O tempo médio de falha para o aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="681bd-165">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="681bd-166">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="681bd-166">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="681bd-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="681bd-167">Response</span></span>
<span data-ttu-id="681bd-168">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="681bd-168">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="681bd-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="681bd-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="681bd-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="681bd-170">Request</span></span>
<span data-ttu-id="681bd-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="681bd-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="681bd-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="681bd-172">Response</span></span>
<span data-ttu-id="681bd-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="681bd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




