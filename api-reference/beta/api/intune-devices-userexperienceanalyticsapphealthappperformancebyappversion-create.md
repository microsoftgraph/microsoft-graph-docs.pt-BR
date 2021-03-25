---
title: Criar userExperienceAnalyticsAppHealthAppPerformanceByAppVersion
description: Crie um novo objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 34dbfeed9093fb0a2508df391deff101941e315b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158091"
---
# <a name="create-userexperienceanalyticsapphealthappperformancebyappversion"></a><span data-ttu-id="a6b8f-103">Criar userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span><span class="sxs-lookup"><span data-stu-id="a6b8f-103">Create userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span></span>

<span data-ttu-id="a6b8f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6b8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6b8f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6b8f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6b8f-107">Crie um novo [objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)</span><span class="sxs-lookup"><span data-stu-id="a6b8f-107">Create a new [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6b8f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6b8f-108">Prerequisites</span></span>
<span data-ttu-id="a6b8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6b8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6b8f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6b8f-111">Permission type</span></span>|<span data-ttu-id="a6b8f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6b8f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6b8f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6b8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6b8f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6b8f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a6b8f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6b8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6b8f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-116">Not supported.</span></span>|
|<span data-ttu-id="a6b8f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6b8f-117">Application</span></span>|<span data-ttu-id="a6b8f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6b8f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6b8f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6b8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion
```

## <a name="request-headers"></a><span data-ttu-id="a6b8f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6b8f-120">Request headers</span></span>
|<span data-ttu-id="a6b8f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6b8f-121">Header</span></span>|<span data-ttu-id="a6b8f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a6b8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6b8f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6b8f-123">Authorization</span></span>|<span data-ttu-id="a6b8f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6b8f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6b8f-125">Accept</span></span>|<span data-ttu-id="a6b8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6b8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6b8f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6b8f-127">Request body</span></span>
<span data-ttu-id="a6b8f-128">No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthAppPerformanceByAppVersion object.</span></span>

<span data-ttu-id="a6b8f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.</span></span>

|<span data-ttu-id="a6b8f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6b8f-130">Property</span></span>|<span data-ttu-id="a6b8f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6b8f-131">Type</span></span>|<span data-ttu-id="a6b8f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6b8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6b8f-133">id</span><span class="sxs-lookup"><span data-stu-id="a6b8f-133">id</span></span>|<span data-ttu-id="a6b8f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6b8f-134">String</span></span>|<span data-ttu-id="a6b8f-135">O identificador exclusivo do objeto de desempenho do aplicativo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="a6b8f-136">appVersion</span><span class="sxs-lookup"><span data-stu-id="a6b8f-136">appVersion</span></span>|<span data-ttu-id="a6b8f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6b8f-137">String</span></span>|<span data-ttu-id="a6b8f-138">A versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-138">The version of the application.</span></span>|
|<span data-ttu-id="a6b8f-139">appName</span><span class="sxs-lookup"><span data-stu-id="a6b8f-139">appName</span></span>|<span data-ttu-id="a6b8f-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6b8f-140">String</span></span>|<span data-ttu-id="a6b8f-141">O nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-141">The name of the application.</span></span>|
|<span data-ttu-id="a6b8f-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="a6b8f-142">appDisplayName</span></span>|<span data-ttu-id="a6b8f-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6b8f-143">String</span></span>|<span data-ttu-id="a6b8f-144">O nome amigável do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-144">The friendly name of the application.</span></span>|
|<span data-ttu-id="a6b8f-145">appPublisher</span><span class="sxs-lookup"><span data-stu-id="a6b8f-145">appPublisher</span></span>|<span data-ttu-id="a6b8f-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6b8f-146">String</span></span>|<span data-ttu-id="a6b8f-147">O editor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-147">The publisher of the application.</span></span>|
|<span data-ttu-id="a6b8f-148">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="a6b8f-148">appUsageDuration</span></span>|<span data-ttu-id="a6b8f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a6b8f-149">Int32</span></span>|<span data-ttu-id="a6b8f-150">O tempo total de uso do aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-150">The total usage time of the application in minutes.</span></span> <span data-ttu-id="a6b8f-151">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="a6b8f-151">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="a6b8f-152">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="a6b8f-152">appCrashCount</span></span>|<span data-ttu-id="a6b8f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a6b8f-153">Int32</span></span>|<span data-ttu-id="a6b8f-154">O número de falhas para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-154">The number of crashes for the app.</span></span> <span data-ttu-id="a6b8f-155">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="a6b8f-155">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="a6b8f-156">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="a6b8f-156">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="a6b8f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="a6b8f-157">Int32</span></span>|<span data-ttu-id="a6b8f-158">O tempo de falha média do aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-158">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="a6b8f-159">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="a6b8f-159">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="a6b8f-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6b8f-160">Response</span></span>
<span data-ttu-id="a6b8f-161">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-161">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6b8f-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6b8f-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6b8f-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6b8f-163">Request</span></span>
<span data-ttu-id="a6b8f-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion
Content-type: application/json
Content-length: 346

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersion",
  "appVersion": "App Version value",
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```

### <a name="response"></a><span data-ttu-id="a6b8f-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6b8f-165">Response</span></span>
<span data-ttu-id="a6b8f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6b8f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 395

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersion",
  "id": "257804c8-04c8-2578-c804-7825c8047825",
  "appVersion": "App Version value",
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```




