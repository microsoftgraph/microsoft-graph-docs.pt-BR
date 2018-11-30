---
title: Atualizar importedDeviceIdentity
description: Atualize as propriedades de um objeto importedDeviceIdentity.
ms.openlocfilehash: 4c5ce8e592f04cbda5d5ffbbde0e38bbf7ee3602
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036081"
---
# <a name="update-importeddeviceidentity"></a><span data-ttu-id="aaac3-103">Atualizar importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="aaac3-103">Update importedDeviceIdentity</span></span>

> <span data-ttu-id="aaac3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="aaac3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aaac3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="aaac3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aaac3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="aaac3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aaac3-107">Atualize as propriedades de um objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="aaac3-107">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aaac3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aaac3-108">Prerequisites</span></span>
<span data-ttu-id="aaac3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaac3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaac3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aaac3-111">Permission type</span></span>|<span data-ttu-id="aaac3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aaac3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaac3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aaac3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aaac3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaac3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="aaac3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aaac3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaac3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aaac3-116">Not supported.</span></span>|
|<span data-ttu-id="aaac3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aaac3-117">Application</span></span>|<span data-ttu-id="aaac3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aaac3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaac3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aaac3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="aaac3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aaac3-120">Request headers</span></span>
|<span data-ttu-id="aaac3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aaac3-121">Header</span></span>|<span data-ttu-id="aaac3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="aaac3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaac3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aaac3-123">Authorization</span></span>|<span data-ttu-id="aaac3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aaac3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaac3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aaac3-125">Accept</span></span>|<span data-ttu-id="aaac3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aaac3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaac3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aaac3-127">Request body</span></span>
<span data-ttu-id="aaac3-128">No corpo da solicitação, fornece uma representação JSON para o objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="aaac3-128">In the request body, supply a JSON representation for the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

<span data-ttu-id="aaac3-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="aaac3-129">The following table shows the properties that are required when you create the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>

|<span data-ttu-id="aaac3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aaac3-130">Property</span></span>|<span data-ttu-id="aaac3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aaac3-131">Type</span></span>|<span data-ttu-id="aaac3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aaac3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaac3-133">id</span><span class="sxs-lookup"><span data-stu-id="aaac3-133">id</span></span>|<span data-ttu-id="aaac3-134">String</span><span class="sxs-lookup"><span data-stu-id="aaac3-134">String</span></span>|<span data-ttu-id="aaac3-135">ID da identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="aaac3-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="aaac3-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="aaac3-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="aaac3-137">String</span><span class="sxs-lookup"><span data-stu-id="aaac3-137">String</span></span>|<span data-ttu-id="aaac3-138">Identificador de dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="aaac3-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="aaac3-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="aaac3-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="aaac3-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="aaac3-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="aaac3-141">Tipo de identidade do dispositivo importada.</span><span class="sxs-lookup"><span data-stu-id="aaac3-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="aaac3-142">Os valores possíveis são: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="aaac3-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="aaac3-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aaac3-143">lastModifiedDateTime</span></span>|<span data-ttu-id="aaac3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaac3-144">DateTimeOffset</span></span>|<span data-ttu-id="aaac3-145">Última data e hora modificadas da descrição</span><span class="sxs-lookup"><span data-stu-id="aaac3-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="aaac3-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aaac3-146">createdDateTime</span></span>|<span data-ttu-id="aaac3-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaac3-147">DateTimeOffset</span></span>|<span data-ttu-id="aaac3-148">Criada data hora do dispositivo</span><span class="sxs-lookup"><span data-stu-id="aaac3-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="aaac3-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="aaac3-149">lastContactedDateTime</span></span>|<span data-ttu-id="aaac3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaac3-150">DateTimeOffset</span></span>|<span data-ttu-id="aaac3-151">Última contatado data hora do dispositivo</span><span class="sxs-lookup"><span data-stu-id="aaac3-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="aaac3-152">description</span><span class="sxs-lookup"><span data-stu-id="aaac3-152">description</span></span>|<span data-ttu-id="aaac3-153">String</span><span class="sxs-lookup"><span data-stu-id="aaac3-153">String</span></span>|<span data-ttu-id="aaac3-154">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="aaac3-154">The description of the device</span></span>|
|<span data-ttu-id="aaac3-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="aaac3-155">enrollmentState</span></span>|[<span data-ttu-id="aaac3-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="aaac3-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="aaac3-157">O estado do dispositivo em Intune.</span><span class="sxs-lookup"><span data-stu-id="aaac3-157">The state of the device in Intune.</span></span> <span data-ttu-id="aaac3-158">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="aaac3-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="aaac3-159">platform</span><span class="sxs-lookup"><span data-stu-id="aaac3-159">platform</span></span>|[<span data-ttu-id="aaac3-160">plataforma</span><span class="sxs-lookup"><span data-stu-id="aaac3-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="aaac3-161">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aaac3-161">The platform of the Device.</span></span> <span data-ttu-id="aaac3-162">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="aaac3-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="aaac3-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaac3-163">Response</span></span>
<span data-ttu-id="aaac3-164">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aaac3-164">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaac3-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aaac3-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="aaac3-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aaac3-166">Request</span></span>
<span data-ttu-id="aaac3-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aaac3-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 335

{
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="aaac3-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaac3-168">Response</span></span>
<span data-ttu-id="aaac3-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aaac3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





