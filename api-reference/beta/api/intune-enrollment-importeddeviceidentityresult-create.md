---
title: Criar importedDeviceIdentityResult
description: Crie um novo objeto de importedDeviceIdentityResult.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05f3880d005d78463c3225b0eef501dba5e21299
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416269"
---
# <a name="create-importeddeviceidentityresult"></a><span data-ttu-id="248dc-103">Criar importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="248dc-103">Create importedDeviceIdentityResult</span></span>

> <span data-ttu-id="248dc-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="248dc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="248dc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="248dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="248dc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="248dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="248dc-107">Crie um novo objeto de [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="248dc-107">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="248dc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="248dc-108">Prerequisites</span></span>
<span data-ttu-id="248dc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="248dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="248dc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="248dc-111">Permission type</span></span>|<span data-ttu-id="248dc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="248dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="248dc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="248dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="248dc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="248dc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="248dc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="248dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="248dc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="248dc-116">Not supported.</span></span>|
|<span data-ttu-id="248dc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="248dc-117">Application</span></span>|<span data-ttu-id="248dc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="248dc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="248dc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="248dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="248dc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="248dc-120">Request headers</span></span>
|<span data-ttu-id="248dc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="248dc-121">Header</span></span>|<span data-ttu-id="248dc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="248dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="248dc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="248dc-123">Authorization</span></span>|<span data-ttu-id="248dc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="248dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="248dc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="248dc-125">Accept</span></span>|<span data-ttu-id="248dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="248dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="248dc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="248dc-127">Request body</span></span>
<span data-ttu-id="248dc-128">No corpo da solicitação, fornece uma representação JSON para o objeto importedDeviceIdentityResult.</span><span class="sxs-lookup"><span data-stu-id="248dc-128">In the request body, supply a JSON representation for the importedDeviceIdentityResult object.</span></span>

<span data-ttu-id="248dc-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o importedDeviceIdentityResult.</span><span class="sxs-lookup"><span data-stu-id="248dc-129">The following table shows the properties that are required when you create the importedDeviceIdentityResult.</span></span>

|<span data-ttu-id="248dc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="248dc-130">Property</span></span>|<span data-ttu-id="248dc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="248dc-131">Type</span></span>|<span data-ttu-id="248dc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="248dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="248dc-133">id</span><span class="sxs-lookup"><span data-stu-id="248dc-133">id</span></span>|<span data-ttu-id="248dc-134">String</span><span class="sxs-lookup"><span data-stu-id="248dc-134">String</span></span>|<span data-ttu-id="248dc-135">ID da identidade do dispositivo importada Inherited de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="248dc-135">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="248dc-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="248dc-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="248dc-137">String</span><span class="sxs-lookup"><span data-stu-id="248dc-137">String</span></span>|<span data-ttu-id="248dc-138">Importados dispositivo identificador herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="248dc-138">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="248dc-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="248dc-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="248dc-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="248dc-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="248dc-141">Tipo de importado herdadas de identidade do dispositivo de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="248dc-141">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="248dc-142">Os valores possíveis são: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="248dc-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="248dc-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="248dc-143">lastModifiedDateTime</span></span>|<span data-ttu-id="248dc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="248dc-144">DateTimeOffset</span></span>|<span data-ttu-id="248dc-145">Última DateTime modificação da descrição Inherited de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="248dc-145">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="248dc-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="248dc-146">createdDateTime</span></span>|<span data-ttu-id="248dc-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="248dc-147">DateTimeOffset</span></span>|<span data-ttu-id="248dc-148">Data-hora do dispositivo Inherited de criação de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="248dc-148">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="248dc-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="248dc-149">lastContactedDateTime</span></span>|<span data-ttu-id="248dc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="248dc-150">DateTimeOffset</span></span>|<span data-ttu-id="248dc-151">Última contatado data hora do dispositivo Inherited de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="248dc-151">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="248dc-152">description</span><span class="sxs-lookup"><span data-stu-id="248dc-152">description</span></span>|<span data-ttu-id="248dc-153">String</span><span class="sxs-lookup"><span data-stu-id="248dc-153">String</span></span>|<span data-ttu-id="248dc-154">A descrição do dispositivo Inherited de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="248dc-154">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="248dc-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="248dc-155">enrollmentState</span></span>|[<span data-ttu-id="248dc-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="248dc-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="248dc-157">O estado do dispositivo em Intune herdada do [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="248dc-157">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="248dc-158">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="248dc-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="248dc-159">platform</span><span class="sxs-lookup"><span data-stu-id="248dc-159">platform</span></span>|[<span data-ttu-id="248dc-160">plataforma</span><span class="sxs-lookup"><span data-stu-id="248dc-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="248dc-161">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="248dc-161">The platform of the Device.</span></span> <span data-ttu-id="248dc-162">Herdada do [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="248dc-162">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="248dc-163">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="248dc-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="248dc-164">status</span><span class="sxs-lookup"><span data-stu-id="248dc-164">status</span></span>|<span data-ttu-id="248dc-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="248dc-165">Boolean</span></span>|<span data-ttu-id="248dc-166">Status da identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="248dc-166">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="248dc-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="248dc-167">Response</span></span>
<span data-ttu-id="248dc-168">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="248dc-168">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="248dc-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="248dc-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="248dc-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="248dc-170">Request</span></span>
<span data-ttu-id="248dc-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="248dc-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="248dc-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="248dc-172">Response</span></span>
<span data-ttu-id="248dc-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="248dc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




