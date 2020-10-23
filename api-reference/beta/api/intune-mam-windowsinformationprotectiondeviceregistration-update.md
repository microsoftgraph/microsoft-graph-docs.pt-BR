---
title: Atualizar windowsInformationProtectionDeviceRegistration
description: Atualiza as propriedades de um objeto windowsInformationProtectionDeviceRegistration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e73c9664b0946e2c02d8f60ec95ae9832a7e3b3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694358"
---
# <a name="update-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="42581-103">Atualizar windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="42581-103">Update windowsInformationProtectionDeviceRegistration</span></span>

<span data-ttu-id="42581-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42581-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42581-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42581-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42581-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42581-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42581-107">Atualiza as propriedades de um objeto [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .</span><span class="sxs-lookup"><span data-stu-id="42581-107">Update the properties of a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42581-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42581-108">Prerequisites</span></span>
<span data-ttu-id="42581-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42581-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42581-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42581-111">Permission type</span></span>|<span data-ttu-id="42581-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42581-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42581-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42581-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42581-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42581-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="42581-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42581-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42581-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42581-116">Not supported.</span></span>|
|<span data-ttu-id="42581-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42581-117">Application</span></span>|<span data-ttu-id="42581-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42581-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42581-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42581-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="42581-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42581-120">Request headers</span></span>
|<span data-ttu-id="42581-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42581-121">Header</span></span>|<span data-ttu-id="42581-122">Valor</span><span class="sxs-lookup"><span data-stu-id="42581-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42581-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="42581-123">Authorization</span></span>|<span data-ttu-id="42581-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42581-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42581-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42581-125">Accept</span></span>|<span data-ttu-id="42581-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42581-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42581-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42581-127">Request body</span></span>
<span data-ttu-id="42581-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .</span><span class="sxs-lookup"><span data-stu-id="42581-128">In the request body, supply a JSON representation for the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

<span data-ttu-id="42581-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span><span class="sxs-lookup"><span data-stu-id="42581-129">The following table shows the properties that are required when you create the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span></span>

|<span data-ttu-id="42581-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42581-130">Property</span></span>|<span data-ttu-id="42581-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="42581-131">Type</span></span>|<span data-ttu-id="42581-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="42581-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42581-133">id</span><span class="sxs-lookup"><span data-stu-id="42581-133">id</span></span>|<span data-ttu-id="42581-134">String</span><span class="sxs-lookup"><span data-stu-id="42581-134">String</span></span>|<span data-ttu-id="42581-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="42581-135">Key of the entity.</span></span>|
|<span data-ttu-id="42581-136">userId</span><span class="sxs-lookup"><span data-stu-id="42581-136">userId</span></span>|<span data-ttu-id="42581-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42581-137">String</span></span>|<span data-ttu-id="42581-138">UserId associado a este registro de registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42581-138">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="42581-139">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="42581-139">deviceRegistrationId</span></span>|<span data-ttu-id="42581-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42581-140">String</span></span>|<span data-ttu-id="42581-141">Identificador de dispositivo para este registro de registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42581-141">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="42581-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="42581-142">deviceName</span></span>|<span data-ttu-id="42581-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42581-143">String</span></span>|<span data-ttu-id="42581-144">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42581-144">Device name.</span></span>|
|<span data-ttu-id="42581-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="42581-145">deviceType</span></span>|<span data-ttu-id="42581-146">String</span><span class="sxs-lookup"><span data-stu-id="42581-146">String</span></span>|<span data-ttu-id="42581-147">Tipo de dispositivo, por exemplo, Windows laptop VS Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="42581-147">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="42581-148">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="42581-148">deviceMacAddress</span></span>|<span data-ttu-id="42581-149">String</span><span class="sxs-lookup"><span data-stu-id="42581-149">String</span></span>|<span data-ttu-id="42581-150">Endereço MAC do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42581-150">Device Mac address.</span></span>|
|<span data-ttu-id="42581-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="42581-151">lastCheckInDateTime</span></span>|<span data-ttu-id="42581-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42581-152">DateTimeOffset</span></span>|<span data-ttu-id="42581-153">Hora da última verificação do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42581-153">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="42581-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="42581-154">Response</span></span>
<span data-ttu-id="42581-155">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42581-155">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42581-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42581-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="42581-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42581-157">Request</span></span>
<span data-ttu-id="42581-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42581-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="42581-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="42581-159">Response</span></span>
<span data-ttu-id="42581-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42581-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





