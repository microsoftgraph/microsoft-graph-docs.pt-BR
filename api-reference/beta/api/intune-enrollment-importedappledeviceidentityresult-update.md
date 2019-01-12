---
title: Atualizar importedAppleDeviceIdentityResult
description: Atualize as propriedades de um objeto importedAppleDeviceIdentityResult.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 434bc2f19e708041b93ff79a8708f30bed086855
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915491"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="0a8a9-103">Atualizar importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="0a8a9-103">Update importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="0a8a9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0a8a9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a8a9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0a8a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a8a9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0a8a9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a8a9-107">Atualize as propriedades de um objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="0a8a9-107">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0a8a9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0a8a9-108">Prerequisites</span></span>
<span data-ttu-id="0a8a9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a8a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a8a9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a8a9-111">Permission type</span></span>|<span data-ttu-id="0a8a9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0a8a9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a8a9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a8a9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a8a9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a8a9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0a8a9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a8a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a8a9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a8a9-116">Not supported.</span></span>|
|<span data-ttu-id="0a8a9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a8a9-117">Application</span></span>|<span data-ttu-id="0a8a9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a8a9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a8a9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a8a9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="0a8a9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a8a9-120">Request headers</span></span>
|<span data-ttu-id="0a8a9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a8a9-121">Header</span></span>|<span data-ttu-id="0a8a9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0a8a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a8a9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a8a9-123">Authorization</span></span>|<span data-ttu-id="0a8a9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a8a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a8a9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0a8a9-125">Accept</span></span>|<span data-ttu-id="0a8a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a8a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a8a9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a8a9-127">Request body</span></span>
<span data-ttu-id="0a8a9-128">No corpo da solicitação, fornece uma representação JSON para o objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="0a8a9-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="0a8a9-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="0a8a9-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="0a8a9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a8a9-130">Property</span></span>|<span data-ttu-id="0a8a9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a8a9-131">Type</span></span>|<span data-ttu-id="0a8a9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a8a9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a8a9-133">id</span><span class="sxs-lookup"><span data-stu-id="0a8a9-133">id</span></span>|<span data-ttu-id="0a8a9-134">String</span><span class="sxs-lookup"><span data-stu-id="0a8a9-134">String</span></span>|<span data-ttu-id="0a8a9-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0a8a9-135">Key of the entity.</span></span> <span data-ttu-id="0a8a9-136">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="0a8a9-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0a8a9-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="0a8a9-137">serialNumber</span></span>|<span data-ttu-id="0a8a9-138">String</span><span class="sxs-lookup"><span data-stu-id="0a8a9-138">String</span></span>|<span data-ttu-id="0a8a9-139">Número de série do dispositivo Inherited do [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="0a8a9-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0a8a9-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="0a8a9-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="0a8a9-141">String</span><span class="sxs-lookup"><span data-stu-id="0a8a9-141">String</span></span>|<span data-ttu-id="0a8a9-142">Administração de Id de perfil de inscrição pretende aplicar ao dispositivo durante o próximo registro Inherited de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="0a8a9-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0a8a9-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="0a8a9-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="0a8a9-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a8a9-144">DateTimeOffset</span></span>|<span data-ttu-id="0a8a9-145">O perfil de horário de inscrição foi atribuído ao dispositivo Inherited a partir [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="0a8a9-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0a8a9-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="0a8a9-146">isSupervised</span></span>|<span data-ttu-id="0a8a9-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="0a8a9-147">Boolean</span></span>|<span data-ttu-id="0a8a9-148">Indica se o dispositivo Apple seja supervisionado.</span><span class="sxs-lookup"><span data-stu-id="0a8a9-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="0a8a9-149">Mais informações estão em: https://support.apple.com/en-us/HT202837 herdados de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="0a8a9-149">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0a8a9-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="0a8a9-150">discoverySource</span></span>|[<span data-ttu-id="0a8a9-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="0a8a9-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="0a8a9-152">Fonte de descoberta do dispositivo Apple.</span><span class="sxs-lookup"><span data-stu-id="0a8a9-152">Apple device discovery source.</span></span> <span data-ttu-id="0a8a9-153">Herdada do [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="0a8a9-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="0a8a9-154">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="0a8a9-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="0a8a9-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a8a9-155">createdDateTime</span></span>|<span data-ttu-id="0a8a9-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a8a9-156">DateTimeOffset</span></span>|<span data-ttu-id="0a8a9-157">Data-hora do dispositivo Inherited de criação de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="0a8a9-157">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0a8a9-158">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a8a9-158">lastContactedDateTime</span></span>|<span data-ttu-id="0a8a9-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a8a9-159">DateTimeOffset</span></span>|<span data-ttu-id="0a8a9-160">Última contatado data hora do dispositivo Inherited de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="0a8a9-160">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0a8a9-161">description</span><span class="sxs-lookup"><span data-stu-id="0a8a9-161">description</span></span>|<span data-ttu-id="0a8a9-162">String</span><span class="sxs-lookup"><span data-stu-id="0a8a9-162">String</span></span>|<span data-ttu-id="0a8a9-163">A descrição do dispositivo Inherited de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="0a8a9-163">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="0a8a9-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="0a8a9-164">enrollmentState</span></span>|[<span data-ttu-id="0a8a9-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="0a8a9-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="0a8a9-166">O estado do dispositivo em Intune herdada do [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="0a8a9-166">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="0a8a9-167">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="0a8a9-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="0a8a9-168">platform</span><span class="sxs-lookup"><span data-stu-id="0a8a9-168">platform</span></span>|[<span data-ttu-id="0a8a9-169">plataforma</span><span class="sxs-lookup"><span data-stu-id="0a8a9-169">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="0a8a9-170">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0a8a9-170">The platform of the Device.</span></span> <span data-ttu-id="0a8a9-171">Herdada do [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="0a8a9-171">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="0a8a9-172">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="0a8a9-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="0a8a9-173">status</span><span class="sxs-lookup"><span data-stu-id="0a8a9-173">status</span></span>|<span data-ttu-id="0a8a9-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="0a8a9-174">Boolean</span></span>|<span data-ttu-id="0a8a9-175">Status da identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="0a8a9-175">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="0a8a9-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a8a9-176">Response</span></span>
<span data-ttu-id="0a8a9-177">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a8a9-177">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a8a9-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a8a9-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="0a8a9-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a8a9-179">Request</span></span>
<span data-ttu-id="0a8a9-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a8a9-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 450

{
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

### <a name="response"></a><span data-ttu-id="0a8a9-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a8a9-181">Response</span></span>
<span data-ttu-id="0a8a9-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a8a9-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





