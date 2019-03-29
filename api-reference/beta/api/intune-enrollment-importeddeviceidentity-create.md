---
title: Criar importedDeviceIdentity
description: Criar um novo objeto importedDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d91ebc37a348f86a83d0a17c3b2af1ab7f0292e6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977727"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="6062d-103">Criar importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="6062d-103">Create importedDeviceIdentity</span></span>

> <span data-ttu-id="6062d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6062d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6062d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6062d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6062d-106">Criar um novo objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="6062d-106">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6062d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6062d-107">Prerequisites</span></span>
<span data-ttu-id="6062d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6062d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6062d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6062d-110">Permission type</span></span>|<span data-ttu-id="6062d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6062d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6062d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6062d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6062d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6062d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6062d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6062d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6062d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6062d-115">Not supported.</span></span>|
|<span data-ttu-id="6062d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6062d-116">Application</span></span>|<span data-ttu-id="6062d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6062d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6062d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6062d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="6062d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6062d-119">Request headers</span></span>
|<span data-ttu-id="6062d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6062d-120">Header</span></span>|<span data-ttu-id="6062d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6062d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6062d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6062d-122">Authorization</span></span>|<span data-ttu-id="6062d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6062d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6062d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6062d-124">Accept</span></span>|<span data-ttu-id="6062d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6062d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6062d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6062d-126">Request body</span></span>
<span data-ttu-id="6062d-127">No corpo da solicitação, forneça uma representação JSON do objeto importedDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="6062d-127">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="6062d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar importedDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="6062d-128">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="6062d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6062d-129">Property</span></span>|<span data-ttu-id="6062d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6062d-130">Type</span></span>|<span data-ttu-id="6062d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6062d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6062d-132">id</span><span class="sxs-lookup"><span data-stu-id="6062d-132">id</span></span>|<span data-ttu-id="6062d-133">String</span><span class="sxs-lookup"><span data-stu-id="6062d-133">String</span></span>|<span data-ttu-id="6062d-134">ID da identidade do dispositivo importado</span><span class="sxs-lookup"><span data-stu-id="6062d-134">Id of the imported device identity</span></span>|
|<span data-ttu-id="6062d-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="6062d-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="6062d-136">String</span><span class="sxs-lookup"><span data-stu-id="6062d-136">String</span></span>|<span data-ttu-id="6062d-137">Identificador de dispositivo imPortado</span><span class="sxs-lookup"><span data-stu-id="6062d-137">Imported Device Identifier</span></span>|
|<span data-ttu-id="6062d-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="6062d-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="6062d-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="6062d-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="6062d-140">Tipo de identidade de dispositivo imPortada.</span><span class="sxs-lookup"><span data-stu-id="6062d-140">Type of Imported Device Identity.</span></span> <span data-ttu-id="6062d-141">Os valores possíveis são: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="6062d-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="6062d-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6062d-142">lastModifiedDateTime</span></span>|<span data-ttu-id="6062d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6062d-143">DateTimeOffset</span></span>|<span data-ttu-id="6062d-144">Data e hora da última modificação da descrição</span><span class="sxs-lookup"><span data-stu-id="6062d-144">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="6062d-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6062d-145">createdDateTime</span></span>|<span data-ttu-id="6062d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6062d-146">DateTimeOffset</span></span>|<span data-ttu-id="6062d-147">Data e hora de criação do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6062d-147">Created Date Time of the device</span></span>|
|<span data-ttu-id="6062d-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="6062d-148">lastContactedDateTime</span></span>|<span data-ttu-id="6062d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6062d-149">DateTimeOffset</span></span>|<span data-ttu-id="6062d-150">Data e hora do último contato do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6062d-150">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="6062d-151">descrição</span><span class="sxs-lookup"><span data-stu-id="6062d-151">description</span></span>|<span data-ttu-id="6062d-152">String</span><span class="sxs-lookup"><span data-stu-id="6062d-152">String</span></span>|<span data-ttu-id="6062d-153">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6062d-153">The description of the device</span></span>|
|<span data-ttu-id="6062d-154">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="6062d-154">enrollmentState</span></span>|[<span data-ttu-id="6062d-155">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="6062d-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="6062d-156">O estado do dispositivo no Intune.</span><span class="sxs-lookup"><span data-stu-id="6062d-156">The state of the device in Intune.</span></span> <span data-ttu-id="6062d-157">Os valores possíveis são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="6062d-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="6062d-158">platform</span><span class="sxs-lookup"><span data-stu-id="6062d-158">platform</span></span>|[<span data-ttu-id="6062d-159">plataforma</span><span class="sxs-lookup"><span data-stu-id="6062d-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="6062d-160">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6062d-160">The platform of the Device.</span></span> <span data-ttu-id="6062d-161">Os valores possíveis são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="6062d-161">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="6062d-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="6062d-162">Response</span></span>
<span data-ttu-id="6062d-163">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6062d-163">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6062d-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6062d-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="6062d-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6062d-165">Request</span></span>
<span data-ttu-id="6062d-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6062d-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="6062d-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="6062d-167">Response</span></span>
<span data-ttu-id="6062d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6062d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




