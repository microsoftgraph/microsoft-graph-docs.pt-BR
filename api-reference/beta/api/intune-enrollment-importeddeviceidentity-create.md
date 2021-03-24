---
title: Criar importedDeviceIdentity
description: Crie um novo objeto importedDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a803d8916da8ffeaed9d3e642c802143413152cf
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142370"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="26594-103">Criar importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="26594-103">Create importedDeviceIdentity</span></span>

<span data-ttu-id="26594-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26594-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26594-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26594-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26594-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26594-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26594-107">Crie um novo [objeto importedDeviceIdentity.](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="26594-107">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26594-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26594-108">Prerequisites</span></span>
<span data-ttu-id="26594-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26594-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26594-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26594-111">Permission type</span></span>|<span data-ttu-id="26594-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26594-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26594-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26594-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26594-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26594-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="26594-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26594-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26594-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26594-116">Not supported.</span></span>|
|<span data-ttu-id="26594-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26594-117">Application</span></span>|<span data-ttu-id="26594-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26594-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26594-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26594-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="26594-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26594-120">Request headers</span></span>
|<span data-ttu-id="26594-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26594-121">Header</span></span>|<span data-ttu-id="26594-122">Valor</span><span class="sxs-lookup"><span data-stu-id="26594-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26594-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="26594-123">Authorization</span></span>|<span data-ttu-id="26594-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26594-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26594-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26594-125">Accept</span></span>|<span data-ttu-id="26594-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26594-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26594-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26594-127">Request body</span></span>
<span data-ttu-id="26594-128">No corpo da solicitação, fornece uma representação JSON para o objeto importedDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="26594-128">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="26594-129">A tabela a seguir mostra as propriedades que são necessárias ao criar importDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="26594-129">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="26594-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26594-130">Property</span></span>|<span data-ttu-id="26594-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="26594-131">Type</span></span>|<span data-ttu-id="26594-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="26594-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26594-133">id</span><span class="sxs-lookup"><span data-stu-id="26594-133">id</span></span>|<span data-ttu-id="26594-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26594-134">String</span></span>|<span data-ttu-id="26594-135">ID da identidade do dispositivo importado</span><span class="sxs-lookup"><span data-stu-id="26594-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="26594-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="26594-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="26594-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26594-137">String</span></span>|<span data-ttu-id="26594-138">Identificador de Dispositivo Importado</span><span class="sxs-lookup"><span data-stu-id="26594-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="26594-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="26594-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="26594-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="26594-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="26594-141">Tipo de Identidade de Dispositivo Importado.</span><span class="sxs-lookup"><span data-stu-id="26594-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="26594-142">Os valores possíveis são: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="26594-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="26594-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26594-143">lastModifiedDateTime</span></span>|<span data-ttu-id="26594-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26594-144">DateTimeOffset</span></span>|<span data-ttu-id="26594-145">Last Modified DateTime of the description</span><span class="sxs-lookup"><span data-stu-id="26594-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="26594-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26594-146">createdDateTime</span></span>|<span data-ttu-id="26594-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26594-147">DateTimeOffset</span></span>|<span data-ttu-id="26594-148">Data de criação hora do dispositivo</span><span class="sxs-lookup"><span data-stu-id="26594-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="26594-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="26594-149">lastContactedDateTime</span></span>|<span data-ttu-id="26594-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26594-150">DateTimeOffset</span></span>|<span data-ttu-id="26594-151">Hora da Última Data Contata do dispositivo</span><span class="sxs-lookup"><span data-stu-id="26594-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="26594-152">descrição</span><span class="sxs-lookup"><span data-stu-id="26594-152">description</span></span>|<span data-ttu-id="26594-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26594-153">String</span></span>|<span data-ttu-id="26594-154">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="26594-154">The description of the device</span></span>|
|<span data-ttu-id="26594-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="26594-155">enrollmentState</span></span>|[<span data-ttu-id="26594-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="26594-156">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="26594-157">O estado do dispositivo no Intune.</span><span class="sxs-lookup"><span data-stu-id="26594-157">The state of the device in Intune.</span></span> <span data-ttu-id="26594-158">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="26594-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="26594-159">plataforma</span><span class="sxs-lookup"><span data-stu-id="26594-159">platform</span></span>|[<span data-ttu-id="26594-160">platform</span><span class="sxs-lookup"><span data-stu-id="26594-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="26594-161">A plataforma do Dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26594-161">The platform of the Device.</span></span> <span data-ttu-id="26594-162">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="26594-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="26594-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="26594-163">Response</span></span>
<span data-ttu-id="26594-164">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26594-164">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26594-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26594-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="26594-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26594-166">Request</span></span>
<span data-ttu-id="26594-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26594-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="26594-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="26594-168">Response</span></span>
<span data-ttu-id="26594-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26594-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




