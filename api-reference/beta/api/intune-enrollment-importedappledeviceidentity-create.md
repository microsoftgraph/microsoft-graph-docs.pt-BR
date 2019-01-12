---
title: Criar importedAppleDeviceIdentity
description: Crie um novo objeto de importedAppleDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cf6f897d44774ceba92b2d2c965f7cc561001383
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925073"
---
# <a name="create-importedappledeviceidentity"></a><span data-ttu-id="9edec-103">Criar importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="9edec-103">Create importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="9edec-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9edec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9edec-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9edec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9edec-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9edec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9edec-107">Crie um novo objeto de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="9edec-107">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9edec-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9edec-108">Prerequisites</span></span>
<span data-ttu-id="9edec-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9edec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9edec-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9edec-111">Permission type</span></span>|<span data-ttu-id="9edec-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9edec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9edec-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9edec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9edec-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9edec-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9edec-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9edec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9edec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9edec-116">Not supported.</span></span>|
|<span data-ttu-id="9edec-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9edec-117">Application</span></span>|<span data-ttu-id="9edec-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9edec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9edec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9edec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="9edec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9edec-120">Request headers</span></span>
|<span data-ttu-id="9edec-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9edec-121">Header</span></span>|<span data-ttu-id="9edec-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9edec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9edec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9edec-123">Authorization</span></span>|<span data-ttu-id="9edec-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9edec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9edec-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9edec-125">Accept</span></span>|<span data-ttu-id="9edec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9edec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9edec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9edec-127">Request body</span></span>
<span data-ttu-id="9edec-128">No corpo da solicitação, fornece uma representação JSON para o objeto importedAppleDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="9edec-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentity object.</span></span>

<span data-ttu-id="9edec-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o importedAppleDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="9edec-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentity.</span></span>

|<span data-ttu-id="9edec-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9edec-130">Property</span></span>|<span data-ttu-id="9edec-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9edec-131">Type</span></span>|<span data-ttu-id="9edec-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9edec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9edec-133">id</span><span class="sxs-lookup"><span data-stu-id="9edec-133">id</span></span>|<span data-ttu-id="9edec-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9edec-134">String</span></span>|<span data-ttu-id="9edec-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9edec-135">Key of the entity.</span></span>|
|<span data-ttu-id="9edec-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="9edec-136">serialNumber</span></span>|<span data-ttu-id="9edec-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9edec-137">String</span></span>|<span data-ttu-id="9edec-138">Número de série do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9edec-138">Device serial number</span></span>|
|<span data-ttu-id="9edec-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="9edec-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="9edec-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9edec-140">String</span></span>|<span data-ttu-id="9edec-141">Administração de Id de perfil de inscrição pretende aplicáveis ao dispositivo durante o próximo registro</span><span class="sxs-lookup"><span data-stu-id="9edec-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="9edec-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="9edec-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="9edec-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9edec-143">DateTimeOffset</span></span>|<span data-ttu-id="9edec-144">O perfil de inscrição de tempo foi atribuído ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="9edec-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="9edec-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="9edec-145">isSupervised</span></span>|<span data-ttu-id="9edec-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="9edec-146">Boolean</span></span>|<span data-ttu-id="9edec-147">Indica se o dispositivo Apple seja supervisionado.</span><span class="sxs-lookup"><span data-stu-id="9edec-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="9edec-148">Mais informações estão em:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="9edec-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="9edec-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="9edec-149">discoverySource</span></span>|[<span data-ttu-id="9edec-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="9edec-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="9edec-151">Fonte de descoberta do dispositivo Apple.</span><span class="sxs-lookup"><span data-stu-id="9edec-151">Apple device discovery source.</span></span> <span data-ttu-id="9edec-152">Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="9edec-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="9edec-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9edec-153">createdDateTime</span></span>|<span data-ttu-id="9edec-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9edec-154">DateTimeOffset</span></span>|<span data-ttu-id="9edec-155">Criada data hora do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9edec-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="9edec-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="9edec-156">lastContactedDateTime</span></span>|<span data-ttu-id="9edec-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9edec-157">DateTimeOffset</span></span>|<span data-ttu-id="9edec-158">Última contatado data hora do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9edec-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="9edec-159">description</span><span class="sxs-lookup"><span data-stu-id="9edec-159">description</span></span>|<span data-ttu-id="9edec-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9edec-160">String</span></span>|<span data-ttu-id="9edec-161">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9edec-161">The description of the device</span></span>|
|<span data-ttu-id="9edec-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="9edec-162">enrollmentState</span></span>|[<span data-ttu-id="9edec-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="9edec-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="9edec-164">O estado do dispositivo em Intune.</span><span class="sxs-lookup"><span data-stu-id="9edec-164">The state of the device in Intune.</span></span> <span data-ttu-id="9edec-165">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="9edec-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="9edec-166">platform</span><span class="sxs-lookup"><span data-stu-id="9edec-166">platform</span></span>|[<span data-ttu-id="9edec-167">plataforma</span><span class="sxs-lookup"><span data-stu-id="9edec-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="9edec-168">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9edec-168">The platform of the Device.</span></span> <span data-ttu-id="9edec-169">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="9edec-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="9edec-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="9edec-170">Response</span></span>
<span data-ttu-id="9edec-171">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9edec-171">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9edec-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9edec-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="9edec-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9edec-173">Request</span></span>
<span data-ttu-id="9edec-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9edec-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="9edec-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="9edec-175">Response</span></span>
<span data-ttu-id="9edec-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9edec-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





