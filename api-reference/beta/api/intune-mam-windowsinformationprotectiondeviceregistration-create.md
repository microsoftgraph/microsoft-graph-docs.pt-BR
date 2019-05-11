---
title: Criar windowsInformationProtectionDeviceRegistration
description: Criar um novo objeto windowsInformationProtectionDeviceRegistration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3fa83295e3c5dc53d5a1e94e498154be9381d8de
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33903015"
---
# <a name="create-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="22d6f-103">Criar windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="22d6f-103">Create windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="22d6f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22d6f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22d6f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22d6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22d6f-106">Criar um novo objeto [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .</span><span class="sxs-lookup"><span data-stu-id="22d6f-106">Create a new [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22d6f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22d6f-107">Prerequisites</span></span>
<span data-ttu-id="22d6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22d6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22d6f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22d6f-110">Permission type</span></span>|<span data-ttu-id="22d6f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22d6f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22d6f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22d6f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22d6f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22d6f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="22d6f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22d6f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22d6f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22d6f-115">Not supported.</span></span>|
|<span data-ttu-id="22d6f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22d6f-116">Application</span></span>|<span data-ttu-id="22d6f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22d6f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22d6f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22d6f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="22d6f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22d6f-119">Request headers</span></span>
|<span data-ttu-id="22d6f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22d6f-120">Header</span></span>|<span data-ttu-id="22d6f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="22d6f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22d6f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="22d6f-122">Authorization</span></span>|<span data-ttu-id="22d6f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22d6f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22d6f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22d6f-124">Accept</span></span>|<span data-ttu-id="22d6f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="22d6f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22d6f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22d6f-126">Request body</span></span>
<span data-ttu-id="22d6f-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionDeviceRegistration.</span><span class="sxs-lookup"><span data-stu-id="22d6f-127">In the request body, supply a JSON representation for the windowsInformationProtectionDeviceRegistration object.</span></span>

<span data-ttu-id="22d6f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionDeviceRegistration.</span><span class="sxs-lookup"><span data-stu-id="22d6f-128">The following table shows the properties that are required when you create the windowsInformationProtectionDeviceRegistration.</span></span>

|<span data-ttu-id="22d6f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22d6f-129">Property</span></span>|<span data-ttu-id="22d6f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="22d6f-130">Type</span></span>|<span data-ttu-id="22d6f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="22d6f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22d6f-132">id</span><span class="sxs-lookup"><span data-stu-id="22d6f-132">id</span></span>|<span data-ttu-id="22d6f-133">String</span><span class="sxs-lookup"><span data-stu-id="22d6f-133">String</span></span>|<span data-ttu-id="22d6f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="22d6f-134">Key of the entity.</span></span>|
|<span data-ttu-id="22d6f-135">userId</span><span class="sxs-lookup"><span data-stu-id="22d6f-135">userId</span></span>|<span data-ttu-id="22d6f-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22d6f-136">String</span></span>|<span data-ttu-id="22d6f-137">UserId associado a este registro de registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22d6f-137">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="22d6f-138">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="22d6f-138">deviceRegistrationId</span></span>|<span data-ttu-id="22d6f-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22d6f-139">String</span></span>|<span data-ttu-id="22d6f-140">Identificador de dispositivo para este registro de registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22d6f-140">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="22d6f-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="22d6f-141">deviceName</span></span>|<span data-ttu-id="22d6f-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22d6f-142">String</span></span>|<span data-ttu-id="22d6f-143">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22d6f-143">Device name.</span></span>|
|<span data-ttu-id="22d6f-144">deviceType</span><span class="sxs-lookup"><span data-stu-id="22d6f-144">deviceType</span></span>|<span data-ttu-id="22d6f-145">String</span><span class="sxs-lookup"><span data-stu-id="22d6f-145">String</span></span>|<span data-ttu-id="22d6f-146">Tipo de dispositivo, por exemplo, Windows laptop VS Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="22d6f-146">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="22d6f-147">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="22d6f-147">deviceMacAddress</span></span>|<span data-ttu-id="22d6f-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22d6f-148">String</span></span>|<span data-ttu-id="22d6f-149">Endereço MAC do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22d6f-149">Device Mac address.</span></span>|
|<span data-ttu-id="22d6f-150">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="22d6f-150">lastCheckInDateTime</span></span>|<span data-ttu-id="22d6f-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22d6f-151">DateTimeOffset</span></span>|<span data-ttu-id="22d6f-152">Hora da última verificação do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22d6f-152">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="22d6f-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="22d6f-153">Response</span></span>
<span data-ttu-id="22d6f-154">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22d6f-154">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22d6f-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22d6f-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="22d6f-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22d6f-156">Request</span></span>
<span data-ttu-id="22d6f-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22d6f-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations
Content-type: application/json
Content-length: 366

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "userId": "User Id value",
  "deviceRegistrationId": "Device Registration Id value",
  "deviceName": "Device Name value",
  "deviceType": "Device Type value",
  "deviceMacAddress": "Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```

### <a name="response"></a><span data-ttu-id="22d6f-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="22d6f-158">Response</span></span>
<span data-ttu-id="22d6f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22d6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 415

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "id": "dd72e2c8-e2c8-dd72-c8e2-72ddc8e272dd",
  "userId": "User Id value",
  "deviceRegistrationId": "Device Registration Id value",
  "deviceName": "Device Name value",
  "deviceType": "Device Type value",
  "deviceMacAddress": "Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```




