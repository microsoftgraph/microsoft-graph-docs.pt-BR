---
title: Atualizar importedDeviceIdentityResult
description: Atualiza as propriedades de um objeto importedDeviceIdentityResult.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f57ba2365b91764ae54ef16a60d4095eeff8a13
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535860"
---
# <a name="update-importeddeviceidentityresult"></a><span data-ttu-id="995ed-103">Atualizar importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="995ed-103">Update importedDeviceIdentityResult</span></span>

> <span data-ttu-id="995ed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="995ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="995ed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="995ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="995ed-106">Atualiza as propriedades de um objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="995ed-106">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="995ed-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="995ed-107">Prerequisites</span></span>
<span data-ttu-id="995ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="995ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="995ed-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="995ed-110">Permission type</span></span>|<span data-ttu-id="995ed-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="995ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="995ed-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="995ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="995ed-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="995ed-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="995ed-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="995ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="995ed-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="995ed-115">Not supported.</span></span>|
|<span data-ttu-id="995ed-116">Application</span><span class="sxs-lookup"><span data-stu-id="995ed-116">Application</span></span>|<span data-ttu-id="995ed-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="995ed-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="995ed-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="995ed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="995ed-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="995ed-119">Request headers</span></span>
|<span data-ttu-id="995ed-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="995ed-120">Header</span></span>|<span data-ttu-id="995ed-121">Valor</span><span class="sxs-lookup"><span data-stu-id="995ed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="995ed-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="995ed-122">Authorization</span></span>|<span data-ttu-id="995ed-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="995ed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="995ed-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="995ed-124">Accept</span></span>|<span data-ttu-id="995ed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="995ed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="995ed-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="995ed-126">Request body</span></span>
<span data-ttu-id="995ed-127">No corpo da solicitação, forneça uma representação JSON do objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="995ed-127">In the request body, supply a JSON representation for the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

<span data-ttu-id="995ed-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="995ed-128">The following table shows the properties that are required when you create the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>

|<span data-ttu-id="995ed-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="995ed-129">Property</span></span>|<span data-ttu-id="995ed-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="995ed-130">Type</span></span>|<span data-ttu-id="995ed-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="995ed-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="995ed-132">id</span><span class="sxs-lookup"><span data-stu-id="995ed-132">id</span></span>|<span data-ttu-id="995ed-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="995ed-133">String</span></span>|<span data-ttu-id="995ed-134">ID da identidade de dispositivo importada herdada de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="995ed-134">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="995ed-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="995ed-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="995ed-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="995ed-136">String</span></span>|<span data-ttu-id="995ed-137">Identificador de dispositivo importado herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="995ed-137">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="995ed-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="995ed-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="995ed-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="995ed-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="995ed-140">Tipo de identidade de dispositivo importado herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="995ed-140">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="995ed-141">Os valores possíveis são: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="995ed-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="995ed-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="995ed-142">lastModifiedDateTime</span></span>|<span data-ttu-id="995ed-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="995ed-143">DateTimeOffset</span></span>|<span data-ttu-id="995ed-144">Data e hora da última modificação da descrição herdadas de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="995ed-144">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="995ed-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="995ed-145">createdDateTime</span></span>|<span data-ttu-id="995ed-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="995ed-146">DateTimeOffset</span></span>|<span data-ttu-id="995ed-147">Data e hora de criação do dispositivo herdadas de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="995ed-147">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="995ed-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="995ed-148">lastContactedDateTime</span></span>|<span data-ttu-id="995ed-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="995ed-149">DateTimeOffset</span></span>|<span data-ttu-id="995ed-150">Data e hora do último contato do dispositivo herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="995ed-150">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="995ed-151">description</span><span class="sxs-lookup"><span data-stu-id="995ed-151">description</span></span>|<span data-ttu-id="995ed-152">String</span><span class="sxs-lookup"><span data-stu-id="995ed-152">String</span></span>|<span data-ttu-id="995ed-153">A descrição do dispositivo herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="995ed-153">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="995ed-154">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="995ed-154">enrollmentState</span></span>|[<span data-ttu-id="995ed-155">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="995ed-155">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="995ed-156">O estado do dispositivo no Intune herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="995ed-156">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="995ed-157">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="995ed-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="995ed-158">platform</span><span class="sxs-lookup"><span data-stu-id="995ed-158">platform</span></span>|[<span data-ttu-id="995ed-159">plataforma</span><span class="sxs-lookup"><span data-stu-id="995ed-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="995ed-160">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="995ed-160">The platform of the Device.</span></span> <span data-ttu-id="995ed-161">Herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="995ed-161">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="995ed-162">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="995ed-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="995ed-163">status</span><span class="sxs-lookup"><span data-stu-id="995ed-163">status</span></span>|<span data-ttu-id="995ed-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="995ed-164">Boolean</span></span>|<span data-ttu-id="995ed-165">Status da identidade do dispositivo importado</span><span class="sxs-lookup"><span data-stu-id="995ed-165">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="995ed-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="995ed-166">Response</span></span>
<span data-ttu-id="995ed-167">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="995ed-167">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="995ed-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="995ed-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="995ed-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="995ed-169">Request</span></span>
<span data-ttu-id="995ed-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="995ed-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="995ed-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="995ed-171">Response</span></span>
<span data-ttu-id="995ed-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="995ed-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






