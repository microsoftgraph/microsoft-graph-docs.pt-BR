---
title: Criar iosVppAppAssignedDeviceLicense
description: Crie um novo objeto iosVppAppAssignedDeviceLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b6ea8cf269a3b5735a366000fb49fd8479eebef2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140635"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="67de3-103">Criar iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="67de3-103">Create iosVppAppAssignedDeviceLicense</span></span>

<span data-ttu-id="67de3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67de3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67de3-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67de3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67de3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67de3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67de3-107">Crie um novo [objeto iosVppAppAssignedDeviceLicense.](../resources/intune-apps-iosvppappassigneddevicelicense.md)</span><span class="sxs-lookup"><span data-stu-id="67de3-107">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67de3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67de3-108">Prerequisites</span></span>
<span data-ttu-id="67de3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67de3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67de3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67de3-111">Permission type</span></span>|<span data-ttu-id="67de3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67de3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67de3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67de3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67de3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67de3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="67de3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67de3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67de3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67de3-116">Not supported.</span></span>|
|<span data-ttu-id="67de3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67de3-117">Application</span></span>|<span data-ttu-id="67de3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67de3-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67de3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67de3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="67de3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67de3-120">Request headers</span></span>
|<span data-ttu-id="67de3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67de3-121">Header</span></span>|<span data-ttu-id="67de3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="67de3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67de3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="67de3-123">Authorization</span></span>|<span data-ttu-id="67de3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67de3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67de3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67de3-125">Accept</span></span>|<span data-ttu-id="67de3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67de3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67de3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67de3-127">Request body</span></span>
<span data-ttu-id="67de3-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosVppAppAssignedDeviceLicense.</span><span class="sxs-lookup"><span data-stu-id="67de3-128">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="67de3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o iosVppAppAssignedDeviceLicense.</span><span class="sxs-lookup"><span data-stu-id="67de3-129">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="67de3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67de3-130">Property</span></span>|<span data-ttu-id="67de3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="67de3-131">Type</span></span>|<span data-ttu-id="67de3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="67de3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67de3-133">id</span><span class="sxs-lookup"><span data-stu-id="67de3-133">id</span></span>|<span data-ttu-id="67de3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67de3-134">String</span></span>|<span data-ttu-id="67de3-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="67de3-135">Key of the entity.</span></span> <span data-ttu-id="67de3-136">Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="67de3-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="67de3-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="67de3-137">userEmailAddress</span></span>|<span data-ttu-id="67de3-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67de3-138">String</span></span>|<span data-ttu-id="67de3-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="67de3-139">The user email address.</span></span> <span data-ttu-id="67de3-140">Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="67de3-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="67de3-141">userId</span><span class="sxs-lookup"><span data-stu-id="67de3-141">userId</span></span>|<span data-ttu-id="67de3-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67de3-142">String</span></span>|<span data-ttu-id="67de3-143">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="67de3-143">The user ID.</span></span> <span data-ttu-id="67de3-144">Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="67de3-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="67de3-145">userName</span><span class="sxs-lookup"><span data-stu-id="67de3-145">userName</span></span>|<span data-ttu-id="67de3-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67de3-146">String</span></span>|<span data-ttu-id="67de3-147">O nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="67de3-147">The user name.</span></span> <span data-ttu-id="67de3-148">Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="67de3-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="67de3-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="67de3-149">userPrincipalName</span></span>|<span data-ttu-id="67de3-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67de3-150">String</span></span>|<span data-ttu-id="67de3-151">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="67de3-151">The user principal name.</span></span> <span data-ttu-id="67de3-152">Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="67de3-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="67de3-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="67de3-153">managedDeviceId</span></span>|<span data-ttu-id="67de3-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67de3-154">String</span></span>|<span data-ttu-id="67de3-155">A ID do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="67de3-155">The managed device ID.</span></span>|
|<span data-ttu-id="67de3-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="67de3-156">deviceName</span></span>|<span data-ttu-id="67de3-157">String</span><span class="sxs-lookup"><span data-stu-id="67de3-157">String</span></span>|<span data-ttu-id="67de3-158">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67de3-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="67de3-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="67de3-159">Response</span></span>
<span data-ttu-id="67de3-160">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67de3-160">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67de3-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67de3-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="67de3-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67de3-162">Request</span></span>
<span data-ttu-id="67de3-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67de3-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="67de3-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="67de3-164">Response</span></span>
<span data-ttu-id="67de3-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67de3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




