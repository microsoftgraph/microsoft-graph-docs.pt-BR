---
title: Atualizar windowsManagementAppHealthState
description: Atualiza as propriedades de um objeto windowsManagementAppHealthState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7724051789f00d1cc1c8a0ccb625f838e6e2eee7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972179"
---
# <a name="update-windowsmanagementapphealthstate"></a><span data-ttu-id="f76b7-103">Atualizar windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="f76b7-103">Update windowsManagementAppHealthState</span></span>

<span data-ttu-id="f76b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f76b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f76b7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f76b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f76b7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f76b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f76b7-107">Atualiza as propriedades de um objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="f76b7-107">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f76b7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f76b7-108">Prerequisites</span></span>
<span data-ttu-id="f76b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f76b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f76b7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f76b7-111">Permission type</span></span>|<span data-ttu-id="f76b7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f76b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f76b7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f76b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f76b7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f76b7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f76b7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f76b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f76b7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f76b7-116">Not supported.</span></span>|
|<span data-ttu-id="f76b7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f76b7-117">Application</span></span>|<span data-ttu-id="f76b7-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f76b7-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f76b7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f76b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a><span data-ttu-id="f76b7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f76b7-120">Request headers</span></span>
|<span data-ttu-id="f76b7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f76b7-121">Header</span></span>|<span data-ttu-id="f76b7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f76b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f76b7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f76b7-123">Authorization</span></span>|<span data-ttu-id="f76b7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f76b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f76b7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f76b7-125">Accept</span></span>|<span data-ttu-id="f76b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f76b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f76b7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f76b7-127">Request body</span></span>
<span data-ttu-id="f76b7-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="f76b7-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

<span data-ttu-id="f76b7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span><span class="sxs-lookup"><span data-stu-id="f76b7-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>

|<span data-ttu-id="f76b7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f76b7-130">Property</span></span>|<span data-ttu-id="f76b7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f76b7-131">Type</span></span>|<span data-ttu-id="f76b7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f76b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f76b7-133">id</span><span class="sxs-lookup"><span data-stu-id="f76b7-133">id</span></span>|<span data-ttu-id="f76b7-134">String</span><span class="sxs-lookup"><span data-stu-id="f76b7-134">String</span></span>|<span data-ttu-id="f76b7-135">Identificador exclusivo do estado de integridade do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="f76b7-135">Unique Identifier for the Windows management app health state.</span></span> <span data-ttu-id="f76b7-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f76b7-136">This property is read-only.</span></span>|
|<span data-ttu-id="f76b7-137">HealthState</span><span class="sxs-lookup"><span data-stu-id="f76b7-137">healthState</span></span>|[<span data-ttu-id="f76b7-138">HealthState</span><span class="sxs-lookup"><span data-stu-id="f76b7-138">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="f76b7-139">Estado de integridade do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="f76b7-139">Windows management app health state.</span></span> <span data-ttu-id="f76b7-140">Os valores possíveis são: `unknown`, `healthy`, `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="f76b7-140">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="f76b7-141">installedVersion</span><span class="sxs-lookup"><span data-stu-id="f76b7-141">installedVersion</span></span>|<span data-ttu-id="f76b7-142">String</span><span class="sxs-lookup"><span data-stu-id="f76b7-142">String</span></span>|<span data-ttu-id="f76b7-143">Versão instalada do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="f76b7-143">Windows management app installed version.</span></span>|
|<span data-ttu-id="f76b7-144">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="f76b7-144">lastCheckInDateTime</span></span>|<span data-ttu-id="f76b7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f76b7-145">DateTimeOffset</span></span>|<span data-ttu-id="f76b7-146">Tempo de check-in do aplicativo de gerenciamento do Windows por último.</span><span class="sxs-lookup"><span data-stu-id="f76b7-146">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="f76b7-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="f76b7-147">deviceName</span></span>|<span data-ttu-id="f76b7-148">String</span><span class="sxs-lookup"><span data-stu-id="f76b7-148">String</span></span>|<span data-ttu-id="f76b7-149">Nome do dispositivo no qual o aplicativo de gerenciamento do Windows está instalado.</span><span class="sxs-lookup"><span data-stu-id="f76b7-149">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="f76b7-150">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="f76b7-150">deviceOSVersion</span></span>|<span data-ttu-id="f76b7-151">String</span><span class="sxs-lookup"><span data-stu-id="f76b7-151">String</span></span>|<span data-ttu-id="f76b7-152">Versão do Windows 10 so do dispositivo no qual o aplicativo de gerenciamento do Windows está instalado.</span><span class="sxs-lookup"><span data-stu-id="f76b7-152">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="f76b7-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="f76b7-153">Response</span></span>
<span data-ttu-id="f76b7-154">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f76b7-154">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f76b7-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f76b7-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="f76b7-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f76b7-156">Request</span></span>
<span data-ttu-id="f76b7-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f76b7-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f76b7-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="f76b7-158">Response</span></span>
<span data-ttu-id="f76b7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f76b7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






