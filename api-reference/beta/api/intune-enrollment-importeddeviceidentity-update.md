---
title: Atualizar importedDeviceIdentity
description: Atualiza as propriedades de um objeto importedDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db05bc349c4d5556d5d44db3aabaf12f4cb8159f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356372"
---
# <a name="update-importeddeviceidentity"></a><span data-ttu-id="f4288-103">Atualizar importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f4288-103">Update importedDeviceIdentity</span></span>

> <span data-ttu-id="f4288-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4288-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4288-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4288-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4288-106">Atualiza as propriedades de um objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="f4288-106">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4288-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4288-107">Prerequisites</span></span>
<span data-ttu-id="f4288-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4288-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4288-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4288-110">Permission type</span></span>|<span data-ttu-id="f4288-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f4288-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4288-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4288-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4288-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4288-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f4288-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4288-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4288-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4288-115">Not supported.</span></span>|
|<span data-ttu-id="f4288-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4288-116">Application</span></span>|<span data-ttu-id="f4288-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4288-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4288-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4288-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="f4288-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4288-119">Request headers</span></span>
|<span data-ttu-id="f4288-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4288-120">Header</span></span>|<span data-ttu-id="f4288-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f4288-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4288-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4288-122">Authorization</span></span>|<span data-ttu-id="f4288-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4288-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4288-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4288-124">Accept</span></span>|<span data-ttu-id="f4288-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4288-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4288-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4288-126">Request body</span></span>
<span data-ttu-id="f4288-127">No corpo da solicitação, forneça uma representação JSON do objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="f4288-127">In the request body, supply a JSON representation for the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

<span data-ttu-id="f4288-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="f4288-128">The following table shows the properties that are required when you create the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>

|<span data-ttu-id="f4288-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4288-129">Property</span></span>|<span data-ttu-id="f4288-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4288-130">Type</span></span>|<span data-ttu-id="f4288-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4288-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4288-132">id</span><span class="sxs-lookup"><span data-stu-id="f4288-132">id</span></span>|<span data-ttu-id="f4288-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4288-133">String</span></span>|<span data-ttu-id="f4288-134">ID da identidade do dispositivo importado</span><span class="sxs-lookup"><span data-stu-id="f4288-134">Id of the imported device identity</span></span>|
|<span data-ttu-id="f4288-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f4288-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="f4288-136">String</span><span class="sxs-lookup"><span data-stu-id="f4288-136">String</span></span>|<span data-ttu-id="f4288-137">Identificador de dispositivo importado</span><span class="sxs-lookup"><span data-stu-id="f4288-137">Imported Device Identifier</span></span>|
|<span data-ttu-id="f4288-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="f4288-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="f4288-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="f4288-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="f4288-140">Tipo de identidade de dispositivo importada.</span><span class="sxs-lookup"><span data-stu-id="f4288-140">Type of Imported Device Identity.</span></span> <span data-ttu-id="f4288-141">Os valores possíveis são: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="f4288-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="f4288-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4288-142">lastModifiedDateTime</span></span>|<span data-ttu-id="f4288-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4288-143">DateTimeOffset</span></span>|<span data-ttu-id="f4288-144">Data e hora da última modificação da descrição</span><span class="sxs-lookup"><span data-stu-id="f4288-144">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="f4288-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4288-145">createdDateTime</span></span>|<span data-ttu-id="f4288-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4288-146">DateTimeOffset</span></span>|<span data-ttu-id="f4288-147">Data e hora de criação do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f4288-147">Created Date Time of the device</span></span>|
|<span data-ttu-id="f4288-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4288-148">lastContactedDateTime</span></span>|<span data-ttu-id="f4288-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4288-149">DateTimeOffset</span></span>|<span data-ttu-id="f4288-150">Data e hora do último contato do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f4288-150">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="f4288-151">descrição</span><span class="sxs-lookup"><span data-stu-id="f4288-151">description</span></span>|<span data-ttu-id="f4288-152">String</span><span class="sxs-lookup"><span data-stu-id="f4288-152">String</span></span>|<span data-ttu-id="f4288-153">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f4288-153">The description of the device</span></span>|
|<span data-ttu-id="f4288-154">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="f4288-154">enrollmentState</span></span>|[<span data-ttu-id="f4288-155">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="f4288-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="f4288-156">O estado do dispositivo no Intune.</span><span class="sxs-lookup"><span data-stu-id="f4288-156">The state of the device in Intune.</span></span> <span data-ttu-id="f4288-157">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="f4288-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="f4288-158">platform</span><span class="sxs-lookup"><span data-stu-id="f4288-158">platform</span></span>|[<span data-ttu-id="f4288-159">plataforma</span><span class="sxs-lookup"><span data-stu-id="f4288-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="f4288-160">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4288-160">The platform of the Device.</span></span> <span data-ttu-id="f4288-161">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="f4288-161">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="f4288-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4288-162">Response</span></span>
<span data-ttu-id="f4288-163">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4288-163">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4288-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4288-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4288-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4288-165">Request</span></span>
<span data-ttu-id="f4288-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4288-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 332

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="f4288-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4288-167">Response</span></span>
<span data-ttu-id="f4288-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4288-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






