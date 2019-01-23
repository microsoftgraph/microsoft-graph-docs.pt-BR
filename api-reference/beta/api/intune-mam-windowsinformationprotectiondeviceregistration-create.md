---
title: Criar windowsInformationProtectionDeviceRegistration
description: Crie um novo objeto de windowsInformationProtectionDeviceRegistration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ea5e3bac32e0511b54e08cb37063084f359e554a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428842"
---
# <a name="create-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="27178-103">Criar windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="27178-103">Create windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="27178-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="27178-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="27178-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="27178-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27178-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="27178-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27178-107">Crie um novo objeto de [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .</span><span class="sxs-lookup"><span data-stu-id="27178-107">Create a new [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27178-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27178-108">Prerequisites</span></span>
<span data-ttu-id="27178-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="27178-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="27178-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27178-111">Permission type</span></span>|<span data-ttu-id="27178-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27178-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27178-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27178-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27178-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27178-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="27178-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27178-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27178-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27178-116">Not supported.</span></span>|
|<span data-ttu-id="27178-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27178-117">Application</span></span>|<span data-ttu-id="27178-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27178-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27178-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27178-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="27178-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27178-120">Request headers</span></span>
|<span data-ttu-id="27178-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27178-121">Header</span></span>|<span data-ttu-id="27178-122">Valor</span><span class="sxs-lookup"><span data-stu-id="27178-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27178-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="27178-123">Authorization</span></span>|<span data-ttu-id="27178-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27178-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27178-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="27178-125">Accept</span></span>|<span data-ttu-id="27178-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27178-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27178-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27178-127">Request body</span></span>
<span data-ttu-id="27178-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsInformationProtectionDeviceRegistration.</span><span class="sxs-lookup"><span data-stu-id="27178-128">In the request body, supply a JSON representation for the windowsInformationProtectionDeviceRegistration object.</span></span>

<span data-ttu-id="27178-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsInformationProtectionDeviceRegistration.</span><span class="sxs-lookup"><span data-stu-id="27178-129">The following table shows the properties that are required when you create the windowsInformationProtectionDeviceRegistration.</span></span>

|<span data-ttu-id="27178-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27178-130">Property</span></span>|<span data-ttu-id="27178-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="27178-131">Type</span></span>|<span data-ttu-id="27178-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="27178-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27178-133">id</span><span class="sxs-lookup"><span data-stu-id="27178-133">id</span></span>|<span data-ttu-id="27178-134">String</span><span class="sxs-lookup"><span data-stu-id="27178-134">String</span></span>|<span data-ttu-id="27178-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="27178-135">Key of the entity.</span></span>|
|<span data-ttu-id="27178-136">userId</span><span class="sxs-lookup"><span data-stu-id="27178-136">userId</span></span>|<span data-ttu-id="27178-137">String</span><span class="sxs-lookup"><span data-stu-id="27178-137">String</span></span>|<span data-ttu-id="27178-138">ID do usuário associado a este registro de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27178-138">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="27178-139">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="27178-139">deviceRegistrationId</span></span>|<span data-ttu-id="27178-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27178-140">String</span></span>|<span data-ttu-id="27178-141">Identificador de dispositivo para este registro de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27178-141">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="27178-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="27178-142">deviceName</span></span>|<span data-ttu-id="27178-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27178-143">String</span></span>|<span data-ttu-id="27178-144">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27178-144">Device name.</span></span>|
|<span data-ttu-id="27178-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="27178-145">deviceType</span></span>|<span data-ttu-id="27178-146">String</span><span class="sxs-lookup"><span data-stu-id="27178-146">String</span></span>|<span data-ttu-id="27178-147">Tipo de dispositivo, por exemplo, Windows laptop VERSUS Windows phone.</span><span class="sxs-lookup"><span data-stu-id="27178-147">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="27178-148">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="27178-148">deviceMacAddress</span></span>|<span data-ttu-id="27178-149">String</span><span class="sxs-lookup"><span data-stu-id="27178-149">String</span></span>|<span data-ttu-id="27178-150">Endereço Mac de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27178-150">Device Mac address.</span></span>|
|<span data-ttu-id="27178-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="27178-151">lastCheckInDateTime</span></span>|<span data-ttu-id="27178-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27178-152">DateTimeOffset</span></span>|<span data-ttu-id="27178-153">Última hora de check-in do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27178-153">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="27178-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="27178-154">Response</span></span>
<span data-ttu-id="27178-155">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27178-155">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27178-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27178-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="27178-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27178-157">Request</span></span>
<span data-ttu-id="27178-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27178-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="27178-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="27178-159">Response</span></span>
<span data-ttu-id="27178-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27178-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




