---
title: Atualizar importedAppleDeviceIdentity
description: Atualize as propriedades de um objeto importedAppleDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c280965a3624bd86fc91290b9a517c89986c0aa
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867564"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="95d79-103">Atualizar importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="95d79-103">Update importedAppleDeviceIdentity</span></span>

<span data-ttu-id="95d79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95d79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95d79-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="95d79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95d79-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95d79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95d79-107">Atualize as propriedades de [um objeto importedAppleDeviceIdentity.](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="95d79-107">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95d79-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="95d79-108">Prerequisites</span></span>
<span data-ttu-id="95d79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95d79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95d79-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95d79-111">Permission type</span></span>|<span data-ttu-id="95d79-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95d79-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95d79-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95d79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95d79-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95d79-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="95d79-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95d79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95d79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95d79-116">Not supported.</span></span>|
|<span data-ttu-id="95d79-117">Application</span><span class="sxs-lookup"><span data-stu-id="95d79-117">Application</span></span>|<span data-ttu-id="95d79-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95d79-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95d79-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95d79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="95d79-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95d79-120">Request headers</span></span>
|<span data-ttu-id="95d79-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95d79-121">Header</span></span>|<span data-ttu-id="95d79-122">Valor</span><span class="sxs-lookup"><span data-stu-id="95d79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95d79-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="95d79-123">Authorization</span></span>|<span data-ttu-id="95d79-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95d79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95d79-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="95d79-125">Accept</span></span>|<span data-ttu-id="95d79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95d79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95d79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95d79-127">Request body</span></span>
<span data-ttu-id="95d79-128">No corpo da solicitação, fornece uma representação JSON para o [objeto importedAppleDeviceIdentity.](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="95d79-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="95d79-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [importAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="95d79-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="95d79-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95d79-130">Property</span></span>|<span data-ttu-id="95d79-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="95d79-131">Type</span></span>|<span data-ttu-id="95d79-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="95d79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95d79-133">id</span><span class="sxs-lookup"><span data-stu-id="95d79-133">id</span></span>|<span data-ttu-id="95d79-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95d79-134">String</span></span>|<span data-ttu-id="95d79-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="95d79-135">Key of the entity.</span></span>|
|<span data-ttu-id="95d79-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="95d79-136">serialNumber</span></span>|<span data-ttu-id="95d79-137">String</span><span class="sxs-lookup"><span data-stu-id="95d79-137">String</span></span>|<span data-ttu-id="95d79-138">Número de série do dispositivo</span><span class="sxs-lookup"><span data-stu-id="95d79-138">Device serial number</span></span>|
|<span data-ttu-id="95d79-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="95d79-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="95d79-140">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="95d79-140">String</span></span>|<span data-ttu-id="95d79-141">O administrador de ID do perfil de registro pretende aplicar-se ao dispositivo durante o próximo registro</span><span class="sxs-lookup"><span data-stu-id="95d79-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="95d79-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="95d79-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="95d79-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95d79-143">DateTimeOffset</span></span>|<span data-ttu-id="95d79-144">O perfil de registro de hora foi atribuído ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="95d79-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="95d79-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="95d79-145">isSupervised</span></span>|<span data-ttu-id="95d79-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="95d79-146">Boolean</span></span>|<span data-ttu-id="95d79-147">Indica se o dispositivo Apple é supervisionado.</span><span class="sxs-lookup"><span data-stu-id="95d79-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="95d79-148">Mais informações estão em: https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="95d79-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="95d79-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="95d79-149">discoverySource</span></span>|[<span data-ttu-id="95d79-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="95d79-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="95d79-151">Fonte de descoberta de dispositivo Apple.</span><span class="sxs-lookup"><span data-stu-id="95d79-151">Apple device discovery source.</span></span> <span data-ttu-id="95d79-152">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="95d79-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="95d79-153">isDeleted</span><span class="sxs-lookup"><span data-stu-id="95d79-153">isDeleted</span></span>|<span data-ttu-id="95d79-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="95d79-154">Boolean</span></span>|<span data-ttu-id="95d79-155">Indica se o dispositivo é excluído do Apple Business Manager</span><span class="sxs-lookup"><span data-stu-id="95d79-155">Indicates if the device is deleted from Apple Business Manager</span></span>|
|<span data-ttu-id="95d79-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95d79-156">createdDateTime</span></span>|<span data-ttu-id="95d79-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95d79-157">DateTimeOffset</span></span>|<span data-ttu-id="95d79-158">Data de criação hora do dispositivo</span><span class="sxs-lookup"><span data-stu-id="95d79-158">Created Date Time of the device</span></span>|
|<span data-ttu-id="95d79-159">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="95d79-159">lastContactedDateTime</span></span>|<span data-ttu-id="95d79-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95d79-160">DateTimeOffset</span></span>|<span data-ttu-id="95d79-161">Hora da Última Data Contata do dispositivo</span><span class="sxs-lookup"><span data-stu-id="95d79-161">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="95d79-162">description</span><span class="sxs-lookup"><span data-stu-id="95d79-162">description</span></span>|<span data-ttu-id="95d79-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95d79-163">String</span></span>|<span data-ttu-id="95d79-164">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="95d79-164">The description of the device</span></span>|
|<span data-ttu-id="95d79-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="95d79-165">enrollmentState</span></span>|[<span data-ttu-id="95d79-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="95d79-166">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="95d79-167">O estado do dispositivo no Intune.</span><span class="sxs-lookup"><span data-stu-id="95d79-167">The state of the device in Intune.</span></span> <span data-ttu-id="95d79-168">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="95d79-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="95d79-169">plataforma</span><span class="sxs-lookup"><span data-stu-id="95d79-169">platform</span></span>|[<span data-ttu-id="95d79-170">platform</span><span class="sxs-lookup"><span data-stu-id="95d79-170">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="95d79-171">A plataforma do Dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95d79-171">The platform of the Device.</span></span> <span data-ttu-id="95d79-172">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="95d79-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="95d79-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="95d79-173">Response</span></span>
<span data-ttu-id="95d79-174">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95d79-174">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95d79-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95d79-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="95d79-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95d79-176">Request</span></span>
<span data-ttu-id="95d79-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95d79-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="95d79-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="95d79-178">Response</span></span>
<span data-ttu-id="95d79-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95d79-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




