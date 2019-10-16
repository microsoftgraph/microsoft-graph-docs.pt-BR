---
title: Criar importedAppleDeviceIdentity
description: Criar um novo objeto importedAppleDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 522e2eb48b6ccc0bd6cc56bc3fa7a32f98374d6d
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535944"
---
# <a name="create-importedappledeviceidentity"></a><span data-ttu-id="e6543-103">Criar importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="e6543-103">Create importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="e6543-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e6543-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6543-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6543-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6543-106">Criar um novo objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="e6543-106">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6543-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e6543-107">Prerequisites</span></span>
<span data-ttu-id="e6543-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6543-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6543-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6543-110">Permission type</span></span>|<span data-ttu-id="e6543-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e6543-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6543-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6543-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e6543-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6543-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e6543-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6543-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6543-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6543-115">Not supported.</span></span>|
|<span data-ttu-id="e6543-116">Application</span><span class="sxs-lookup"><span data-stu-id="e6543-116">Application</span></span>|<span data-ttu-id="e6543-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6543-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6543-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6543-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="e6543-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6543-119">Request headers</span></span>
|<span data-ttu-id="e6543-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6543-120">Header</span></span>|<span data-ttu-id="e6543-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e6543-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6543-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6543-122">Authorization</span></span>|<span data-ttu-id="e6543-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6543-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6543-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e6543-124">Accept</span></span>|<span data-ttu-id="e6543-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e6543-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6543-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6543-126">Request body</span></span>
<span data-ttu-id="e6543-127">No corpo da solicitação, forneça uma representação JSON do objeto importedAppleDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="e6543-127">In the request body, supply a JSON representation for the importedAppleDeviceIdentity object.</span></span>

<span data-ttu-id="e6543-128">A tabela a seguir mostra as propriedades que são necessárias ao criar importedAppleDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="e6543-128">The following table shows the properties that are required when you create the importedAppleDeviceIdentity.</span></span>

|<span data-ttu-id="e6543-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6543-129">Property</span></span>|<span data-ttu-id="e6543-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6543-130">Type</span></span>|<span data-ttu-id="e6543-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6543-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6543-132">id</span><span class="sxs-lookup"><span data-stu-id="e6543-132">id</span></span>|<span data-ttu-id="e6543-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6543-133">String</span></span>|<span data-ttu-id="e6543-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e6543-134">Key of the entity.</span></span>|
|<span data-ttu-id="e6543-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="e6543-135">serialNumber</span></span>|<span data-ttu-id="e6543-136">String</span><span class="sxs-lookup"><span data-stu-id="e6543-136">String</span></span>|<span data-ttu-id="e6543-137">Número de série do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e6543-137">Device serial number</span></span>|
|<span data-ttu-id="e6543-138">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="e6543-138">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="e6543-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6543-139">String</span></span>|<span data-ttu-id="e6543-140">ID do perfil de registro o administrador pretende aplicar ao dispositivo durante o próximo registro</span><span class="sxs-lookup"><span data-stu-id="e6543-140">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="e6543-141">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="e6543-141">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="e6543-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6543-142">DateTimeOffset</span></span>|<span data-ttu-id="e6543-143">O perfil de registro de tempo foi atribuído ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="e6543-143">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="e6543-144">isSupervised</span><span class="sxs-lookup"><span data-stu-id="e6543-144">isSupervised</span></span>|<span data-ttu-id="e6543-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6543-145">Boolean</span></span>|<span data-ttu-id="e6543-146">Indica se o dispositivo Apple é supervisionado.</span><span class="sxs-lookup"><span data-stu-id="e6543-146">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="e6543-147">Mais informações em:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="e6543-147">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="e6543-148">discoverySource</span><span class="sxs-lookup"><span data-stu-id="e6543-148">discoverySource</span></span>|[<span data-ttu-id="e6543-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="e6543-149">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="e6543-150">Fonte de descoberta de dispositivos Apple.</span><span class="sxs-lookup"><span data-stu-id="e6543-150">Apple device discovery source.</span></span> <span data-ttu-id="e6543-151">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="e6543-151">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="e6543-152">isDeleted</span><span class="sxs-lookup"><span data-stu-id="e6543-152">isDeleted</span></span>|<span data-ttu-id="e6543-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="e6543-153">Boolean</span></span>|<span data-ttu-id="e6543-154">Indica se o dispositivo é excluído do Apple Business Manager</span><span class="sxs-lookup"><span data-stu-id="e6543-154">Indicates if the device is deleted from Apple Business Manager</span></span>|
|<span data-ttu-id="e6543-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6543-155">createdDateTime</span></span>|<span data-ttu-id="e6543-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6543-156">DateTimeOffset</span></span>|<span data-ttu-id="e6543-157">Data e hora de criação do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e6543-157">Created Date Time of the device</span></span>|
|<span data-ttu-id="e6543-158">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6543-158">lastContactedDateTime</span></span>|<span data-ttu-id="e6543-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6543-159">DateTimeOffset</span></span>|<span data-ttu-id="e6543-160">Data e hora do último contato do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e6543-160">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="e6543-161">description</span><span class="sxs-lookup"><span data-stu-id="e6543-161">description</span></span>|<span data-ttu-id="e6543-162">String</span><span class="sxs-lookup"><span data-stu-id="e6543-162">String</span></span>|<span data-ttu-id="e6543-163">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e6543-163">The description of the device</span></span>|
|<span data-ttu-id="e6543-164">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="e6543-164">enrollmentState</span></span>|[<span data-ttu-id="e6543-165">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="e6543-165">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="e6543-166">O estado do dispositivo no Intune.</span><span class="sxs-lookup"><span data-stu-id="e6543-166">The state of the device in Intune.</span></span> <span data-ttu-id="e6543-167">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="e6543-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="e6543-168">platform</span><span class="sxs-lookup"><span data-stu-id="e6543-168">platform</span></span>|[<span data-ttu-id="e6543-169">plataforma</span><span class="sxs-lookup"><span data-stu-id="e6543-169">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="e6543-170">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e6543-170">The platform of the Device.</span></span> <span data-ttu-id="e6543-171">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="e6543-171">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="e6543-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6543-172">Response</span></span>
<span data-ttu-id="e6543-173">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6543-173">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6543-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6543-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6543-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6543-175">Request</span></span>
<span data-ttu-id="e6543-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6543-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="e6543-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6543-177">Response</span></span>
<span data-ttu-id="e6543-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6543-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






