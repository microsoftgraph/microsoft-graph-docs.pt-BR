---
title: Atualizar importedAppleDeviceIdentityResult
description: Atualiza as propriedades de um objeto importedAppleDeviceIdentityResult.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c52a6c6dc591a2ccb5c8bd71dbc7f5c074d8564
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969600"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="ff560-103">Atualizar importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="ff560-103">Update importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="ff560-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff560-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff560-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff560-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff560-106">Atualiza as propriedades de um objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="ff560-106">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff560-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff560-107">Prerequisites</span></span>
<span data-ttu-id="ff560-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff560-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff560-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff560-110">Permission type</span></span>|<span data-ttu-id="ff560-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff560-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff560-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff560-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ff560-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff560-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ff560-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff560-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff560-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff560-115">Not supported.</span></span>|
|<span data-ttu-id="ff560-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff560-116">Application</span></span>|<span data-ttu-id="ff560-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff560-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff560-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff560-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="ff560-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff560-119">Request headers</span></span>
|<span data-ttu-id="ff560-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff560-120">Header</span></span>|<span data-ttu-id="ff560-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ff560-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff560-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff560-122">Authorization</span></span>|<span data-ttu-id="ff560-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff560-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff560-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff560-124">Accept</span></span>|<span data-ttu-id="ff560-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ff560-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff560-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff560-126">Request body</span></span>
<span data-ttu-id="ff560-127">No corpo da solicitação, forneça uma representação JSON do objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="ff560-127">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="ff560-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="ff560-128">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="ff560-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff560-129">Property</span></span>|<span data-ttu-id="ff560-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff560-130">Type</span></span>|<span data-ttu-id="ff560-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff560-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff560-132">id</span><span class="sxs-lookup"><span data-stu-id="ff560-132">id</span></span>|<span data-ttu-id="ff560-133">String</span><span class="sxs-lookup"><span data-stu-id="ff560-133">String</span></span>|<span data-ttu-id="ff560-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ff560-134">Key of the entity.</span></span> <span data-ttu-id="ff560-135">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ff560-135">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="ff560-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ff560-136">serialNumber</span></span>|<span data-ttu-id="ff560-137">String</span><span class="sxs-lookup"><span data-stu-id="ff560-137">String</span></span>|<span data-ttu-id="ff560-138">Número de série do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ff560-138">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="ff560-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="ff560-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="ff560-140">String</span><span class="sxs-lookup"><span data-stu-id="ff560-140">String</span></span>|<span data-ttu-id="ff560-141">ID de perfil de registro o administrador pretende aplicar ao dispositivo durante o próximo registro herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ff560-141">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="ff560-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="ff560-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="ff560-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff560-143">DateTimeOffset</span></span>|<span data-ttu-id="ff560-144">O perfil de registro de tempo foi atribuído ao dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ff560-144">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="ff560-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="ff560-145">isSupervised</span></span>|<span data-ttu-id="ff560-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff560-146">Boolean</span></span>|<span data-ttu-id="ff560-147">Indica se o dispositivo Apple é supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ff560-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="ff560-148">Mais informações em: https://support.apple.com/en-us/HT202837 herdadas de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ff560-148">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="ff560-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="ff560-149">discoverySource</span></span>|[<span data-ttu-id="ff560-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="ff560-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="ff560-151">Fonte de descoberta de dispositivos Apple.</span><span class="sxs-lookup"><span data-stu-id="ff560-151">Apple device discovery source.</span></span> <span data-ttu-id="ff560-152">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="ff560-152">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="ff560-153">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="ff560-153">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="ff560-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff560-154">createdDateTime</span></span>|<span data-ttu-id="ff560-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff560-155">DateTimeOffset</span></span>|<span data-ttu-id="ff560-156">Data e hora de criação do dispositivo herdadas de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ff560-156">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="ff560-157">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff560-157">lastContactedDateTime</span></span>|<span data-ttu-id="ff560-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff560-158">DateTimeOffset</span></span>|<span data-ttu-id="ff560-159">Data e hora do último contato do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ff560-159">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="ff560-160">descrição</span><span class="sxs-lookup"><span data-stu-id="ff560-160">description</span></span>|<span data-ttu-id="ff560-161">String</span><span class="sxs-lookup"><span data-stu-id="ff560-161">String</span></span>|<span data-ttu-id="ff560-162">A descrição do dispositivo herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ff560-162">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="ff560-163">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="ff560-163">enrollmentState</span></span>|[<span data-ttu-id="ff560-164">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="ff560-164">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="ff560-165">O estado do dispositivo no Intune herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="ff560-165">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="ff560-166">Os valores possíveis são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="ff560-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="ff560-167">platform</span><span class="sxs-lookup"><span data-stu-id="ff560-167">platform</span></span>|[<span data-ttu-id="ff560-168">plataforma</span><span class="sxs-lookup"><span data-stu-id="ff560-168">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="ff560-169">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff560-169">The platform of the Device.</span></span> <span data-ttu-id="ff560-170">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="ff560-170">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="ff560-171">Os valores possíveis são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="ff560-171">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="ff560-172">status</span><span class="sxs-lookup"><span data-stu-id="ff560-172">status</span></span>|<span data-ttu-id="ff560-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff560-173">Boolean</span></span>|<span data-ttu-id="ff560-174">Status da identidade do dispositivo importado</span><span class="sxs-lookup"><span data-stu-id="ff560-174">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="ff560-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff560-175">Response</span></span>
<span data-ttu-id="ff560-176">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff560-176">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff560-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff560-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff560-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff560-178">Request</span></span>
<span data-ttu-id="ff560-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff560-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ff560-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff560-180">Response</span></span>
<span data-ttu-id="ff560-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff560-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




