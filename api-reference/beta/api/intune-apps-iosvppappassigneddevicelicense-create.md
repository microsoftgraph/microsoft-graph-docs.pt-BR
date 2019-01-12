---
title: Criar iosVppAppAssignedDeviceLicense
description: Crie um novo objeto de iosVppAppAssignedDeviceLicense.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c4eecadae91eb857a5b90c88d66af1721f268ddb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914378"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="fd476-103">Criar iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="fd476-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="fd476-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fd476-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd476-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fd476-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd476-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fd476-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd476-107">Crie um novo objeto de [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="fd476-107">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd476-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd476-108">Prerequisites</span></span>
<span data-ttu-id="fd476-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd476-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd476-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd476-111">Permission type</span></span>|<span data-ttu-id="fd476-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fd476-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd476-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd476-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fd476-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd476-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fd476-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd476-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd476-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd476-116">Not supported.</span></span>|
|<span data-ttu-id="fd476-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd476-117">Application</span></span>|<span data-ttu-id="fd476-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd476-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd476-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd476-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="fd476-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd476-120">Request headers</span></span>
|<span data-ttu-id="fd476-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd476-121">Header</span></span>|<span data-ttu-id="fd476-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fd476-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd476-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd476-123">Authorization</span></span>|<span data-ttu-id="fd476-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd476-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd476-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fd476-125">Accept</span></span>|<span data-ttu-id="fd476-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fd476-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd476-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd476-127">Request body</span></span>
<span data-ttu-id="fd476-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosVppAppAssignedDeviceLicense.</span><span class="sxs-lookup"><span data-stu-id="fd476-128">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="fd476-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosVppAppAssignedDeviceLicense.</span><span class="sxs-lookup"><span data-stu-id="fd476-129">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="fd476-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd476-130">Property</span></span>|<span data-ttu-id="fd476-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd476-131">Type</span></span>|<span data-ttu-id="fd476-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd476-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd476-133">id</span><span class="sxs-lookup"><span data-stu-id="fd476-133">id</span></span>|<span data-ttu-id="fd476-134">String</span><span class="sxs-lookup"><span data-stu-id="fd476-134">String</span></span>|<span data-ttu-id="fd476-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fd476-135">Key of the entity.</span></span> <span data-ttu-id="fd476-136">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="fd476-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="fd476-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="fd476-137">userEmailAddress</span></span>|<span data-ttu-id="fd476-138">String</span><span class="sxs-lookup"><span data-stu-id="fd476-138">String</span></span>|<span data-ttu-id="fd476-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="fd476-139">The user email address.</span></span> <span data-ttu-id="fd476-140">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="fd476-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="fd476-141">userId</span><span class="sxs-lookup"><span data-stu-id="fd476-141">userId</span></span>|<span data-ttu-id="fd476-142">String</span><span class="sxs-lookup"><span data-stu-id="fd476-142">String</span></span>|<span data-ttu-id="fd476-143">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="fd476-143">The user ID.</span></span> <span data-ttu-id="fd476-144">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="fd476-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="fd476-145">userName</span><span class="sxs-lookup"><span data-stu-id="fd476-145">userName</span></span>|<span data-ttu-id="fd476-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd476-146">String</span></span>|<span data-ttu-id="fd476-147">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="fd476-147">The user name.</span></span> <span data-ttu-id="fd476-148">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="fd476-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="fd476-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fd476-149">userPrincipalName</span></span>|<span data-ttu-id="fd476-150">String</span><span class="sxs-lookup"><span data-stu-id="fd476-150">String</span></span>|<span data-ttu-id="fd476-151">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="fd476-151">The user principal name.</span></span> <span data-ttu-id="fd476-152">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="fd476-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="fd476-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="fd476-153">managedDeviceId</span></span>|<span data-ttu-id="fd476-154">String</span><span class="sxs-lookup"><span data-stu-id="fd476-154">String</span></span>|<span data-ttu-id="fd476-155">A ID do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="fd476-155">The managed device ID.</span></span>|
|<span data-ttu-id="fd476-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="fd476-156">deviceName</span></span>|<span data-ttu-id="fd476-157">String</span><span class="sxs-lookup"><span data-stu-id="fd476-157">String</span></span>|<span data-ttu-id="fd476-158">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd476-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="fd476-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd476-159">Response</span></span>
<span data-ttu-id="fd476-160">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd476-160">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd476-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd476-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd476-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd476-162">Request</span></span>
<span data-ttu-id="fd476-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd476-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fd476-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd476-164">Response</span></span>
<span data-ttu-id="fd476-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd476-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





