---
title: Criar importedDeviceIdentity
description: Crie um novo objeto de importedDeviceIdentity.
ms.openlocfilehash: d679c45121cdad960e4a60cf4be6f359da9eb16a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037453"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="10280-103">Criar importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="10280-103">Create importedDeviceIdentity</span></span>

> <span data-ttu-id="10280-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="10280-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10280-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="10280-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10280-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="10280-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10280-107">Crie um novo objeto de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="10280-107">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="10280-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="10280-108">Prerequisites</span></span>
<span data-ttu-id="10280-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10280-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10280-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10280-111">Permission type</span></span>|<span data-ttu-id="10280-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="10280-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10280-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10280-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10280-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10280-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="10280-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10280-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10280-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10280-116">Not supported.</span></span>|
|<span data-ttu-id="10280-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10280-117">Application</span></span>|<span data-ttu-id="10280-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10280-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10280-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10280-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="10280-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10280-120">Request headers</span></span>
|<span data-ttu-id="10280-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="10280-121">Header</span></span>|<span data-ttu-id="10280-122">Valor</span><span class="sxs-lookup"><span data-stu-id="10280-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10280-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="10280-123">Authorization</span></span>|<span data-ttu-id="10280-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10280-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10280-125">Accept</span><span class="sxs-lookup"><span data-stu-id="10280-125">Accept</span></span>|<span data-ttu-id="10280-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10280-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10280-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10280-127">Request body</span></span>
<span data-ttu-id="10280-128">No corpo da solicitação, fornece uma representação JSON para o objeto importedDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="10280-128">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="10280-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o importedDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="10280-129">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="10280-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10280-130">Property</span></span>|<span data-ttu-id="10280-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="10280-131">Type</span></span>|<span data-ttu-id="10280-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="10280-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10280-133">id</span><span class="sxs-lookup"><span data-stu-id="10280-133">id</span></span>|<span data-ttu-id="10280-134">String</span><span class="sxs-lookup"><span data-stu-id="10280-134">String</span></span>|<span data-ttu-id="10280-135">ID da identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="10280-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="10280-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="10280-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="10280-137">String</span><span class="sxs-lookup"><span data-stu-id="10280-137">String</span></span>|<span data-ttu-id="10280-138">Identificador de dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="10280-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="10280-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="10280-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="10280-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="10280-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="10280-141">Tipo de identidade do dispositivo importada.</span><span class="sxs-lookup"><span data-stu-id="10280-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="10280-142">Os valores possíveis são: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="10280-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="10280-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10280-143">lastModifiedDateTime</span></span>|<span data-ttu-id="10280-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10280-144">DateTimeOffset</span></span>|<span data-ttu-id="10280-145">Última data e hora modificadas da descrição</span><span class="sxs-lookup"><span data-stu-id="10280-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="10280-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10280-146">createdDateTime</span></span>|<span data-ttu-id="10280-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10280-147">DateTimeOffset</span></span>|<span data-ttu-id="10280-148">Criada data hora do dispositivo</span><span class="sxs-lookup"><span data-stu-id="10280-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="10280-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="10280-149">lastContactedDateTime</span></span>|<span data-ttu-id="10280-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10280-150">DateTimeOffset</span></span>|<span data-ttu-id="10280-151">Última contatado data hora do dispositivo</span><span class="sxs-lookup"><span data-stu-id="10280-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="10280-152">description</span><span class="sxs-lookup"><span data-stu-id="10280-152">description</span></span>|<span data-ttu-id="10280-153">String</span><span class="sxs-lookup"><span data-stu-id="10280-153">String</span></span>|<span data-ttu-id="10280-154">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="10280-154">The description of the device</span></span>|
|<span data-ttu-id="10280-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="10280-155">enrollmentState</span></span>|[<span data-ttu-id="10280-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="10280-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="10280-157">O estado do dispositivo em Intune.</span><span class="sxs-lookup"><span data-stu-id="10280-157">The state of the device in Intune.</span></span> <span data-ttu-id="10280-158">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="10280-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="10280-159">platform</span><span class="sxs-lookup"><span data-stu-id="10280-159">platform</span></span>|[<span data-ttu-id="10280-160">plataforma</span><span class="sxs-lookup"><span data-stu-id="10280-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="10280-161">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="10280-161">The platform of the Device.</span></span> <span data-ttu-id="10280-162">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="10280-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="10280-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="10280-163">Response</span></span>
<span data-ttu-id="10280-164">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10280-164">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10280-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10280-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="10280-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10280-166">Request</span></span>
<span data-ttu-id="10280-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10280-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
Content-type: application/json
Content-length: 396

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="10280-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="10280-168">Response</span></span>
<span data-ttu-id="10280-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10280-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```





