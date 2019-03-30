---
title: Criar iosVppAppAssignedDeviceLicense
description: Criar um novo objeto iosVppAppAssignedDeviceLicense.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42109f11ffb01fa90b5ecde9e7952d4113fb23ba
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972904"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="21197-103">Criar iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="21197-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="21197-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21197-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21197-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21197-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21197-106">Criar um novo objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="21197-106">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21197-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21197-107">Prerequisites</span></span>
<span data-ttu-id="21197-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21197-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21197-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21197-110">Permission type</span></span>|<span data-ttu-id="21197-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21197-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21197-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21197-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21197-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21197-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="21197-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21197-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21197-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21197-115">Not supported.</span></span>|
|<span data-ttu-id="21197-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21197-116">Application</span></span>|<span data-ttu-id="21197-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21197-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21197-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21197-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="21197-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21197-119">Request headers</span></span>
|<span data-ttu-id="21197-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21197-120">Header</span></span>|<span data-ttu-id="21197-121">Valor</span><span class="sxs-lookup"><span data-stu-id="21197-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21197-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="21197-122">Authorization</span></span>|<span data-ttu-id="21197-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21197-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21197-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21197-124">Accept</span></span>|<span data-ttu-id="21197-125">application/json</span><span class="sxs-lookup"><span data-stu-id="21197-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21197-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21197-126">Request body</span></span>
<span data-ttu-id="21197-127">No corpo da solicitação, forneça uma representação JSON do objeto iosVppAppAssignedDeviceLicense.</span><span class="sxs-lookup"><span data-stu-id="21197-127">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="21197-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppAppAssignedDeviceLicense.</span><span class="sxs-lookup"><span data-stu-id="21197-128">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="21197-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21197-129">Property</span></span>|<span data-ttu-id="21197-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="21197-130">Type</span></span>|<span data-ttu-id="21197-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="21197-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21197-132">id</span><span class="sxs-lookup"><span data-stu-id="21197-132">id</span></span>|<span data-ttu-id="21197-133">String</span><span class="sxs-lookup"><span data-stu-id="21197-133">String</span></span>|<span data-ttu-id="21197-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="21197-134">Key of the entity.</span></span> <span data-ttu-id="21197-135">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="21197-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="21197-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="21197-136">userEmailAddress</span></span>|<span data-ttu-id="21197-137">String</span><span class="sxs-lookup"><span data-stu-id="21197-137">String</span></span>|<span data-ttu-id="21197-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="21197-138">The user email address.</span></span> <span data-ttu-id="21197-139">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="21197-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="21197-140">userId</span><span class="sxs-lookup"><span data-stu-id="21197-140">userId</span></span>|<span data-ttu-id="21197-141">String</span><span class="sxs-lookup"><span data-stu-id="21197-141">String</span></span>|<span data-ttu-id="21197-142">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="21197-142">The user ID.</span></span> <span data-ttu-id="21197-143">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="21197-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="21197-144">userName</span><span class="sxs-lookup"><span data-stu-id="21197-144">userName</span></span>|<span data-ttu-id="21197-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21197-145">String</span></span>|<span data-ttu-id="21197-146">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="21197-146">The user name.</span></span> <span data-ttu-id="21197-147">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="21197-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="21197-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="21197-148">userPrincipalName</span></span>|<span data-ttu-id="21197-149">String</span><span class="sxs-lookup"><span data-stu-id="21197-149">String</span></span>|<span data-ttu-id="21197-150">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="21197-150">The user principal name.</span></span> <span data-ttu-id="21197-151">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="21197-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="21197-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="21197-152">managedDeviceId</span></span>|<span data-ttu-id="21197-153">String</span><span class="sxs-lookup"><span data-stu-id="21197-153">String</span></span>|<span data-ttu-id="21197-154">A ID do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="21197-154">The managed device ID.</span></span>|
|<span data-ttu-id="21197-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="21197-155">deviceName</span></span>|<span data-ttu-id="21197-156">String</span><span class="sxs-lookup"><span data-stu-id="21197-156">String</span></span>|<span data-ttu-id="21197-157">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21197-157">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="21197-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="21197-158">Response</span></span>
<span data-ttu-id="21197-159">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21197-159">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21197-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21197-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="21197-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21197-161">Request</span></span>
<span data-ttu-id="21197-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21197-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="21197-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="21197-163">Response</span></span>
<span data-ttu-id="21197-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21197-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




