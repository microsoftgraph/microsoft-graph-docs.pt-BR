---
title: Criar userExperienceAnalyticsAppHealthOSVersionPerformance
description: Criar um novo objeto userExperienceAnalyticsAppHealthOSVersionPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7bd76e0d5938f80c0a45923b5eb95f278e2edf38
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202567"
---
# <a name="create-userexperienceanalyticsapphealthosversionperformance"></a><span data-ttu-id="90035-103">Criar userExperienceAnalyticsAppHealthOSVersionPerformance</span><span class="sxs-lookup"><span data-stu-id="90035-103">Create userExperienceAnalyticsAppHealthOSVersionPerformance</span></span>

<span data-ttu-id="90035-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90035-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90035-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="90035-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90035-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90035-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90035-107">Criar um novo objeto [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="90035-107">Create a new [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90035-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90035-108">Prerequisites</span></span>
<span data-ttu-id="90035-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90035-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90035-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90035-111">Permission type</span></span>|<span data-ttu-id="90035-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90035-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90035-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90035-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90035-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90035-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="90035-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90035-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90035-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90035-116">Not supported.</span></span>|
|<span data-ttu-id="90035-117">Application</span><span class="sxs-lookup"><span data-stu-id="90035-117">Application</span></span>|<span data-ttu-id="90035-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90035-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90035-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90035-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance
```

## <a name="request-headers"></a><span data-ttu-id="90035-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90035-120">Request headers</span></span>
|<span data-ttu-id="90035-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90035-121">Header</span></span>|<span data-ttu-id="90035-122">Valor</span><span class="sxs-lookup"><span data-stu-id="90035-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90035-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="90035-123">Authorization</span></span>|<span data-ttu-id="90035-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90035-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90035-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90035-125">Accept</span></span>|<span data-ttu-id="90035-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90035-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90035-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90035-127">Request body</span></span>
<span data-ttu-id="90035-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsAppHealthOSVersionPerformance.</span><span class="sxs-lookup"><span data-stu-id="90035-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthOSVersionPerformance object.</span></span>

<span data-ttu-id="90035-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsAppHealthOSVersionPerformance.</span><span class="sxs-lookup"><span data-stu-id="90035-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthOSVersionPerformance.</span></span>

|<span data-ttu-id="90035-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90035-130">Property</span></span>|<span data-ttu-id="90035-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="90035-131">Type</span></span>|<span data-ttu-id="90035-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="90035-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90035-133">id</span><span class="sxs-lookup"><span data-stu-id="90035-133">id</span></span>|<span data-ttu-id="90035-134">String</span><span class="sxs-lookup"><span data-stu-id="90035-134">String</span></span>|<span data-ttu-id="90035-135">O identificador exclusivo do objeto de desempenho da versão da experiência do usuário do Analytics OS.</span><span class="sxs-lookup"><span data-stu-id="90035-135">The unique identifier of the user experience analytics OS version performance object.</span></span>|
|<span data-ttu-id="90035-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="90035-136">osVersion</span></span>|<span data-ttu-id="90035-137">String</span><span class="sxs-lookup"><span data-stu-id="90035-137">String</span></span>|<span data-ttu-id="90035-138">A versão do sistema operacional instalada no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="90035-138">The OS version installed on the device.</span></span>|
|<span data-ttu-id="90035-139">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="90035-139">osBuildNumber</span></span>|<span data-ttu-id="90035-140">String</span><span class="sxs-lookup"><span data-stu-id="90035-140">String</span></span>|<span data-ttu-id="90035-141">O número de compilação do sistema operacional instalado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="90035-141">The OS build number installed on the device.</span></span>|
|<span data-ttu-id="90035-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="90035-142">activeDeviceCount</span></span>|<span data-ttu-id="90035-143">Int32</span><span class="sxs-lookup"><span data-stu-id="90035-143">Int32</span></span>|<span data-ttu-id="90035-144">O número de dispositivos ativos para a versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="90035-144">The number of active devices for the OS version.</span></span> <span data-ttu-id="90035-145">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="90035-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="90035-146">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="90035-146">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="90035-147">Int32</span><span class="sxs-lookup"><span data-stu-id="90035-147">Int32</span></span>|<span data-ttu-id="90035-148">O tempo médio de falha para a versão do sistema operacional em minutos.</span><span class="sxs-lookup"><span data-stu-id="90035-148">The mean time to failure for the OS version in minutes.</span></span> <span data-ttu-id="90035-149">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="90035-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="90035-150">osVersionAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="90035-150">osVersionAppHealthScore</span></span>|<span data-ttu-id="90035-151">Duplo</span><span class="sxs-lookup"><span data-stu-id="90035-151">Double</span></span>|<span data-ttu-id="90035-152">A pontuação de integridade do aplicativo da versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="90035-152">The app health score of the OS version.</span></span> <span data-ttu-id="90035-153">Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="90035-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="90035-154">osVersionAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="90035-154">osVersionAppHealthStatus</span></span>|<span data-ttu-id="90035-155">String</span><span class="sxs-lookup"><span data-stu-id="90035-155">String</span></span>|<span data-ttu-id="90035-156">O status de integridade geral do aplicativo da versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="90035-156">The overall app health status of the OS version.</span></span>|



## <a name="response"></a><span data-ttu-id="90035-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="90035-157">Response</span></span>
<span data-ttu-id="90035-158">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90035-158">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90035-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90035-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="90035-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90035-160">Request</span></span>
<span data-ttu-id="90035-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90035-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance
Content-type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "osVersionAppHealthScore": 7.666666666666667,
  "osVersionAppHealthStatus": "Os Version App Health Status value"
}
```

### <a name="response"></a><span data-ttu-id="90035-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="90035-162">Response</span></span>
<span data-ttu-id="90035-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90035-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 406

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
  "id": "7c28e16b-e16b-7c28-6be1-287c6be1287c",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "osVersionAppHealthScore": 7.666666666666667,
  "osVersionAppHealthStatus": "Os Version App Health Status value"
}
```




