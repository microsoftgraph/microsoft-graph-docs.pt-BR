---
title: Atualizar importedAppleDeviceIdentityResult
description: Atualiza as propriedades de um objeto importedAppleDeviceIdentityResult.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 260915684c68b55cff0b7cc09aea534f0215c28b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35985034"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="25696-103">Atualizar importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="25696-103">Update importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="25696-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="25696-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25696-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25696-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25696-106">Atualiza as propriedades de um objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="25696-106">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25696-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="25696-107">Prerequisites</span></span>
<span data-ttu-id="25696-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25696-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25696-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25696-110">Permission type</span></span>|<span data-ttu-id="25696-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="25696-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25696-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25696-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25696-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25696-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="25696-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25696-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25696-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25696-115">Not supported.</span></span>|
|<span data-ttu-id="25696-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25696-116">Application</span></span>|<span data-ttu-id="25696-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25696-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25696-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25696-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="25696-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25696-119">Request headers</span></span>
|<span data-ttu-id="25696-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25696-120">Header</span></span>|<span data-ttu-id="25696-121">Valor</span><span class="sxs-lookup"><span data-stu-id="25696-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25696-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="25696-122">Authorization</span></span>|<span data-ttu-id="25696-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25696-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25696-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="25696-124">Accept</span></span>|<span data-ttu-id="25696-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25696-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25696-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25696-126">Request body</span></span>
<span data-ttu-id="25696-127">No corpo da solicitação, forneça uma representação JSON do objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="25696-127">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="25696-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="25696-128">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="25696-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25696-129">Property</span></span>|<span data-ttu-id="25696-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="25696-130">Type</span></span>|<span data-ttu-id="25696-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="25696-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25696-132">id</span><span class="sxs-lookup"><span data-stu-id="25696-132">id</span></span>|<span data-ttu-id="25696-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25696-133">String</span></span>|<span data-ttu-id="25696-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="25696-134">Key of the entity.</span></span> <span data-ttu-id="25696-135">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="25696-135">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="25696-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="25696-136">serialNumber</span></span>|<span data-ttu-id="25696-137">String</span><span class="sxs-lookup"><span data-stu-id="25696-137">String</span></span>|<span data-ttu-id="25696-138">Número de série do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="25696-138">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="25696-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="25696-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="25696-140">String</span><span class="sxs-lookup"><span data-stu-id="25696-140">String</span></span>|<span data-ttu-id="25696-141">ID de perfil de registro o administrador pretende aplicar ao dispositivo durante o próximo registro herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="25696-141">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="25696-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="25696-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="25696-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25696-143">DateTimeOffset</span></span>|<span data-ttu-id="25696-144">O perfil de registro de tempo foi atribuído ao dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="25696-144">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="25696-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="25696-145">isSupervised</span></span>|<span data-ttu-id="25696-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="25696-146">Boolean</span></span>|<span data-ttu-id="25696-147">Indica se o dispositivo Apple é supervisionado.</span><span class="sxs-lookup"><span data-stu-id="25696-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="25696-148">Mais informações em: https://support.apple.com/en-us/HT202837 herdadas de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="25696-148">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="25696-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="25696-149">discoverySource</span></span>|[<span data-ttu-id="25696-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="25696-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="25696-151">Fonte de descoberta de dispositivos Apple.</span><span class="sxs-lookup"><span data-stu-id="25696-151">Apple device discovery source.</span></span> <span data-ttu-id="25696-152">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="25696-152">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="25696-153">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="25696-153">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="25696-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25696-154">createdDateTime</span></span>|<span data-ttu-id="25696-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25696-155">DateTimeOffset</span></span>|<span data-ttu-id="25696-156">Data e hora de criação do dispositivo herdadas de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="25696-156">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="25696-157">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="25696-157">lastContactedDateTime</span></span>|<span data-ttu-id="25696-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25696-158">DateTimeOffset</span></span>|<span data-ttu-id="25696-159">Data e hora do último contato do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="25696-159">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="25696-160">descrição</span><span class="sxs-lookup"><span data-stu-id="25696-160">description</span></span>|<span data-ttu-id="25696-161">String</span><span class="sxs-lookup"><span data-stu-id="25696-161">String</span></span>|<span data-ttu-id="25696-162">A descrição do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="25696-162">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="25696-163">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="25696-163">enrollmentState</span></span>|[<span data-ttu-id="25696-164">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="25696-164">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="25696-165">O estado do dispositivo no Intune herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="25696-165">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="25696-166">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="25696-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="25696-167">platform</span><span class="sxs-lookup"><span data-stu-id="25696-167">platform</span></span>|[<span data-ttu-id="25696-168">plataforma</span><span class="sxs-lookup"><span data-stu-id="25696-168">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="25696-169">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25696-169">The platform of the Device.</span></span> <span data-ttu-id="25696-170">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="25696-170">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="25696-171">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="25696-171">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="25696-172">status</span><span class="sxs-lookup"><span data-stu-id="25696-172">status</span></span>|<span data-ttu-id="25696-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="25696-173">Boolean</span></span>|<span data-ttu-id="25696-174">Status da identidade do dispositivo importado</span><span class="sxs-lookup"><span data-stu-id="25696-174">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="25696-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="25696-175">Response</span></span>
<span data-ttu-id="25696-176">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25696-176">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25696-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25696-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="25696-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25696-178">Request</span></span>
<span data-ttu-id="25696-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25696-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="25696-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="25696-180">Response</span></span>
<span data-ttu-id="25696-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25696-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





