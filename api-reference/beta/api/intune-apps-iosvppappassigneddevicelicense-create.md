---
title: Criar iosVppAppAssignedDeviceLicense
description: Criar um novo objeto iosVppAppAssignedDeviceLicense.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f65c2ec57dddbab87ba54302f14b0bca72cc5b5
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33936494"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="74e20-103">Criar iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="74e20-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="74e20-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="74e20-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74e20-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="74e20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74e20-106">Criar um novo objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="74e20-106">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74e20-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="74e20-107">Prerequisites</span></span>
<span data-ttu-id="74e20-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74e20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74e20-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74e20-110">Permission type</span></span>|<span data-ttu-id="74e20-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="74e20-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74e20-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74e20-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74e20-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74e20-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="74e20-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74e20-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74e20-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74e20-115">Not supported.</span></span>|
|<span data-ttu-id="74e20-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74e20-116">Application</span></span>|<span data-ttu-id="74e20-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74e20-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74e20-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74e20-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="74e20-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74e20-119">Request headers</span></span>
|<span data-ttu-id="74e20-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74e20-120">Header</span></span>|<span data-ttu-id="74e20-121">Valor</span><span class="sxs-lookup"><span data-stu-id="74e20-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74e20-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="74e20-122">Authorization</span></span>|<span data-ttu-id="74e20-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74e20-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74e20-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="74e20-124">Accept</span></span>|<span data-ttu-id="74e20-125">application/json</span><span class="sxs-lookup"><span data-stu-id="74e20-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74e20-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74e20-126">Request body</span></span>
<span data-ttu-id="74e20-127">No corpo da solicitação, forneça uma representação JSON do objeto iosVppAppAssignedDeviceLicense.</span><span class="sxs-lookup"><span data-stu-id="74e20-127">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="74e20-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppAppAssignedDeviceLicense.</span><span class="sxs-lookup"><span data-stu-id="74e20-128">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="74e20-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74e20-129">Property</span></span>|<span data-ttu-id="74e20-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="74e20-130">Type</span></span>|<span data-ttu-id="74e20-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="74e20-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74e20-132">id</span><span class="sxs-lookup"><span data-stu-id="74e20-132">id</span></span>|<span data-ttu-id="74e20-133">String</span><span class="sxs-lookup"><span data-stu-id="74e20-133">String</span></span>|<span data-ttu-id="74e20-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="74e20-134">Key of the entity.</span></span> <span data-ttu-id="74e20-135">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="74e20-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="74e20-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="74e20-136">userEmailAddress</span></span>|<span data-ttu-id="74e20-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74e20-137">String</span></span>|<span data-ttu-id="74e20-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="74e20-138">The user email address.</span></span> <span data-ttu-id="74e20-139">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="74e20-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="74e20-140">userId</span><span class="sxs-lookup"><span data-stu-id="74e20-140">userId</span></span>|<span data-ttu-id="74e20-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74e20-141">String</span></span>|<span data-ttu-id="74e20-142">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="74e20-142">The user ID.</span></span> <span data-ttu-id="74e20-143">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="74e20-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="74e20-144">userName</span><span class="sxs-lookup"><span data-stu-id="74e20-144">userName</span></span>|<span data-ttu-id="74e20-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74e20-145">String</span></span>|<span data-ttu-id="74e20-146">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="74e20-146">The user name.</span></span> <span data-ttu-id="74e20-147">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="74e20-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="74e20-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="74e20-148">userPrincipalName</span></span>|<span data-ttu-id="74e20-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74e20-149">String</span></span>|<span data-ttu-id="74e20-150">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="74e20-150">The user principal name.</span></span> <span data-ttu-id="74e20-151">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="74e20-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="74e20-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="74e20-152">managedDeviceId</span></span>|<span data-ttu-id="74e20-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74e20-153">String</span></span>|<span data-ttu-id="74e20-154">A ID do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="74e20-154">The managed device ID.</span></span>|
|<span data-ttu-id="74e20-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="74e20-155">deviceName</span></span>|<span data-ttu-id="74e20-156">String</span><span class="sxs-lookup"><span data-stu-id="74e20-156">String</span></span>|<span data-ttu-id="74e20-157">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="74e20-157">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="74e20-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="74e20-158">Response</span></span>
<span data-ttu-id="74e20-159">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74e20-159">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74e20-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74e20-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="74e20-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74e20-161">Request</span></span>
<span data-ttu-id="74e20-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74e20-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="74e20-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="74e20-163">Response</span></span>
<span data-ttu-id="74e20-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74e20-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




