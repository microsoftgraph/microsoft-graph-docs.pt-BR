---
title: Criar windowsManagementAppHealthState
description: Criar um novo objeto windowsManagementAppHealthState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c275825fb5222fcb1a77ed2bd8abce6d76c75594
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785052"
---
# <a name="create-windowsmanagementapphealthstate"></a><span data-ttu-id="f55a3-103">Criar windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="f55a3-103">Create windowsManagementAppHealthState</span></span>

> <span data-ttu-id="f55a3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f55a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f55a3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f55a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f55a3-106">Criar um novo objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="f55a3-106">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f55a3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f55a3-107">Prerequisites</span></span>
<span data-ttu-id="f55a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f55a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f55a3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f55a3-110">Permission type</span></span>|<span data-ttu-id="f55a3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f55a3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f55a3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f55a3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f55a3-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f55a3-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f55a3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f55a3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f55a3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f55a3-115">Not supported.</span></span>|
|<span data-ttu-id="f55a3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f55a3-116">Application</span></span>|<span data-ttu-id="f55a3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f55a3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f55a3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f55a3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="f55a3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f55a3-119">Request headers</span></span>
|<span data-ttu-id="f55a3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f55a3-120">Header</span></span>|<span data-ttu-id="f55a3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f55a3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f55a3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f55a3-122">Authorization</span></span>|<span data-ttu-id="f55a3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f55a3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f55a3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f55a3-124">Accept</span></span>|<span data-ttu-id="f55a3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f55a3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f55a3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f55a3-126">Request body</span></span>
<span data-ttu-id="f55a3-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsManagementAppHealthState.</span><span class="sxs-lookup"><span data-stu-id="f55a3-127">In the request body, supply a JSON representation for the windowsManagementAppHealthState object.</span></span>

<span data-ttu-id="f55a3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsManagementAppHealthState.</span><span class="sxs-lookup"><span data-stu-id="f55a3-128">The following table shows the properties that are required when you create the windowsManagementAppHealthState.</span></span>

|<span data-ttu-id="f55a3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f55a3-129">Property</span></span>|<span data-ttu-id="f55a3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f55a3-130">Type</span></span>|<span data-ttu-id="f55a3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f55a3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f55a3-132">id</span><span class="sxs-lookup"><span data-stu-id="f55a3-132">id</span></span>|<span data-ttu-id="f55a3-133">String</span><span class="sxs-lookup"><span data-stu-id="f55a3-133">String</span></span>|<span data-ttu-id="f55a3-134">Identificador exclusivo para o estado de integridade do aplicativo de gerenciamento do Windows</span><span class="sxs-lookup"><span data-stu-id="f55a3-134">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="f55a3-135">HealthState</span><span class="sxs-lookup"><span data-stu-id="f55a3-135">healthState</span></span>|[<span data-ttu-id="f55a3-136">HealthState</span><span class="sxs-lookup"><span data-stu-id="f55a3-136">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="f55a3-137">Estado de integridade do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="f55a3-137">Windows management app health state.</span></span> <span data-ttu-id="f55a3-138">Os valores possíveis são: `unknown`, `healthy`, `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="f55a3-138">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="f55a3-139">installedVersion</span><span class="sxs-lookup"><span data-stu-id="f55a3-139">installedVersion</span></span>|<span data-ttu-id="f55a3-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f55a3-140">String</span></span>|<span data-ttu-id="f55a3-141">Versão instalada do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="f55a3-141">Windows management app installed version.</span></span>|
|<span data-ttu-id="f55a3-142">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="f55a3-142">lastCheckInDateTime</span></span>|<span data-ttu-id="f55a3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f55a3-143">DateTimeOffset</span></span>|<span data-ttu-id="f55a3-144">Tempo de check-in do aplicativo de gerenciamento do Windows por último.</span><span class="sxs-lookup"><span data-stu-id="f55a3-144">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="f55a3-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="f55a3-145">deviceName</span></span>|<span data-ttu-id="f55a3-146">String</span><span class="sxs-lookup"><span data-stu-id="f55a3-146">String</span></span>|<span data-ttu-id="f55a3-147">Nome do dispositivo no qual o aplicativo de gerenciamento do Windows está instalado.</span><span class="sxs-lookup"><span data-stu-id="f55a3-147">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="f55a3-148">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="f55a3-148">deviceOSVersion</span></span>|<span data-ttu-id="f55a3-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f55a3-149">String</span></span>|<span data-ttu-id="f55a3-150">Versão do Windows 10 so do dispositivo no qual o aplicativo de gerenciamento do Windows está instalado.</span><span class="sxs-lookup"><span data-stu-id="f55a3-150">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="f55a3-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="f55a3-151">Response</span></span>
<span data-ttu-id="f55a3-152">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f55a3-152">If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f55a3-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f55a3-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="f55a3-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f55a3-154">Request</span></span>
<span data-ttu-id="f55a3-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f55a3-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f55a3-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="f55a3-156">Response</span></span>
<span data-ttu-id="f55a3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f55a3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





