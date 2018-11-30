---
title: Criar iosVppAppAssignedDeviceLicense
description: Crie um novo objeto de iosVppAppAssignedDeviceLicense.
ms.openlocfilehash: 968f272fae21ccf78d41b384c34675f6a5d3f4c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039078"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="0c58e-103">Criar iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="0c58e-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="0c58e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0c58e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c58e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0c58e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c58e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0c58e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c58e-107">Crie um novo objeto de [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="0c58e-107">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0c58e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c58e-108">Prerequisites</span></span>
<span data-ttu-id="0c58e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c58e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c58e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c58e-111">Permission type</span></span>|<span data-ttu-id="0c58e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c58e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c58e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c58e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c58e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c58e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0c58e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c58e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c58e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c58e-116">Not supported.</span></span>|
|<span data-ttu-id="0c58e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c58e-117">Application</span></span>|<span data-ttu-id="0c58e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c58e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c58e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c58e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="0c58e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c58e-120">Request headers</span></span>
|<span data-ttu-id="0c58e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c58e-121">Header</span></span>|<span data-ttu-id="0c58e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0c58e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c58e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c58e-123">Authorization</span></span>|<span data-ttu-id="0c58e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c58e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c58e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0c58e-125">Accept</span></span>|<span data-ttu-id="0c58e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c58e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c58e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c58e-127">Request body</span></span>
<span data-ttu-id="0c58e-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosVppAppAssignedDeviceLicense.</span><span class="sxs-lookup"><span data-stu-id="0c58e-128">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="0c58e-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosVppAppAssignedDeviceLicense.</span><span class="sxs-lookup"><span data-stu-id="0c58e-129">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="0c58e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c58e-130">Property</span></span>|<span data-ttu-id="0c58e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c58e-131">Type</span></span>|<span data-ttu-id="0c58e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c58e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c58e-133">id</span><span class="sxs-lookup"><span data-stu-id="0c58e-133">id</span></span>|<span data-ttu-id="0c58e-134">String</span><span class="sxs-lookup"><span data-stu-id="0c58e-134">String</span></span>|<span data-ttu-id="0c58e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0c58e-135">Key of the entity.</span></span> <span data-ttu-id="0c58e-136">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="0c58e-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="0c58e-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0c58e-137">userEmailAddress</span></span>|<span data-ttu-id="0c58e-138">String</span><span class="sxs-lookup"><span data-stu-id="0c58e-138">String</span></span>|<span data-ttu-id="0c58e-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="0c58e-139">The user email address.</span></span> <span data-ttu-id="0c58e-140">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="0c58e-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="0c58e-141">userId</span><span class="sxs-lookup"><span data-stu-id="0c58e-141">userId</span></span>|<span data-ttu-id="0c58e-142">String</span><span class="sxs-lookup"><span data-stu-id="0c58e-142">String</span></span>|<span data-ttu-id="0c58e-143">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="0c58e-143">The user ID.</span></span> <span data-ttu-id="0c58e-144">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="0c58e-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="0c58e-145">userName</span><span class="sxs-lookup"><span data-stu-id="0c58e-145">userName</span></span>|<span data-ttu-id="0c58e-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c58e-146">String</span></span>|<span data-ttu-id="0c58e-147">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="0c58e-147">The user name.</span></span> <span data-ttu-id="0c58e-148">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="0c58e-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="0c58e-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0c58e-149">userPrincipalName</span></span>|<span data-ttu-id="0c58e-150">String</span><span class="sxs-lookup"><span data-stu-id="0c58e-150">String</span></span>|<span data-ttu-id="0c58e-151">O nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="0c58e-151">The user principal name.</span></span> <span data-ttu-id="0c58e-152">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="0c58e-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="0c58e-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="0c58e-153">managedDeviceId</span></span>|<span data-ttu-id="0c58e-154">String</span><span class="sxs-lookup"><span data-stu-id="0c58e-154">String</span></span>|<span data-ttu-id="0c58e-155">A ID do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="0c58e-155">The managed device ID.</span></span>|
|<span data-ttu-id="0c58e-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="0c58e-156">deviceName</span></span>|<span data-ttu-id="0c58e-157">String</span><span class="sxs-lookup"><span data-stu-id="0c58e-157">String</span></span>|<span data-ttu-id="0c58e-158">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c58e-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="0c58e-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c58e-159">Response</span></span>
<span data-ttu-id="0c58e-160">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c58e-160">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c58e-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c58e-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="0c58e-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c58e-162">Request</span></span>
<span data-ttu-id="0c58e-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c58e-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c58e-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c58e-164">Response</span></span>
<span data-ttu-id="0c58e-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c58e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





