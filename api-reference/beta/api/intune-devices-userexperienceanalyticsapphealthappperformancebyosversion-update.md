---
title: Atualizar userExperienceAnalyticsAppHealthAppPerformanceByOSVersion
description: Atualiza as propriedades de um objeto userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3945087d9e8b992f49de0fc07fcc4e11dedefe63
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49203078"
---
# <a name="update-userexperienceanalyticsapphealthappperformancebyosversion"></a><span data-ttu-id="d0ccb-103">Atualizar userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span><span class="sxs-lookup"><span data-stu-id="d0ccb-103">Update userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span></span>

<span data-ttu-id="d0ccb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0ccb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0ccb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0ccb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0ccb-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) .</span><span class="sxs-lookup"><span data-stu-id="d0ccb-107">Update the properties of a [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0ccb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d0ccb-108">Prerequisites</span></span>
<span data-ttu-id="d0ccb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0ccb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0ccb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0ccb-111">Permission type</span></span>|<span data-ttu-id="d0ccb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d0ccb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0ccb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0ccb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d0ccb-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0ccb-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d0ccb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0ccb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0ccb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-116">Not supported.</span></span>|
|<span data-ttu-id="d0ccb-117">Application</span><span class="sxs-lookup"><span data-stu-id="d0ccb-117">Application</span></span>|<span data-ttu-id="d0ccb-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0ccb-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0ccb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0ccb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion/{userExperienceAnalyticsAppHealthAppPerformanceByOSVersionId}
```

## <a name="request-headers"></a><span data-ttu-id="d0ccb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0ccb-120">Request headers</span></span>
|<span data-ttu-id="d0ccb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0ccb-121">Header</span></span>|<span data-ttu-id="d0ccb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d0ccb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0ccb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0ccb-123">Authorization</span></span>|<span data-ttu-id="d0ccb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0ccb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d0ccb-125">Accept</span></span>|<span data-ttu-id="d0ccb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0ccb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0ccb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0ccb-127">Request body</span></span>
<span data-ttu-id="d0ccb-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) .</span><span class="sxs-lookup"><span data-stu-id="d0ccb-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object.</span></span>

<span data-ttu-id="d0ccb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md).</span><span class="sxs-lookup"><span data-stu-id="d0ccb-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md).</span></span>

|<span data-ttu-id="d0ccb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0ccb-130">Property</span></span>|<span data-ttu-id="d0ccb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0ccb-131">Type</span></span>|<span data-ttu-id="d0ccb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0ccb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0ccb-133">id</span><span class="sxs-lookup"><span data-stu-id="d0ccb-133">id</span></span>|<span data-ttu-id="d0ccb-134">String</span><span class="sxs-lookup"><span data-stu-id="d0ccb-134">String</span></span>|<span data-ttu-id="d0ccb-135">O identificador exclusivo do objeto de desempenho da versão do aplicativo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-135">The unique identifier of the user experience analytics app version performance object.</span></span>|
|<span data-ttu-id="d0ccb-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="d0ccb-136">osVersion</span></span>|<span data-ttu-id="d0ccb-137">String</span><span class="sxs-lookup"><span data-stu-id="d0ccb-137">String</span></span>|<span data-ttu-id="d0ccb-138">A versão do sistema operacional do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-138">The os version of the application.</span></span>|
|<span data-ttu-id="d0ccb-139">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="d0ccb-139">osBuildNumber</span></span>|<span data-ttu-id="d0ccb-140">String</span><span class="sxs-lookup"><span data-stu-id="d0ccb-140">String</span></span>|<span data-ttu-id="d0ccb-141">O número de compilação do sistema operacional do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-141">The os build number of the application.</span></span>|
|<span data-ttu-id="d0ccb-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d0ccb-142">activeDeviceCount</span></span>|<span data-ttu-id="d0ccb-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d0ccb-143">Int32</span></span>|<span data-ttu-id="d0ccb-144">O número de dispositivos em que o aplicativo está ativo.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-144">The number of devices where the app has been active.</span></span> <span data-ttu-id="d0ccb-145">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="d0ccb-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="d0ccb-146">appName</span><span class="sxs-lookup"><span data-stu-id="d0ccb-146">appName</span></span>|<span data-ttu-id="d0ccb-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0ccb-147">String</span></span>|<span data-ttu-id="d0ccb-148">O nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-148">The name of the application.</span></span>|
|<span data-ttu-id="d0ccb-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="d0ccb-149">appDisplayName</span></span>|<span data-ttu-id="d0ccb-150">String</span><span class="sxs-lookup"><span data-stu-id="d0ccb-150">String</span></span>|<span data-ttu-id="d0ccb-151">O nome amigável do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-151">The friendly name of the application.</span></span>|
|<span data-ttu-id="d0ccb-152">appPublisher</span><span class="sxs-lookup"><span data-stu-id="d0ccb-152">appPublisher</span></span>|<span data-ttu-id="d0ccb-153">String</span><span class="sxs-lookup"><span data-stu-id="d0ccb-153">String</span></span>|<span data-ttu-id="d0ccb-154">O fornecedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-154">The publisher of the application.</span></span>|
|<span data-ttu-id="d0ccb-155">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="d0ccb-155">appUsageDuration</span></span>|<span data-ttu-id="d0ccb-156">Int32</span><span class="sxs-lookup"><span data-stu-id="d0ccb-156">Int32</span></span>|<span data-ttu-id="d0ccb-157">O tempo total de uso do aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-157">The total usage time of the application in minutes.</span></span> <span data-ttu-id="d0ccb-158">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="d0ccb-158">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="d0ccb-159">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="d0ccb-159">appCrashCount</span></span>|<span data-ttu-id="d0ccb-160">Int32</span><span class="sxs-lookup"><span data-stu-id="d0ccb-160">Int32</span></span>|<span data-ttu-id="d0ccb-161">O número de falhas para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-161">The number of crashes for the app.</span></span> <span data-ttu-id="d0ccb-162">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="d0ccb-162">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="d0ccb-163">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="d0ccb-163">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="d0ccb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d0ccb-164">Int32</span></span>|<span data-ttu-id="d0ccb-165">O tempo médio de falha para o aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-165">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="d0ccb-166">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="d0ccb-166">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="d0ccb-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0ccb-167">Response</span></span>
<span data-ttu-id="d0ccb-168">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-168">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0ccb-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0ccb-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0ccb-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0ccb-170">Request</span></span>
<span data-ttu-id="d0ccb-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion/{userExperienceAnalyticsAppHealthAppPerformanceByOSVersionId}
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

### <a name="response"></a><span data-ttu-id="d0ccb-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0ccb-172">Response</span></span>
<span data-ttu-id="d0ccb-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0ccb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




