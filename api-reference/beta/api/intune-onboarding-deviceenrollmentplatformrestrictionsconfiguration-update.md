---
title: Atualizar deviceEnrollmentPlatformRestrictionsConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5d4583a226148a5b54bcb04d860ae7bc6125e92a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000116"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="6fe54-103">Atualizar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="6fe54-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="6fe54-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fe54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fe54-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6fe54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fe54-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6fe54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fe54-107">Atualizar as propriedades de um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6fe54-107">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fe54-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6fe54-108">Prerequisites</span></span>
<span data-ttu-id="6fe54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fe54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fe54-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fe54-111">Permission type</span></span>|<span data-ttu-id="6fe54-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6fe54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fe54-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fe54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6fe54-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fe54-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6fe54-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fe54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fe54-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fe54-116">Not supported.</span></span>|
|<span data-ttu-id="6fe54-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fe54-117">Application</span></span>|<span data-ttu-id="6fe54-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fe54-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fe54-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fe54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6fe54-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fe54-120">Request headers</span></span>
|<span data-ttu-id="6fe54-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6fe54-121">Header</span></span>|<span data-ttu-id="6fe54-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6fe54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fe54-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fe54-123">Authorization</span></span>|<span data-ttu-id="6fe54-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fe54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fe54-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6fe54-125">Accept</span></span>|<span data-ttu-id="6fe54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6fe54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fe54-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fe54-127">Request body</span></span>
<span data-ttu-id="6fe54-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6fe54-128">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="6fe54-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6fe54-129">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="6fe54-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fe54-130">Property</span></span>|<span data-ttu-id="6fe54-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fe54-131">Type</span></span>|<span data-ttu-id="6fe54-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fe54-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fe54-133">id</span><span class="sxs-lookup"><span data-stu-id="6fe54-133">id</span></span>|<span data-ttu-id="6fe54-134">String</span><span class="sxs-lookup"><span data-stu-id="6fe54-134">String</span></span>|<span data-ttu-id="6fe54-135">Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fe54-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6fe54-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6fe54-136">displayName</span></span>|<span data-ttu-id="6fe54-137">String</span><span class="sxs-lookup"><span data-stu-id="6fe54-137">String</span></span>|<span data-ttu-id="6fe54-138">O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fe54-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6fe54-139">description</span><span class="sxs-lookup"><span data-stu-id="6fe54-139">description</span></span>|<span data-ttu-id="6fe54-140">String</span><span class="sxs-lookup"><span data-stu-id="6fe54-140">String</span></span>|<span data-ttu-id="6fe54-141">A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fe54-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6fe54-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="6fe54-142">priority</span></span>|<span data-ttu-id="6fe54-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6fe54-143">Int32</span></span>|<span data-ttu-id="6fe54-144">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="6fe54-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="6fe54-145">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="6fe54-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="6fe54-146">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fe54-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6fe54-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fe54-147">createdDateTime</span></span>|<span data-ttu-id="6fe54-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fe54-148">DateTimeOffset</span></span>|<span data-ttu-id="6fe54-149">Data e hora de criação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fe54-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6fe54-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fe54-150">lastModifiedDateTime</span></span>|<span data-ttu-id="6fe54-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fe54-151">DateTimeOffset</span></span>|<span data-ttu-id="6fe54-152">Data e hora da última modificação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fe54-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6fe54-153">versão</span><span class="sxs-lookup"><span data-stu-id="6fe54-153">version</span></span>|<span data-ttu-id="6fe54-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6fe54-154">Int32</span></span>|<span data-ttu-id="6fe54-155">A versão da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fe54-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6fe54-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6fe54-156">roleScopeTagIds</span></span>|<span data-ttu-id="6fe54-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6fe54-157">String collection</span></span>|<span data-ttu-id="6fe54-158">Marcas de escopo de função opcional para as restrições de registro.</span><span class="sxs-lookup"><span data-stu-id="6fe54-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="6fe54-159">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fe54-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6fe54-160">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="6fe54-160">iosRestriction</span></span>|[<span data-ttu-id="6fe54-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="6fe54-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="6fe54-162">Restrições do IOS com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6fe54-162">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="6fe54-163">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="6fe54-163">windowsRestriction</span></span>|[<span data-ttu-id="6fe54-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="6fe54-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="6fe54-165">Restrições do Windows com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6fe54-165">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="6fe54-166">windowsHomeSkuRestriction</span><span class="sxs-lookup"><span data-stu-id="6fe54-166">windowsHomeSkuRestriction</span></span>|[<span data-ttu-id="6fe54-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="6fe54-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="6fe54-168">Restrições do Windows Home SKU com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6fe54-168">Windows Home Sku restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="6fe54-169">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="6fe54-169">windowsMobileRestriction</span></span>|[<span data-ttu-id="6fe54-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="6fe54-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="6fe54-171">Restrições do Windows Mobile com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6fe54-171">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="6fe54-172">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="6fe54-172">androidRestriction</span></span>|[<span data-ttu-id="6fe54-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="6fe54-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="6fe54-174">Restrições do Android com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6fe54-174">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="6fe54-175">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="6fe54-175">androidForWorkRestriction</span></span>|[<span data-ttu-id="6fe54-176">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="6fe54-176">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="6fe54-177">O Android para restrições de trabalho com base na plataforma, na versão do sistema operacional da plataforma e na Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6fe54-177">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="6fe54-178">macRestriction</span><span class="sxs-lookup"><span data-stu-id="6fe54-178">macRestriction</span></span>|[<span data-ttu-id="6fe54-179">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="6fe54-179">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="6fe54-180">Restrições de Mac com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6fe54-180">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="6fe54-181">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="6fe54-181">macOSRestriction</span></span>|[<span data-ttu-id="6fe54-182">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="6fe54-182">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="6fe54-183">Restrições de Mac com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6fe54-183">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="6fe54-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fe54-184">Response</span></span>
<span data-ttu-id="6fe54-185">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fe54-185">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fe54-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fe54-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fe54-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fe54-187">Request</span></span>
<span data-ttu-id="6fe54-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fe54-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 3197

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "windowsHomeSkuRestriction": {
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

### <a name="response"></a><span data-ttu-id="6fe54-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fe54-189">Response</span></span>
<span data-ttu-id="6fe54-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6fe54-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3369

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "windowsHomeSkuRestriction": {
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






