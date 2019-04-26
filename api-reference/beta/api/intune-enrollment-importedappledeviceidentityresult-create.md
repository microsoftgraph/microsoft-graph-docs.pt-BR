---
title: Criar importedAppleDeviceIdentityResult
description: Criar um novo objeto importedAppleDeviceIdentityResult.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 56300cc036e0184d53a68113fad3d0d38e494582
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32533000"
---
# <a name="create-importedappledeviceidentityresult"></a><span data-ttu-id="944d2-103">Criar importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="944d2-103">Create importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="944d2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="944d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="944d2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="944d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="944d2-106">Criar um novo objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="944d2-106">Create a new [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="944d2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="944d2-107">Prerequisites</span></span>
<span data-ttu-id="944d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="944d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="944d2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="944d2-110">Permission type</span></span>|<span data-ttu-id="944d2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="944d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="944d2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="944d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="944d2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="944d2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="944d2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="944d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="944d2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="944d2-115">Not supported.</span></span>|
|<span data-ttu-id="944d2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="944d2-116">Application</span></span>|<span data-ttu-id="944d2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="944d2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="944d2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="944d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="944d2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="944d2-119">Request headers</span></span>
|<span data-ttu-id="944d2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="944d2-120">Header</span></span>|<span data-ttu-id="944d2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="944d2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="944d2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="944d2-122">Authorization</span></span>|<span data-ttu-id="944d2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="944d2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="944d2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="944d2-124">Accept</span></span>|<span data-ttu-id="944d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="944d2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="944d2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="944d2-126">Request body</span></span>
<span data-ttu-id="944d2-127">No corpo da solicitação, forneça uma representação JSON do objeto importedAppleDeviceIdentityResult.</span><span class="sxs-lookup"><span data-stu-id="944d2-127">In the request body, supply a JSON representation for the importedAppleDeviceIdentityResult object.</span></span>

<span data-ttu-id="944d2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar importedAppleDeviceIdentityResult.</span><span class="sxs-lookup"><span data-stu-id="944d2-128">The following table shows the properties that are required when you create the importedAppleDeviceIdentityResult.</span></span>

|<span data-ttu-id="944d2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="944d2-129">Property</span></span>|<span data-ttu-id="944d2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="944d2-130">Type</span></span>|<span data-ttu-id="944d2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="944d2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="944d2-132">id</span><span class="sxs-lookup"><span data-stu-id="944d2-132">id</span></span>|<span data-ttu-id="944d2-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="944d2-133">String</span></span>|<span data-ttu-id="944d2-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="944d2-134">Key of the entity.</span></span> <span data-ttu-id="944d2-135">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="944d2-135">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="944d2-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="944d2-136">serialNumber</span></span>|<span data-ttu-id="944d2-137">String</span><span class="sxs-lookup"><span data-stu-id="944d2-137">String</span></span>|<span data-ttu-id="944d2-138">Número de série do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="944d2-138">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="944d2-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="944d2-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="944d2-140">String</span><span class="sxs-lookup"><span data-stu-id="944d2-140">String</span></span>|<span data-ttu-id="944d2-141">ID de perfil de registro o administrador pretende aplicar ao dispositivo durante o próximo registro herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="944d2-141">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="944d2-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="944d2-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="944d2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="944d2-143">DateTimeOffset</span></span>|<span data-ttu-id="944d2-144">O perfil de registro de tempo foi atribuído ao dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="944d2-144">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="944d2-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="944d2-145">isSupervised</span></span>|<span data-ttu-id="944d2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="944d2-146">Boolean</span></span>|<span data-ttu-id="944d2-147">Indica se o dispositivo Apple é supervisionado.</span><span class="sxs-lookup"><span data-stu-id="944d2-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="944d2-148">Mais informações em: https://support.apple.com/en-us/HT202837 herdadas de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="944d2-148">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="944d2-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="944d2-149">discoverySource</span></span>|[<span data-ttu-id="944d2-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="944d2-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="944d2-151">Fonte de descoberta de dispositivos Apple.</span><span class="sxs-lookup"><span data-stu-id="944d2-151">Apple device discovery source.</span></span> <span data-ttu-id="944d2-152">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="944d2-152">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="944d2-153">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="944d2-153">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="944d2-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="944d2-154">createdDateTime</span></span>|<span data-ttu-id="944d2-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="944d2-155">DateTimeOffset</span></span>|<span data-ttu-id="944d2-156">Data e hora de criação do dispositivo herdadas de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="944d2-156">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="944d2-157">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="944d2-157">lastContactedDateTime</span></span>|<span data-ttu-id="944d2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="944d2-158">DateTimeOffset</span></span>|<span data-ttu-id="944d2-159">Data e hora do último contato do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="944d2-159">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="944d2-160">description</span><span class="sxs-lookup"><span data-stu-id="944d2-160">description</span></span>|<span data-ttu-id="944d2-161">String</span><span class="sxs-lookup"><span data-stu-id="944d2-161">String</span></span>|<span data-ttu-id="944d2-162">A descrição do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="944d2-162">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="944d2-163">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="944d2-163">enrollmentState</span></span>|[<span data-ttu-id="944d2-164">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="944d2-164">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="944d2-165">O estado do dispositivo no Intune herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="944d2-165">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="944d2-166">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="944d2-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="944d2-167">platform</span><span class="sxs-lookup"><span data-stu-id="944d2-167">platform</span></span>|[<span data-ttu-id="944d2-168">plataforma</span><span class="sxs-lookup"><span data-stu-id="944d2-168">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="944d2-169">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="944d2-169">The platform of the Device.</span></span> <span data-ttu-id="944d2-170">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="944d2-170">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="944d2-171">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="944d2-171">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="944d2-172">status</span><span class="sxs-lookup"><span data-stu-id="944d2-172">status</span></span>|<span data-ttu-id="944d2-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="944d2-173">Boolean</span></span>|<span data-ttu-id="944d2-174">Status da identidade do dispositivo importado</span><span class="sxs-lookup"><span data-stu-id="944d2-174">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="944d2-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="944d2-175">Response</span></span>
<span data-ttu-id="944d2-176">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="944d2-176">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="944d2-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="944d2-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="944d2-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="944d2-178">Request</span></span>
<span data-ttu-id="944d2-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="944d2-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
Content-type: application/json
Content-length: 522

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="944d2-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="944d2-180">Response</span></span>
<span data-ttu-id="944d2-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="944d2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 630

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```





