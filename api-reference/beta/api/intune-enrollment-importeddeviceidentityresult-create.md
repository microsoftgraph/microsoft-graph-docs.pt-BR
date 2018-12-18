---
title: Criar importedDeviceIdentityResult
description: Crie um novo objeto de importedDeviceIdentityResult.
author: tfitzmac
ms.openlocfilehash: 2613cd100ccb1803464907821d56eb75fc4024fb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359714"
---
# <a name="create-importeddeviceidentityresult"></a><span data-ttu-id="4bf46-103">Criar importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="4bf46-103">Create importedDeviceIdentityResult</span></span>

> <span data-ttu-id="4bf46-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4bf46-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bf46-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4bf46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4bf46-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4bf46-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4bf46-107">Crie um novo objeto de [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="4bf46-107">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4bf46-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4bf46-108">Prerequisites</span></span>
<span data-ttu-id="4bf46-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bf46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bf46-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bf46-111">Permission type</span></span>|<span data-ttu-id="4bf46-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4bf46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bf46-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bf46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4bf46-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bf46-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4bf46-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bf46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bf46-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bf46-116">Not supported.</span></span>|
|<span data-ttu-id="4bf46-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bf46-117">Application</span></span>|<span data-ttu-id="4bf46-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bf46-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bf46-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bf46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="4bf46-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bf46-120">Request headers</span></span>
|<span data-ttu-id="4bf46-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4bf46-121">Header</span></span>|<span data-ttu-id="4bf46-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4bf46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bf46-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bf46-123">Authorization</span></span>|<span data-ttu-id="4bf46-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bf46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bf46-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4bf46-125">Accept</span></span>|<span data-ttu-id="4bf46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4bf46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bf46-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bf46-127">Request body</span></span>
<span data-ttu-id="4bf46-128">No corpo da solicitação, fornece uma representação JSON para o objeto importedDeviceIdentityResult.</span><span class="sxs-lookup"><span data-stu-id="4bf46-128">In the request body, supply a JSON representation for the importedDeviceIdentityResult object.</span></span>

<span data-ttu-id="4bf46-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o importedDeviceIdentityResult.</span><span class="sxs-lookup"><span data-stu-id="4bf46-129">The following table shows the properties that are required when you create the importedDeviceIdentityResult.</span></span>

|<span data-ttu-id="4bf46-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4bf46-130">Property</span></span>|<span data-ttu-id="4bf46-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bf46-131">Type</span></span>|<span data-ttu-id="4bf46-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bf46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bf46-133">id</span><span class="sxs-lookup"><span data-stu-id="4bf46-133">id</span></span>|<span data-ttu-id="4bf46-134">String</span><span class="sxs-lookup"><span data-stu-id="4bf46-134">String</span></span>|<span data-ttu-id="4bf46-135">ID da identidade do dispositivo importada Inherited de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4bf46-135">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="4bf46-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="4bf46-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="4bf46-137">String</span><span class="sxs-lookup"><span data-stu-id="4bf46-137">String</span></span>|<span data-ttu-id="4bf46-138">Importados dispositivo identificador herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4bf46-138">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="4bf46-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="4bf46-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="4bf46-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="4bf46-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="4bf46-141">Tipo de importado herdadas de identidade do dispositivo de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="4bf46-141">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="4bf46-142">Os valores possíveis são: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="4bf46-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="4bf46-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4bf46-143">lastModifiedDateTime</span></span>|<span data-ttu-id="4bf46-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bf46-144">DateTimeOffset</span></span>|<span data-ttu-id="4bf46-145">Última DateTime modificação da descrição Inherited de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4bf46-145">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="4bf46-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4bf46-146">createdDateTime</span></span>|<span data-ttu-id="4bf46-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bf46-147">DateTimeOffset</span></span>|<span data-ttu-id="4bf46-148">Data-hora do dispositivo Inherited de criação de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4bf46-148">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="4bf46-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="4bf46-149">lastContactedDateTime</span></span>|<span data-ttu-id="4bf46-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bf46-150">DateTimeOffset</span></span>|<span data-ttu-id="4bf46-151">Última contatado data hora do dispositivo Inherited de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4bf46-151">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="4bf46-152">description</span><span class="sxs-lookup"><span data-stu-id="4bf46-152">description</span></span>|<span data-ttu-id="4bf46-153">String</span><span class="sxs-lookup"><span data-stu-id="4bf46-153">String</span></span>|<span data-ttu-id="4bf46-154">A descrição do dispositivo Inherited de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4bf46-154">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="4bf46-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="4bf46-155">enrollmentState</span></span>|[<span data-ttu-id="4bf46-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="4bf46-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="4bf46-157">O estado do dispositivo em Intune herdada do [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="4bf46-157">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="4bf46-158">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="4bf46-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="4bf46-159">platform</span><span class="sxs-lookup"><span data-stu-id="4bf46-159">platform</span></span>|[<span data-ttu-id="4bf46-160">plataforma</span><span class="sxs-lookup"><span data-stu-id="4bf46-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="4bf46-161">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4bf46-161">The platform of the Device.</span></span> <span data-ttu-id="4bf46-162">Herdada do [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="4bf46-162">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="4bf46-163">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="4bf46-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="4bf46-164">status</span><span class="sxs-lookup"><span data-stu-id="4bf46-164">status</span></span>|<span data-ttu-id="4bf46-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bf46-165">Boolean</span></span>|<span data-ttu-id="4bf46-166">Status da identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="4bf46-166">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="4bf46-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bf46-167">Response</span></span>
<span data-ttu-id="4bf46-168">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bf46-168">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bf46-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bf46-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="4bf46-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bf46-170">Request</span></span>
<span data-ttu-id="4bf46-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bf46-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
Content-type: application/json
Content-length: 421

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="4bf46-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bf46-172">Response</span></span>
<span data-ttu-id="4bf46-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4bf46-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```





