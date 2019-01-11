---
title: Atualizar importedDeviceIdentityResult
description: Atualize as propriedades de um objeto importedDeviceIdentityResult.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7fe9472b0f63ada966c61dd8fc56a7865cf94408
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827570"
---
# <a name="update-importeddeviceidentityresult"></a><span data-ttu-id="d5f4c-103">Atualizar importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="d5f4c-103">Update importedDeviceIdentityResult</span></span>

> <span data-ttu-id="d5f4c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d5f4c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5f4c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d5f4c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5f4c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d5f4c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5f4c-107">Atualize as propriedades de um objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="d5f4c-107">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5f4c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d5f4c-108">Prerequisites</span></span>
<span data-ttu-id="d5f4c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5f4c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5f4c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5f4c-111">Permission type</span></span>|<span data-ttu-id="d5f4c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d5f4c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5f4c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5f4c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5f4c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5f4c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d5f4c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5f4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5f4c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5f4c-116">Not supported.</span></span>|
|<span data-ttu-id="d5f4c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5f4c-117">Application</span></span>|<span data-ttu-id="d5f4c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5f4c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5f4c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5f4c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="d5f4c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5f4c-120">Request headers</span></span>
|<span data-ttu-id="d5f4c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5f4c-121">Header</span></span>|<span data-ttu-id="d5f4c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d5f4c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5f4c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5f4c-123">Authorization</span></span>|<span data-ttu-id="d5f4c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5f4c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5f4c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d5f4c-125">Accept</span></span>|<span data-ttu-id="d5f4c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5f4c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5f4c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5f4c-127">Request body</span></span>
<span data-ttu-id="d5f4c-128">No corpo da solicitação, fornece uma representação JSON para o objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="d5f4c-128">In the request body, supply a JSON representation for the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

<span data-ttu-id="d5f4c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="d5f4c-129">The following table shows the properties that are required when you create the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>

|<span data-ttu-id="d5f4c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5f4c-130">Property</span></span>|<span data-ttu-id="d5f4c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5f4c-131">Type</span></span>|<span data-ttu-id="d5f4c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5f4c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5f4c-133">id</span><span class="sxs-lookup"><span data-stu-id="d5f4c-133">id</span></span>|<span data-ttu-id="d5f4c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5f4c-134">String</span></span>|<span data-ttu-id="d5f4c-135">ID da identidade do dispositivo importada Inherited de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d5f4c-135">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="d5f4c-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="d5f4c-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="d5f4c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5f4c-137">String</span></span>|<span data-ttu-id="d5f4c-138">Importados dispositivo identificador herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d5f4c-138">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="d5f4c-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="d5f4c-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="d5f4c-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="d5f4c-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="d5f4c-141">Tipo de importado herdadas de identidade do dispositivo de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="d5f4c-141">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="d5f4c-142">Os valores possíveis são: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="d5f4c-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="d5f4c-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5f4c-143">lastModifiedDateTime</span></span>|<span data-ttu-id="d5f4c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5f4c-144">DateTimeOffset</span></span>|<span data-ttu-id="d5f4c-145">Última DateTime modificação da descrição Inherited de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d5f4c-145">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="d5f4c-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5f4c-146">createdDateTime</span></span>|<span data-ttu-id="d5f4c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5f4c-147">DateTimeOffset</span></span>|<span data-ttu-id="d5f4c-148">Data-hora do dispositivo Inherited de criação de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d5f4c-148">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="d5f4c-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5f4c-149">lastContactedDateTime</span></span>|<span data-ttu-id="d5f4c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5f4c-150">DateTimeOffset</span></span>|<span data-ttu-id="d5f4c-151">Última contatado data hora do dispositivo Inherited de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d5f4c-151">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="d5f4c-152">description</span><span class="sxs-lookup"><span data-stu-id="d5f4c-152">description</span></span>|<span data-ttu-id="d5f4c-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5f4c-153">String</span></span>|<span data-ttu-id="d5f4c-154">A descrição do dispositivo Inherited de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d5f4c-154">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="d5f4c-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="d5f4c-155">enrollmentState</span></span>|[<span data-ttu-id="d5f4c-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="d5f4c-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="d5f4c-157">O estado do dispositivo em Intune herdada do [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="d5f4c-157">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="d5f4c-158">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="d5f4c-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="d5f4c-159">platform</span><span class="sxs-lookup"><span data-stu-id="d5f4c-159">platform</span></span>|[<span data-ttu-id="d5f4c-160">plataforma</span><span class="sxs-lookup"><span data-stu-id="d5f4c-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="d5f4c-161">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5f4c-161">The platform of the Device.</span></span> <span data-ttu-id="d5f4c-162">Herdada do [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="d5f4c-162">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="d5f4c-163">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="d5f4c-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="d5f4c-164">status</span><span class="sxs-lookup"><span data-stu-id="d5f4c-164">status</span></span>|<span data-ttu-id="d5f4c-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="d5f4c-165">Boolean</span></span>|<span data-ttu-id="d5f4c-166">Status da identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="d5f4c-166">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="d5f4c-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5f4c-167">Response</span></span>
<span data-ttu-id="d5f4c-168">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5f4c-168">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5f4c-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5f4c-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="d5f4c-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5f4c-170">Request</span></span>
<span data-ttu-id="d5f4c-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5f4c-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 354

{
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

### <a name="response"></a><span data-ttu-id="d5f4c-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5f4c-172">Response</span></span>
<span data-ttu-id="d5f4c-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5f4c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





