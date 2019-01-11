---
title: Atualizar iosVppAppAssignedDeviceLicense
description: Atualize as propriedades de um objeto iosVppAppAssignedDeviceLicense.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d8e22eed756a0c1946ae13ce6dac9cf2c63cd3a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828753"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="bb3ab-103">Atualizar iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="bb3ab-103">Update iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="bb3ab-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bb3ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb3ab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bb3ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb3ab-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bb3ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb3ab-107">Atualize as propriedades de um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="bb3ab-107">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bb3ab-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb3ab-108">Prerequisites</span></span>
<span data-ttu-id="bb3ab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb3ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb3ab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb3ab-111">Permission type</span></span>|<span data-ttu-id="bb3ab-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb3ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb3ab-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb3ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb3ab-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb3ab-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bb3ab-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb3ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb3ab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb3ab-116">Not supported.</span></span>|
|<span data-ttu-id="bb3ab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb3ab-117">Application</span></span>|<span data-ttu-id="bb3ab-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb3ab-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb3ab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb3ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="bb3ab-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb3ab-120">Request headers</span></span>
|<span data-ttu-id="bb3ab-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb3ab-121">Header</span></span>|<span data-ttu-id="bb3ab-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bb3ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb3ab-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb3ab-123">Authorization</span></span>|<span data-ttu-id="bb3ab-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb3ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb3ab-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bb3ab-125">Accept</span></span>|<span data-ttu-id="bb3ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb3ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb3ab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb3ab-127">Request body</span></span>
<span data-ttu-id="bb3ab-128">No corpo da solicitação, fornece uma representação JSON para o objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="bb3ab-128">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="bb3ab-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span><span class="sxs-lookup"><span data-stu-id="bb3ab-129">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="bb3ab-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb3ab-130">Property</span></span>|<span data-ttu-id="bb3ab-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb3ab-131">Type</span></span>|<span data-ttu-id="bb3ab-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb3ab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb3ab-133">id</span><span class="sxs-lookup"><span data-stu-id="bb3ab-133">id</span></span>|<span data-ttu-id="bb3ab-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb3ab-134">String</span></span>|<span data-ttu-id="bb3ab-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bb3ab-135">Key of the entity.</span></span> <span data-ttu-id="bb3ab-136">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="bb3ab-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="bb3ab-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="bb3ab-137">userEmailAddress</span></span>|<span data-ttu-id="bb3ab-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb3ab-138">String</span></span>|<span data-ttu-id="bb3ab-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="bb3ab-139">The user email address.</span></span> <span data-ttu-id="bb3ab-140">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="bb3ab-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="bb3ab-141">userId</span><span class="sxs-lookup"><span data-stu-id="bb3ab-141">userId</span></span>|<span data-ttu-id="bb3ab-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb3ab-142">String</span></span>|<span data-ttu-id="bb3ab-143">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="bb3ab-143">The user ID.</span></span> <span data-ttu-id="bb3ab-144">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="bb3ab-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="bb3ab-145">userName</span><span class="sxs-lookup"><span data-stu-id="bb3ab-145">userName</span></span>|<span data-ttu-id="bb3ab-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb3ab-146">String</span></span>|<span data-ttu-id="bb3ab-147">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="bb3ab-147">The user name.</span></span> <span data-ttu-id="bb3ab-148">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="bb3ab-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="bb3ab-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bb3ab-149">userPrincipalName</span></span>|<span data-ttu-id="bb3ab-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb3ab-150">String</span></span>|<span data-ttu-id="bb3ab-151">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="bb3ab-151">The user principal name.</span></span> <span data-ttu-id="bb3ab-152">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="bb3ab-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="bb3ab-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="bb3ab-153">managedDeviceId</span></span>|<span data-ttu-id="bb3ab-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb3ab-154">String</span></span>|<span data-ttu-id="bb3ab-155">A ID do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="bb3ab-155">The managed device ID.</span></span>|
|<span data-ttu-id="bb3ab-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="bb3ab-156">deviceName</span></span>|<span data-ttu-id="bb3ab-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb3ab-157">String</span></span>|<span data-ttu-id="bb3ab-158">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb3ab-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="bb3ab-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb3ab-159">Response</span></span>
<span data-ttu-id="bb3ab-160">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb3ab-160">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb3ab-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb3ab-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="bb3ab-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb3ab-162">Request</span></span>
<span data-ttu-id="bb3ab-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb3ab-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 258

{
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="bb3ab-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb3ab-164">Response</span></span>
<span data-ttu-id="bb3ab-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb3ab-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





