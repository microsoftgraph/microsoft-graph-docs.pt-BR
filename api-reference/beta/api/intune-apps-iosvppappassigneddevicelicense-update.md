---
title: Atualizar iosVppAppAssignedDeviceLicense
description: Atualiza as propriedades de um objeto iosVppAppAssignedDeviceLicense.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 50de14fa5080c41e1636fc385fef057ef6aacac3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981192"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="f8210-103">Atualizar iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="f8210-103">Update iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="f8210-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8210-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8210-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8210-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8210-106">Atualiza as propriedades de um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="f8210-106">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8210-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8210-107">Prerequisites</span></span>
<span data-ttu-id="f8210-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8210-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8210-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8210-110">Permission type</span></span>|<span data-ttu-id="f8210-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8210-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8210-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8210-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8210-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8210-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f8210-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8210-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8210-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8210-115">Not supported.</span></span>|
|<span data-ttu-id="f8210-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8210-116">Application</span></span>|<span data-ttu-id="f8210-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8210-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8210-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8210-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="f8210-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8210-119">Request headers</span></span>
|<span data-ttu-id="f8210-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8210-120">Header</span></span>|<span data-ttu-id="f8210-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f8210-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8210-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8210-122">Authorization</span></span>|<span data-ttu-id="f8210-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8210-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8210-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8210-124">Accept</span></span>|<span data-ttu-id="f8210-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8210-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8210-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8210-126">Request body</span></span>
<span data-ttu-id="f8210-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="f8210-127">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="f8210-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span><span class="sxs-lookup"><span data-stu-id="f8210-128">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="f8210-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8210-129">Property</span></span>|<span data-ttu-id="f8210-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8210-130">Type</span></span>|<span data-ttu-id="f8210-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8210-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8210-132">id</span><span class="sxs-lookup"><span data-stu-id="f8210-132">id</span></span>|<span data-ttu-id="f8210-133">String</span><span class="sxs-lookup"><span data-stu-id="f8210-133">String</span></span>|<span data-ttu-id="f8210-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f8210-134">Key of the entity.</span></span> <span data-ttu-id="f8210-135">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f8210-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f8210-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="f8210-136">userEmailAddress</span></span>|<span data-ttu-id="f8210-137">String</span><span class="sxs-lookup"><span data-stu-id="f8210-137">String</span></span>|<span data-ttu-id="f8210-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="f8210-138">The user email address.</span></span> <span data-ttu-id="f8210-139">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f8210-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f8210-140">userId</span><span class="sxs-lookup"><span data-stu-id="f8210-140">userId</span></span>|<span data-ttu-id="f8210-141">String</span><span class="sxs-lookup"><span data-stu-id="f8210-141">String</span></span>|<span data-ttu-id="f8210-142">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="f8210-142">The user ID.</span></span> <span data-ttu-id="f8210-143">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f8210-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f8210-144">userName</span><span class="sxs-lookup"><span data-stu-id="f8210-144">userName</span></span>|<span data-ttu-id="f8210-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8210-145">String</span></span>|<span data-ttu-id="f8210-146">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="f8210-146">The user name.</span></span> <span data-ttu-id="f8210-147">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f8210-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f8210-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f8210-148">userPrincipalName</span></span>|<span data-ttu-id="f8210-149">String</span><span class="sxs-lookup"><span data-stu-id="f8210-149">String</span></span>|<span data-ttu-id="f8210-150">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="f8210-150">The user principal name.</span></span> <span data-ttu-id="f8210-151">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f8210-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f8210-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="f8210-152">managedDeviceId</span></span>|<span data-ttu-id="f8210-153">String</span><span class="sxs-lookup"><span data-stu-id="f8210-153">String</span></span>|<span data-ttu-id="f8210-154">A ID do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="f8210-154">The managed device ID.</span></span>|
|<span data-ttu-id="f8210-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="f8210-155">deviceName</span></span>|<span data-ttu-id="f8210-156">String</span><span class="sxs-lookup"><span data-stu-id="f8210-156">String</span></span>|<span data-ttu-id="f8210-157">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8210-157">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="f8210-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8210-158">Response</span></span>
<span data-ttu-id="f8210-159">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8210-159">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8210-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8210-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8210-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8210-161">Request</span></span>
<span data-ttu-id="f8210-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8210-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f8210-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8210-163">Response</span></span>
<span data-ttu-id="f8210-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8210-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




