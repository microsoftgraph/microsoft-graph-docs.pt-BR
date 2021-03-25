---
title: Atualizar userExperienceAnalyticsDeviceStartupProcess
description: Atualize as propriedades de um objeto userExperienceAnalyticsDeviceStartupProcess.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8439c1ddcd646fc208950195224fc9241b4ae435
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154053"
---
# <a name="update-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="d0999-103">Atualizar userExperienceAnalyticsDeviceStartupProcess</span><span class="sxs-lookup"><span data-stu-id="d0999-103">Update userExperienceAnalyticsDeviceStartupProcess</span></span>

<span data-ttu-id="d0999-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0999-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0999-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d0999-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0999-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d0999-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0999-107">Atualize as propriedades de [um objeto userExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)</span><span class="sxs-lookup"><span data-stu-id="d0999-107">Update the properties of a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0999-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d0999-108">Prerequisites</span></span>
<span data-ttu-id="d0999-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0999-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0999-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0999-111">Permission type</span></span>|<span data-ttu-id="d0999-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0999-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0999-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0999-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d0999-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0999-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d0999-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0999-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0999-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0999-116">Not supported.</span></span>|
|<span data-ttu-id="d0999-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0999-117">Application</span></span>|<span data-ttu-id="d0999-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0999-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0999-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0999-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

## <a name="request-headers"></a><span data-ttu-id="d0999-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0999-120">Request headers</span></span>
|<span data-ttu-id="d0999-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0999-121">Header</span></span>|<span data-ttu-id="d0999-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d0999-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0999-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0999-123">Authorization</span></span>|<span data-ttu-id="d0999-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0999-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0999-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d0999-125">Accept</span></span>|<span data-ttu-id="d0999-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0999-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0999-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0999-127">Request body</span></span>
<span data-ttu-id="d0999-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)</span><span class="sxs-lookup"><span data-stu-id="d0999-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

<span data-ttu-id="d0999-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).</span><span class="sxs-lookup"><span data-stu-id="d0999-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).</span></span>

|<span data-ttu-id="d0999-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0999-130">Property</span></span>|<span data-ttu-id="d0999-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0999-131">Type</span></span>|<span data-ttu-id="d0999-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0999-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0999-133">id</span><span class="sxs-lookup"><span data-stu-id="d0999-133">id</span></span>|<span data-ttu-id="d0999-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0999-134">String</span></span>|<span data-ttu-id="d0999-135">O identificador exclusivo do processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="d0999-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="d0999-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="d0999-136">managedDeviceId</span></span>|<span data-ttu-id="d0999-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0999-137">String</span></span>|<span data-ttu-id="d0999-138">A ID do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="d0999-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="d0999-139">processName</span><span class="sxs-lookup"><span data-stu-id="d0999-139">processName</span></span>|<span data-ttu-id="d0999-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0999-140">String</span></span>|<span data-ttu-id="d0999-141">Nome do processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="d0999-141">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="d0999-142">productName</span><span class="sxs-lookup"><span data-stu-id="d0999-142">productName</span></span>|<span data-ttu-id="d0999-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0999-143">String</span></span>|<span data-ttu-id="d0999-144">O nome do produto do processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="d0999-144">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="d0999-145">publicador</span><span class="sxs-lookup"><span data-stu-id="d0999-145">publisher</span></span>|<span data-ttu-id="d0999-146">String</span><span class="sxs-lookup"><span data-stu-id="d0999-146">String</span></span>|<span data-ttu-id="d0999-147">O editor de processo de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="d0999-147">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="d0999-148">startupImpactInMs</span><span class="sxs-lookup"><span data-stu-id="d0999-148">startupImpactInMs</span></span>|<span data-ttu-id="d0999-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d0999-149">Int32</span></span>|<span data-ttu-id="d0999-150">Impacto no processo de inicialização do dispositivo de análise de experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="d0999-150">User experience analytics device startup process impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="d0999-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0999-151">Response</span></span>
<span data-ttu-id="d0999-152">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0999-152">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0999-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0999-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0999-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0999-154">Request</span></span>
<span data-ttu-id="d0999-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0999-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
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

### <a name="response"></a><span data-ttu-id="d0999-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0999-156">Response</span></span>
<span data-ttu-id="d0999-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0999-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




