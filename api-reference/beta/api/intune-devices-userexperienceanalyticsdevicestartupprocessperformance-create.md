---
title: Criar userExperienceAnalyticsDeviceStartupProcessPerformance
description: Crie um novo objeto userExperienceAnalyticsDeviceStartupProcessPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5da588641c970adf10d3631f232669743d011c2d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154025"
---
# <a name="create-userexperienceanalyticsdevicestartupprocessperformance"></a><span data-ttu-id="9bada-103">Criar userExperienceAnalyticsDeviceStartupProcessPerformance</span><span class="sxs-lookup"><span data-stu-id="9bada-103">Create userExperienceAnalyticsDeviceStartupProcessPerformance</span></span>

<span data-ttu-id="9bada-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bada-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bada-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9bada-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bada-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9bada-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bada-107">Crie um novo [objeto userExperienceAnalyticsDeviceStartupProcessPerformance.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)</span><span class="sxs-lookup"><span data-stu-id="9bada-107">Create a new [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bada-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9bada-108">Prerequisites</span></span>
<span data-ttu-id="9bada-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bada-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bada-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bada-111">Permission type</span></span>|<span data-ttu-id="9bada-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9bada-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bada-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bada-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9bada-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bada-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9bada-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bada-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bada-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bada-116">Not supported.</span></span>|
|<span data-ttu-id="9bada-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bada-117">Application</span></span>|<span data-ttu-id="9bada-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bada-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bada-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bada-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

## <a name="request-headers"></a><span data-ttu-id="9bada-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bada-120">Request headers</span></span>
|<span data-ttu-id="9bada-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9bada-121">Header</span></span>|<span data-ttu-id="9bada-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9bada-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bada-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bada-123">Authorization</span></span>|<span data-ttu-id="9bada-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bada-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bada-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9bada-125">Accept</span></span>|<span data-ttu-id="9bada-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9bada-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bada-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bada-127">Request body</span></span>
<span data-ttu-id="9bada-128">No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsDeviceStartupProcessPerformance.</span><span class="sxs-lookup"><span data-stu-id="9bada-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupProcessPerformance object.</span></span>

<span data-ttu-id="9bada-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsDeviceStartupProcessPerformance.</span><span class="sxs-lookup"><span data-stu-id="9bada-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupProcessPerformance.</span></span>

|<span data-ttu-id="9bada-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bada-130">Property</span></span>|<span data-ttu-id="9bada-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bada-131">Type</span></span>|<span data-ttu-id="9bada-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bada-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bada-133">id</span><span class="sxs-lookup"><span data-stu-id="9bada-133">id</span></span>|<span data-ttu-id="9bada-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bada-134">String</span></span>|<span data-ttu-id="9bada-135">O identificador exclusivo do desempenho do processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9bada-135">The unique identifier of the user experience analytics device startup process performance.</span></span>|
|<span data-ttu-id="9bada-136">processName</span><span class="sxs-lookup"><span data-stu-id="9bada-136">processName</span></span>|<span data-ttu-id="9bada-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bada-137">String</span></span>|<span data-ttu-id="9bada-138">Nome do processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9bada-138">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="9bada-139">productName</span><span class="sxs-lookup"><span data-stu-id="9bada-139">productName</span></span>|<span data-ttu-id="9bada-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bada-140">String</span></span>|<span data-ttu-id="9bada-141">O nome do produto do processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9bada-141">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="9bada-142">publicador</span><span class="sxs-lookup"><span data-stu-id="9bada-142">publisher</span></span>|<span data-ttu-id="9bada-143">String</span><span class="sxs-lookup"><span data-stu-id="9bada-143">String</span></span>|<span data-ttu-id="9bada-144">O editor de processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9bada-144">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="9bada-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="9bada-145">deviceCount</span></span>|<span data-ttu-id="9bada-146">Int64</span><span class="sxs-lookup"><span data-stu-id="9bada-146">Int64</span></span>|<span data-ttu-id="9bada-147">Contagem resumida do processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9bada-147">User experience analytics device startup process summarized count.</span></span>|
|<span data-ttu-id="9bada-148">medianImpactInMs</span><span class="sxs-lookup"><span data-stu-id="9bada-148">medianImpactInMs</span></span>|<span data-ttu-id="9bada-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9bada-149">Int32</span></span>|<span data-ttu-id="9bada-150">Impacto mediano do processo de inicialização do dispositivo de análise da experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="9bada-150">User experience analytics device startup process median impact in milliseconds.</span></span>|
|<span data-ttu-id="9bada-151">totalImpactInMs</span><span class="sxs-lookup"><span data-stu-id="9bada-151">totalImpactInMs</span></span>|<span data-ttu-id="9bada-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9bada-152">Int32</span></span>|<span data-ttu-id="9bada-153">Impacto total do processo de inicialização do dispositivo de análise de experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="9bada-153">User experience analytics device startup process total impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="9bada-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bada-154">Response</span></span>
<span data-ttu-id="9bada-155">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bada-155">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bada-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bada-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bada-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bada-157">Request</span></span>
<span data-ttu-id="9bada-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bada-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9bada-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bada-159">Response</span></span>
<span data-ttu-id="9bada-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9bada-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




