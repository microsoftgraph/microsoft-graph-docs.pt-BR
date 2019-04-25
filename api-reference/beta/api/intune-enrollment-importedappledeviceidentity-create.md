---
title: Criar importedAppleDeviceIdentity
description: Criar um novo objeto importedAppleDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f9dc95cb141b923b9e9d34b6e9a0de4ab610fe5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532951"
---
# <a name="create-importedappledeviceidentity"></a><span data-ttu-id="cc0d7-103">Criar importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="cc0d7-103">Create importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="cc0d7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc0d7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc0d7-106">Criar um novo objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="cc0d7-106">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc0d7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cc0d7-107">Prerequisites</span></span>
<span data-ttu-id="cc0d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc0d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc0d7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc0d7-110">Permission type</span></span>|<span data-ttu-id="cc0d7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cc0d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc0d7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc0d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc0d7-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc0d7-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cc0d7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc0d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc0d7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-115">Not supported.</span></span>|
|<span data-ttu-id="cc0d7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc0d7-116">Application</span></span>|<span data-ttu-id="cc0d7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc0d7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc0d7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="cc0d7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc0d7-119">Request headers</span></span>
|<span data-ttu-id="cc0d7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc0d7-120">Header</span></span>|<span data-ttu-id="cc0d7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cc0d7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc0d7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc0d7-122">Authorization</span></span>|<span data-ttu-id="cc0d7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc0d7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cc0d7-124">Accept</span></span>|<span data-ttu-id="cc0d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cc0d7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc0d7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc0d7-126">Request body</span></span>
<span data-ttu-id="cc0d7-127">No corpo da solicitação, forneça uma representação JSON do objeto importedAppleDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-127">In the request body, supply a JSON representation for the importedAppleDeviceIdentity object.</span></span>

<span data-ttu-id="cc0d7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar importedAppleDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-128">The following table shows the properties that are required when you create the importedAppleDeviceIdentity.</span></span>

|<span data-ttu-id="cc0d7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc0d7-129">Property</span></span>|<span data-ttu-id="cc0d7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc0d7-130">Type</span></span>|<span data-ttu-id="cc0d7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc0d7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc0d7-132">id</span><span class="sxs-lookup"><span data-stu-id="cc0d7-132">id</span></span>|<span data-ttu-id="cc0d7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc0d7-133">String</span></span>|<span data-ttu-id="cc0d7-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-134">Key of the entity.</span></span>|
|<span data-ttu-id="cc0d7-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="cc0d7-135">serialNumber</span></span>|<span data-ttu-id="cc0d7-136">String</span><span class="sxs-lookup"><span data-stu-id="cc0d7-136">String</span></span>|<span data-ttu-id="cc0d7-137">Número de série do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cc0d7-137">Device serial number</span></span>|
|<span data-ttu-id="cc0d7-138">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="cc0d7-138">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="cc0d7-139">String</span><span class="sxs-lookup"><span data-stu-id="cc0d7-139">String</span></span>|<span data-ttu-id="cc0d7-140">ID do perfil de registro o administrador pretende aplicar ao dispositivo durante o próximo registro</span><span class="sxs-lookup"><span data-stu-id="cc0d7-140">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="cc0d7-141">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="cc0d7-141">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="cc0d7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc0d7-142">DateTimeOffset</span></span>|<span data-ttu-id="cc0d7-143">O perfil de registro de tempo foi atribuído ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="cc0d7-143">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="cc0d7-144">isSupervised</span><span class="sxs-lookup"><span data-stu-id="cc0d7-144">isSupervised</span></span>|<span data-ttu-id="cc0d7-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc0d7-145">Boolean</span></span>|<span data-ttu-id="cc0d7-146">Indica se o dispositivo Apple é supervisionado.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-146">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="cc0d7-147">Mais informações em:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="cc0d7-147">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="cc0d7-148">discoverySource</span><span class="sxs-lookup"><span data-stu-id="cc0d7-148">discoverySource</span></span>|[<span data-ttu-id="cc0d7-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="cc0d7-149">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="cc0d7-150">Fonte de descoberta de dispositivos Apple.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-150">Apple device discovery source.</span></span> <span data-ttu-id="cc0d7-151">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-151">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="cc0d7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc0d7-152">createdDateTime</span></span>|<span data-ttu-id="cc0d7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc0d7-153">DateTimeOffset</span></span>|<span data-ttu-id="cc0d7-154">Data e hora de criação do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cc0d7-154">Created Date Time of the device</span></span>|
|<span data-ttu-id="cc0d7-155">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc0d7-155">lastContactedDateTime</span></span>|<span data-ttu-id="cc0d7-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc0d7-156">DateTimeOffset</span></span>|<span data-ttu-id="cc0d7-157">Data e hora do último contato do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cc0d7-157">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="cc0d7-158">description</span><span class="sxs-lookup"><span data-stu-id="cc0d7-158">description</span></span>|<span data-ttu-id="cc0d7-159">String</span><span class="sxs-lookup"><span data-stu-id="cc0d7-159">String</span></span>|<span data-ttu-id="cc0d7-160">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cc0d7-160">The description of the device</span></span>|
|<span data-ttu-id="cc0d7-161">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="cc0d7-161">enrollmentState</span></span>|[<span data-ttu-id="cc0d7-162">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="cc0d7-162">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="cc0d7-163">O estado do dispositivo no Intune.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-163">The state of the device in Intune.</span></span> <span data-ttu-id="cc0d7-164">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-164">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="cc0d7-165">platform</span><span class="sxs-lookup"><span data-stu-id="cc0d7-165">platform</span></span>|[<span data-ttu-id="cc0d7-166">plataforma</span><span class="sxs-lookup"><span data-stu-id="cc0d7-166">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="cc0d7-167">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-167">The platform of the Device.</span></span> <span data-ttu-id="cc0d7-168">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-168">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="cc0d7-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc0d7-169">Response</span></span>
<span data-ttu-id="cc0d7-170">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-170">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc0d7-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc0d7-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc0d7-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc0d7-172">Request</span></span>
<span data-ttu-id="cc0d7-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
Content-type: application/json
Content-length: 497

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="cc0d7-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc0d7-174">Response</span></span>
<span data-ttu-id="cc0d7-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc0d7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 605

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```





