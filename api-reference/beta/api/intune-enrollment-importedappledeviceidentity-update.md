---
title: Atualizar importedAppleDeviceIdentity
description: Atualize as propriedades de um objeto importedAppleDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4019621eb6f69b288575a592b59b0018582c0b06
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870501"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="eaf13-103">Atualizar importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="eaf13-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="eaf13-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eaf13-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eaf13-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eaf13-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eaf13-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="eaf13-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eaf13-107">Atualize as propriedades de um objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="eaf13-107">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eaf13-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eaf13-108">Prerequisites</span></span>
<span data-ttu-id="eaf13-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaf13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaf13-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eaf13-111">Permission type</span></span>|<span data-ttu-id="eaf13-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eaf13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eaf13-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eaf13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eaf13-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaf13-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="eaf13-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eaf13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eaf13-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eaf13-116">Not supported.</span></span>|
|<span data-ttu-id="eaf13-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eaf13-117">Application</span></span>|<span data-ttu-id="eaf13-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eaf13-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaf13-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eaf13-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="eaf13-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eaf13-120">Request headers</span></span>
|<span data-ttu-id="eaf13-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eaf13-121">Header</span></span>|<span data-ttu-id="eaf13-122">Valor</span><span class="sxs-lookup"><span data-stu-id="eaf13-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eaf13-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eaf13-123">Authorization</span></span>|<span data-ttu-id="eaf13-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eaf13-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eaf13-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eaf13-125">Accept</span></span>|<span data-ttu-id="eaf13-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eaf13-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaf13-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eaf13-127">Request body</span></span>
<span data-ttu-id="eaf13-128">No corpo da solicitação, fornece uma representação JSON para o objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="eaf13-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="eaf13-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="eaf13-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="eaf13-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eaf13-130">Property</span></span>|<span data-ttu-id="eaf13-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaf13-131">Type</span></span>|<span data-ttu-id="eaf13-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaf13-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaf13-133">id</span><span class="sxs-lookup"><span data-stu-id="eaf13-133">id</span></span>|<span data-ttu-id="eaf13-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eaf13-134">String</span></span>|<span data-ttu-id="eaf13-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="eaf13-135">Key of the entity.</span></span>|
|<span data-ttu-id="eaf13-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="eaf13-136">serialNumber</span></span>|<span data-ttu-id="eaf13-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eaf13-137">String</span></span>|<span data-ttu-id="eaf13-138">Número de série do dispositivo</span><span class="sxs-lookup"><span data-stu-id="eaf13-138">Device serial number</span></span>|
|<span data-ttu-id="eaf13-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="eaf13-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="eaf13-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eaf13-140">String</span></span>|<span data-ttu-id="eaf13-141">Administração de Id de perfil de inscrição pretende aplicáveis ao dispositivo durante o próximo registro</span><span class="sxs-lookup"><span data-stu-id="eaf13-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="eaf13-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="eaf13-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="eaf13-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaf13-143">DateTimeOffset</span></span>|<span data-ttu-id="eaf13-144">O perfil de inscrição de tempo foi atribuído ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="eaf13-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="eaf13-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="eaf13-145">isSupervised</span></span>|<span data-ttu-id="eaf13-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="eaf13-146">Boolean</span></span>|<span data-ttu-id="eaf13-147">Indica se o dispositivo Apple seja supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eaf13-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="eaf13-148">Mais informações estão em:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="eaf13-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="eaf13-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="eaf13-149">discoverySource</span></span>|[<span data-ttu-id="eaf13-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="eaf13-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="eaf13-151">Fonte de descoberta do dispositivo Apple.</span><span class="sxs-lookup"><span data-stu-id="eaf13-151">Apple device discovery source.</span></span> <span data-ttu-id="eaf13-152">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="eaf13-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="eaf13-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eaf13-153">createdDateTime</span></span>|<span data-ttu-id="eaf13-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaf13-154">DateTimeOffset</span></span>|<span data-ttu-id="eaf13-155">Criada data hora do dispositivo</span><span class="sxs-lookup"><span data-stu-id="eaf13-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="eaf13-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="eaf13-156">lastContactedDateTime</span></span>|<span data-ttu-id="eaf13-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaf13-157">DateTimeOffset</span></span>|<span data-ttu-id="eaf13-158">Última contatado data hora do dispositivo</span><span class="sxs-lookup"><span data-stu-id="eaf13-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="eaf13-159">description</span><span class="sxs-lookup"><span data-stu-id="eaf13-159">description</span></span>|<span data-ttu-id="eaf13-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eaf13-160">String</span></span>|<span data-ttu-id="eaf13-161">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="eaf13-161">The description of the device</span></span>|
|<span data-ttu-id="eaf13-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="eaf13-162">enrollmentState</span></span>|[<span data-ttu-id="eaf13-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="eaf13-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="eaf13-164">O estado do dispositivo em Intune.</span><span class="sxs-lookup"><span data-stu-id="eaf13-164">The state of the device in Intune.</span></span> <span data-ttu-id="eaf13-165">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="eaf13-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="eaf13-166">platform</span><span class="sxs-lookup"><span data-stu-id="eaf13-166">platform</span></span>|[<span data-ttu-id="eaf13-167">plataforma</span><span class="sxs-lookup"><span data-stu-id="eaf13-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="eaf13-168">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eaf13-168">The platform of the Device.</span></span> <span data-ttu-id="eaf13-169">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="eaf13-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="eaf13-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaf13-170">Response</span></span>
<span data-ttu-id="eaf13-171">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eaf13-171">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaf13-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eaf13-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="eaf13-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eaf13-173">Request</span></span>
<span data-ttu-id="eaf13-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eaf13-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 431

{
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

### <a name="response"></a><span data-ttu-id="eaf13-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaf13-175">Response</span></span>
<span data-ttu-id="eaf13-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eaf13-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





