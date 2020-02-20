---
title: Atualizar userExperienceAnalyticsDeviceStartupProcessPerformance
description: Atualiza as propriedades de um objeto userExperienceAnalyticsDeviceStartupProcessPerformance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fdcfbb5ac8ff2ce37873a5b9dd9cdac923f237e0
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161942"
---
# <a name="update-userexperienceanalyticsdevicestartupprocessperformance"></a><span data-ttu-id="8101c-103">Atualizar userExperienceAnalyticsDeviceStartupProcessPerformance</span><span class="sxs-lookup"><span data-stu-id="8101c-103">Update userExperienceAnalyticsDeviceStartupProcessPerformance</span></span>

> <span data-ttu-id="8101c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8101c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8101c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8101c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8101c-106">Atualiza as propriedades de um objeto [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="8101c-106">Update the properties of a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8101c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8101c-107">Prerequisites</span></span>
<span data-ttu-id="8101c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8101c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8101c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8101c-110">Permission type</span></span>|<span data-ttu-id="8101c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8101c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8101c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8101c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8101c-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8101c-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8101c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8101c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8101c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8101c-115">Not supported.</span></span>|
|<span data-ttu-id="8101c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8101c-116">Application</span></span>|<span data-ttu-id="8101c-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8101c-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8101c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8101c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance/{userExperienceAnalyticsDeviceStartupProcessPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="8101c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8101c-119">Request headers</span></span>
|<span data-ttu-id="8101c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8101c-120">Header</span></span>|<span data-ttu-id="8101c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8101c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8101c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8101c-122">Authorization</span></span>|<span data-ttu-id="8101c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8101c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8101c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8101c-124">Accept</span></span>|<span data-ttu-id="8101c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8101c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8101c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8101c-126">Request body</span></span>
<span data-ttu-id="8101c-127">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="8101c-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

<span data-ttu-id="8101c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md).</span><span class="sxs-lookup"><span data-stu-id="8101c-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md).</span></span>

|<span data-ttu-id="8101c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8101c-129">Property</span></span>|<span data-ttu-id="8101c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8101c-130">Type</span></span>|<span data-ttu-id="8101c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8101c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8101c-132">id</span><span class="sxs-lookup"><span data-stu-id="8101c-132">id</span></span>|<span data-ttu-id="8101c-133">String</span><span class="sxs-lookup"><span data-stu-id="8101c-133">String</span></span>|<span data-ttu-id="8101c-134">O identificador exclusivo do desempenho do processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8101c-134">The unique identifier of the user experience analytics device startup process performance.</span></span>|
|<span data-ttu-id="8101c-135">Process</span><span class="sxs-lookup"><span data-stu-id="8101c-135">processName</span></span>|<span data-ttu-id="8101c-136">String</span><span class="sxs-lookup"><span data-stu-id="8101c-136">String</span></span>|<span data-ttu-id="8101c-137">Nome do processo de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8101c-137">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="8101c-138">productName</span><span class="sxs-lookup"><span data-stu-id="8101c-138">productName</span></span>|<span data-ttu-id="8101c-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8101c-139">String</span></span>|<span data-ttu-id="8101c-140">O nome do produto do processo de inicialização do dispositivo analítico da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8101c-140">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="8101c-141">publicador</span><span class="sxs-lookup"><span data-stu-id="8101c-141">publisher</span></span>|<span data-ttu-id="8101c-142">String</span><span class="sxs-lookup"><span data-stu-id="8101c-142">String</span></span>|<span data-ttu-id="8101c-143">O fornecedor da experiência do usuário do processo de inicialização do dispositivo de análise.</span><span class="sxs-lookup"><span data-stu-id="8101c-143">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="8101c-144">deviceCount</span><span class="sxs-lookup"><span data-stu-id="8101c-144">deviceCount</span></span>|<span data-ttu-id="8101c-145">Int64</span><span class="sxs-lookup"><span data-stu-id="8101c-145">Int64</span></span>|<span data-ttu-id="8101c-146">Contagem resumida do processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8101c-146">User experience analytics device startup process summarized count.</span></span>|
|<span data-ttu-id="8101c-147">medianImpactInMs</span><span class="sxs-lookup"><span data-stu-id="8101c-147">medianImpactInMs</span></span>|<span data-ttu-id="8101c-148">Int32</span><span class="sxs-lookup"><span data-stu-id="8101c-148">Int32</span></span>|<span data-ttu-id="8101c-149">Experiência do usuário do processo de inicialização do dispositivo de análise o impacto médio em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="8101c-149">User experience analytics device startup process median impact in milliseconds.</span></span>|
|<span data-ttu-id="8101c-150">totalImpactInMs</span><span class="sxs-lookup"><span data-stu-id="8101c-150">totalImpactInMs</span></span>|<span data-ttu-id="8101c-151">Int32</span><span class="sxs-lookup"><span data-stu-id="8101c-151">Int32</span></span>|<span data-ttu-id="8101c-152">Experiência do usuário do processo de inicialização do dispositivo de análise o impacto total em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="8101c-152">User experience analytics device startup process total impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="8101c-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="8101c-153">Response</span></span>
<span data-ttu-id="8101c-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8101c-154">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8101c-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8101c-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="8101c-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8101c-156">Request</span></span>
<span data-ttu-id="8101c-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8101c-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance/{userExperienceAnalyticsDeviceStartupProcessPerformanceId}
Content-type: application/json
Content-length: 285

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "processName": "Process Name value",
  "productName": "Product Name value",
  "publisher": "Publisher value",
  "deviceCount": 11,
  "medianImpactInMs": 0,
  "totalImpactInMs": 15
}
```

### <a name="response"></a><span data-ttu-id="8101c-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="8101c-158">Response</span></span>
<span data-ttu-id="8101c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8101c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 334

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "id": "86c4355c-355c-86c4-5c35-c4865c35c486",
  "processName": "Process Name value",
  "productName": "Product Name value",
  "publisher": "Publisher value",
  "deviceCount": 11,
  "medianImpactInMs": 0,
  "totalImpactInMs": 15
}
```





