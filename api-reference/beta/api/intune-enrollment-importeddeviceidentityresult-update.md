---
title: Atualizar importedDeviceIdentityResult
description: Atualize as propriedades de um objeto importedDeviceIdentityResult.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 36f71f2d4d1494e459e2cf9f9867d354a931a2f1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142216"
---
# <a name="update-importeddeviceidentityresult"></a><span data-ttu-id="38431-103">Atualizar importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="38431-103">Update importedDeviceIdentityResult</span></span>

<span data-ttu-id="38431-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38431-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38431-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="38431-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38431-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="38431-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38431-107">Atualize as propriedades de [um objeto importedDeviceIdentityResult.](../resources/intune-enrollment-importeddeviceidentityresult.md)</span><span class="sxs-lookup"><span data-stu-id="38431-107">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38431-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38431-108">Prerequisites</span></span>
<span data-ttu-id="38431-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38431-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38431-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38431-111">Permission type</span></span>|<span data-ttu-id="38431-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38431-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38431-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38431-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38431-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38431-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="38431-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38431-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38431-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38431-116">Not supported.</span></span>|
|<span data-ttu-id="38431-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38431-117">Application</span></span>|<span data-ttu-id="38431-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38431-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38431-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38431-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="38431-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38431-120">Request headers</span></span>
|<span data-ttu-id="38431-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38431-121">Header</span></span>|<span data-ttu-id="38431-122">Valor</span><span class="sxs-lookup"><span data-stu-id="38431-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38431-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="38431-123">Authorization</span></span>|<span data-ttu-id="38431-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38431-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38431-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="38431-125">Accept</span></span>|<span data-ttu-id="38431-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38431-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38431-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38431-127">Request body</span></span>
<span data-ttu-id="38431-128">No corpo da solicitação, fornece uma representação JSON para o [objeto importedDeviceIdentityResult.](../resources/intune-enrollment-importeddeviceidentityresult.md)</span><span class="sxs-lookup"><span data-stu-id="38431-128">In the request body, supply a JSON representation for the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

<span data-ttu-id="38431-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [importDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="38431-129">The following table shows the properties that are required when you create the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>

|<span data-ttu-id="38431-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38431-130">Property</span></span>|<span data-ttu-id="38431-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="38431-131">Type</span></span>|<span data-ttu-id="38431-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="38431-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38431-133">id</span><span class="sxs-lookup"><span data-stu-id="38431-133">id</span></span>|<span data-ttu-id="38431-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38431-134">String</span></span>|<span data-ttu-id="38431-135">ID da identidade do dispositivo importado Herdada de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="38431-135">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="38431-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="38431-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="38431-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38431-137">String</span></span>|<span data-ttu-id="38431-138">Identificador de Dispositivo Importado Herdado [de importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="38431-138">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="38431-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="38431-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="38431-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="38431-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="38431-141">Tipo de Identidade de Dispositivo Importado Herdada [de importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="38431-141">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="38431-142">Os valores possíveis são: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="38431-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="38431-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38431-143">lastModifiedDateTime</span></span>|<span data-ttu-id="38431-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38431-144">DateTimeOffset</span></span>|<span data-ttu-id="38431-145">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="38431-145">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="38431-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38431-146">createdDateTime</span></span>|<span data-ttu-id="38431-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38431-147">DateTimeOffset</span></span>|<span data-ttu-id="38431-148">Data de criação Hora do dispositivo Herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="38431-148">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="38431-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="38431-149">lastContactedDateTime</span></span>|<span data-ttu-id="38431-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38431-150">DateTimeOffset</span></span>|<span data-ttu-id="38431-151">Hora da Última Data Contada do dispositivo Herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="38431-151">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="38431-152">descrição</span><span class="sxs-lookup"><span data-stu-id="38431-152">description</span></span>|<span data-ttu-id="38431-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38431-153">String</span></span>|<span data-ttu-id="38431-154">A descrição do dispositivo Herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="38431-154">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="38431-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="38431-155">enrollmentState</span></span>|[<span data-ttu-id="38431-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="38431-156">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="38431-157">O estado do dispositivo no Intune Herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="38431-157">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="38431-158">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="38431-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="38431-159">plataforma</span><span class="sxs-lookup"><span data-stu-id="38431-159">platform</span></span>|[<span data-ttu-id="38431-160">platform</span><span class="sxs-lookup"><span data-stu-id="38431-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="38431-161">A plataforma do Dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38431-161">The platform of the Device.</span></span> <span data-ttu-id="38431-162">Herdado [de importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="38431-162">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="38431-163">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="38431-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="38431-164">status</span><span class="sxs-lookup"><span data-stu-id="38431-164">status</span></span>|<span data-ttu-id="38431-165">Booleano</span><span class="sxs-lookup"><span data-stu-id="38431-165">Boolean</span></span>|<span data-ttu-id="38431-166">Status da identidade do dispositivo importado</span><span class="sxs-lookup"><span data-stu-id="38431-166">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="38431-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="38431-167">Response</span></span>
<span data-ttu-id="38431-168">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38431-168">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38431-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38431-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="38431-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38431-170">Request</span></span>
<span data-ttu-id="38431-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38431-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="38431-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="38431-172">Response</span></span>
<span data-ttu-id="38431-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38431-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




