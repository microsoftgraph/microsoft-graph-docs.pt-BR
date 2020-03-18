---
title: Criar windowsInformationProtectionDeviceRegistration
description: Criar um novo objeto windowsInformationProtectionDeviceRegistration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a8db315c9e910babd8f05c78080080c952d5b022
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803299"
---
# <a name="create-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="dc3d7-103">Criar windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="dc3d7-103">Create windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="dc3d7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc3d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc3d7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc3d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc3d7-106">Criar um novo objeto [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .</span><span class="sxs-lookup"><span data-stu-id="dc3d7-106">Create a new [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc3d7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc3d7-107">Prerequisites</span></span>
<span data-ttu-id="dc3d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc3d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc3d7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc3d7-110">Permission type</span></span>|<span data-ttu-id="dc3d7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dc3d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc3d7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc3d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc3d7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc3d7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dc3d7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc3d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc3d7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc3d7-115">Not supported.</span></span>|
|<span data-ttu-id="dc3d7-116">Application</span><span class="sxs-lookup"><span data-stu-id="dc3d7-116">Application</span></span>|<span data-ttu-id="dc3d7-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc3d7-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc3d7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc3d7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="dc3d7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc3d7-119">Request headers</span></span>
|<span data-ttu-id="dc3d7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc3d7-120">Header</span></span>|<span data-ttu-id="dc3d7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dc3d7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc3d7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc3d7-122">Authorization</span></span>|<span data-ttu-id="dc3d7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc3d7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc3d7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc3d7-124">Accept</span></span>|<span data-ttu-id="dc3d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dc3d7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc3d7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc3d7-126">Request body</span></span>
<span data-ttu-id="dc3d7-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionDeviceRegistration.</span><span class="sxs-lookup"><span data-stu-id="dc3d7-127">In the request body, supply a JSON representation for the windowsInformationProtectionDeviceRegistration object.</span></span>

<span data-ttu-id="dc3d7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionDeviceRegistration.</span><span class="sxs-lookup"><span data-stu-id="dc3d7-128">The following table shows the properties that are required when you create the windowsInformationProtectionDeviceRegistration.</span></span>

|<span data-ttu-id="dc3d7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc3d7-129">Property</span></span>|<span data-ttu-id="dc3d7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc3d7-130">Type</span></span>|<span data-ttu-id="dc3d7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc3d7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc3d7-132">id</span><span class="sxs-lookup"><span data-stu-id="dc3d7-132">id</span></span>|<span data-ttu-id="dc3d7-133">String</span><span class="sxs-lookup"><span data-stu-id="dc3d7-133">String</span></span>|<span data-ttu-id="dc3d7-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dc3d7-134">Key of the entity.</span></span>|
|<span data-ttu-id="dc3d7-135">userId</span><span class="sxs-lookup"><span data-stu-id="dc3d7-135">userId</span></span>|<span data-ttu-id="dc3d7-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc3d7-136">String</span></span>|<span data-ttu-id="dc3d7-137">UserId associado a este registro de registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dc3d7-137">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="dc3d7-138">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="dc3d7-138">deviceRegistrationId</span></span>|<span data-ttu-id="dc3d7-139">String</span><span class="sxs-lookup"><span data-stu-id="dc3d7-139">String</span></span>|<span data-ttu-id="dc3d7-140">Identificador de dispositivo para este registro de registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dc3d7-140">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="dc3d7-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="dc3d7-141">deviceName</span></span>|<span data-ttu-id="dc3d7-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc3d7-142">String</span></span>|<span data-ttu-id="dc3d7-143">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dc3d7-143">Device name.</span></span>|
|<span data-ttu-id="dc3d7-144">deviceType</span><span class="sxs-lookup"><span data-stu-id="dc3d7-144">deviceType</span></span>|<span data-ttu-id="dc3d7-145">String</span><span class="sxs-lookup"><span data-stu-id="dc3d7-145">String</span></span>|<span data-ttu-id="dc3d7-146">Tipo de dispositivo, por exemplo, Windows laptop VS Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="dc3d7-146">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="dc3d7-147">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="dc3d7-147">deviceMacAddress</span></span>|<span data-ttu-id="dc3d7-148">String</span><span class="sxs-lookup"><span data-stu-id="dc3d7-148">String</span></span>|<span data-ttu-id="dc3d7-149">Endereço MAC do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dc3d7-149">Device Mac address.</span></span>|
|<span data-ttu-id="dc3d7-150">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="dc3d7-150">lastCheckInDateTime</span></span>|<span data-ttu-id="dc3d7-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc3d7-151">DateTimeOffset</span></span>|<span data-ttu-id="dc3d7-152">Hora da última verificação do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dc3d7-152">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="dc3d7-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc3d7-153">Response</span></span>
<span data-ttu-id="dc3d7-154">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc3d7-154">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc3d7-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc3d7-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc3d7-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc3d7-156">Request</span></span>
<span data-ttu-id="dc3d7-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc3d7-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dc3d7-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc3d7-158">Response</span></span>
<span data-ttu-id="dc3d7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc3d7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




