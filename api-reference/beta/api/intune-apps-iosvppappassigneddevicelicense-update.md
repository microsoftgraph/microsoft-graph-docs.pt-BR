---
title: Atualizar iosVppAppAssignedDeviceLicense
description: Atualiza as propriedades de um objeto iosVppAppAssignedDeviceLicense.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0eb6a7835ff280f0267824c6d838035a5bf8fa2d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173497"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="db880-103">Atualizar iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="db880-103">Update iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="db880-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="db880-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db880-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db880-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db880-106">Atualiza as propriedades de um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="db880-106">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db880-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="db880-107">Prerequisites</span></span>
<span data-ttu-id="db880-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db880-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db880-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db880-110">Permission type</span></span>|<span data-ttu-id="db880-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="db880-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db880-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db880-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db880-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db880-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="db880-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db880-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db880-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db880-115">Not supported.</span></span>|
|<span data-ttu-id="db880-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db880-116">Application</span></span>|<span data-ttu-id="db880-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db880-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db880-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db880-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="db880-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db880-119">Request headers</span></span>
|<span data-ttu-id="db880-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db880-120">Header</span></span>|<span data-ttu-id="db880-121">Valor</span><span class="sxs-lookup"><span data-stu-id="db880-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db880-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="db880-122">Authorization</span></span>|<span data-ttu-id="db880-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db880-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db880-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="db880-124">Accept</span></span>|<span data-ttu-id="db880-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db880-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db880-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db880-126">Request body</span></span>
<span data-ttu-id="db880-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="db880-127">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="db880-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span><span class="sxs-lookup"><span data-stu-id="db880-128">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="db880-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db880-129">Property</span></span>|<span data-ttu-id="db880-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="db880-130">Type</span></span>|<span data-ttu-id="db880-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="db880-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db880-132">id</span><span class="sxs-lookup"><span data-stu-id="db880-132">id</span></span>|<span data-ttu-id="db880-133">String</span><span class="sxs-lookup"><span data-stu-id="db880-133">String</span></span>|<span data-ttu-id="db880-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="db880-134">Key of the entity.</span></span> <span data-ttu-id="db880-135">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="db880-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="db880-136">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="db880-136">userEmailAddress</span></span>|<span data-ttu-id="db880-137">String</span><span class="sxs-lookup"><span data-stu-id="db880-137">String</span></span>|<span data-ttu-id="db880-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="db880-138">The user email address.</span></span> <span data-ttu-id="db880-139">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="db880-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="db880-140">userId</span><span class="sxs-lookup"><span data-stu-id="db880-140">userId</span></span>|<span data-ttu-id="db880-141">String</span><span class="sxs-lookup"><span data-stu-id="db880-141">String</span></span>|<span data-ttu-id="db880-142">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="db880-142">The user ID.</span></span> <span data-ttu-id="db880-143">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="db880-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="db880-144">userName</span><span class="sxs-lookup"><span data-stu-id="db880-144">userName</span></span>|<span data-ttu-id="db880-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db880-145">String</span></span>|<span data-ttu-id="db880-146">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="db880-146">The user name.</span></span> <span data-ttu-id="db880-147">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="db880-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="db880-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="db880-148">userPrincipalName</span></span>|<span data-ttu-id="db880-149">String</span><span class="sxs-lookup"><span data-stu-id="db880-149">String</span></span>|<span data-ttu-id="db880-150">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="db880-150">The user principal name.</span></span> <span data-ttu-id="db880-151">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="db880-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="db880-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="db880-152">managedDeviceId</span></span>|<span data-ttu-id="db880-153">String</span><span class="sxs-lookup"><span data-stu-id="db880-153">String</span></span>|<span data-ttu-id="db880-154">A ID do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="db880-154">The managed device ID.</span></span>|
|<span data-ttu-id="db880-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="db880-155">deviceName</span></span>|<span data-ttu-id="db880-156">String</span><span class="sxs-lookup"><span data-stu-id="db880-156">String</span></span>|<span data-ttu-id="db880-157">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db880-157">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="db880-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="db880-158">Response</span></span>
<span data-ttu-id="db880-159">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db880-159">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db880-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db880-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="db880-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db880-161">Request</span></span>
<span data-ttu-id="db880-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db880-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
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

### <a name="response"></a><span data-ttu-id="db880-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="db880-163">Response</span></span>
<span data-ttu-id="db880-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db880-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




