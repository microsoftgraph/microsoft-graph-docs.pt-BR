---
title: Criar iosVppAppAssignedDeviceLicense
description: Criar um novo objeto iosVppAppAssignedDeviceLicense.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3157c49f1ed9f0b05df9115a0370edf881a3ab3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172636"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="dc4e0-103">Criar iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="dc4e0-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="dc4e0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc4e0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc4e0-106">Criar um novo objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="dc4e0-106">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc4e0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc4e0-107">Prerequisites</span></span>
<span data-ttu-id="dc4e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dc4e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dc4e0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc4e0-110">Permission type</span></span>|<span data-ttu-id="dc4e0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dc4e0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc4e0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc4e0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc4e0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc4e0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dc4e0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc4e0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc4e0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-115">Not supported.</span></span>|
|<span data-ttu-id="dc4e0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc4e0-116">Application</span></span>|<span data-ttu-id="dc4e0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc4e0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc4e0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="dc4e0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc4e0-119">Request headers</span></span>
|<span data-ttu-id="dc4e0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc4e0-120">Header</span></span>|<span data-ttu-id="dc4e0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dc4e0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc4e0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc4e0-122">Authorization</span></span>|<span data-ttu-id="dc4e0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc4e0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc4e0-124">Accept</span></span>|<span data-ttu-id="dc4e0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dc4e0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc4e0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc4e0-126">Request body</span></span>
<span data-ttu-id="dc4e0-127">No corpo da solicitação, forneça uma representação JSON do objeto iosVppAppAssignedDeviceLicense.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-127">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="dc4e0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppAppAssignedDeviceLicense.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-128">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="dc4e0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc4e0-129">Property</span></span>|<span data-ttu-id="dc4e0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc4e0-130">Type</span></span>|<span data-ttu-id="dc4e0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc4e0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc4e0-132">id</span><span class="sxs-lookup"><span data-stu-id="dc4e0-132">id</span></span>|<span data-ttu-id="dc4e0-133">String</span><span class="sxs-lookup"><span data-stu-id="dc4e0-133">String</span></span>|<span data-ttu-id="dc4e0-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-134">Key of the entity.</span></span> <span data-ttu-id="dc4e0-135">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="dc4e0-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="dc4e0-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="dc4e0-136">userEmailAddress</span></span>|<span data-ttu-id="dc4e0-137">String</span><span class="sxs-lookup"><span data-stu-id="dc4e0-137">String</span></span>|<span data-ttu-id="dc4e0-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-138">The user email address.</span></span> <span data-ttu-id="dc4e0-139">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="dc4e0-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="dc4e0-140">userId</span><span class="sxs-lookup"><span data-stu-id="dc4e0-140">userId</span></span>|<span data-ttu-id="dc4e0-141">String</span><span class="sxs-lookup"><span data-stu-id="dc4e0-141">String</span></span>|<span data-ttu-id="dc4e0-142">A ID de usuário.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-142">The user ID.</span></span> <span data-ttu-id="dc4e0-143">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="dc4e0-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="dc4e0-144">userName</span><span class="sxs-lookup"><span data-stu-id="dc4e0-144">userName</span></span>|<span data-ttu-id="dc4e0-145">String</span><span class="sxs-lookup"><span data-stu-id="dc4e0-145">String</span></span>|<span data-ttu-id="dc4e0-146">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-146">The user name.</span></span> <span data-ttu-id="dc4e0-147">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="dc4e0-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="dc4e0-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dc4e0-148">userPrincipalName</span></span>|<span data-ttu-id="dc4e0-149">String</span><span class="sxs-lookup"><span data-stu-id="dc4e0-149">String</span></span>|<span data-ttu-id="dc4e0-150">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-150">The user principal name.</span></span> <span data-ttu-id="dc4e0-151">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="dc4e0-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="dc4e0-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="dc4e0-152">managedDeviceId</span></span>|<span data-ttu-id="dc4e0-153">String</span><span class="sxs-lookup"><span data-stu-id="dc4e0-153">String</span></span>|<span data-ttu-id="dc4e0-154">A ID do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-154">The managed device ID.</span></span>|
|<span data-ttu-id="dc4e0-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="dc4e0-155">deviceName</span></span>|<span data-ttu-id="dc4e0-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc4e0-156">String</span></span>|<span data-ttu-id="dc4e0-157">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-157">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="dc4e0-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc4e0-158">Response</span></span>
<span data-ttu-id="dc4e0-159">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-159">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc4e0-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc4e0-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc4e0-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc4e0-161">Request</span></span>
<span data-ttu-id="dc4e0-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
Content-type: application/json
Content-length: 327

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="dc4e0-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc4e0-163">Response</span></span>
<span data-ttu-id="dc4e0-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc4e0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 376

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
  "id": "bed943d0-43d0-bed9-d043-d9bed043d9be",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value"
}
```




