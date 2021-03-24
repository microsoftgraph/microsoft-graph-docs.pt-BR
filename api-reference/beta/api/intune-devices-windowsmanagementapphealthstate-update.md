---
title: Atualizar windowsManagementAppHealthState
description: Atualize as propriedades de um objeto windowsManagementAppHealthState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 88bfa7732662a1a3d2d0f7b60835a3a83bde90ad
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126322"
---
# <a name="update-windowsmanagementapphealthstate"></a><span data-ttu-id="67c3c-103">Atualizar windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="67c3c-103">Update windowsManagementAppHealthState</span></span>

<span data-ttu-id="67c3c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67c3c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67c3c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67c3c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67c3c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67c3c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67c3c-107">Atualize as propriedades de um [objeto windowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)</span><span class="sxs-lookup"><span data-stu-id="67c3c-107">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67c3c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67c3c-108">Prerequisites</span></span>
<span data-ttu-id="67c3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67c3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67c3c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67c3c-111">Permission type</span></span>|<span data-ttu-id="67c3c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67c3c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67c3c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67c3c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67c3c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67c3c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="67c3c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67c3c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67c3c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67c3c-116">Not supported.</span></span>|
|<span data-ttu-id="67c3c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67c3c-117">Application</span></span>|<span data-ttu-id="67c3c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67c3c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67c3c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67c3c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a><span data-ttu-id="67c3c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67c3c-120">Request headers</span></span>
|<span data-ttu-id="67c3c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67c3c-121">Header</span></span>|<span data-ttu-id="67c3c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="67c3c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67c3c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="67c3c-123">Authorization</span></span>|<span data-ttu-id="67c3c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67c3c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67c3c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67c3c-125">Accept</span></span>|<span data-ttu-id="67c3c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67c3c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67c3c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67c3c-127">Request body</span></span>
<span data-ttu-id="67c3c-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)</span><span class="sxs-lookup"><span data-stu-id="67c3c-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

<span data-ttu-id="67c3c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span><span class="sxs-lookup"><span data-stu-id="67c3c-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>

|<span data-ttu-id="67c3c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67c3c-130">Property</span></span>|<span data-ttu-id="67c3c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="67c3c-131">Type</span></span>|<span data-ttu-id="67c3c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="67c3c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67c3c-133">id</span><span class="sxs-lookup"><span data-stu-id="67c3c-133">id</span></span>|<span data-ttu-id="67c3c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67c3c-134">String</span></span>|<span data-ttu-id="67c3c-135">Identificador exclusivo para o estado de saúde do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="67c3c-135">Unique Identifier for the Windows management app health state.</span></span> <span data-ttu-id="67c3c-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="67c3c-136">This property is read-only.</span></span>|
|<span data-ttu-id="67c3c-137">healthState</span><span class="sxs-lookup"><span data-stu-id="67c3c-137">healthState</span></span>|[<span data-ttu-id="67c3c-138">healthState</span><span class="sxs-lookup"><span data-stu-id="67c3c-138">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="67c3c-139">Estado de saúde do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="67c3c-139">Windows management app health state.</span></span> <span data-ttu-id="67c3c-140">Os valores possíveis são: `unknown`, `healthy`, `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="67c3c-140">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="67c3c-141">installedVersion</span><span class="sxs-lookup"><span data-stu-id="67c3c-141">installedVersion</span></span>|<span data-ttu-id="67c3c-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67c3c-142">String</span></span>|<span data-ttu-id="67c3c-143">Versão instalada do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="67c3c-143">Windows management app installed version.</span></span>|
|<span data-ttu-id="67c3c-144">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="67c3c-144">lastCheckInDateTime</span></span>|<span data-ttu-id="67c3c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67c3c-145">DateTimeOffset</span></span>|<span data-ttu-id="67c3c-146">Última hora de check-in do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="67c3c-146">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="67c3c-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="67c3c-147">deviceName</span></span>|<span data-ttu-id="67c3c-148">String</span><span class="sxs-lookup"><span data-stu-id="67c3c-148">String</span></span>|<span data-ttu-id="67c3c-149">Nome do dispositivo no qual o aplicativo de gerenciamento do Windows está instalado.</span><span class="sxs-lookup"><span data-stu-id="67c3c-149">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="67c3c-150">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="67c3c-150">deviceOSVersion</span></span>|<span data-ttu-id="67c3c-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67c3c-151">String</span></span>|<span data-ttu-id="67c3c-152">Versão do sistema operacional Windows 10 do dispositivo no qual o aplicativo de gerenciamento do Windows está instalado.</span><span class="sxs-lookup"><span data-stu-id="67c3c-152">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="67c3c-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="67c3c-153">Response</span></span>
<span data-ttu-id="67c3c-154">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67c3c-154">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67c3c-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67c3c-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="67c3c-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67c3c-156">Request</span></span>
<span data-ttu-id="67c3c-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67c3c-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="67c3c-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="67c3c-158">Response</span></span>
<span data-ttu-id="67c3c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67c3c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




