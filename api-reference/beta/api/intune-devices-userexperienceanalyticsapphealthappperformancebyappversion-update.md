---
title: Atualizar userExperienceAnalyticsAppHealthAppPerformanceByAppVersion
description: Atualiza as propriedades de um objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f3a4abe784a3e023f80c1a3e84dcd8a5b4110de4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49203162"
---
# <a name="update-userexperienceanalyticsapphealthappperformancebyappversion"></a><span data-ttu-id="3709d-103">Atualizar userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span><span class="sxs-lookup"><span data-stu-id="3709d-103">Update userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span></span>

<span data-ttu-id="3709d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3709d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3709d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3709d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3709d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3709d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3709d-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) .</span><span class="sxs-lookup"><span data-stu-id="3709d-107">Update the properties of a [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3709d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3709d-108">Prerequisites</span></span>
<span data-ttu-id="3709d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3709d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3709d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3709d-111">Permission type</span></span>|<span data-ttu-id="3709d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3709d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3709d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3709d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3709d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3709d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3709d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3709d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3709d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3709d-116">Not supported.</span></span>|
|<span data-ttu-id="3709d-117">Application</span><span class="sxs-lookup"><span data-stu-id="3709d-117">Application</span></span>|<span data-ttu-id="3709d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3709d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3709d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3709d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion/{userExperienceAnalyticsAppHealthAppPerformanceByAppVersionId}
```

## <a name="request-headers"></a><span data-ttu-id="3709d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3709d-120">Request headers</span></span>
|<span data-ttu-id="3709d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3709d-121">Header</span></span>|<span data-ttu-id="3709d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3709d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3709d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3709d-123">Authorization</span></span>|<span data-ttu-id="3709d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3709d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3709d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3709d-125">Accept</span></span>|<span data-ttu-id="3709d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3709d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3709d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3709d-127">Request body</span></span>
<span data-ttu-id="3709d-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) .</span><span class="sxs-lookup"><span data-stu-id="3709d-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

<span data-ttu-id="3709d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md).</span><span class="sxs-lookup"><span data-stu-id="3709d-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md).</span></span>

|<span data-ttu-id="3709d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3709d-130">Property</span></span>|<span data-ttu-id="3709d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3709d-131">Type</span></span>|<span data-ttu-id="3709d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3709d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3709d-133">id</span><span class="sxs-lookup"><span data-stu-id="3709d-133">id</span></span>|<span data-ttu-id="3709d-134">String</span><span class="sxs-lookup"><span data-stu-id="3709d-134">String</span></span>|<span data-ttu-id="3709d-135">O identificador exclusivo do objeto de desempenho do aplicativo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="3709d-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="3709d-136">appVersion</span><span class="sxs-lookup"><span data-stu-id="3709d-136">appVersion</span></span>|<span data-ttu-id="3709d-137">String</span><span class="sxs-lookup"><span data-stu-id="3709d-137">String</span></span>|<span data-ttu-id="3709d-138">A versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3709d-138">The version of the application.</span></span>|
|<span data-ttu-id="3709d-139">appName</span><span class="sxs-lookup"><span data-stu-id="3709d-139">appName</span></span>|<span data-ttu-id="3709d-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3709d-140">String</span></span>|<span data-ttu-id="3709d-141">O nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3709d-141">The name of the application.</span></span>|
|<span data-ttu-id="3709d-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="3709d-142">appDisplayName</span></span>|<span data-ttu-id="3709d-143">String</span><span class="sxs-lookup"><span data-stu-id="3709d-143">String</span></span>|<span data-ttu-id="3709d-144">O nome amigável do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3709d-144">The friendly name of the application.</span></span>|
|<span data-ttu-id="3709d-145">appPublisher</span><span class="sxs-lookup"><span data-stu-id="3709d-145">appPublisher</span></span>|<span data-ttu-id="3709d-146">String</span><span class="sxs-lookup"><span data-stu-id="3709d-146">String</span></span>|<span data-ttu-id="3709d-147">O fornecedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3709d-147">The publisher of the application.</span></span>|
|<span data-ttu-id="3709d-148">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="3709d-148">appUsageDuration</span></span>|<span data-ttu-id="3709d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3709d-149">Int32</span></span>|<span data-ttu-id="3709d-150">O tempo total de uso do aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="3709d-150">The total usage time of the application in minutes.</span></span> <span data-ttu-id="3709d-151">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="3709d-151">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="3709d-152">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="3709d-152">appCrashCount</span></span>|<span data-ttu-id="3709d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3709d-153">Int32</span></span>|<span data-ttu-id="3709d-154">O número de falhas para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3709d-154">The number of crashes for the app.</span></span> <span data-ttu-id="3709d-155">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="3709d-155">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="3709d-156">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="3709d-156">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="3709d-157">Int32</span><span class="sxs-lookup"><span data-stu-id="3709d-157">Int32</span></span>|<span data-ttu-id="3709d-158">O tempo médio de falha para o aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="3709d-158">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="3709d-159">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="3709d-159">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="3709d-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="3709d-160">Response</span></span>
<span data-ttu-id="3709d-161">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3709d-161">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3709d-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3709d-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="3709d-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3709d-163">Request</span></span>
<span data-ttu-id="3709d-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3709d-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3709d-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="3709d-165">Response</span></span>
<span data-ttu-id="3709d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3709d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




