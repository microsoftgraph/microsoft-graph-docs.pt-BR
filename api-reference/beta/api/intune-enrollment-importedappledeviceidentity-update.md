---
title: Atualizar importedAppleDeviceIdentity
description: Atualiza as propriedades de um objeto importedAppleDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6ca19f2b386da467ea3b71e1a95c6a30ad205787
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122620"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="403c5-103">Atualizar importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="403c5-103">Update importedAppleDeviceIdentity</span></span>

<span data-ttu-id="403c5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="403c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="403c5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="403c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="403c5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="403c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="403c5-107">Atualiza as propriedades de um objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="403c5-107">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="403c5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="403c5-108">Prerequisites</span></span>
<span data-ttu-id="403c5-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="403c5-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="403c5-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="403c5-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="403c5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="403c5-111">Permission type</span></span>|<span data-ttu-id="403c5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="403c5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="403c5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="403c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="403c5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="403c5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="403c5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="403c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="403c5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="403c5-116">Not supported.</span></span>|
|<span data-ttu-id="403c5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="403c5-117">Application</span></span>|<span data-ttu-id="403c5-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="403c5-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="403c5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="403c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="403c5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="403c5-120">Request headers</span></span>
|<span data-ttu-id="403c5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="403c5-121">Header</span></span>|<span data-ttu-id="403c5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="403c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="403c5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="403c5-123">Authorization</span></span>|<span data-ttu-id="403c5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="403c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="403c5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="403c5-125">Accept</span></span>|<span data-ttu-id="403c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="403c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="403c5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="403c5-127">Request body</span></span>
<span data-ttu-id="403c5-128">No corpo da solicitação, forneça uma representação JSON do objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="403c5-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="403c5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="403c5-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="403c5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="403c5-130">Property</span></span>|<span data-ttu-id="403c5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="403c5-131">Type</span></span>|<span data-ttu-id="403c5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="403c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="403c5-133">id</span><span class="sxs-lookup"><span data-stu-id="403c5-133">id</span></span>|<span data-ttu-id="403c5-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="403c5-134">String</span></span>|<span data-ttu-id="403c5-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="403c5-135">Key of the entity.</span></span>|
|<span data-ttu-id="403c5-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="403c5-136">serialNumber</span></span>|<span data-ttu-id="403c5-137">String</span><span class="sxs-lookup"><span data-stu-id="403c5-137">String</span></span>|<span data-ttu-id="403c5-138">Número de série do dispositivo</span><span class="sxs-lookup"><span data-stu-id="403c5-138">Device serial number</span></span>|
|<span data-ttu-id="403c5-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="403c5-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="403c5-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="403c5-140">String</span></span>|<span data-ttu-id="403c5-141">ID do perfil de registro o administrador pretende aplicar ao dispositivo durante o próximo registro</span><span class="sxs-lookup"><span data-stu-id="403c5-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="403c5-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="403c5-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="403c5-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="403c5-143">DateTimeOffset</span></span>|<span data-ttu-id="403c5-144">O perfil de registro de tempo foi atribuído ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="403c5-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="403c5-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="403c5-145">isSupervised</span></span>|<span data-ttu-id="403c5-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="403c5-146">Boolean</span></span>|<span data-ttu-id="403c5-147">Indica se o dispositivo Apple é supervisionado.</span><span class="sxs-lookup"><span data-stu-id="403c5-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="403c5-148">Mais informações em:https://support.apple.com/HT202837</span><span class="sxs-lookup"><span data-stu-id="403c5-148">More information is at: https://support.apple.com/HT202837</span></span>|
|<span data-ttu-id="403c5-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="403c5-149">discoverySource</span></span>|[<span data-ttu-id="403c5-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="403c5-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="403c5-151">Fonte de descoberta de dispositivos Apple.</span><span class="sxs-lookup"><span data-stu-id="403c5-151">Apple device discovery source.</span></span> <span data-ttu-id="403c5-152">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="403c5-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="403c5-153">isDeleted</span><span class="sxs-lookup"><span data-stu-id="403c5-153">isDeleted</span></span>|<span data-ttu-id="403c5-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="403c5-154">Boolean</span></span>|<span data-ttu-id="403c5-155">Indica se o dispositivo é excluído do Apple Business Manager</span><span class="sxs-lookup"><span data-stu-id="403c5-155">Indicates if the device is deleted from Apple Business Manager</span></span>|
|<span data-ttu-id="403c5-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="403c5-156">createdDateTime</span></span>|<span data-ttu-id="403c5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="403c5-157">DateTimeOffset</span></span>|<span data-ttu-id="403c5-158">Data e hora de criação do dispositivo</span><span class="sxs-lookup"><span data-stu-id="403c5-158">Created Date Time of the device</span></span>|
|<span data-ttu-id="403c5-159">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="403c5-159">lastContactedDateTime</span></span>|<span data-ttu-id="403c5-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="403c5-160">DateTimeOffset</span></span>|<span data-ttu-id="403c5-161">Data e hora do último contato do dispositivo</span><span class="sxs-lookup"><span data-stu-id="403c5-161">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="403c5-162">descrição</span><span class="sxs-lookup"><span data-stu-id="403c5-162">description</span></span>|<span data-ttu-id="403c5-163">String</span><span class="sxs-lookup"><span data-stu-id="403c5-163">String</span></span>|<span data-ttu-id="403c5-164">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="403c5-164">The description of the device</span></span>|
|<span data-ttu-id="403c5-165">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="403c5-165">enrollmentState</span></span>|[<span data-ttu-id="403c5-166">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="403c5-166">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="403c5-167">O estado do dispositivo no Intune.</span><span class="sxs-lookup"><span data-stu-id="403c5-167">The state of the device in Intune.</span></span> <span data-ttu-id="403c5-168">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="403c5-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="403c5-169">platform</span><span class="sxs-lookup"><span data-stu-id="403c5-169">platform</span></span>|[<span data-ttu-id="403c5-170">plataforma</span><span class="sxs-lookup"><span data-stu-id="403c5-170">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="403c5-171">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="403c5-171">The platform of the Device.</span></span> <span data-ttu-id="403c5-172">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="403c5-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="403c5-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="403c5-173">Response</span></span>
<span data-ttu-id="403c5-174">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="403c5-174">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="403c5-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="403c5-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="403c5-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="403c5-176">Request</span></span>
<span data-ttu-id="403c5-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="403c5-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="403c5-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="403c5-178">Response</span></span>
<span data-ttu-id="403c5-179">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="403c5-179">Here is an example of the response.</span></span> <span data-ttu-id="403c5-180">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="403c5-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="403c5-181">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="403c5-181">All of the properties will be returned from an actual call.</span></span>
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



