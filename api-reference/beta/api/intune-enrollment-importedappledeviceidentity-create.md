---
title: Criar importedAppleDeviceIdentity
description: Criar um novo objeto importedAppleDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 958f63a8dc64fc0a4b554cc29846a00d8fdf221c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451240"
---
# <a name="create-importedappledeviceidentity"></a><span data-ttu-id="9b497-103">Criar importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="9b497-103">Create importedAppleDeviceIdentity</span></span>

<span data-ttu-id="9b497-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b497-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b497-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9b497-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b497-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b497-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b497-107">Criar um novo objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="9b497-107">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b497-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9b497-108">Prerequisites</span></span>
<span data-ttu-id="9b497-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b497-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b497-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b497-111">Permission type</span></span>|<span data-ttu-id="9b497-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9b497-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b497-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b497-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b497-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b497-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9b497-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b497-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b497-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b497-116">Not supported.</span></span>|
|<span data-ttu-id="9b497-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b497-117">Application</span></span>|<span data-ttu-id="9b497-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b497-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b497-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b497-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="9b497-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b497-120">Request headers</span></span>
|<span data-ttu-id="9b497-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9b497-121">Header</span></span>|<span data-ttu-id="9b497-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9b497-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b497-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b497-123">Authorization</span></span>|<span data-ttu-id="9b497-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b497-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b497-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9b497-125">Accept</span></span>|<span data-ttu-id="9b497-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b497-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b497-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b497-127">Request body</span></span>
<span data-ttu-id="9b497-128">No corpo da solicitação, forneça uma representação JSON do objeto importedAppleDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="9b497-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentity object.</span></span>

<span data-ttu-id="9b497-129">A tabela a seguir mostra as propriedades que são necessárias ao criar importedAppleDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="9b497-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentity.</span></span>

|<span data-ttu-id="9b497-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b497-130">Property</span></span>|<span data-ttu-id="9b497-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b497-131">Type</span></span>|<span data-ttu-id="9b497-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b497-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b497-133">id</span><span class="sxs-lookup"><span data-stu-id="9b497-133">id</span></span>|<span data-ttu-id="9b497-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b497-134">String</span></span>|<span data-ttu-id="9b497-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9b497-135">Key of the entity.</span></span>|
|<span data-ttu-id="9b497-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="9b497-136">serialNumber</span></span>|<span data-ttu-id="9b497-137">String</span><span class="sxs-lookup"><span data-stu-id="9b497-137">String</span></span>|<span data-ttu-id="9b497-138">Número de série do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9b497-138">Device serial number</span></span>|
|<span data-ttu-id="9b497-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="9b497-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="9b497-140">String</span><span class="sxs-lookup"><span data-stu-id="9b497-140">String</span></span>|<span data-ttu-id="9b497-141">ID do perfil de registro o administrador pretende aplicar ao dispositivo durante o próximo registro</span><span class="sxs-lookup"><span data-stu-id="9b497-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="9b497-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="9b497-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="9b497-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b497-143">DateTimeOffset</span></span>|<span data-ttu-id="9b497-144">O perfil de registro de tempo foi atribuído ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="9b497-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="9b497-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="9b497-145">isSupervised</span></span>|<span data-ttu-id="9b497-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b497-146">Boolean</span></span>|<span data-ttu-id="9b497-147">Indica se o dispositivo Apple é supervisionado.</span><span class="sxs-lookup"><span data-stu-id="9b497-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="9b497-148">Mais informações em:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="9b497-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="9b497-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="9b497-149">discoverySource</span></span>|[<span data-ttu-id="9b497-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="9b497-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="9b497-151">Fonte de descoberta de dispositivos Apple.</span><span class="sxs-lookup"><span data-stu-id="9b497-151">Apple device discovery source.</span></span> <span data-ttu-id="9b497-152">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="9b497-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="9b497-153">isDeleted</span><span class="sxs-lookup"><span data-stu-id="9b497-153">isDeleted</span></span>|<span data-ttu-id="9b497-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b497-154">Boolean</span></span>|<span data-ttu-id="9b497-155">Indica se o dispositivo é excluído do Apple Business Manager</span><span class="sxs-lookup"><span data-stu-id="9b497-155">Indicates if the device is deleted from Apple Business Manager</span></span>|
|<span data-ttu-id="9b497-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b497-156">createdDateTime</span></span>|<span data-ttu-id="9b497-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b497-157">DateTimeOffset</span></span>|<span data-ttu-id="9b497-158">Data e hora de criação do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9b497-158">Created Date Time of the device</span></span>|
|<span data-ttu-id="9b497-159">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b497-159">lastContactedDateTime</span></span>|<span data-ttu-id="9b497-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b497-160">DateTimeOffset</span></span>|<span data-ttu-id="9b497-161">Data e hora do último contato do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9b497-161">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="9b497-162">description</span><span class="sxs-lookup"><span data-stu-id="9b497-162">description</span></span>|<span data-ttu-id="9b497-163">String</span><span class="sxs-lookup"><span data-stu-id="9b497-163">String</span></span>|<span data-ttu-id="9b497-164">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9b497-164">The description of the device</span></span>|
|<span data-ttu-id="9b497-165">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="9b497-165">enrollmentState</span></span>|[<span data-ttu-id="9b497-166">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="9b497-166">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="9b497-167">O estado do dispositivo no Intune.</span><span class="sxs-lookup"><span data-stu-id="9b497-167">The state of the device in Intune.</span></span> <span data-ttu-id="9b497-168">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="9b497-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="9b497-169">platform</span><span class="sxs-lookup"><span data-stu-id="9b497-169">platform</span></span>|[<span data-ttu-id="9b497-170">plataforma</span><span class="sxs-lookup"><span data-stu-id="9b497-170">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="9b497-171">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9b497-171">The platform of the Device.</span></span> <span data-ttu-id="9b497-172">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="9b497-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="9b497-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b497-173">Response</span></span>
<span data-ttu-id="9b497-174">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b497-174">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b497-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b497-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b497-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b497-176">Request</span></span>
<span data-ttu-id="9b497-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b497-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9b497-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b497-178">Response</span></span>
<span data-ttu-id="9b497-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b497-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



