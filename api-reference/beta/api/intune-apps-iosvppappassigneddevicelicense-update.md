---
title: Atualizar iosVppAppAssignedDeviceLicense
description: Atualiza as propriedades de um objeto iosVppAppAssignedDeviceLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd87a37eb6679799f5ab74007c8c455c258a2c77
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49252015"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="f2fa9-103">Atualizar iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="f2fa9-103">Update iosVppAppAssignedDeviceLicense</span></span>

<span data-ttu-id="f2fa9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2fa9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2fa9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2fa9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2fa9-107">Atualiza as propriedades de um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="f2fa9-107">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2fa9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2fa9-108">Prerequisites</span></span>
<span data-ttu-id="f2fa9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2fa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2fa9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2fa9-111">Permission type</span></span>|<span data-ttu-id="f2fa9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2fa9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2fa9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2fa9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2fa9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2fa9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2fa9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2fa9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2fa9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-116">Not supported.</span></span>|
|<span data-ttu-id="f2fa9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2fa9-117">Application</span></span>|<span data-ttu-id="f2fa9-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2fa9-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2fa9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2fa9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="f2fa9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2fa9-120">Request headers</span></span>
|<span data-ttu-id="f2fa9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2fa9-121">Header</span></span>|<span data-ttu-id="f2fa9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f2fa9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2fa9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2fa9-123">Authorization</span></span>|<span data-ttu-id="f2fa9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2fa9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2fa9-125">Accept</span></span>|<span data-ttu-id="f2fa9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2fa9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2fa9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2fa9-127">Request body</span></span>
<span data-ttu-id="f2fa9-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="f2fa9-128">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="f2fa9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span><span class="sxs-lookup"><span data-stu-id="f2fa9-129">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="f2fa9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2fa9-130">Property</span></span>|<span data-ttu-id="f2fa9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2fa9-131">Type</span></span>|<span data-ttu-id="f2fa9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2fa9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2fa9-133">id</span><span class="sxs-lookup"><span data-stu-id="f2fa9-133">id</span></span>|<span data-ttu-id="f2fa9-134">String</span><span class="sxs-lookup"><span data-stu-id="f2fa9-134">String</span></span>|<span data-ttu-id="f2fa9-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-135">Key of the entity.</span></span> <span data-ttu-id="f2fa9-136">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f2fa9-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f2fa9-137">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="f2fa9-137">userEmailAddress</span></span>|<span data-ttu-id="f2fa9-138">String</span><span class="sxs-lookup"><span data-stu-id="f2fa9-138">String</span></span>|<span data-ttu-id="f2fa9-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-139">The user email address.</span></span> <span data-ttu-id="f2fa9-140">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f2fa9-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f2fa9-141">userId</span><span class="sxs-lookup"><span data-stu-id="f2fa9-141">userId</span></span>|<span data-ttu-id="f2fa9-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2fa9-142">String</span></span>|<span data-ttu-id="f2fa9-143">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-143">The user ID.</span></span> <span data-ttu-id="f2fa9-144">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f2fa9-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f2fa9-145">userName</span><span class="sxs-lookup"><span data-stu-id="f2fa9-145">userName</span></span>|<span data-ttu-id="f2fa9-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2fa9-146">String</span></span>|<span data-ttu-id="f2fa9-147">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-147">The user name.</span></span> <span data-ttu-id="f2fa9-148">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f2fa9-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f2fa9-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f2fa9-149">userPrincipalName</span></span>|<span data-ttu-id="f2fa9-150">String</span><span class="sxs-lookup"><span data-stu-id="f2fa9-150">String</span></span>|<span data-ttu-id="f2fa9-151">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-151">The user principal name.</span></span> <span data-ttu-id="f2fa9-152">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f2fa9-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f2fa9-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="f2fa9-153">managedDeviceId</span></span>|<span data-ttu-id="f2fa9-154">String</span><span class="sxs-lookup"><span data-stu-id="f2fa9-154">String</span></span>|<span data-ttu-id="f2fa9-155">A ID do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-155">The managed device ID.</span></span>|
|<span data-ttu-id="f2fa9-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="f2fa9-156">deviceName</span></span>|<span data-ttu-id="f2fa9-157">String</span><span class="sxs-lookup"><span data-stu-id="f2fa9-157">String</span></span>|<span data-ttu-id="f2fa9-158">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="f2fa9-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2fa9-159">Response</span></span>
<span data-ttu-id="f2fa9-160">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-160">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2fa9-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2fa9-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2fa9-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2fa9-162">Request</span></span>
<span data-ttu-id="f2fa9-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f2fa9-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2fa9-164">Response</span></span>
<span data-ttu-id="f2fa9-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




