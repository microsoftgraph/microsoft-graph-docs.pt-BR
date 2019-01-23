---
title: Criar importedDeviceIdentity
description: Crie um novo objeto de importedDeviceIdentity.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d0274f3a48c3481cc5540eb9025da353f0ea0bf2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396711"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="5ab4c-103">Criar importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="5ab4c-103">Create importedDeviceIdentity</span></span>

> <span data-ttu-id="5ab4c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5ab4c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5ab4c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ab4c-107">Crie um novo objeto de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="5ab4c-107">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ab4c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ab4c-108">Prerequisites</span></span>
<span data-ttu-id="5ab4c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5ab4c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5ab4c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ab4c-111">Permission type</span></span>|<span data-ttu-id="5ab4c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ab4c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ab4c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ab4c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ab4c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ab4c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5ab4c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ab4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ab4c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-116">Not supported.</span></span>|
|<span data-ttu-id="5ab4c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ab4c-117">Application</span></span>|<span data-ttu-id="5ab4c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ab4c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ab4c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="5ab4c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ab4c-120">Request headers</span></span>
|<span data-ttu-id="5ab4c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ab4c-121">Header</span></span>|<span data-ttu-id="5ab4c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5ab4c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ab4c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ab4c-123">Authorization</span></span>|<span data-ttu-id="5ab4c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ab4c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ab4c-125">Accept</span></span>|<span data-ttu-id="5ab4c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ab4c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ab4c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ab4c-127">Request body</span></span>
<span data-ttu-id="5ab4c-128">No corpo da solicitação, fornece uma representação JSON para o objeto importedDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-128">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="5ab4c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o importedDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-129">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="5ab4c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ab4c-130">Property</span></span>|<span data-ttu-id="5ab4c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ab4c-131">Type</span></span>|<span data-ttu-id="5ab4c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ab4c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ab4c-133">id</span><span class="sxs-lookup"><span data-stu-id="5ab4c-133">id</span></span>|<span data-ttu-id="5ab4c-134">String</span><span class="sxs-lookup"><span data-stu-id="5ab4c-134">String</span></span>|<span data-ttu-id="5ab4c-135">ID da identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="5ab4c-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="5ab4c-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="5ab4c-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="5ab4c-137">String</span><span class="sxs-lookup"><span data-stu-id="5ab4c-137">String</span></span>|<span data-ttu-id="5ab4c-138">Identificador de dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="5ab4c-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="5ab4c-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="5ab4c-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="5ab4c-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="5ab4c-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="5ab4c-141">Tipo de identidade do dispositivo importada.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="5ab4c-142">Os valores possíveis são: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="5ab4c-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ab4c-143">lastModifiedDateTime</span></span>|<span data-ttu-id="5ab4c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ab4c-144">DateTimeOffset</span></span>|<span data-ttu-id="5ab4c-145">Última data e hora modificadas da descrição</span><span class="sxs-lookup"><span data-stu-id="5ab4c-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="5ab4c-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ab4c-146">createdDateTime</span></span>|<span data-ttu-id="5ab4c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ab4c-147">DateTimeOffset</span></span>|<span data-ttu-id="5ab4c-148">Criada data hora do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5ab4c-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="5ab4c-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ab4c-149">lastContactedDateTime</span></span>|<span data-ttu-id="5ab4c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ab4c-150">DateTimeOffset</span></span>|<span data-ttu-id="5ab4c-151">Última contatado data hora do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5ab4c-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="5ab4c-152">description</span><span class="sxs-lookup"><span data-stu-id="5ab4c-152">description</span></span>|<span data-ttu-id="5ab4c-153">String</span><span class="sxs-lookup"><span data-stu-id="5ab4c-153">String</span></span>|<span data-ttu-id="5ab4c-154">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5ab4c-154">The description of the device</span></span>|
|<span data-ttu-id="5ab4c-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="5ab4c-155">enrollmentState</span></span>|[<span data-ttu-id="5ab4c-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="5ab4c-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="5ab4c-157">O estado do dispositivo em Intune.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-157">The state of the device in Intune.</span></span> <span data-ttu-id="5ab4c-158">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="5ab4c-159">platform</span><span class="sxs-lookup"><span data-stu-id="5ab4c-159">platform</span></span>|[<span data-ttu-id="5ab4c-160">plataforma</span><span class="sxs-lookup"><span data-stu-id="5ab4c-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="5ab4c-161">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-161">The platform of the Device.</span></span> <span data-ttu-id="5ab4c-162">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="5ab4c-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ab4c-163">Response</span></span>
<span data-ttu-id="5ab4c-164">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-164">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ab4c-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ab4c-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ab4c-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ab4c-166">Request</span></span>
<span data-ttu-id="5ab4c-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5ab4c-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ab4c-168">Response</span></span>
<span data-ttu-id="5ab4c-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ab4c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




