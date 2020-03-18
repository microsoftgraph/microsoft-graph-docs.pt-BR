---
title: Atualizar userExperienceAnalyticsDeviceStartupProcess
description: Atualiza as propriedades de um objeto userExperienceAnalyticsDeviceStartupProcess.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 64f52f9a08543ae0cef610bd32e6c58e81f5a45c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813884"
---
# <a name="update-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="f0aef-103">Atualizar userExperienceAnalyticsDeviceStartupProcess</span><span class="sxs-lookup"><span data-stu-id="f0aef-103">Update userExperienceAnalyticsDeviceStartupProcess</span></span>

> <span data-ttu-id="f0aef-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f0aef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0aef-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0aef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0aef-106">Atualiza as propriedades de um objeto [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .</span><span class="sxs-lookup"><span data-stu-id="f0aef-106">Update the properties of a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0aef-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f0aef-107">Prerequisites</span></span>
<span data-ttu-id="f0aef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0aef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0aef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0aef-110">Permission type</span></span>|<span data-ttu-id="f0aef-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f0aef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0aef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0aef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f0aef-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0aef-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f0aef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0aef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0aef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0aef-115">Not supported.</span></span>|
|<span data-ttu-id="f0aef-116">Application</span><span class="sxs-lookup"><span data-stu-id="f0aef-116">Application</span></span>|<span data-ttu-id="f0aef-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0aef-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0aef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0aef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

## <a name="request-headers"></a><span data-ttu-id="f0aef-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0aef-119">Request headers</span></span>
|<span data-ttu-id="f0aef-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f0aef-120">Header</span></span>|<span data-ttu-id="f0aef-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f0aef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0aef-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0aef-122">Authorization</span></span>|<span data-ttu-id="f0aef-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0aef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0aef-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f0aef-124">Accept</span></span>|<span data-ttu-id="f0aef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f0aef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0aef-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0aef-126">Request body</span></span>
<span data-ttu-id="f0aef-127">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .</span><span class="sxs-lookup"><span data-stu-id="f0aef-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

<span data-ttu-id="f0aef-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).</span><span class="sxs-lookup"><span data-stu-id="f0aef-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).</span></span>

|<span data-ttu-id="f0aef-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0aef-129">Property</span></span>|<span data-ttu-id="f0aef-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0aef-130">Type</span></span>|<span data-ttu-id="f0aef-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0aef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0aef-132">id</span><span class="sxs-lookup"><span data-stu-id="f0aef-132">id</span></span>|<span data-ttu-id="f0aef-133">String</span><span class="sxs-lookup"><span data-stu-id="f0aef-133">String</span></span>|<span data-ttu-id="f0aef-134">O identificador exclusivo do processo de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="f0aef-134">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="f0aef-135">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="f0aef-135">managedDeviceId</span></span>|<span data-ttu-id="f0aef-136">String</span><span class="sxs-lookup"><span data-stu-id="f0aef-136">String</span></span>|<span data-ttu-id="f0aef-137">A ID do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="f0aef-137">The user experience analytics device id.</span></span>|
|<span data-ttu-id="f0aef-138">Process</span><span class="sxs-lookup"><span data-stu-id="f0aef-138">processName</span></span>|<span data-ttu-id="f0aef-139">String</span><span class="sxs-lookup"><span data-stu-id="f0aef-139">String</span></span>|<span data-ttu-id="f0aef-140">Nome do processo de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="f0aef-140">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="f0aef-141">productName</span><span class="sxs-lookup"><span data-stu-id="f0aef-141">productName</span></span>|<span data-ttu-id="f0aef-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0aef-142">String</span></span>|<span data-ttu-id="f0aef-143">O nome do produto do processo de inicialização do dispositivo analítico da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="f0aef-143">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="f0aef-144">publicador</span><span class="sxs-lookup"><span data-stu-id="f0aef-144">publisher</span></span>|<span data-ttu-id="f0aef-145">String</span><span class="sxs-lookup"><span data-stu-id="f0aef-145">String</span></span>|<span data-ttu-id="f0aef-146">O fornecedor da experiência do usuário do processo de inicialização do dispositivo de análise.</span><span class="sxs-lookup"><span data-stu-id="f0aef-146">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="f0aef-147">startupImpactInMs</span><span class="sxs-lookup"><span data-stu-id="f0aef-147">startupImpactInMs</span></span>|<span data-ttu-id="f0aef-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aef-148">Int32</span></span>|<span data-ttu-id="f0aef-149">Impacto do processo de inicialização do dispositivo de análise de experiência do usuário em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="f0aef-149">User experience analytics device startup process impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="f0aef-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0aef-150">Response</span></span>
<span data-ttu-id="f0aef-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0aef-151">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0aef-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0aef-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0aef-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0aef-153">Request</span></span>
<span data-ttu-id="f0aef-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0aef-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f0aef-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0aef-155">Response</span></span>
<span data-ttu-id="f0aef-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0aef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




