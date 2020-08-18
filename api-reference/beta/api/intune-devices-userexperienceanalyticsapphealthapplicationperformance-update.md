---
title: Atualizar userExperienceAnalyticsAppHealthApplicationPerformance
description: Atualiza as propriedades de um objeto userExperienceAnalyticsAppHealthApplicationPerformance.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e845c25f1174b36941f22c249f91d365a83a590
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793186"
---
# <a name="update-userexperienceanalyticsapphealthapplicationperformance"></a><span data-ttu-id="57f1a-103">Atualizar userExperienceAnalyticsAppHealthApplicationPerformance</span><span class="sxs-lookup"><span data-stu-id="57f1a-103">Update userExperienceAnalyticsAppHealthApplicationPerformance</span></span>

<span data-ttu-id="57f1a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57f1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57f1a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57f1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57f1a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57f1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57f1a-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="57f1a-107">Update the properties of a [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57f1a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57f1a-108">Prerequisites</span></span>
<span data-ttu-id="57f1a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57f1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57f1a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57f1a-111">Permission type</span></span>|<span data-ttu-id="57f1a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57f1a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57f1a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57f1a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57f1a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57f1a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="57f1a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57f1a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57f1a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57f1a-116">Not supported.</span></span>|
|<span data-ttu-id="57f1a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57f1a-117">Application</span></span>|<span data-ttu-id="57f1a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57f1a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57f1a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57f1a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="57f1a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57f1a-120">Request headers</span></span>
|<span data-ttu-id="57f1a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57f1a-121">Header</span></span>|<span data-ttu-id="57f1a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="57f1a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57f1a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="57f1a-123">Authorization</span></span>|<span data-ttu-id="57f1a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57f1a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57f1a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57f1a-125">Accept</span></span>|<span data-ttu-id="57f1a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57f1a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57f1a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57f1a-127">Request body</span></span>
<span data-ttu-id="57f1a-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="57f1a-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

<span data-ttu-id="57f1a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).</span><span class="sxs-lookup"><span data-stu-id="57f1a-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).</span></span>

