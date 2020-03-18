---
title: Criar deviceEnrollmentPlatformRestrictionsConfiguration
description: Criar um novo objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: afb50a310085a0c82aa521be220ca0e9f3ac562f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803004"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="a8f53-103">Criar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8f53-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="a8f53-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8f53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8f53-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8f53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8f53-106">Criar um novo objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8f53-106">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8f53-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a8f53-107">Prerequisites</span></span>
<span data-ttu-id="a8f53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8f53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8f53-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8f53-110">Permission type</span></span>|<span data-ttu-id="a8f53-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a8f53-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8f53-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8f53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8f53-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8f53-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a8f53-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8f53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8f53-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8f53-115">Not supported.</span></span>|
|<span data-ttu-id="a8f53-116">Application</span><span class="sxs-lookup"><span data-stu-id="a8f53-116">Application</span></span>|<span data-ttu-id="a8f53-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8f53-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8f53-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8f53-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a8f53-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8f53-119">Request headers</span></span>
|<span data-ttu-id="a8f53-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8f53-120">Header</span></span>|<span data-ttu-id="a8f53-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a8f53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8f53-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8f53-122">Authorization</span></span>|<span data-ttu-id="a8f53-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8f53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8f53-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a8f53-124">Accept</span></span>|<span data-ttu-id="a8f53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a8f53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8f53-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8f53-126">Request body</span></span>
<span data-ttu-id="a8f53-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a8f53-127">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="a8f53-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a8f53-128">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="a8f53-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8f53-129">Property</span></span>|<span data-ttu-id="a8f53-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8f53-130">Type</span></span>|<span data-ttu-id="a8f53-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8f53-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8f53-132">id</span><span class="sxs-lookup"><span data-stu-id="a8f53-132">id</span></span>|<span data-ttu-id="a8f53-133">String</span><span class="sxs-lookup"><span data-stu-id="a8f53-133">String</span></span>|<span data-ttu-id="a8f53-134">Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8f53-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a8f53-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a8f53-135">displayName</span></span>|<span data-ttu-id="a8f53-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8f53-136">String</span></span>|<span data-ttu-id="a8f53-137">O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8f53-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a8f53-138">description</span><span class="sxs-lookup"><span data-stu-id="a8f53-138">description</span></span>|<span data-ttu-id="a8f53-139">String</span><span class="sxs-lookup"><span data-stu-id="a8f53-139">String</span></span>|<span data-ttu-id="a8f53-140">A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8f53-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a8f53-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="a8f53-141">priority</span></span>|<span data-ttu-id="a8f53-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a8f53-142">Int32</span></span>|<span data-ttu-id="a8f53-143">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="a8f53-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="a8f53-144">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="a8f53-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="a8f53-145">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8f53-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a8f53-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8f53-146">createdDateTime</span></span>|<span data-ttu-id="a8f53-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8f53-147">DateTimeOffset</span></span>|<span data-ttu-id="a8f53-148">Data e hora de criação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8f53-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a8f53-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8f53-149">lastModifiedDateTime</span></span>|<span data-ttu-id="a8f53-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8f53-150">DateTimeOffset</span></span>|<span data-ttu-id="a8f53-151">Data e hora da última modificação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8f53-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a8f53-152">versão</span><span class="sxs-lookup"><span data-stu-id="a8f53-152">version</span></span>|<span data-ttu-id="a8f53-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a8f53-153">Int32</span></span>|<span data-ttu-id="a8f53-154">A versão da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8f53-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a8f53-155">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="a8f53-155">iosRestriction</span></span>|[<span data-ttu-id="a8f53-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a8f53-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a8f53-157">Restrições do IOS com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a8f53-157">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="a8f53-158">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="a8f53-158">windowsRestriction</span></span>|[<span data-ttu-id="a8f53-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a8f53-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a8f53-160">Restrições do Windows com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a8f53-160">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="a8f53-161">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="a8f53-161">windowsMobileRestriction</span></span>|[<span data-ttu-id="a8f53-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a8f53-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a8f53-163">Restrições do Windows Mobile com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a8f53-163">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="a8f53-164">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="a8f53-164">androidRestriction</span></span>|[<span data-ttu-id="a8f53-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a8f53-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a8f53-166">Restrições do Android com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a8f53-166">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="a8f53-167">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="a8f53-167">androidForWorkRestriction</span></span>|[<span data-ttu-id="a8f53-168">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a8f53-168">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a8f53-169">O Android para restrições de trabalho com base na plataforma, na versão do sistema operacional da plataforma e na Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a8f53-169">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="a8f53-170">macRestriction</span><span class="sxs-lookup"><span data-stu-id="a8f53-170">macRestriction</span></span>|[<span data-ttu-id="a8f53-171">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a8f53-171">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a8f53-172">Restrições de Mac com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a8f53-172">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="a8f53-173">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="a8f53-173">macOSRestriction</span></span>|[<span data-ttu-id="a8f53-174">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a8f53-174">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a8f53-175">Restrições de Mac com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a8f53-175">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="a8f53-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8f53-176">Response</span></span>
<span data-ttu-id="a8f53-177">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8f53-177">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8f53-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8f53-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8f53-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8f53-179">Request</span></span>
<span data-ttu-id="a8f53-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8f53-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="a8f53-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8f53-181">Response</span></span>
<span data-ttu-id="a8f53-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8f53-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




