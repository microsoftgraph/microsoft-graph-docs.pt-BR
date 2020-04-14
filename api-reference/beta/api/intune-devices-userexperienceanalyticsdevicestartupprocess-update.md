---
title: Atualizar userExperienceAnalyticsDeviceStartupProcess
description: Atualiza as propriedades de um objeto userExperienceAnalyticsDeviceStartupProcess.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7efdaddcb73c2ffa8c3aa4013c63ecd04520130b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43424914"
---
# <a name="update-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="a09ea-103">Atualizar userExperienceAnalyticsDeviceStartupProcess</span><span class="sxs-lookup"><span data-stu-id="a09ea-103">Update userExperienceAnalyticsDeviceStartupProcess</span></span>

<span data-ttu-id="a09ea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a09ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a09ea-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a09ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a09ea-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a09ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a09ea-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .</span><span class="sxs-lookup"><span data-stu-id="a09ea-107">Update the properties of a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a09ea-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a09ea-108">Prerequisites</span></span>
<span data-ttu-id="a09ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a09ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a09ea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a09ea-111">Permission type</span></span>|<span data-ttu-id="a09ea-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a09ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a09ea-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a09ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a09ea-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a09ea-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a09ea-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a09ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a09ea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a09ea-116">Not supported.</span></span>|
|<span data-ttu-id="a09ea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a09ea-117">Application</span></span>|<span data-ttu-id="a09ea-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a09ea-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a09ea-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a09ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

## <a name="request-headers"></a><span data-ttu-id="a09ea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a09ea-120">Request headers</span></span>
|<span data-ttu-id="a09ea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a09ea-121">Header</span></span>|<span data-ttu-id="a09ea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a09ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a09ea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a09ea-123">Authorization</span></span>|<span data-ttu-id="a09ea-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a09ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a09ea-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a09ea-125">Accept</span></span>|<span data-ttu-id="a09ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a09ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a09ea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a09ea-127">Request body</span></span>
<span data-ttu-id="a09ea-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .</span><span class="sxs-lookup"><span data-stu-id="a09ea-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

<span data-ttu-id="a09ea-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).</span><span class="sxs-lookup"><span data-stu-id="a09ea-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).</span></span>

|<span data-ttu-id="a09ea-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a09ea-130">Property</span></span>|<span data-ttu-id="a09ea-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a09ea-131">Type</span></span>|<span data-ttu-id="a09ea-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a09ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a09ea-133">id</span><span class="sxs-lookup"><span data-stu-id="a09ea-133">id</span></span>|<span data-ttu-id="a09ea-134">String</span><span class="sxs-lookup"><span data-stu-id="a09ea-134">String</span></span>|<span data-ttu-id="a09ea-135">O identificador exclusivo do processo de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a09ea-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="a09ea-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="a09ea-136">managedDeviceId</span></span>|<span data-ttu-id="a09ea-137">String</span><span class="sxs-lookup"><span data-stu-id="a09ea-137">String</span></span>|<span data-ttu-id="a09ea-138">A ID do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a09ea-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="a09ea-139">Process</span><span class="sxs-lookup"><span data-stu-id="a09ea-139">processName</span></span>|<span data-ttu-id="a09ea-140">String</span><span class="sxs-lookup"><span data-stu-id="a09ea-140">String</span></span>|<span data-ttu-id="a09ea-141">Nome do processo de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a09ea-141">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="a09ea-142">productName</span><span class="sxs-lookup"><span data-stu-id="a09ea-142">productName</span></span>|<span data-ttu-id="a09ea-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a09ea-143">String</span></span>|<span data-ttu-id="a09ea-144">O nome do produto do processo de inicialização do dispositivo analítico da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a09ea-144">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="a09ea-145">publicador</span><span class="sxs-lookup"><span data-stu-id="a09ea-145">publisher</span></span>|<span data-ttu-id="a09ea-146">String</span><span class="sxs-lookup"><span data-stu-id="a09ea-146">String</span></span>|<span data-ttu-id="a09ea-147">O fornecedor da experiência do usuário do processo de inicialização do dispositivo de análise.</span><span class="sxs-lookup"><span data-stu-id="a09ea-147">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="a09ea-148">startupImpactInMs</span><span class="sxs-lookup"><span data-stu-id="a09ea-148">startupImpactInMs</span></span>|<span data-ttu-id="a09ea-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a09ea-149">Int32</span></span>|<span data-ttu-id="a09ea-150">Impacto do processo de inicialização do dispositivo de análise de experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="a09ea-150">User experience analytics device startup process impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="a09ea-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a09ea-151">Response</span></span>
<span data-ttu-id="a09ea-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a09ea-152">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a09ea-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a09ea-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="a09ea-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a09ea-154">Request</span></span>
<span data-ttu-id="a09ea-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a09ea-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a09ea-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="a09ea-156">Response</span></span>
<span data-ttu-id="a09ea-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a09ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



