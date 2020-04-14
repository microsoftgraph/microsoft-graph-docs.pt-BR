---
title: Criar deviceEnrollmentPlatformRestrictionsConfiguration
description: Criar um novo objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 87d2bf92540e15b2f27675580b4a0b2ecafc5365
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450428"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="11125-103">Criar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="11125-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="11125-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11125-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11125-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="11125-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11125-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11125-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11125-107">Criar um novo objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="11125-107">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11125-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="11125-108">Prerequisites</span></span>
<span data-ttu-id="11125-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11125-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11125-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11125-111">Permission type</span></span>|<span data-ttu-id="11125-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="11125-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11125-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11125-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11125-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11125-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="11125-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11125-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11125-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11125-116">Not supported.</span></span>|
|<span data-ttu-id="11125-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11125-117">Application</span></span>|<span data-ttu-id="11125-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11125-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="11125-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11125-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="11125-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11125-120">Request headers</span></span>
|<span data-ttu-id="11125-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11125-121">Header</span></span>|<span data-ttu-id="11125-122">Valor</span><span class="sxs-lookup"><span data-stu-id="11125-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11125-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="11125-123">Authorization</span></span>|<span data-ttu-id="11125-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11125-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11125-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="11125-125">Accept</span></span>|<span data-ttu-id="11125-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11125-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11125-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11125-127">Request body</span></span>
<span data-ttu-id="11125-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="11125-128">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="11125-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="11125-129">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="11125-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11125-130">Property</span></span>|<span data-ttu-id="11125-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="11125-131">Type</span></span>|<span data-ttu-id="11125-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="11125-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11125-133">id</span><span class="sxs-lookup"><span data-stu-id="11125-133">id</span></span>|<span data-ttu-id="11125-134">String</span><span class="sxs-lookup"><span data-stu-id="11125-134">String</span></span>|<span data-ttu-id="11125-135">Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11125-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11125-136">displayName</span><span class="sxs-lookup"><span data-stu-id="11125-136">displayName</span></span>|<span data-ttu-id="11125-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11125-137">String</span></span>|<span data-ttu-id="11125-138">O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11125-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11125-139">description</span><span class="sxs-lookup"><span data-stu-id="11125-139">description</span></span>|<span data-ttu-id="11125-140">String</span><span class="sxs-lookup"><span data-stu-id="11125-140">String</span></span>|<span data-ttu-id="11125-141">A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11125-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11125-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="11125-142">priority</span></span>|<span data-ttu-id="11125-143">Int32</span><span class="sxs-lookup"><span data-stu-id="11125-143">Int32</span></span>|<span data-ttu-id="11125-144">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="11125-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="11125-145">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="11125-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="11125-146">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11125-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11125-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11125-147">createdDateTime</span></span>|<span data-ttu-id="11125-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11125-148">DateTimeOffset</span></span>|<span data-ttu-id="11125-149">Data e hora de criação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11125-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11125-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11125-150">lastModifiedDateTime</span></span>|<span data-ttu-id="11125-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11125-151">DateTimeOffset</span></span>|<span data-ttu-id="11125-152">Data e hora da última modificação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11125-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11125-153">versão</span><span class="sxs-lookup"><span data-stu-id="11125-153">version</span></span>|<span data-ttu-id="11125-154">Int32</span><span class="sxs-lookup"><span data-stu-id="11125-154">Int32</span></span>|<span data-ttu-id="11125-155">A versão da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11125-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11125-156">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="11125-156">iosRestriction</span></span>|[<span data-ttu-id="11125-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11125-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11125-158">Restrições do IOS com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="11125-158">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="11125-159">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="11125-159">windowsRestriction</span></span>|[<span data-ttu-id="11125-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11125-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11125-161">Restrições do Windows com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="11125-161">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="11125-162">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="11125-162">windowsMobileRestriction</span></span>|[<span data-ttu-id="11125-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11125-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11125-164">Restrições do Windows Mobile com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="11125-164">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="11125-165">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="11125-165">androidRestriction</span></span>|[<span data-ttu-id="11125-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11125-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11125-167">Restrições do Android com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="11125-167">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="11125-168">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="11125-168">androidForWorkRestriction</span></span>|[<span data-ttu-id="11125-169">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11125-169">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11125-170">O Android para restrições de trabalho com base na plataforma, na versão do sistema operacional da plataforma e na Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="11125-170">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="11125-171">macRestriction</span><span class="sxs-lookup"><span data-stu-id="11125-171">macRestriction</span></span>|[<span data-ttu-id="11125-172">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11125-172">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11125-173">Restrições de Mac com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="11125-173">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="11125-174">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="11125-174">macOSRestriction</span></span>|[<span data-ttu-id="11125-175">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11125-175">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11125-176">Restrições de Mac com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="11125-176">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="11125-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="11125-177">Response</span></span>
<span data-ttu-id="11125-178">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11125-178">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11125-179">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11125-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="11125-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11125-180">Request</span></span>
<span data-ttu-id="11125-181">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11125-181">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="11125-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="11125-182">Response</span></span>
<span data-ttu-id="11125-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11125-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



