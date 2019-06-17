---
title: Atualizar windowsInformationProtectionDeviceRegistration
description: Atualiza as propriedades de um objeto windowsInformationProtectionDeviceRegistration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de29f6e511a21f4d59f45d66f6552771684dfaa1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984307"
---
# <a name="update-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="60232-103">Atualizar windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="60232-103">Update windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="60232-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="60232-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60232-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60232-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60232-106">Atualiza as propriedades de um objeto [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .</span><span class="sxs-lookup"><span data-stu-id="60232-106">Update the properties of a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60232-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60232-107">Prerequisites</span></span>
<span data-ttu-id="60232-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60232-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60232-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60232-110">Permission type</span></span>|<span data-ttu-id="60232-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="60232-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60232-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60232-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60232-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60232-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="60232-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60232-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60232-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60232-115">Not supported.</span></span>|
|<span data-ttu-id="60232-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60232-116">Application</span></span>|<span data-ttu-id="60232-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60232-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60232-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60232-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="60232-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60232-119">Request headers</span></span>
|<span data-ttu-id="60232-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60232-120">Header</span></span>|<span data-ttu-id="60232-121">Valor</span><span class="sxs-lookup"><span data-stu-id="60232-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60232-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="60232-122">Authorization</span></span>|<span data-ttu-id="60232-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60232-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60232-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60232-124">Accept</span></span>|<span data-ttu-id="60232-125">application/json</span><span class="sxs-lookup"><span data-stu-id="60232-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60232-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60232-126">Request body</span></span>
<span data-ttu-id="60232-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .</span><span class="sxs-lookup"><span data-stu-id="60232-127">In the request body, supply a JSON representation for the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

<span data-ttu-id="60232-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span><span class="sxs-lookup"><span data-stu-id="60232-128">The following table shows the properties that are required when you create the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span></span>

|<span data-ttu-id="60232-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60232-129">Property</span></span>|<span data-ttu-id="60232-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="60232-130">Type</span></span>|<span data-ttu-id="60232-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="60232-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60232-132">id</span><span class="sxs-lookup"><span data-stu-id="60232-132">id</span></span>|<span data-ttu-id="60232-133">String</span><span class="sxs-lookup"><span data-stu-id="60232-133">String</span></span>|<span data-ttu-id="60232-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="60232-134">Key of the entity.</span></span>|
|<span data-ttu-id="60232-135">userId</span><span class="sxs-lookup"><span data-stu-id="60232-135">userId</span></span>|<span data-ttu-id="60232-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60232-136">String</span></span>|<span data-ttu-id="60232-137">UserId associado a este registro de registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="60232-137">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="60232-138">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="60232-138">deviceRegistrationId</span></span>|<span data-ttu-id="60232-139">String</span><span class="sxs-lookup"><span data-stu-id="60232-139">String</span></span>|<span data-ttu-id="60232-140">Identificador de dispositivo para este registro de registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="60232-140">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="60232-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="60232-141">deviceName</span></span>|<span data-ttu-id="60232-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60232-142">String</span></span>|<span data-ttu-id="60232-143">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="60232-143">Device name.</span></span>|
|<span data-ttu-id="60232-144">deviceType</span><span class="sxs-lookup"><span data-stu-id="60232-144">deviceType</span></span>|<span data-ttu-id="60232-145">String</span><span class="sxs-lookup"><span data-stu-id="60232-145">String</span></span>|<span data-ttu-id="60232-146">Tipo de dispositivo, por exemplo, Windows laptop VS Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="60232-146">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="60232-147">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="60232-147">deviceMacAddress</span></span>|<span data-ttu-id="60232-148">String</span><span class="sxs-lookup"><span data-stu-id="60232-148">String</span></span>|<span data-ttu-id="60232-149">Endereço MAC do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="60232-149">Device Mac address.</span></span>|
|<span data-ttu-id="60232-150">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="60232-150">lastCheckInDateTime</span></span>|<span data-ttu-id="60232-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60232-151">DateTimeOffset</span></span>|<span data-ttu-id="60232-152">Hora da última verificação do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="60232-152">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="60232-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="60232-153">Response</span></span>
<span data-ttu-id="60232-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60232-154">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60232-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60232-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="60232-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60232-156">Request</span></span>
<span data-ttu-id="60232-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60232-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
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

### <a name="response"></a><span data-ttu-id="60232-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="60232-158">Response</span></span>
<span data-ttu-id="60232-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60232-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





