---
title: Criar windowsManagementAppHealthState
description: Crie um novo objeto windowsManagementAppHealthState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0ba082150ea5b032a4621bfea33b7d85f5ad2a16
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126379"
---
# <a name="create-windowsmanagementapphealthstate"></a><span data-ttu-id="4ecf9-103">Criar windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="4ecf9-103">Create windowsManagementAppHealthState</span></span>

<span data-ttu-id="4ecf9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ecf9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ecf9-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ecf9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ecf9-107">Crie um novo [objeto windowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)</span><span class="sxs-lookup"><span data-stu-id="4ecf9-107">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ecf9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ecf9-108">Prerequisites</span></span>
<span data-ttu-id="4ecf9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ecf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ecf9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ecf9-111">Permission type</span></span>|<span data-ttu-id="4ecf9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ecf9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ecf9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ecf9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ecf9-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ecf9-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4ecf9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ecf9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ecf9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-116">Not supported.</span></span>|
|<span data-ttu-id="4ecf9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ecf9-117">Application</span></span>|<span data-ttu-id="4ecf9-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ecf9-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ecf9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ecf9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="4ecf9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ecf9-120">Request headers</span></span>
|<span data-ttu-id="4ecf9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ecf9-121">Header</span></span>|<span data-ttu-id="4ecf9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4ecf9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ecf9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ecf9-123">Authorization</span></span>|<span data-ttu-id="4ecf9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ecf9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4ecf9-125">Accept</span></span>|<span data-ttu-id="4ecf9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ecf9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ecf9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ecf9-127">Request body</span></span>
<span data-ttu-id="4ecf9-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsManagementAppHealthState.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-128">In the request body, supply a JSON representation for the windowsManagementAppHealthState object.</span></span>

<span data-ttu-id="4ecf9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o windowsManagementAppHealthState.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-129">The following table shows the properties that are required when you create the windowsManagementAppHealthState.</span></span>

|<span data-ttu-id="4ecf9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ecf9-130">Property</span></span>|<span data-ttu-id="4ecf9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ecf9-131">Type</span></span>|<span data-ttu-id="4ecf9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ecf9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ecf9-133">id</span><span class="sxs-lookup"><span data-stu-id="4ecf9-133">id</span></span>|<span data-ttu-id="4ecf9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ecf9-134">String</span></span>|<span data-ttu-id="4ecf9-135">Identificador exclusivo para o estado de saúde do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-135">Unique Identifier for the Windows management app health state.</span></span> <span data-ttu-id="4ecf9-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-136">This property is read-only.</span></span>|
|<span data-ttu-id="4ecf9-137">healthState</span><span class="sxs-lookup"><span data-stu-id="4ecf9-137">healthState</span></span>|[<span data-ttu-id="4ecf9-138">healthState</span><span class="sxs-lookup"><span data-stu-id="4ecf9-138">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="4ecf9-139">Estado de saúde do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-139">Windows management app health state.</span></span> <span data-ttu-id="4ecf9-140">Os valores possíveis são: `unknown`, `healthy`, `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-140">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="4ecf9-141">installedVersion</span><span class="sxs-lookup"><span data-stu-id="4ecf9-141">installedVersion</span></span>|<span data-ttu-id="4ecf9-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ecf9-142">String</span></span>|<span data-ttu-id="4ecf9-143">Versão instalada do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-143">Windows management app installed version.</span></span>|
|<span data-ttu-id="4ecf9-144">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="4ecf9-144">lastCheckInDateTime</span></span>|<span data-ttu-id="4ecf9-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ecf9-145">DateTimeOffset</span></span>|<span data-ttu-id="4ecf9-146">Última hora de check-in do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-146">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="4ecf9-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="4ecf9-147">deviceName</span></span>|<span data-ttu-id="4ecf9-148">String</span><span class="sxs-lookup"><span data-stu-id="4ecf9-148">String</span></span>|<span data-ttu-id="4ecf9-149">Nome do dispositivo no qual o aplicativo de gerenciamento do Windows está instalado.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-149">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="4ecf9-150">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="4ecf9-150">deviceOSVersion</span></span>|<span data-ttu-id="4ecf9-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ecf9-151">String</span></span>|<span data-ttu-id="4ecf9-152">Versão do sistema operacional Windows 10 do dispositivo no qual o aplicativo de gerenciamento do Windows está instalado.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-152">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="4ecf9-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ecf9-153">Response</span></span>
<span data-ttu-id="4ecf9-154">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-154">If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ecf9-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ecf9-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ecf9-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ecf9-156">Request</span></span>
<span data-ttu-id="4ecf9-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "healthState": "healthy",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```

### <a name="response"></a><span data-ttu-id="4ecf9-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ecf9-158">Response</span></span>
<span data-ttu-id="4ecf9-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ecf9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "5c7e50fb-50fb-5c7e-fb50-7e5cfb507e5c",
  "healthState": "healthy",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```




