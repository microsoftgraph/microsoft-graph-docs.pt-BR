---
title: Atualizar importedDeviceIdentityResult
description: Atualiza as propriedades de um objeto importedDeviceIdentityResult.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 950c28c2ad8281667c7458cc321c470f4100b53d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466518"
---
# <a name="update-importeddeviceidentityresult"></a><span data-ttu-id="227ec-103">Atualizar importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="227ec-103">Update importedDeviceIdentityResult</span></span>

<span data-ttu-id="227ec-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="227ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="227ec-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="227ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="227ec-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="227ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="227ec-107">Atualiza as propriedades de um objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="227ec-107">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="227ec-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="227ec-108">Prerequisites</span></span>
<span data-ttu-id="227ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="227ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="227ec-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="227ec-111">Permission type</span></span>|<span data-ttu-id="227ec-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="227ec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="227ec-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="227ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="227ec-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="227ec-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="227ec-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="227ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="227ec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="227ec-116">Not supported.</span></span>|
|<span data-ttu-id="227ec-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="227ec-117">Application</span></span>|<span data-ttu-id="227ec-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="227ec-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="227ec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="227ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="227ec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="227ec-120">Request headers</span></span>
|<span data-ttu-id="227ec-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="227ec-121">Header</span></span>|<span data-ttu-id="227ec-122">Valor</span><span class="sxs-lookup"><span data-stu-id="227ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="227ec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="227ec-123">Authorization</span></span>|<span data-ttu-id="227ec-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="227ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="227ec-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="227ec-125">Accept</span></span>|<span data-ttu-id="227ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="227ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="227ec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="227ec-127">Request body</span></span>
<span data-ttu-id="227ec-128">No corpo da solicitação, forneça uma representação JSON do objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="227ec-128">In the request body, supply a JSON representation for the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

<span data-ttu-id="227ec-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="227ec-129">The following table shows the properties that are required when you create the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>

|<span data-ttu-id="227ec-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="227ec-130">Property</span></span>|<span data-ttu-id="227ec-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="227ec-131">Type</span></span>|<span data-ttu-id="227ec-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="227ec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="227ec-133">id</span><span class="sxs-lookup"><span data-stu-id="227ec-133">id</span></span>|<span data-ttu-id="227ec-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="227ec-134">String</span></span>|<span data-ttu-id="227ec-135">ID da identidade de dispositivo importada herdada de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="227ec-135">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="227ec-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="227ec-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="227ec-137">String</span><span class="sxs-lookup"><span data-stu-id="227ec-137">String</span></span>|<span data-ttu-id="227ec-138">Identificador de dispositivo importado herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="227ec-138">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="227ec-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="227ec-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="227ec-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="227ec-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="227ec-141">Tipo de identidade de dispositivo importado herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="227ec-141">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="227ec-142">Os valores possíveis são: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="227ec-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="227ec-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="227ec-143">lastModifiedDateTime</span></span>|<span data-ttu-id="227ec-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="227ec-144">DateTimeOffset</span></span>|<span data-ttu-id="227ec-145">Data e hora da última modificação da descrição herdadas de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="227ec-145">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="227ec-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="227ec-146">createdDateTime</span></span>|<span data-ttu-id="227ec-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="227ec-147">DateTimeOffset</span></span>|<span data-ttu-id="227ec-148">Data e hora de criação do dispositivo herdadas de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="227ec-148">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="227ec-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="227ec-149">lastContactedDateTime</span></span>|<span data-ttu-id="227ec-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="227ec-150">DateTimeOffset</span></span>|<span data-ttu-id="227ec-151">Data e hora do último contato do dispositivo herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="227ec-151">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="227ec-152">description</span><span class="sxs-lookup"><span data-stu-id="227ec-152">description</span></span>|<span data-ttu-id="227ec-153">String</span><span class="sxs-lookup"><span data-stu-id="227ec-153">String</span></span>|<span data-ttu-id="227ec-154">A descrição do dispositivo herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="227ec-154">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="227ec-155">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="227ec-155">enrollmentState</span></span>|[<span data-ttu-id="227ec-156">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="227ec-156">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="227ec-157">O estado do dispositivo no Intune herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="227ec-157">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="227ec-158">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="227ec-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="227ec-159">platform</span><span class="sxs-lookup"><span data-stu-id="227ec-159">platform</span></span>|[<span data-ttu-id="227ec-160">plataforma</span><span class="sxs-lookup"><span data-stu-id="227ec-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="227ec-161">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="227ec-161">The platform of the Device.</span></span> <span data-ttu-id="227ec-162">Herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="227ec-162">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="227ec-163">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="227ec-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="227ec-164">status</span><span class="sxs-lookup"><span data-stu-id="227ec-164">status</span></span>|<span data-ttu-id="227ec-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="227ec-165">Boolean</span></span>|<span data-ttu-id="227ec-166">Status da identidade do dispositivo importado</span><span class="sxs-lookup"><span data-stu-id="227ec-166">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="227ec-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="227ec-167">Response</span></span>
<span data-ttu-id="227ec-168">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="227ec-168">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="227ec-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="227ec-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="227ec-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="227ec-170">Request</span></span>
<span data-ttu-id="227ec-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="227ec-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="227ec-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="227ec-172">Response</span></span>
<span data-ttu-id="227ec-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="227ec-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





