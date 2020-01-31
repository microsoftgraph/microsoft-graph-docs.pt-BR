---
title: Atualizar deviceEnrollmentPlatformRestrictionsConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b67571700f94ac292268c2e164bc2e483cc36420
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41634967"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="81ff6-103">Atualizar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="81ff6-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="81ff6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81ff6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81ff6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81ff6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81ff6-106">Atualizar as propriedades de um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81ff6-106">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81ff6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81ff6-107">Prerequisites</span></span>
<span data-ttu-id="81ff6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81ff6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81ff6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81ff6-110">Permission type</span></span>|<span data-ttu-id="81ff6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81ff6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81ff6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81ff6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81ff6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81ff6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="81ff6-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81ff6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81ff6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81ff6-115">Not supported.</span></span>|
|<span data-ttu-id="81ff6-116">Application</span><span class="sxs-lookup"><span data-stu-id="81ff6-116">Application</span></span>|<span data-ttu-id="81ff6-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81ff6-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81ff6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81ff6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="81ff6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81ff6-119">Request headers</span></span>
|<span data-ttu-id="81ff6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81ff6-120">Header</span></span>|<span data-ttu-id="81ff6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="81ff6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81ff6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="81ff6-122">Authorization</span></span>|<span data-ttu-id="81ff6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81ff6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81ff6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81ff6-124">Accept</span></span>|<span data-ttu-id="81ff6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81ff6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81ff6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81ff6-126">Request body</span></span>
<span data-ttu-id="81ff6-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81ff6-127">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="81ff6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81ff6-128">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="81ff6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81ff6-129">Property</span></span>|<span data-ttu-id="81ff6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="81ff6-130">Type</span></span>|<span data-ttu-id="81ff6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="81ff6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81ff6-132">id</span><span class="sxs-lookup"><span data-stu-id="81ff6-132">id</span></span>|<span data-ttu-id="81ff6-133">String</span><span class="sxs-lookup"><span data-stu-id="81ff6-133">String</span></span>|<span data-ttu-id="81ff6-134">Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ff6-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="81ff6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="81ff6-135">displayName</span></span>|<span data-ttu-id="81ff6-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81ff6-136">String</span></span>|<span data-ttu-id="81ff6-137">O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ff6-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="81ff6-138">description</span><span class="sxs-lookup"><span data-stu-id="81ff6-138">description</span></span>|<span data-ttu-id="81ff6-139">String</span><span class="sxs-lookup"><span data-stu-id="81ff6-139">String</span></span>|<span data-ttu-id="81ff6-140">A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ff6-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="81ff6-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="81ff6-141">priority</span></span>|<span data-ttu-id="81ff6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="81ff6-142">Int32</span></span>|<span data-ttu-id="81ff6-143">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="81ff6-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="81ff6-144">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="81ff6-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="81ff6-145">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ff6-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="81ff6-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81ff6-146">createdDateTime</span></span>|<span data-ttu-id="81ff6-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81ff6-147">DateTimeOffset</span></span>|<span data-ttu-id="81ff6-148">Data e hora de criação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ff6-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="81ff6-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81ff6-149">lastModifiedDateTime</span></span>|<span data-ttu-id="81ff6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81ff6-150">DateTimeOffset</span></span>|<span data-ttu-id="81ff6-151">Data e hora da última modificação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ff6-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="81ff6-152">versão</span><span class="sxs-lookup"><span data-stu-id="81ff6-152">version</span></span>|<span data-ttu-id="81ff6-153">Int32</span><span class="sxs-lookup"><span data-stu-id="81ff6-153">Int32</span></span>|<span data-ttu-id="81ff6-154">A versão da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81ff6-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="81ff6-155">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="81ff6-155">iosRestriction</span></span>|[<span data-ttu-id="81ff6-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="81ff6-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="81ff6-157">Restrições do IOS com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="81ff6-157">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="81ff6-158">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="81ff6-158">windowsRestriction</span></span>|[<span data-ttu-id="81ff6-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="81ff6-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="81ff6-160">Restrições do Windows com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="81ff6-160">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="81ff6-161">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="81ff6-161">windowsMobileRestriction</span></span>|[<span data-ttu-id="81ff6-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="81ff6-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="81ff6-163">Restrições do Windows Mobile com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="81ff6-163">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="81ff6-164">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="81ff6-164">androidRestriction</span></span>|[<span data-ttu-id="81ff6-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="81ff6-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="81ff6-166">Restrições do Android com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="81ff6-166">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="81ff6-167">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="81ff6-167">androidForWorkRestriction</span></span>|[<span data-ttu-id="81ff6-168">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="81ff6-168">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="81ff6-169">O Android para restrições de trabalho com base na plataforma, na versão do sistema operacional da plataforma e na Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="81ff6-169">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="81ff6-170">macRestriction</span><span class="sxs-lookup"><span data-stu-id="81ff6-170">macRestriction</span></span>|[<span data-ttu-id="81ff6-171">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="81ff6-171">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="81ff6-172">Restrições de Mac com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="81ff6-172">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="81ff6-173">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="81ff6-173">macOSRestriction</span></span>|[<span data-ttu-id="81ff6-174">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="81ff6-174">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="81ff6-175">Restrições de Mac com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="81ff6-175">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="81ff6-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="81ff6-176">Response</span></span>
<span data-ttu-id="81ff6-177">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81ff6-177">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81ff6-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81ff6-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="81ff6-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81ff6-179">Request</span></span>
<span data-ttu-id="81ff6-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81ff6-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 2763

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="81ff6-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="81ff6-181">Response</span></span>
<span data-ttu-id="81ff6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81ff6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2935

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  }
}
```





