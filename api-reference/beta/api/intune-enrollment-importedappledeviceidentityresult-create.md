---
title: Criar importedAppleDeviceIdentityResult
description: Crie um novo objeto de importedAppleDeviceIdentityResult.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bd48716e7268997305a5b8840beacbab9106cf42
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417725"
---
# <a name="create-importedappledeviceidentityresult"></a><span data-ttu-id="ab23e-103">Criar importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="ab23e-103">Create importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="ab23e-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ab23e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ab23e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ab23e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab23e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ab23e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab23e-107">Crie um novo objeto de [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="ab23e-107">Create a new [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab23e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ab23e-108">Prerequisites</span></span>
<span data-ttu-id="ab23e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ab23e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ab23e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab23e-111">Permission type</span></span>|<span data-ttu-id="ab23e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ab23e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab23e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab23e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab23e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab23e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ab23e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab23e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab23e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab23e-116">Not supported.</span></span>|
|<span data-ttu-id="ab23e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab23e-117">Application</span></span>|<span data-ttu-id="ab23e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab23e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab23e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab23e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="ab23e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab23e-120">Request headers</span></span>
|<span data-ttu-id="ab23e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab23e-121">Header</span></span>|<span data-ttu-id="ab23e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ab23e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab23e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab23e-123">Authorization</span></span>|<span data-ttu-id="ab23e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab23e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab23e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ab23e-125">Accept</span></span>|<span data-ttu-id="ab23e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab23e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab23e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab23e-127">Request body</span></span>
<span data-ttu-id="ab23e-128">No corpo da solicitação, fornece uma representação JSON para o objeto importedAppleDeviceIdentityResult.</span><span class="sxs-lookup"><span data-stu-id="ab23e-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentityResult object.</span></span>

<span data-ttu-id="ab23e-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o importedAppleDeviceIdentityResult.</span><span class="sxs-lookup"><span data-stu-id="ab23e-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentityResult.</span></span>

|<span data-ttu-id="ab23e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab23e-130">Property</span></span>|<span data-ttu-id="ab23e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab23e-131">Type</span></span>|<span data-ttu-id="ab23e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab23e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab23e-133">id</span><span class="sxs-lookup"><span data-stu-id="ab23e-133">id</span></span>|<span data-ttu-id="ab23e-134">String</span><span class="sxs-lookup"><span data-stu-id="ab23e-134">String</span></span>|<span data-ttu-id="ab23e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ab23e-135">Key of the entity.</span></span> <span data-ttu-id="ab23e-136">Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ab23e-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="ab23e-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ab23e-137">serialNumber</span></span>|<span data-ttu-id="ab23e-138">String</span><span class="sxs-lookup"><span data-stu-id="ab23e-138">String</span></span>|<span data-ttu-id="ab23e-139">Número de série do dispositivo Inherited do [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ab23e-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="ab23e-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="ab23e-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="ab23e-141">String</span><span class="sxs-lookup"><span data-stu-id="ab23e-141">String</span></span>|<span data-ttu-id="ab23e-142">Administração de Id de perfil de inscrição pretende aplicar ao dispositivo durante o próximo registro Inherited de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ab23e-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="ab23e-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="ab23e-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="ab23e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab23e-144">DateTimeOffset</span></span>|<span data-ttu-id="ab23e-145">O perfil de horário de inscrição foi atribuído ao dispositivo Inherited a partir [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ab23e-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="ab23e-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="ab23e-146">isSupervised</span></span>|<span data-ttu-id="ab23e-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab23e-147">Boolean</span></span>|<span data-ttu-id="ab23e-148">Indica se o dispositivo Apple seja supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ab23e-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="ab23e-149">Mais informações estão em: https://support.apple.com/en-us/HT202837 herdados de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ab23e-149">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="ab23e-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="ab23e-150">discoverySource</span></span>|[<span data-ttu-id="ab23e-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="ab23e-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="ab23e-152">Fonte de descoberta do dispositivo Apple.</span><span class="sxs-lookup"><span data-stu-id="ab23e-152">Apple device discovery source.</span></span> <span data-ttu-id="ab23e-153">Herdada do [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="ab23e-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="ab23e-154">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="ab23e-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="ab23e-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab23e-155">createdDateTime</span></span>|<span data-ttu-id="ab23e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab23e-156">DateTimeOffset</span></span>|<span data-ttu-id="ab23e-157">Data-hora do dispositivo Inherited de criação de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ab23e-157">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="ab23e-158">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab23e-158">lastContactedDateTime</span></span>|<span data-ttu-id="ab23e-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab23e-159">DateTimeOffset</span></span>|<span data-ttu-id="ab23e-160">Última contatado data hora do dispositivo Inherited de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ab23e-160">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="ab23e-161">description</span><span class="sxs-lookup"><span data-stu-id="ab23e-161">description</span></span>|<span data-ttu-id="ab23e-162">String</span><span class="sxs-lookup"><span data-stu-id="ab23e-162">String</span></span>|<span data-ttu-id="ab23e-163">A descrição do dispositivo Inherited de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ab23e-163">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="ab23e-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="ab23e-164">enrollmentState</span></span>|[<span data-ttu-id="ab23e-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="ab23e-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="ab23e-166">O estado do dispositivo em Intune herdada do [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="ab23e-166">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="ab23e-167">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="ab23e-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="ab23e-168">platform</span><span class="sxs-lookup"><span data-stu-id="ab23e-168">platform</span></span>|[<span data-ttu-id="ab23e-169">plataforma</span><span class="sxs-lookup"><span data-stu-id="ab23e-169">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="ab23e-170">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab23e-170">The platform of the Device.</span></span> <span data-ttu-id="ab23e-171">Herdada do [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="ab23e-171">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="ab23e-172">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="ab23e-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="ab23e-173">status</span><span class="sxs-lookup"><span data-stu-id="ab23e-173">status</span></span>|<span data-ttu-id="ab23e-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab23e-174">Boolean</span></span>|<span data-ttu-id="ab23e-175">Status da identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="ab23e-175">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="ab23e-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab23e-176">Response</span></span>
<span data-ttu-id="ab23e-177">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab23e-177">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab23e-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab23e-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab23e-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab23e-179">Request</span></span>
<span data-ttu-id="ab23e-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab23e-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="ab23e-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab23e-181">Response</span></span>
<span data-ttu-id="ab23e-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab23e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




