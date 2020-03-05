---
title: Atualizar importedAppleDeviceIdentityResult
description: Atualiza as propriedades de um objeto importedAppleDeviceIdentityResult.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0963be570d436b142dd853989ba4bb36c8e1ded9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466679"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="4fd2f-103">Atualizar importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="4fd2f-103">Update importedAppleDeviceIdentityResult</span></span>

<span data-ttu-id="4fd2f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4fd2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4fd2f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4fd2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fd2f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4fd2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fd2f-107">Atualiza as propriedades de um objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="4fd2f-107">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fd2f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4fd2f-108">Prerequisites</span></span>
<span data-ttu-id="4fd2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fd2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fd2f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4fd2f-111">Permission type</span></span>|<span data-ttu-id="4fd2f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4fd2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fd2f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4fd2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4fd2f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fd2f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4fd2f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4fd2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fd2f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4fd2f-116">Not supported.</span></span>|
|<span data-ttu-id="4fd2f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4fd2f-117">Application</span></span>|<span data-ttu-id="4fd2f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fd2f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fd2f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4fd2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="4fd2f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4fd2f-120">Request headers</span></span>
|<span data-ttu-id="4fd2f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4fd2f-121">Header</span></span>|<span data-ttu-id="4fd2f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4fd2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fd2f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4fd2f-123">Authorization</span></span>|<span data-ttu-id="4fd2f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4fd2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fd2f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4fd2f-125">Accept</span></span>|<span data-ttu-id="4fd2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4fd2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fd2f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4fd2f-127">Request body</span></span>
<span data-ttu-id="4fd2f-128">No corpo da solicitação, forneça uma representação JSON do objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="4fd2f-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="4fd2f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="4fd2f-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="4fd2f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4fd2f-130">Property</span></span>|<span data-ttu-id="4fd2f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fd2f-131">Type</span></span>|<span data-ttu-id="4fd2f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fd2f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fd2f-133">id</span><span class="sxs-lookup"><span data-stu-id="4fd2f-133">id</span></span>|<span data-ttu-id="4fd2f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4fd2f-134">String</span></span>|<span data-ttu-id="4fd2f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4fd2f-135">Key of the entity.</span></span> <span data-ttu-id="4fd2f-136">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4fd2f-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="4fd2f-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="4fd2f-137">serialNumber</span></span>|<span data-ttu-id="4fd2f-138">String</span><span class="sxs-lookup"><span data-stu-id="4fd2f-138">String</span></span>|<span data-ttu-id="4fd2f-139">Número de série do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4fd2f-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="4fd2f-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="4fd2f-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="4fd2f-141">String</span><span class="sxs-lookup"><span data-stu-id="4fd2f-141">String</span></span>|<span data-ttu-id="4fd2f-142">ID de perfil de registro o administrador pretende aplicar ao dispositivo durante o próximo registro herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4fd2f-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="4fd2f-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="4fd2f-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="4fd2f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fd2f-144">DateTimeOffset</span></span>|<span data-ttu-id="4fd2f-145">O perfil de registro de tempo foi atribuído ao dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4fd2f-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="4fd2f-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="4fd2f-146">isSupervised</span></span>|<span data-ttu-id="4fd2f-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fd2f-147">Boolean</span></span>|<span data-ttu-id="4fd2f-148">Indica se o dispositivo Apple é supervisionado.</span><span class="sxs-lookup"><span data-stu-id="4fd2f-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="4fd2f-149">Mais informações em: https://support.apple.com/en-us/HT202837 herdadas de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4fd2f-149">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="4fd2f-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="4fd2f-150">discoverySource</span></span>|[<span data-ttu-id="4fd2f-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="4fd2f-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="4fd2f-152">Fonte de descoberta de dispositivos Apple.</span><span class="sxs-lookup"><span data-stu-id="4fd2f-152">Apple device discovery source.</span></span> <span data-ttu-id="4fd2f-153">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="4fd2f-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="4fd2f-154">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="4fd2f-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="4fd2f-155">isDeleted</span><span class="sxs-lookup"><span data-stu-id="4fd2f-155">isDeleted</span></span>|<span data-ttu-id="4fd2f-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fd2f-156">Boolean</span></span>|<span data-ttu-id="4fd2f-157">Indica se o dispositivo é excluído do Apple Business Manager herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4fd2f-157">Indicates if the device is deleted from Apple Business Manager Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="4fd2f-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4fd2f-158">createdDateTime</span></span>|<span data-ttu-id="4fd2f-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fd2f-159">DateTimeOffset</span></span>|<span data-ttu-id="4fd2f-160">Data e hora de criação do dispositivo herdadas de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4fd2f-160">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="4fd2f-161">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="4fd2f-161">lastContactedDateTime</span></span>|<span data-ttu-id="4fd2f-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fd2f-162">DateTimeOffset</span></span>|<span data-ttu-id="4fd2f-163">Data e hora do último contato do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4fd2f-163">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="4fd2f-164">description</span><span class="sxs-lookup"><span data-stu-id="4fd2f-164">description</span></span>|<span data-ttu-id="4fd2f-165">String</span><span class="sxs-lookup"><span data-stu-id="4fd2f-165">String</span></span>|<span data-ttu-id="4fd2f-166">A descrição do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4fd2f-166">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="4fd2f-167">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="4fd2f-167">enrollmentState</span></span>|[<span data-ttu-id="4fd2f-168">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="4fd2f-168">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="4fd2f-169">O estado do dispositivo no Intune herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="4fd2f-169">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="4fd2f-170">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="4fd2f-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="4fd2f-171">platform</span><span class="sxs-lookup"><span data-stu-id="4fd2f-171">platform</span></span>|[<span data-ttu-id="4fd2f-172">plataforma</span><span class="sxs-lookup"><span data-stu-id="4fd2f-172">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="4fd2f-173">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4fd2f-173">The platform of the Device.</span></span> <span data-ttu-id="4fd2f-174">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="4fd2f-174">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="4fd2f-175">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="4fd2f-175">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="4fd2f-176">status</span><span class="sxs-lookup"><span data-stu-id="4fd2f-176">status</span></span>|<span data-ttu-id="4fd2f-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fd2f-177">Boolean</span></span>|<span data-ttu-id="4fd2f-178">Status da identidade do dispositivo importado</span><span class="sxs-lookup"><span data-stu-id="4fd2f-178">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="4fd2f-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fd2f-179">Response</span></span>
<span data-ttu-id="4fd2f-180">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4fd2f-180">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fd2f-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4fd2f-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fd2f-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4fd2f-182">Request</span></span>
<span data-ttu-id="4fd2f-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4fd2f-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4fd2f-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fd2f-184">Response</span></span>
<span data-ttu-id="4fd2f-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4fd2f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





