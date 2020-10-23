---
title: Atualizar importedAppleDeviceIdentityResult
description: Atualiza as propriedades de um objeto importedAppleDeviceIdentityResult.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 255da82493beea47914aafddfaa1050a492cdba7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729121"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="5b0fb-103">Atualizar importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="5b0fb-103">Update importedAppleDeviceIdentityResult</span></span>

<span data-ttu-id="5b0fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b0fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b0fb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5b0fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b0fb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b0fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b0fb-107">Atualiza as propriedades de um objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="5b0fb-107">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b0fb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5b0fb-108">Prerequisites</span></span>
<span data-ttu-id="5b0fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b0fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b0fb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b0fb-111">Permission type</span></span>|<span data-ttu-id="5b0fb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5b0fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b0fb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b0fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b0fb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b0fb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5b0fb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b0fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b0fb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b0fb-116">Not supported.</span></span>|
|<span data-ttu-id="5b0fb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b0fb-117">Application</span></span>|<span data-ttu-id="5b0fb-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b0fb-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b0fb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b0fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="5b0fb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b0fb-120">Request headers</span></span>
|<span data-ttu-id="5b0fb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b0fb-121">Header</span></span>|<span data-ttu-id="5b0fb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5b0fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b0fb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b0fb-123">Authorization</span></span>|<span data-ttu-id="5b0fb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b0fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b0fb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5b0fb-125">Accept</span></span>|<span data-ttu-id="5b0fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b0fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b0fb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b0fb-127">Request body</span></span>
<span data-ttu-id="5b0fb-128">No corpo da solicitação, forneça uma representação JSON do objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="5b0fb-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="5b0fb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="5b0fb-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="5b0fb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b0fb-130">Property</span></span>|<span data-ttu-id="5b0fb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b0fb-131">Type</span></span>|<span data-ttu-id="5b0fb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b0fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b0fb-133">id</span><span class="sxs-lookup"><span data-stu-id="5b0fb-133">id</span></span>|<span data-ttu-id="5b0fb-134">String</span><span class="sxs-lookup"><span data-stu-id="5b0fb-134">String</span></span>|<span data-ttu-id="5b0fb-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5b0fb-135">Key of the entity.</span></span> <span data-ttu-id="5b0fb-136">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5b0fb-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5b0fb-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="5b0fb-137">serialNumber</span></span>|<span data-ttu-id="5b0fb-138">String</span><span class="sxs-lookup"><span data-stu-id="5b0fb-138">String</span></span>|<span data-ttu-id="5b0fb-139">Número de série do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5b0fb-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5b0fb-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="5b0fb-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="5b0fb-141">String</span><span class="sxs-lookup"><span data-stu-id="5b0fb-141">String</span></span>|<span data-ttu-id="5b0fb-142">ID de perfil de registro o administrador pretende aplicar ao dispositivo durante o próximo registro herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5b0fb-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5b0fb-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="5b0fb-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="5b0fb-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b0fb-144">DateTimeOffset</span></span>|<span data-ttu-id="5b0fb-145">O perfil de registro de tempo foi atribuído ao dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5b0fb-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5b0fb-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="5b0fb-146">isSupervised</span></span>|<span data-ttu-id="5b0fb-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b0fb-147">Boolean</span></span>|<span data-ttu-id="5b0fb-148">Indica se o dispositivo Apple é supervisionado.</span><span class="sxs-lookup"><span data-stu-id="5b0fb-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="5b0fb-149">Mais informações em: https://support.apple.com/HT202837 herdadas de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5b0fb-149">More information is at: https://support.apple.com/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5b0fb-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="5b0fb-150">discoverySource</span></span>|[<span data-ttu-id="5b0fb-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="5b0fb-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="5b0fb-152">Fonte de descoberta de dispositivos Apple.</span><span class="sxs-lookup"><span data-stu-id="5b0fb-152">Apple device discovery source.</span></span> <span data-ttu-id="5b0fb-153">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="5b0fb-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="5b0fb-154">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="5b0fb-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="5b0fb-155">isDeleted</span><span class="sxs-lookup"><span data-stu-id="5b0fb-155">isDeleted</span></span>|<span data-ttu-id="5b0fb-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="5b0fb-156">Boolean</span></span>|<span data-ttu-id="5b0fb-157">Indica se o dispositivo é excluído do Apple Business Manager herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5b0fb-157">Indicates if the device is deleted from Apple Business Manager Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5b0fb-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b0fb-158">createdDateTime</span></span>|<span data-ttu-id="5b0fb-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b0fb-159">DateTimeOffset</span></span>|<span data-ttu-id="5b0fb-160">Data e hora de criação do dispositivo herdadas de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5b0fb-160">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5b0fb-161">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b0fb-161">lastContactedDateTime</span></span>|<span data-ttu-id="5b0fb-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b0fb-162">DateTimeOffset</span></span>|<span data-ttu-id="5b0fb-163">Data e hora do último contato do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5b0fb-163">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5b0fb-164">description</span><span class="sxs-lookup"><span data-stu-id="5b0fb-164">description</span></span>|<span data-ttu-id="5b0fb-165">String</span><span class="sxs-lookup"><span data-stu-id="5b0fb-165">String</span></span>|<span data-ttu-id="5b0fb-166">A descrição do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5b0fb-166">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5b0fb-167">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="5b0fb-167">enrollmentState</span></span>|[<span data-ttu-id="5b0fb-168">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="5b0fb-168">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="5b0fb-169">O estado do dispositivo no Intune herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="5b0fb-169">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="5b0fb-170">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="5b0fb-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="5b0fb-171">plataforma</span><span class="sxs-lookup"><span data-stu-id="5b0fb-171">platform</span></span>|[<span data-ttu-id="5b0fb-172">plataforma</span><span class="sxs-lookup"><span data-stu-id="5b0fb-172">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="5b0fb-173">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b0fb-173">The platform of the Device.</span></span> <span data-ttu-id="5b0fb-174">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="5b0fb-174">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="5b0fb-175">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="5b0fb-175">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="5b0fb-176">status</span><span class="sxs-lookup"><span data-stu-id="5b0fb-176">status</span></span>|<span data-ttu-id="5b0fb-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="5b0fb-177">Boolean</span></span>|<span data-ttu-id="5b0fb-178">Status da identidade do dispositivo importado</span><span class="sxs-lookup"><span data-stu-id="5b0fb-178">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="5b0fb-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b0fb-179">Response</span></span>
<span data-ttu-id="5b0fb-180">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b0fb-180">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b0fb-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b0fb-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b0fb-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b0fb-182">Request</span></span>
<span data-ttu-id="5b0fb-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b0fb-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b0fb-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b0fb-184">Response</span></span>
<span data-ttu-id="5b0fb-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b0fb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





