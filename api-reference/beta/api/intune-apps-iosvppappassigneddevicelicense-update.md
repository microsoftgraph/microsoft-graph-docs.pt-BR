---
title: Atualizar iosVppAppAssignedDeviceLicense
description: Atualiza as propriedades de um objeto iosVppAppAssignedDeviceLicense.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 83fabd3202391f5e466c5b5bd9af895ed82af0aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445523"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="f37ea-103">Atualizar iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="f37ea-103">Update iosVppAppAssignedDeviceLicense</span></span>

<span data-ttu-id="f37ea-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f37ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f37ea-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f37ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f37ea-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f37ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f37ea-107">Atualiza as propriedades de um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="f37ea-107">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f37ea-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f37ea-108">Prerequisites</span></span>
<span data-ttu-id="f37ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f37ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f37ea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f37ea-111">Permission type</span></span>|<span data-ttu-id="f37ea-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f37ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f37ea-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f37ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f37ea-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f37ea-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f37ea-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f37ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f37ea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f37ea-116">Not supported.</span></span>|
|<span data-ttu-id="f37ea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f37ea-117">Application</span></span>|<span data-ttu-id="f37ea-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f37ea-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f37ea-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f37ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="f37ea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f37ea-120">Request headers</span></span>
|<span data-ttu-id="f37ea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f37ea-121">Header</span></span>|<span data-ttu-id="f37ea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f37ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f37ea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f37ea-123">Authorization</span></span>|<span data-ttu-id="f37ea-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f37ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f37ea-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f37ea-125">Accept</span></span>|<span data-ttu-id="f37ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f37ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f37ea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f37ea-127">Request body</span></span>
<span data-ttu-id="f37ea-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="f37ea-128">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="f37ea-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span><span class="sxs-lookup"><span data-stu-id="f37ea-129">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="f37ea-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f37ea-130">Property</span></span>|<span data-ttu-id="f37ea-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f37ea-131">Type</span></span>|<span data-ttu-id="f37ea-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f37ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f37ea-133">id</span><span class="sxs-lookup"><span data-stu-id="f37ea-133">id</span></span>|<span data-ttu-id="f37ea-134">String</span><span class="sxs-lookup"><span data-stu-id="f37ea-134">String</span></span>|<span data-ttu-id="f37ea-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f37ea-135">Key of the entity.</span></span> <span data-ttu-id="f37ea-136">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f37ea-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f37ea-137">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="f37ea-137">userEmailAddress</span></span>|<span data-ttu-id="f37ea-138">String</span><span class="sxs-lookup"><span data-stu-id="f37ea-138">String</span></span>|<span data-ttu-id="f37ea-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="f37ea-139">The user email address.</span></span> <span data-ttu-id="f37ea-140">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f37ea-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f37ea-141">userId</span><span class="sxs-lookup"><span data-stu-id="f37ea-141">userId</span></span>|<span data-ttu-id="f37ea-142">String</span><span class="sxs-lookup"><span data-stu-id="f37ea-142">String</span></span>|<span data-ttu-id="f37ea-143">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="f37ea-143">The user ID.</span></span> <span data-ttu-id="f37ea-144">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f37ea-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f37ea-145">userName</span><span class="sxs-lookup"><span data-stu-id="f37ea-145">userName</span></span>|<span data-ttu-id="f37ea-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f37ea-146">String</span></span>|<span data-ttu-id="f37ea-147">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="f37ea-147">The user name.</span></span> <span data-ttu-id="f37ea-148">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f37ea-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f37ea-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f37ea-149">userPrincipalName</span></span>|<span data-ttu-id="f37ea-150">String</span><span class="sxs-lookup"><span data-stu-id="f37ea-150">String</span></span>|<span data-ttu-id="f37ea-151">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="f37ea-151">The user principal name.</span></span> <span data-ttu-id="f37ea-152">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f37ea-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f37ea-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="f37ea-153">managedDeviceId</span></span>|<span data-ttu-id="f37ea-154">String</span><span class="sxs-lookup"><span data-stu-id="f37ea-154">String</span></span>|<span data-ttu-id="f37ea-155">A ID do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="f37ea-155">The managed device ID.</span></span>|
|<span data-ttu-id="f37ea-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="f37ea-156">deviceName</span></span>|<span data-ttu-id="f37ea-157">String</span><span class="sxs-lookup"><span data-stu-id="f37ea-157">String</span></span>|<span data-ttu-id="f37ea-158">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f37ea-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="f37ea-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="f37ea-159">Response</span></span>
<span data-ttu-id="f37ea-160">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f37ea-160">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f37ea-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f37ea-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="f37ea-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f37ea-162">Request</span></span>
<span data-ttu-id="f37ea-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f37ea-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f37ea-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="f37ea-164">Response</span></span>
<span data-ttu-id="f37ea-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f37ea-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





