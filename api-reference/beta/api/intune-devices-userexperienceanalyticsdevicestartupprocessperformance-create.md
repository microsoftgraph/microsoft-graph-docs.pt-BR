---
title: Criar userExperienceAnalyticsDeviceStartupProcessPerformance
description: Criar um novo objeto userExperienceAnalyticsDeviceStartupProcessPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3e6229c411ac5dee65aae2da5aa7f0d90617ea35
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082487"
---
# <a name="create-userexperienceanalyticsdevicestartupprocessperformance"></a><span data-ttu-id="1bdc7-103">Criar userExperienceAnalyticsDeviceStartupProcessPerformance</span><span class="sxs-lookup"><span data-stu-id="1bdc7-103">Create userExperienceAnalyticsDeviceStartupProcessPerformance</span></span>

<span data-ttu-id="1bdc7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bdc7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bdc7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1bdc7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bdc7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1bdc7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bdc7-107">Criar um novo objeto [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="1bdc7-107">Create a new [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bdc7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1bdc7-108">Prerequisites</span></span>
<span data-ttu-id="1bdc7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bdc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bdc7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bdc7-111">Permission type</span></span>|<span data-ttu-id="1bdc7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1bdc7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bdc7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bdc7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1bdc7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bdc7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1bdc7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bdc7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bdc7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bdc7-116">Not supported.</span></span>|
|<span data-ttu-id="1bdc7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1bdc7-117">Application</span></span>|<span data-ttu-id="1bdc7-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bdc7-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bdc7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bdc7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

## <a name="request-headers"></a><span data-ttu-id="1bdc7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bdc7-120">Request headers</span></span>
|<span data-ttu-id="1bdc7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1bdc7-121">Header</span></span>|<span data-ttu-id="1bdc7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1bdc7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bdc7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bdc7-123">Authorization</span></span>|<span data-ttu-id="1bdc7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bdc7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bdc7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1bdc7-125">Accept</span></span>|<span data-ttu-id="1bdc7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1bdc7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bdc7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bdc7-127">Request body</span></span>
<span data-ttu-id="1bdc7-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsDeviceStartupProcessPerformance.</span><span class="sxs-lookup"><span data-stu-id="1bdc7-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupProcessPerformance object.</span></span>

<span data-ttu-id="1bdc7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsDeviceStartupProcessPerformance.</span><span class="sxs-lookup"><span data-stu-id="1bdc7-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupProcessPerformance.</span></span>

|<span data-ttu-id="1bdc7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bdc7-130">Property</span></span>|<span data-ttu-id="1bdc7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bdc7-131">Type</span></span>|<span data-ttu-id="1bdc7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bdc7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bdc7-133">id</span><span class="sxs-lookup"><span data-stu-id="1bdc7-133">id</span></span>|<span data-ttu-id="1bdc7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bdc7-134">String</span></span>|<span data-ttu-id="1bdc7-135">O identificador exclusivo do desempenho do processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="1bdc7-135">The unique identifier of the user experience analytics device startup process performance.</span></span>|
|<span data-ttu-id="1bdc7-136">Process</span><span class="sxs-lookup"><span data-stu-id="1bdc7-136">processName</span></span>|<span data-ttu-id="1bdc7-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bdc7-137">String</span></span>|<span data-ttu-id="1bdc7-138">Nome do processo de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="1bdc7-138">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="1bdc7-139">productName</span><span class="sxs-lookup"><span data-stu-id="1bdc7-139">productName</span></span>|<span data-ttu-id="1bdc7-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bdc7-140">String</span></span>|<span data-ttu-id="1bdc7-141">O nome do produto do processo de inicialização do dispositivo analítico da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="1bdc7-141">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="1bdc7-142">publicador</span><span class="sxs-lookup"><span data-stu-id="1bdc7-142">publisher</span></span>|<span data-ttu-id="1bdc7-143">String</span><span class="sxs-lookup"><span data-stu-id="1bdc7-143">String</span></span>|<span data-ttu-id="1bdc7-144">O fornecedor da experiência do usuário do processo de inicialização do dispositivo de análise.</span><span class="sxs-lookup"><span data-stu-id="1bdc7-144">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="1bdc7-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="1bdc7-145">deviceCount</span></span>|<span data-ttu-id="1bdc7-146">Int64</span><span class="sxs-lookup"><span data-stu-id="1bdc7-146">Int64</span></span>|<span data-ttu-id="1bdc7-147">Contagem resumida do processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="1bdc7-147">User experience analytics device startup process summarized count.</span></span>|
|<span data-ttu-id="1bdc7-148">medianImpactInMs</span><span class="sxs-lookup"><span data-stu-id="1bdc7-148">medianImpactInMs</span></span>|<span data-ttu-id="1bdc7-149">Int32</span><span class="sxs-lookup"><span data-stu-id="1bdc7-149">Int32</span></span>|<span data-ttu-id="1bdc7-150">Experiência do usuário do processo de inicialização do dispositivo de análise o impacto médio em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="1bdc7-150">User experience analytics device startup process median impact in milliseconds.</span></span>|
|<span data-ttu-id="1bdc7-151">totalImpactInMs</span><span class="sxs-lookup"><span data-stu-id="1bdc7-151">totalImpactInMs</span></span>|<span data-ttu-id="1bdc7-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1bdc7-152">Int32</span></span>|<span data-ttu-id="1bdc7-153">Experiência do usuário do processo de inicialização do dispositivo de análise o impacto total em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="1bdc7-153">User experience analytics device startup process total impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="1bdc7-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bdc7-154">Response</span></span>
<span data-ttu-id="1bdc7-155">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bdc7-155">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bdc7-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bdc7-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bdc7-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bdc7-157">Request</span></span>
<span data-ttu-id="1bdc7-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bdc7-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
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

### <a name="response"></a><span data-ttu-id="1bdc7-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bdc7-159">Response</span></span>
<span data-ttu-id="1bdc7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1bdc7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






