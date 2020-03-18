---
title: Atualizar importedAppleDeviceIdentity
description: Atualiza as propriedades de um objeto importedAppleDeviceIdentity.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b1d6836aa23b32418bed1c2cf19e06f82cc661c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813094"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="a1409-103">Atualizar importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a1409-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="a1409-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1409-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1409-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1409-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1409-106">Atualiza as propriedades de um objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="a1409-106">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1409-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1409-107">Prerequisites</span></span>
<span data-ttu-id="a1409-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1409-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1409-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1409-110">Permission type</span></span>|<span data-ttu-id="a1409-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1409-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1409-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1409-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1409-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1409-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a1409-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1409-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1409-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1409-115">Not supported.</span></span>|
|<span data-ttu-id="a1409-116">Application</span><span class="sxs-lookup"><span data-stu-id="a1409-116">Application</span></span>|<span data-ttu-id="a1409-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1409-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1409-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1409-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="a1409-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1409-119">Request headers</span></span>
|<span data-ttu-id="a1409-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1409-120">Header</span></span>|<span data-ttu-id="a1409-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a1409-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1409-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1409-122">Authorization</span></span>|<span data-ttu-id="a1409-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1409-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1409-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1409-124">Accept</span></span>|<span data-ttu-id="a1409-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1409-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1409-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1409-126">Request body</span></span>
<span data-ttu-id="a1409-127">No corpo da solicitação, forneça uma representação JSON do objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="a1409-127">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="a1409-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="a1409-128">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="a1409-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1409-129">Property</span></span>|<span data-ttu-id="a1409-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1409-130">Type</span></span>|<span data-ttu-id="a1409-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1409-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1409-132">id</span><span class="sxs-lookup"><span data-stu-id="a1409-132">id</span></span>|<span data-ttu-id="a1409-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1409-133">String</span></span>|<span data-ttu-id="a1409-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a1409-134">Key of the entity.</span></span>|
|<span data-ttu-id="a1409-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="a1409-135">serialNumber</span></span>|<span data-ttu-id="a1409-136">String</span><span class="sxs-lookup"><span data-stu-id="a1409-136">String</span></span>|<span data-ttu-id="a1409-137">Número de série do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a1409-137">Device serial number</span></span>|
|<span data-ttu-id="a1409-138">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="a1409-138">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="a1409-139">String</span><span class="sxs-lookup"><span data-stu-id="a1409-139">String</span></span>|<span data-ttu-id="a1409-140">ID do perfil de registro o administrador pretende aplicar ao dispositivo durante o próximo registro</span><span class="sxs-lookup"><span data-stu-id="a1409-140">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="a1409-141">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="a1409-141">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="a1409-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1409-142">DateTimeOffset</span></span>|<span data-ttu-id="a1409-143">O perfil de registro de tempo foi atribuído ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="a1409-143">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="a1409-144">isSupervised</span><span class="sxs-lookup"><span data-stu-id="a1409-144">isSupervised</span></span>|<span data-ttu-id="a1409-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1409-145">Boolean</span></span>|<span data-ttu-id="a1409-146">Indica se o dispositivo Apple é supervisionado.</span><span class="sxs-lookup"><span data-stu-id="a1409-146">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="a1409-147">Mais informações em:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="a1409-147">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="a1409-148">discoverySource</span><span class="sxs-lookup"><span data-stu-id="a1409-148">discoverySource</span></span>|[<span data-ttu-id="a1409-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="a1409-149">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="a1409-150">Fonte de descoberta de dispositivos Apple.</span><span class="sxs-lookup"><span data-stu-id="a1409-150">Apple device discovery source.</span></span> <span data-ttu-id="a1409-151">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="a1409-151">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="a1409-152">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a1409-152">isDeleted</span></span>|<span data-ttu-id="a1409-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1409-153">Boolean</span></span>|<span data-ttu-id="a1409-154">Indica se o dispositivo é excluído do Apple Business Manager</span><span class="sxs-lookup"><span data-stu-id="a1409-154">Indicates if the device is deleted from Apple Business Manager</span></span>|
|<span data-ttu-id="a1409-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1409-155">createdDateTime</span></span>|<span data-ttu-id="a1409-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1409-156">DateTimeOffset</span></span>|<span data-ttu-id="a1409-157">Data e hora de criação do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a1409-157">Created Date Time of the device</span></span>|
|<span data-ttu-id="a1409-158">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1409-158">lastContactedDateTime</span></span>|<span data-ttu-id="a1409-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1409-159">DateTimeOffset</span></span>|<span data-ttu-id="a1409-160">Data e hora do último contato do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a1409-160">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="a1409-161">description</span><span class="sxs-lookup"><span data-stu-id="a1409-161">description</span></span>|<span data-ttu-id="a1409-162">String</span><span class="sxs-lookup"><span data-stu-id="a1409-162">String</span></span>|<span data-ttu-id="a1409-163">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a1409-163">The description of the device</span></span>|
|<span data-ttu-id="a1409-164">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="a1409-164">enrollmentState</span></span>|[<span data-ttu-id="a1409-165">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="a1409-165">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="a1409-166">O estado do dispositivo no Intune.</span><span class="sxs-lookup"><span data-stu-id="a1409-166">The state of the device in Intune.</span></span> <span data-ttu-id="a1409-167">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="a1409-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="a1409-168">platform</span><span class="sxs-lookup"><span data-stu-id="a1409-168">platform</span></span>|[<span data-ttu-id="a1409-169">plataforma</span><span class="sxs-lookup"><span data-stu-id="a1409-169">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="a1409-170">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1409-170">The platform of the Device.</span></span> <span data-ttu-id="a1409-171">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="a1409-171">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="a1409-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1409-172">Response</span></span>
<span data-ttu-id="a1409-173">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1409-173">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1409-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1409-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1409-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1409-175">Request</span></span>
<span data-ttu-id="a1409-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1409-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 519

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "isDeleted": true,
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="a1409-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1409-177">Response</span></span>
<span data-ttu-id="a1409-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1409-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 627

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
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
  "platform": "ios"
}
```