|<span data-ttu-id="57f1a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57f1a-130">Property</span></span>|<span data-ttu-id="57f1a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="57f1a-131">Type</span></span>|<span data-ttu-id="57f1a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="57f1a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57f1a-133">id</span><span class="sxs-lookup"><span data-stu-id="57f1a-133">id</span></span>|<span data-ttu-id="57f1a-134">String</span><span class="sxs-lookup"><span data-stu-id="57f1a-134">String</span></span>|<span data-ttu-id="57f1a-135">O identificador exclusivo do objeto de desempenho do aplicativo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="57f1a-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="57f1a-136">appName</span><span class="sxs-lookup"><span data-stu-id="57f1a-136">appName</span></span>|<span data-ttu-id="57f1a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57f1a-137">String</span></span>|<span data-ttu-id="57f1a-138">O nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="57f1a-138">The name of the application.</span></span>|
|<span data-ttu-id="57f1a-139">appFriendlyName</span><span class="sxs-lookup"><span data-stu-id="57f1a-139">appFriendlyName</span></span>|<span data-ttu-id="57f1a-140">String</span><span class="sxs-lookup"><span data-stu-id="57f1a-140">String</span></span>|<span data-ttu-id="57f1a-141">O nome amigável do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="57f1a-141">The friendly name of the application.</span></span>|
|<span data-ttu-id="57f1a-142">appPublisher</span><span class="sxs-lookup"><span data-stu-id="57f1a-142">appPublisher</span></span>|<span data-ttu-id="57f1a-143">String</span><span class="sxs-lookup"><span data-stu-id="57f1a-143">String</span></span>|<span data-ttu-id="57f1a-144">O fornecedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="57f1a-144">The publisher of the application.</span></span>|
|<span data-ttu-id="57f1a-145">activeDevices</span><span class="sxs-lookup"><span data-stu-id="57f1a-145">activeDevices</span></span>|<span data-ttu-id="57f1a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="57f1a-146">Int32</span></span>|<span data-ttu-id="57f1a-147">O número de dispositivos em que o aplicativo está ativo.</span><span class="sxs-lookup"><span data-stu-id="57f1a-147">The number of devices where the app has been active.</span></span> <span data-ttu-id="57f1a-148">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="57f1a-148">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="57f1a-149">totalAppUsageDuration</span><span class="sxs-lookup"><span data-stu-id="57f1a-149">totalAppUsageDuration</span></span>|<span data-ttu-id="57f1a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="57f1a-150">Int32</span></span>|<span data-ttu-id="57f1a-151">O tempo total de uso do aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="57f1a-151">The total usage time of the application in minutes.</span></span> <span data-ttu-id="57f1a-152">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="57f1a-152">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="57f1a-153">totalAppCrashes</span><span class="sxs-lookup"><span data-stu-id="57f1a-153">totalAppCrashes</span></span>|<span data-ttu-id="57f1a-154">Int32</span><span class="sxs-lookup"><span data-stu-id="57f1a-154">Int32</span></span>|<span data-ttu-id="57f1a-155">O número de falhas para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="57f1a-155">The number of crashes for the app.</span></span> <span data-ttu-id="57f1a-156">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="57f1a-156">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="57f1a-157">totalAppHangs</span><span class="sxs-lookup"><span data-stu-id="57f1a-157">totalAppHangs</span></span>|<span data-ttu-id="57f1a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="57f1a-158">Int32</span></span>|<span data-ttu-id="57f1a-159">O número de suspensões para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="57f1a-159">The number of hangs for the app.</span></span> <span data-ttu-id="57f1a-160">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="57f1a-160">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="57f1a-161">meanTimeToFailure</span><span class="sxs-lookup"><span data-stu-id="57f1a-161">meanTimeToFailure</span></span>|<span data-ttu-id="57f1a-162">Int32</span><span class="sxs-lookup"><span data-stu-id="57f1a-162">Int32</span></span>|<span data-ttu-id="57f1a-163">O tempo médio de falha para o aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="57f1a-163">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="57f1a-164">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="57f1a-164">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="57f1a-165">appHealthScore</span><span class="sxs-lookup"><span data-stu-id="57f1a-165">appHealthScore</span></span>|<span data-ttu-id="57f1a-166">Duplo</span><span class="sxs-lookup"><span data-stu-id="57f1a-166">Double</span></span>|<span data-ttu-id="57f1a-167">A pontuação de integridade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="57f1a-167">The health score of the app.</span></span> <span data-ttu-id="57f1a-168">Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="57f1a-168">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="57f1a-169">appHealthStatus</span><span class="sxs-lookup"><span data-stu-id="57f1a-169">appHealthStatus</span></span>|<span data-ttu-id="57f1a-170">String</span><span class="sxs-lookup"><span data-stu-id="57f1a-170">String</span></span>|<span data-ttu-id="57f1a-171">O status de integridade geral do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="57f1a-171">The overall health status of the app.</span></span>|
|<span data-ttu-id="57f1a-172">allOrgsHealthScore</span><span class="sxs-lookup"><span data-stu-id="57f1a-172">allOrgsHealthScore</span></span>|<span data-ttu-id="57f1a-173">Duplo</span><span class="sxs-lookup"><span data-stu-id="57f1a-173">Double</span></span>|<span data-ttu-id="57f1a-174">A pontuação de integridade mediana do aplicativo em todas as organizações.</span><span class="sxs-lookup"><span data-stu-id="57f1a-174">The median health score of the application across all organizations.</span></span> <span data-ttu-id="57f1a-175">Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="57f1a-175">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="57f1a-176">allOrgsMeanTimeToFailure</span><span class="sxs-lookup"><span data-stu-id="57f1a-176">allOrgsMeanTimeToFailure</span></span>|<span data-ttu-id="57f1a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="57f1a-177">Int32</span></span>|<span data-ttu-id="57f1a-178">O tempo médio de falha em todos os organizações expandidas para o aplicativo em minutos.</span><span class="sxs-lookup"><span data-stu-id="57f1a-178">The median mean time to failure across all orgs for the app in minutes.</span></span> <span data-ttu-id="57f1a-179">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="57f1a-179">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="57f1a-180">tenantId</span><span class="sxs-lookup"><span data-stu-id="57f1a-180">tenantId</span></span>|<span data-ttu-id="57f1a-181">String</span><span class="sxs-lookup"><span data-stu-id="57f1a-181">String</span></span>|<span data-ttu-id="57f1a-182">A ID do locatário associado a este objeto de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="57f1a-182">The id of the tenant associated with this app object.</span></span>|
|<span data-ttu-id="57f1a-183">memaTimeGenerated</span><span class="sxs-lookup"><span data-stu-id="57f1a-183">memaTimeGenerated</span></span>|<span data-ttu-id="57f1a-184">String</span><span class="sxs-lookup"><span data-stu-id="57f1a-184">String</span></span>|<span data-ttu-id="57f1a-185">O momento em que a agregação foi realizada no MEMA.</span><span class="sxs-lookup"><span data-stu-id="57f1a-185">The time when aggregation was performed in MEMA.</span></span>|



## <a name="response"></a><span data-ttu-id="57f1a-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="57f1a-186">Response</span></span>
<span data-ttu-id="57f1a-187">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57f1a-187">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57f1a-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57f1a-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="57f1a-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57f1a-189">Request</span></span>
<span data-ttu-id="57f1a-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57f1a-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
Content-type: application/json
Content-length: 591

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "appName": "App Name value",
  "appFriendlyName": "App Friendly Name value",
  "appPublisher": "App Publisher value",
  "activeDevices": 13,
  "totalAppUsageDuration": 5,
  "totalAppCrashes": 15,
  "totalAppHangs": 13,
  "meanTimeToFailure": 1,
  "appHealthScore": 4.666666666666667,
  "appHealthStatus": "App Health Status value",
  "allOrgsHealthScore": 6.0,
  "allOrgsMeanTimeToFailure": 8,
  "tenantId": "Tenant Id value",
  "memaTimeGenerated": "Mema Time Generated value"
}
```

### <a name="response"></a><span data-ttu-id="57f1a-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="57f1a-191">Response</span></span>
<span data-ttu-id="57f1a-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57f1a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 640

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "id": "c7962a87-2a87-c796-872a-96c7872a96c7",
  "appName": "App Name value",
  "appFriendlyName": "App Friendly Name value",
  "appPublisher": "App Publisher value",
  "activeDevices": 13,
  "totalAppUsageDuration": 5,
  "totalAppCrashes": 15,
  "totalAppHangs": 13,
  "meanTimeToFailure": 1,
  "appHealthScore": 4.666666666666667,
  "appHealthStatus": "App Health Status value",
  "allOrgsHealthScore": 6.0,
  "allOrgsMeanTimeToFailure": 8,
  "tenantId": "Tenant Id value",
  "memaTimeGenerated": "Mema Time Generated value"
}
```



