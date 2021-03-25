---
title: Atualizar userExperienceAnalyticsAppHealthAppPerformanceByAppVersion
description: Atualize as propriedades de um objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 41649f902158b198d7edcd0687e49d9c6d65dacb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158035"
---
# <a name="update-userexperienceanalyticsapphealthappperformancebyappversion"></a><span data-ttu-id="11d29-103">Atualizar userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span><span class="sxs-lookup"><span data-stu-id="11d29-103">Update userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span></span>

<span data-ttu-id="11d29-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11d29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11d29-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="11d29-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11d29-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11d29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11d29-107">Atualize as propriedades de [um objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)</span><span class="sxs-lookup"><span data-stu-id="11d29-107">Update the properties of a [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11d29-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="11d29-108">Prerequisites</span></span>
<span data-ttu-id="11d29-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11d29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11d29-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11d29-111">Permission type</span></span>|<span data-ttu-id="11d29-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11d29-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11d29-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11d29-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11d29-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11d29-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="11d29-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11d29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11d29-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11d29-116">Not supported.</span></span>|
|<span data-ttu-id="11d29-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11d29-117">Application</span></span>|<span data-ttu-id="11d29-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11d29-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="11d29-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11d29-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion/{userExperienceAnalyticsAppHealthAppPerformanceByAppVersionId}
```

## <a name="request-headers"></a><span data-ttu-id="11d29-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11d29-120">Request headers</span></span>
|<span data-ttu-id="11d29-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11d29-121">Header</span></span>|<span data-ttu-id="11d29-122">Valor</span><span class="sxs-lookup"><span data-stu-id="11d29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11d29-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="11d29-123">Authorization</span></span>|<span data-ttu-id="11d29-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11d29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11d29-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="11d29-125">Accept</span></span>|<span data-ttu-id="11d29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11d29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11d29-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11d29-127">Request body</span></span>
<span data-ttu-id="11d29-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)</span><span class="sxs-lookup"><span data-stu-id="11d29-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

<span data-ttu-id="11d29-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o usuárioExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md).</span><span class="sxs-lookup"><span data-stu-id="11d29-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md).</span></span>

|<span data-ttu-id="11d29-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11d29-130">Property</span></span>|<span data-ttu-id="11d29-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="11d29-131">Type</span></span>|<span data-ttu-id="11d29-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="11d29-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11d29-133">id</span><span class="sxs-lookup"><span data-stu-id="11d29-133">id</span></span>|<span data-ttu-id="11d29-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11d29-134">String</span></span>|<span data-ttu-id="11d29-135">O identificador exclusivo do objeto de desempenho do aplicativo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="11d29-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="11d29-136">appVersion</span><span class="sxs-lookup"><span data-stu-id="11d29-136">appVersion</span></span>|<span data-ttu-id="11d29-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11d29-137">String</span></span>|<span data-ttu-id="11d29-138">A versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11d29-138">The version of the application.</span></span>|
|<span data-ttu-id="11d29-139">appName</span><span class="sxs-lookup"><span data-stu-id="11d29-139">appName</span></span>|<span data-ttu-id="11d29-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11d29-140">String</span></span>|<span data-ttu-id="11d29-141">O nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11d29-141">The name of the application.</span></span>|
|<span data-ttu-id="11d29-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="11d29-142">appDisplayName</span></span>|<span data-ttu-id="11d29-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11d29-143">String</span></span>|<span data-ttu-id="11d29-144">O nome amigável do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11d29-144">The friendly name of the application.</span></span>|
|<span data-ttu-id="11d29-145">appPublisher</span><span class="sxs-lookup"><span data-stu-id="11d29-145">appPublisher</span></span>|<span data-ttu-id="11d29-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11d29-146">String</span></span>|<span data-ttu-id="11d29-147">O editor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11d29-147">The publisher of the application.</span></span>|
|<span data-ttu-id="11d29-148">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="11d29-148">appUsageDuration</span></span>|<span data-ttu-id="11d29-149">Int32</span><span class="sxs-lookup"><span data-stu-id="11d29-149">Int32</span></span>|<span data-ttu-id="11d29-150">O tempo total de uso do aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="11d29-150">The total usage time of the application in minutes.</span></span> <span data-ttu-id="11d29-151">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="11d29-151">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="11d29-152">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="11d29-152">appCrashCount</span></span>|<span data-ttu-id="11d29-153">Int32</span><span class="sxs-lookup"><span data-stu-id="11d29-153">Int32</span></span>|<span data-ttu-id="11d29-154">O número de falhas para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11d29-154">The number of crashes for the app.</span></span> <span data-ttu-id="11d29-155">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="11d29-155">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="11d29-156">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="11d29-156">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="11d29-157">Int32</span><span class="sxs-lookup"><span data-stu-id="11d29-157">Int32</span></span>|<span data-ttu-id="11d29-158">O tempo de falha média do aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="11d29-158">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="11d29-159">Valores válidos -2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="11d29-159">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="11d29-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="11d29-160">Response</span></span>
<span data-ttu-id="11d29-161">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11d29-161">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11d29-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11d29-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="11d29-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11d29-163">Request</span></span>
<span data-ttu-id="11d29-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11d29-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion/{userExperienceAnalyticsAppHealthAppPerformanceByAppVersionId}
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

### <a name="response"></a><span data-ttu-id="11d29-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="11d29-165">Response</span></span>
<span data-ttu-id="11d29-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11d29-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




