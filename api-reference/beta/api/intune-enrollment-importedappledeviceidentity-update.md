---
title: Atualizar importedAppleDeviceIdentity
description: Atualiza as propriedades de um objeto importedAppleDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 501a8bb31d5b01b184f4a53bb4f68fbd27661675
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982333"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="48b68-103">Atualizar importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="48b68-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="48b68-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48b68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48b68-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48b68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48b68-106">Atualiza as propriedades de um objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="48b68-106">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48b68-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="48b68-107">Prerequisites</span></span>
<span data-ttu-id="48b68-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48b68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48b68-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48b68-110">Permission type</span></span>|<span data-ttu-id="48b68-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="48b68-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48b68-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48b68-112">Delegated (work or school account)</span></span>|<span data-ttu-id="48b68-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48b68-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="48b68-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48b68-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48b68-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48b68-115">Not supported.</span></span>|
|<span data-ttu-id="48b68-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48b68-116">Application</span></span>|<span data-ttu-id="48b68-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48b68-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48b68-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48b68-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="48b68-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48b68-119">Request headers</span></span>
|<span data-ttu-id="48b68-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="48b68-120">Header</span></span>|<span data-ttu-id="48b68-121">Valor</span><span class="sxs-lookup"><span data-stu-id="48b68-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48b68-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="48b68-122">Authorization</span></span>|<span data-ttu-id="48b68-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48b68-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48b68-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="48b68-124">Accept</span></span>|<span data-ttu-id="48b68-125">application/json</span><span class="sxs-lookup"><span data-stu-id="48b68-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48b68-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48b68-126">Request body</span></span>
<span data-ttu-id="48b68-127">No corpo da solicitação, forneça uma representação JSON do objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="48b68-127">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="48b68-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="48b68-128">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="48b68-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48b68-129">Property</span></span>|<span data-ttu-id="48b68-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="48b68-130">Type</span></span>|<span data-ttu-id="48b68-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="48b68-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48b68-132">id</span><span class="sxs-lookup"><span data-stu-id="48b68-132">id</span></span>|<span data-ttu-id="48b68-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48b68-133">String</span></span>|<span data-ttu-id="48b68-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="48b68-134">Key of the entity.</span></span>|
|<span data-ttu-id="48b68-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="48b68-135">serialNumber</span></span>|<span data-ttu-id="48b68-136">String</span><span class="sxs-lookup"><span data-stu-id="48b68-136">String</span></span>|<span data-ttu-id="48b68-137">Número de série do dispositivo</span><span class="sxs-lookup"><span data-stu-id="48b68-137">Device serial number</span></span>|
|<span data-ttu-id="48b68-138">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="48b68-138">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="48b68-139">String</span><span class="sxs-lookup"><span data-stu-id="48b68-139">String</span></span>|<span data-ttu-id="48b68-140">ID do perfil de registro o administrador pretende aplicar ao dispositivo durante o próximo registro</span><span class="sxs-lookup"><span data-stu-id="48b68-140">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="48b68-141">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="48b68-141">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="48b68-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48b68-142">DateTimeOffset</span></span>|<span data-ttu-id="48b68-143">O perfil de registro de tempo foi atribuído ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="48b68-143">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="48b68-144">isSupervised</span><span class="sxs-lookup"><span data-stu-id="48b68-144">isSupervised</span></span>|<span data-ttu-id="48b68-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="48b68-145">Boolean</span></span>|<span data-ttu-id="48b68-146">Indica se o dispositivo Apple é supervisionado.</span><span class="sxs-lookup"><span data-stu-id="48b68-146">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="48b68-147">Mais informações em:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="48b68-147">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="48b68-148">discoverySource</span><span class="sxs-lookup"><span data-stu-id="48b68-148">discoverySource</span></span>|[<span data-ttu-id="48b68-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="48b68-149">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="48b68-150">Fonte de descoberta de dispositivos Apple.</span><span class="sxs-lookup"><span data-stu-id="48b68-150">Apple device discovery source.</span></span> <span data-ttu-id="48b68-151">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="48b68-151">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="48b68-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48b68-152">createdDateTime</span></span>|<span data-ttu-id="48b68-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48b68-153">DateTimeOffset</span></span>|<span data-ttu-id="48b68-154">Data e hora de criação do dispositivo</span><span class="sxs-lookup"><span data-stu-id="48b68-154">Created Date Time of the device</span></span>|
|<span data-ttu-id="48b68-155">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="48b68-155">lastContactedDateTime</span></span>|<span data-ttu-id="48b68-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48b68-156">DateTimeOffset</span></span>|<span data-ttu-id="48b68-157">Data e hora do último contato do dispositivo</span><span class="sxs-lookup"><span data-stu-id="48b68-157">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="48b68-158">descrição</span><span class="sxs-lookup"><span data-stu-id="48b68-158">description</span></span>|<span data-ttu-id="48b68-159">String</span><span class="sxs-lookup"><span data-stu-id="48b68-159">String</span></span>|<span data-ttu-id="48b68-160">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="48b68-160">The description of the device</span></span>|
|<span data-ttu-id="48b68-161">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="48b68-161">enrollmentState</span></span>|[<span data-ttu-id="48b68-162">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="48b68-162">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="48b68-163">O estado do dispositivo no Intune.</span><span class="sxs-lookup"><span data-stu-id="48b68-163">The state of the device in Intune.</span></span> <span data-ttu-id="48b68-164">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="48b68-164">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="48b68-165">platform</span><span class="sxs-lookup"><span data-stu-id="48b68-165">platform</span></span>|[<span data-ttu-id="48b68-166">plataforma</span><span class="sxs-lookup"><span data-stu-id="48b68-166">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="48b68-167">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="48b68-167">The platform of the Device.</span></span> <span data-ttu-id="48b68-168">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="48b68-168">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="48b68-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="48b68-169">Response</span></span>
<span data-ttu-id="48b68-170">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48b68-170">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48b68-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48b68-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="48b68-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48b68-172">Request</span></span>
<span data-ttu-id="48b68-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48b68-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="48b68-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="48b68-174">Response</span></span>
<span data-ttu-id="48b68-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48b68-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





