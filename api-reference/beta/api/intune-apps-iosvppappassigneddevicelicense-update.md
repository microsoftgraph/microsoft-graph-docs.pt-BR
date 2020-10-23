---
title: Atualizar iosVppAppAssignedDeviceLicense
description: Atualiza as propriedades de um objeto iosVppAppAssignedDeviceLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d15b33df38c21127f7e745a7c6cd11f09b6fa0bd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700084"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="74dc7-103">Atualizar iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="74dc7-103">Update iosVppAppAssignedDeviceLicense</span></span>

<span data-ttu-id="74dc7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74dc7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74dc7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="74dc7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74dc7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="74dc7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74dc7-107">Atualiza as propriedades de um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="74dc7-107">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74dc7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="74dc7-108">Prerequisites</span></span>
<span data-ttu-id="74dc7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74dc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74dc7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74dc7-111">Permission type</span></span>|<span data-ttu-id="74dc7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="74dc7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74dc7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74dc7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74dc7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74dc7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="74dc7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74dc7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74dc7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74dc7-116">Not supported.</span></span>|
|<span data-ttu-id="74dc7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74dc7-117">Application</span></span>|<span data-ttu-id="74dc7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74dc7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74dc7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74dc7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="74dc7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74dc7-120">Request headers</span></span>
|<span data-ttu-id="74dc7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74dc7-121">Header</span></span>|<span data-ttu-id="74dc7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="74dc7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74dc7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="74dc7-123">Authorization</span></span>|<span data-ttu-id="74dc7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74dc7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74dc7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="74dc7-125">Accept</span></span>|<span data-ttu-id="74dc7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74dc7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74dc7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74dc7-127">Request body</span></span>
<span data-ttu-id="74dc7-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="74dc7-128">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="74dc7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span><span class="sxs-lookup"><span data-stu-id="74dc7-129">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="74dc7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74dc7-130">Property</span></span>|<span data-ttu-id="74dc7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="74dc7-131">Type</span></span>|<span data-ttu-id="74dc7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="74dc7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74dc7-133">id</span><span class="sxs-lookup"><span data-stu-id="74dc7-133">id</span></span>|<span data-ttu-id="74dc7-134">String</span><span class="sxs-lookup"><span data-stu-id="74dc7-134">String</span></span>|<span data-ttu-id="74dc7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="74dc7-135">Key of the entity.</span></span> <span data-ttu-id="74dc7-136">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="74dc7-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="74dc7-137">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="74dc7-137">userEmailAddress</span></span>|<span data-ttu-id="74dc7-138">String</span><span class="sxs-lookup"><span data-stu-id="74dc7-138">String</span></span>|<span data-ttu-id="74dc7-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="74dc7-139">The user email address.</span></span> <span data-ttu-id="74dc7-140">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="74dc7-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="74dc7-141">userId</span><span class="sxs-lookup"><span data-stu-id="74dc7-141">userId</span></span>|<span data-ttu-id="74dc7-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74dc7-142">String</span></span>|<span data-ttu-id="74dc7-143">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="74dc7-143">The user ID.</span></span> <span data-ttu-id="74dc7-144">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="74dc7-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="74dc7-145">userName</span><span class="sxs-lookup"><span data-stu-id="74dc7-145">userName</span></span>|<span data-ttu-id="74dc7-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74dc7-146">String</span></span>|<span data-ttu-id="74dc7-147">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="74dc7-147">The user name.</span></span> <span data-ttu-id="74dc7-148">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="74dc7-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="74dc7-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="74dc7-149">userPrincipalName</span></span>|<span data-ttu-id="74dc7-150">String</span><span class="sxs-lookup"><span data-stu-id="74dc7-150">String</span></span>|<span data-ttu-id="74dc7-151">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="74dc7-151">The user principal name.</span></span> <span data-ttu-id="74dc7-152">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="74dc7-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="74dc7-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="74dc7-153">managedDeviceId</span></span>|<span data-ttu-id="74dc7-154">String</span><span class="sxs-lookup"><span data-stu-id="74dc7-154">String</span></span>|<span data-ttu-id="74dc7-155">A ID do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="74dc7-155">The managed device ID.</span></span>|
|<span data-ttu-id="74dc7-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="74dc7-156">deviceName</span></span>|<span data-ttu-id="74dc7-157">String</span><span class="sxs-lookup"><span data-stu-id="74dc7-157">String</span></span>|<span data-ttu-id="74dc7-158">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="74dc7-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="74dc7-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="74dc7-159">Response</span></span>
<span data-ttu-id="74dc7-160">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74dc7-160">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74dc7-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74dc7-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="74dc7-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74dc7-162">Request</span></span>
<span data-ttu-id="74dc7-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74dc7-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="74dc7-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="74dc7-164">Response</span></span>
<span data-ttu-id="74dc7-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74dc7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





