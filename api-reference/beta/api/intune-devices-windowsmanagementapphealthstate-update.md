---
title: Atualizar windowsManagementAppHealthState
description: Atualiza as propriedades de um objeto windowsManagementAppHealthState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0222cda3c2fed2afb9ef959ada65e08e001ad30a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35985620"
---
# <a name="update-windowsmanagementapphealthstate"></a><span data-ttu-id="5650b-103">Atualizar windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="5650b-103">Update windowsManagementAppHealthState</span></span>

> <span data-ttu-id="5650b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5650b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5650b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5650b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5650b-106">Atualiza as propriedades de um objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="5650b-106">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5650b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5650b-107">Prerequisites</span></span>
<span data-ttu-id="5650b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5650b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5650b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5650b-110">Permission type</span></span>|<span data-ttu-id="5650b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5650b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5650b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5650b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5650b-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5650b-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5650b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5650b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5650b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5650b-115">Not supported.</span></span>|
|<span data-ttu-id="5650b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5650b-116">Application</span></span>|<span data-ttu-id="5650b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5650b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5650b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5650b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a><span data-ttu-id="5650b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5650b-119">Request headers</span></span>
|<span data-ttu-id="5650b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5650b-120">Header</span></span>|<span data-ttu-id="5650b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5650b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5650b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5650b-122">Authorization</span></span>|<span data-ttu-id="5650b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5650b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5650b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5650b-124">Accept</span></span>|<span data-ttu-id="5650b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5650b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5650b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5650b-126">Request body</span></span>
<span data-ttu-id="5650b-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="5650b-127">In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

<span data-ttu-id="5650b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span><span class="sxs-lookup"><span data-stu-id="5650b-128">The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>

|<span data-ttu-id="5650b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5650b-129">Property</span></span>|<span data-ttu-id="5650b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5650b-130">Type</span></span>|<span data-ttu-id="5650b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5650b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5650b-132">id</span><span class="sxs-lookup"><span data-stu-id="5650b-132">id</span></span>|<span data-ttu-id="5650b-133">String</span><span class="sxs-lookup"><span data-stu-id="5650b-133">String</span></span>|<span data-ttu-id="5650b-134">Identificador exclusivo para o estado de integridade do aplicativo de gerenciamento do Windows</span><span class="sxs-lookup"><span data-stu-id="5650b-134">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="5650b-135">HealthState</span><span class="sxs-lookup"><span data-stu-id="5650b-135">healthState</span></span>|[<span data-ttu-id="5650b-136">HealthState</span><span class="sxs-lookup"><span data-stu-id="5650b-136">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="5650b-137">Estado de integridade do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="5650b-137">Windows management app health state.</span></span> <span data-ttu-id="5650b-138">Os valores possíveis são: `unknown`, `healthy`, `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="5650b-138">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="5650b-139">installedVersion</span><span class="sxs-lookup"><span data-stu-id="5650b-139">installedVersion</span></span>|<span data-ttu-id="5650b-140">String</span><span class="sxs-lookup"><span data-stu-id="5650b-140">String</span></span>|<span data-ttu-id="5650b-141">Versão instalada do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="5650b-141">Windows management app installed version.</span></span>|
|<span data-ttu-id="5650b-142">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="5650b-142">lastCheckInDateTime</span></span>|<span data-ttu-id="5650b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5650b-143">DateTimeOffset</span></span>|<span data-ttu-id="5650b-144">Tempo de check-in do aplicativo de gerenciamento do Windows por último.</span><span class="sxs-lookup"><span data-stu-id="5650b-144">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="5650b-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="5650b-145">deviceName</span></span>|<span data-ttu-id="5650b-146">String</span><span class="sxs-lookup"><span data-stu-id="5650b-146">String</span></span>|<span data-ttu-id="5650b-147">Nome do dispositivo no qual o aplicativo de gerenciamento do Windows está instalado.</span><span class="sxs-lookup"><span data-stu-id="5650b-147">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="5650b-148">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="5650b-148">deviceOSVersion</span></span>|<span data-ttu-id="5650b-149">String</span><span class="sxs-lookup"><span data-stu-id="5650b-149">String</span></span>|<span data-ttu-id="5650b-150">Versão do Windows 10 so do dispositivo no qual o aplicativo de gerenciamento do Windows está instalado.</span><span class="sxs-lookup"><span data-stu-id="5650b-150">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="5650b-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="5650b-151">Response</span></span>
<span data-ttu-id="5650b-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5650b-152">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5650b-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5650b-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="5650b-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5650b-154">Request</span></span>
<span data-ttu-id="5650b-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5650b-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
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

### <a name="response"></a><span data-ttu-id="5650b-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="5650b-156">Response</span></span>
<span data-ttu-id="5650b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5650b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





