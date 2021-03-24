---
title: Criar userExperienceAnalyticsDeviceStartupProcess
description: Crie um novo objeto userExperienceAnalyticsDeviceStartupProcess.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2e269a9ad65db24f3646e49ab80d11edbaeb1952
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135989"
---
# <a name="create-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="ee802-103">Criar userExperienceAnalyticsDeviceStartupProcess</span><span class="sxs-lookup"><span data-stu-id="ee802-103">Create userExperienceAnalyticsDeviceStartupProcess</span></span>

<span data-ttu-id="ee802-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee802-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee802-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ee802-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee802-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee802-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee802-107">Crie um novo [objeto userExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)</span><span class="sxs-lookup"><span data-stu-id="ee802-107">Create a new [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee802-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ee802-108">Prerequisites</span></span>
<span data-ttu-id="ee802-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee802-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee802-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee802-111">Permission type</span></span>|<span data-ttu-id="ee802-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee802-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee802-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee802-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee802-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee802-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ee802-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee802-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee802-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee802-116">Not supported.</span></span>|
|<span data-ttu-id="ee802-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee802-117">Application</span></span>|<span data-ttu-id="ee802-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee802-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee802-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee802-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses
```

## <a name="request-headers"></a><span data-ttu-id="ee802-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee802-120">Request headers</span></span>
|<span data-ttu-id="ee802-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ee802-121">Header</span></span>|<span data-ttu-id="ee802-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ee802-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee802-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee802-123">Authorization</span></span>|<span data-ttu-id="ee802-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee802-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee802-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ee802-125">Accept</span></span>|<span data-ttu-id="ee802-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee802-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee802-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee802-127">Request body</span></span>
<span data-ttu-id="ee802-128">No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsDeviceStartupProcess.</span><span class="sxs-lookup"><span data-stu-id="ee802-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupProcess object.</span></span>

<span data-ttu-id="ee802-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsDeviceStartupProcess.</span><span class="sxs-lookup"><span data-stu-id="ee802-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupProcess.</span></span>

|<span data-ttu-id="ee802-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee802-130">Property</span></span>|<span data-ttu-id="ee802-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee802-131">Type</span></span>|<span data-ttu-id="ee802-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee802-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee802-133">id</span><span class="sxs-lookup"><span data-stu-id="ee802-133">id</span></span>|<span data-ttu-id="ee802-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee802-134">String</span></span>|<span data-ttu-id="ee802-135">O identificador exclusivo do processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ee802-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="ee802-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="ee802-136">managedDeviceId</span></span>|<span data-ttu-id="ee802-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee802-137">String</span></span>|<span data-ttu-id="ee802-138">A ID do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ee802-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="ee802-139">processName</span><span class="sxs-lookup"><span data-stu-id="ee802-139">processName</span></span>|<span data-ttu-id="ee802-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee802-140">String</span></span>|<span data-ttu-id="ee802-141">Nome do processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ee802-141">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="ee802-142">productName</span><span class="sxs-lookup"><span data-stu-id="ee802-142">productName</span></span>|<span data-ttu-id="ee802-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee802-143">String</span></span>|<span data-ttu-id="ee802-144">O nome do produto do processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ee802-144">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="ee802-145">publicador</span><span class="sxs-lookup"><span data-stu-id="ee802-145">publisher</span></span>|<span data-ttu-id="ee802-146">String</span><span class="sxs-lookup"><span data-stu-id="ee802-146">String</span></span>|<span data-ttu-id="ee802-147">O editor de processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ee802-147">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="ee802-148">startupImpactInMs</span><span class="sxs-lookup"><span data-stu-id="ee802-148">startupImpactInMs</span></span>|<span data-ttu-id="ee802-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ee802-149">Int32</span></span>|<span data-ttu-id="ee802-150">Impacto no processo de inicialização do dispositivo de análise de experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="ee802-150">User experience analytics device startup process impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="ee802-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee802-151">Response</span></span>
<span data-ttu-id="ee802-152">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee802-152">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee802-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee802-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee802-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee802-154">Request</span></span>
<span data-ttu-id="ee802-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee802-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcesses
Content-type: application/json
Content-length: 276

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "managedDeviceId": "Managed Device Id value",
  "processName": "Process Name value",
  "productName": "Product Name value",
  "publisher": "Publisher value",
  "startupImpactInMs": 1
}
```

### <a name="response"></a><span data-ttu-id="ee802-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee802-156">Response</span></span>
<span data-ttu-id="ee802-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee802-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 325

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "id": "03b451e6-51e6-03b4-e651-b403e651b403",
  "managedDeviceId": "Managed Device Id value",
  "processName": "Process Name value",
  "productName": "Product Name value",
  "publisher": "Publisher value",
  "startupImpactInMs": 1
}
```




