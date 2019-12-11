---
title: Atualizar importedAppleDeviceIdentityResult
description: Atualiza as propriedades de um objeto importedAppleDeviceIdentityResult.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3b8fcb38ea8a1d35ea84a2278d667352448cca81
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943884"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="f69f8-103">Atualizar importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="f69f8-103">Update importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="f69f8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f69f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f69f8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f69f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f69f8-106">Atualiza as propriedades de um objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="f69f8-106">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f69f8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f69f8-107">Prerequisites</span></span>
<span data-ttu-id="f69f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f69f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f69f8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f69f8-110">Permission type</span></span>|<span data-ttu-id="f69f8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f69f8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f69f8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f69f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f69f8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f69f8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f69f8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f69f8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f69f8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f69f8-115">Not supported.</span></span>|
|<span data-ttu-id="f69f8-116">Application</span><span class="sxs-lookup"><span data-stu-id="f69f8-116">Application</span></span>|<span data-ttu-id="f69f8-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f69f8-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f69f8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f69f8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="f69f8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f69f8-119">Request headers</span></span>
|<span data-ttu-id="f69f8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f69f8-120">Header</span></span>|<span data-ttu-id="f69f8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f69f8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f69f8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f69f8-122">Authorization</span></span>|<span data-ttu-id="f69f8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f69f8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f69f8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f69f8-124">Accept</span></span>|<span data-ttu-id="f69f8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f69f8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f69f8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f69f8-126">Request body</span></span>
<span data-ttu-id="f69f8-127">No corpo da solicitação, forneça uma representação JSON do objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="f69f8-127">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="f69f8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="f69f8-128">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="f69f8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f69f8-129">Property</span></span>|<span data-ttu-id="f69f8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f69f8-130">Type</span></span>|<span data-ttu-id="f69f8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f69f8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f69f8-132">id</span><span class="sxs-lookup"><span data-stu-id="f69f8-132">id</span></span>|<span data-ttu-id="f69f8-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f69f8-133">String</span></span>|<span data-ttu-id="f69f8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f69f8-134">Key of the entity.</span></span> <span data-ttu-id="f69f8-135">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="f69f8-135">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="f69f8-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="f69f8-136">serialNumber</span></span>|<span data-ttu-id="f69f8-137">String</span><span class="sxs-lookup"><span data-stu-id="f69f8-137">String</span></span>|<span data-ttu-id="f69f8-138">Número de série do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="f69f8-138">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="f69f8-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="f69f8-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="f69f8-140">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f69f8-140">String</span></span>|<span data-ttu-id="f69f8-141">ID de perfil de registro o administrador pretende aplicar ao dispositivo durante o próximo registro herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="f69f8-141">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="f69f8-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="f69f8-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="f69f8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f69f8-143">DateTimeOffset</span></span>|<span data-ttu-id="f69f8-144">O perfil de registro de tempo foi atribuído ao dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="f69f8-144">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="f69f8-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="f69f8-145">isSupervised</span></span>|<span data-ttu-id="f69f8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f69f8-146">Boolean</span></span>|<span data-ttu-id="f69f8-147">Indica se o dispositivo Apple é supervisionado.</span><span class="sxs-lookup"><span data-stu-id="f69f8-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="f69f8-148">Mais informações em: https://support.apple.com/en-us/HT202837 herdadas de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="f69f8-148">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="f69f8-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="f69f8-149">discoverySource</span></span>|[<span data-ttu-id="f69f8-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="f69f8-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="f69f8-151">Fonte de descoberta de dispositivos Apple.</span><span class="sxs-lookup"><span data-stu-id="f69f8-151">Apple device discovery source.</span></span> <span data-ttu-id="f69f8-152">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="f69f8-152">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="f69f8-153">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="f69f8-153">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="f69f8-154">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f69f8-154">isDeleted</span></span>|<span data-ttu-id="f69f8-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="f69f8-155">Boolean</span></span>|<span data-ttu-id="f69f8-156">Indica se o dispositivo é excluído do Apple Business Manager herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="f69f8-156">Indicates if the device is deleted from Apple Business Manager Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="f69f8-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f69f8-157">createdDateTime</span></span>|<span data-ttu-id="f69f8-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f69f8-158">DateTimeOffset</span></span>|<span data-ttu-id="f69f8-159">Data e hora de criação do dispositivo herdadas de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="f69f8-159">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="f69f8-160">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="f69f8-160">lastContactedDateTime</span></span>|<span data-ttu-id="f69f8-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f69f8-161">DateTimeOffset</span></span>|<span data-ttu-id="f69f8-162">Data e hora do último contato do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="f69f8-162">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="f69f8-163">description</span><span class="sxs-lookup"><span data-stu-id="f69f8-163">description</span></span>|<span data-ttu-id="f69f8-164">String</span><span class="sxs-lookup"><span data-stu-id="f69f8-164">String</span></span>|<span data-ttu-id="f69f8-165">A descrição do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="f69f8-165">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="f69f8-166">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="f69f8-166">enrollmentState</span></span>|[<span data-ttu-id="f69f8-167">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="f69f8-167">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="f69f8-168">O estado do dispositivo no Intune herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="f69f8-168">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="f69f8-169">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="f69f8-169">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="f69f8-170">platform</span><span class="sxs-lookup"><span data-stu-id="f69f8-170">platform</span></span>|[<span data-ttu-id="f69f8-171">plataforma</span><span class="sxs-lookup"><span data-stu-id="f69f8-171">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="f69f8-172">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f69f8-172">The platform of the Device.</span></span> <span data-ttu-id="f69f8-173">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="f69f8-173">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="f69f8-174">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="f69f8-174">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="f69f8-175">status</span><span class="sxs-lookup"><span data-stu-id="f69f8-175">status</span></span>|<span data-ttu-id="f69f8-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="f69f8-176">Boolean</span></span>|<span data-ttu-id="f69f8-177">Status da identidade do dispositivo importado</span><span class="sxs-lookup"><span data-stu-id="f69f8-177">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="f69f8-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="f69f8-178">Response</span></span>
<span data-ttu-id="f69f8-179">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f69f8-179">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f69f8-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f69f8-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="f69f8-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f69f8-181">Request</span></span>
<span data-ttu-id="f69f8-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f69f8-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 544

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "isDeleted": true,
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="f69f8-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="f69f8-183">Response</span></span>
<span data-ttu-id="f69f8-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f69f8-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 652

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "isDeleted": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```





