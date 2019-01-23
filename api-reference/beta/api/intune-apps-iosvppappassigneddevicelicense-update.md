---
title: Atualizar iosVppAppAssignedDeviceLicense
description: Atualize as propriedades de um objeto iosVppAppAssignedDeviceLicense.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2edd886b0ab9b302e7f224511bb329fe8269a7d9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402122"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="06f24-103">Atualizar iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="06f24-103">Update iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="06f24-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="06f24-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="06f24-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="06f24-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06f24-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="06f24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06f24-107">Atualize as propriedades de um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="06f24-107">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06f24-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06f24-108">Prerequisites</span></span>
<span data-ttu-id="06f24-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="06f24-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="06f24-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06f24-111">Permission type</span></span>|<span data-ttu-id="06f24-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06f24-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06f24-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06f24-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06f24-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06f24-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="06f24-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06f24-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06f24-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06f24-116">Not supported.</span></span>|
|<span data-ttu-id="06f24-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06f24-117">Application</span></span>|<span data-ttu-id="06f24-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06f24-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06f24-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06f24-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="06f24-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06f24-120">Request headers</span></span>
|<span data-ttu-id="06f24-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06f24-121">Header</span></span>|<span data-ttu-id="06f24-122">Valor</span><span class="sxs-lookup"><span data-stu-id="06f24-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06f24-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="06f24-123">Authorization</span></span>|<span data-ttu-id="06f24-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06f24-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06f24-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06f24-125">Accept</span></span>|<span data-ttu-id="06f24-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06f24-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06f24-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06f24-127">Request body</span></span>
<span data-ttu-id="06f24-128">No corpo da solicitação, fornece uma representação JSON para o objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="06f24-128">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="06f24-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span><span class="sxs-lookup"><span data-stu-id="06f24-129">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="06f24-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06f24-130">Property</span></span>|<span data-ttu-id="06f24-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="06f24-131">Type</span></span>|<span data-ttu-id="06f24-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="06f24-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06f24-133">id</span><span class="sxs-lookup"><span data-stu-id="06f24-133">id</span></span>|<span data-ttu-id="06f24-134">String</span><span class="sxs-lookup"><span data-stu-id="06f24-134">String</span></span>|<span data-ttu-id="06f24-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="06f24-135">Key of the entity.</span></span> <span data-ttu-id="06f24-136">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="06f24-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="06f24-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="06f24-137">userEmailAddress</span></span>|<span data-ttu-id="06f24-138">String</span><span class="sxs-lookup"><span data-stu-id="06f24-138">String</span></span>|<span data-ttu-id="06f24-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="06f24-139">The user email address.</span></span> <span data-ttu-id="06f24-140">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="06f24-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="06f24-141">userId</span><span class="sxs-lookup"><span data-stu-id="06f24-141">userId</span></span>|<span data-ttu-id="06f24-142">String</span><span class="sxs-lookup"><span data-stu-id="06f24-142">String</span></span>|<span data-ttu-id="06f24-143">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="06f24-143">The user ID.</span></span> <span data-ttu-id="06f24-144">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="06f24-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="06f24-145">userName</span><span class="sxs-lookup"><span data-stu-id="06f24-145">userName</span></span>|<span data-ttu-id="06f24-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06f24-146">String</span></span>|<span data-ttu-id="06f24-147">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="06f24-147">The user name.</span></span> <span data-ttu-id="06f24-148">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="06f24-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="06f24-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="06f24-149">userPrincipalName</span></span>|<span data-ttu-id="06f24-150">String</span><span class="sxs-lookup"><span data-stu-id="06f24-150">String</span></span>|<span data-ttu-id="06f24-151">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="06f24-151">The user principal name.</span></span> <span data-ttu-id="06f24-152">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="06f24-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="06f24-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="06f24-153">managedDeviceId</span></span>|<span data-ttu-id="06f24-154">String</span><span class="sxs-lookup"><span data-stu-id="06f24-154">String</span></span>|<span data-ttu-id="06f24-155">A ID do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="06f24-155">The managed device ID.</span></span>|
|<span data-ttu-id="06f24-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="06f24-156">deviceName</span></span>|<span data-ttu-id="06f24-157">String</span><span class="sxs-lookup"><span data-stu-id="06f24-157">String</span></span>|<span data-ttu-id="06f24-158">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06f24-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="06f24-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="06f24-159">Response</span></span>
<span data-ttu-id="06f24-160">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06f24-160">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06f24-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06f24-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="06f24-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06f24-162">Request</span></span>
<span data-ttu-id="06f24-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06f24-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="06f24-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="06f24-164">Response</span></span>
<span data-ttu-id="06f24-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06f24-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




