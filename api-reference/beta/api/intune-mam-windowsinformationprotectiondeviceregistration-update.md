---
title: Atualizar windowsInformationProtectionDeviceRegistration
description: Atualize as propriedades de um objeto windowsInformationProtectionDeviceRegistration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0652b9dbd0d81d8d4f02a418d36ff0555809c20e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135226"
---
# <a name="update-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="fbf87-103">Atualizar windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="fbf87-103">Update windowsInformationProtectionDeviceRegistration</span></span>

<span data-ttu-id="fbf87-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbf87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbf87-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fbf87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbf87-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fbf87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbf87-107">Atualize as propriedades de um [objeto windowsInformationProtectionDeviceRegistration.](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)</span><span class="sxs-lookup"><span data-stu-id="fbf87-107">Update the properties of a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbf87-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbf87-108">Prerequisites</span></span>
<span data-ttu-id="fbf87-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbf87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbf87-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbf87-111">Permission type</span></span>|<span data-ttu-id="fbf87-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fbf87-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbf87-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbf87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbf87-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbf87-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fbf87-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbf87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbf87-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbf87-116">Not supported.</span></span>|
|<span data-ttu-id="fbf87-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbf87-117">Application</span></span>|<span data-ttu-id="fbf87-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbf87-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbf87-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbf87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="fbf87-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbf87-120">Request headers</span></span>
|<span data-ttu-id="fbf87-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbf87-121">Header</span></span>|<span data-ttu-id="fbf87-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fbf87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbf87-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbf87-123">Authorization</span></span>|<span data-ttu-id="fbf87-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbf87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbf87-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fbf87-125">Accept</span></span>|<span data-ttu-id="fbf87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbf87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbf87-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbf87-127">Request body</span></span>
<span data-ttu-id="fbf87-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsInformationProtectionDeviceRegistration.](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)</span><span class="sxs-lookup"><span data-stu-id="fbf87-128">In the request body, supply a JSON representation for the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

<span data-ttu-id="fbf87-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span><span class="sxs-lookup"><span data-stu-id="fbf87-129">The following table shows the properties that are required when you create the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span></span>

|<span data-ttu-id="fbf87-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbf87-130">Property</span></span>|<span data-ttu-id="fbf87-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbf87-131">Type</span></span>|<span data-ttu-id="fbf87-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbf87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbf87-133">id</span><span class="sxs-lookup"><span data-stu-id="fbf87-133">id</span></span>|<span data-ttu-id="fbf87-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf87-134">String</span></span>|<span data-ttu-id="fbf87-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fbf87-135">Key of the entity.</span></span>|
|<span data-ttu-id="fbf87-136">userId</span><span class="sxs-lookup"><span data-stu-id="fbf87-136">userId</span></span>|<span data-ttu-id="fbf87-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf87-137">String</span></span>|<span data-ttu-id="fbf87-138">UserId associado a esse registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbf87-138">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="fbf87-139">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="fbf87-139">deviceRegistrationId</span></span>|<span data-ttu-id="fbf87-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf87-140">String</span></span>|<span data-ttu-id="fbf87-141">Identificador de dispositivo para esse registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbf87-141">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="fbf87-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="fbf87-142">deviceName</span></span>|<span data-ttu-id="fbf87-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf87-143">String</span></span>|<span data-ttu-id="fbf87-144">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbf87-144">Device name.</span></span>|
|<span data-ttu-id="fbf87-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="fbf87-145">deviceType</span></span>|<span data-ttu-id="fbf87-146">String</span><span class="sxs-lookup"><span data-stu-id="fbf87-146">String</span></span>|<span data-ttu-id="fbf87-147">Tipo de dispositivo, por exemplo, telefone windows laptop VS Windows.</span><span class="sxs-lookup"><span data-stu-id="fbf87-147">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="fbf87-148">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="fbf87-148">deviceMacAddress</span></span>|<span data-ttu-id="fbf87-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf87-149">String</span></span>|<span data-ttu-id="fbf87-150">Endereço do Device Mac.</span><span class="sxs-lookup"><span data-stu-id="fbf87-150">Device Mac address.</span></span>|
|<span data-ttu-id="fbf87-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="fbf87-151">lastCheckInDateTime</span></span>|<span data-ttu-id="fbf87-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbf87-152">DateTimeOffset</span></span>|<span data-ttu-id="fbf87-153">Última verificação na hora do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbf87-153">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="fbf87-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbf87-154">Response</span></span>
<span data-ttu-id="fbf87-155">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbf87-155">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbf87-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbf87-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbf87-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbf87-157">Request</span></span>
<span data-ttu-id="fbf87-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbf87-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fbf87-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbf87-159">Response</span></span>
<span data-ttu-id="fbf87-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbf87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




