---
title: Atualizar deviceEnrollmentPlatformRestrictionsConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 49f0ac5ef242e1ad2f7332fab5d2bbe147313756
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49274829"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="97c41-103">Atualizar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="97c41-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="97c41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97c41-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97c41-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="97c41-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97c41-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97c41-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97c41-107">Atualizar as propriedades de um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97c41-107">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97c41-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97c41-108">Prerequisites</span></span>
<span data-ttu-id="97c41-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97c41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97c41-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97c41-111">Permission type</span></span>|<span data-ttu-id="97c41-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97c41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97c41-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97c41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97c41-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97c41-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="97c41-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97c41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97c41-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97c41-116">Not supported.</span></span>|
|<span data-ttu-id="97c41-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97c41-117">Application</span></span>|<span data-ttu-id="97c41-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97c41-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97c41-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97c41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="97c41-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97c41-120">Request headers</span></span>
|<span data-ttu-id="97c41-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97c41-121">Header</span></span>|<span data-ttu-id="97c41-122">Valor</span><span class="sxs-lookup"><span data-stu-id="97c41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97c41-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="97c41-123">Authorization</span></span>|<span data-ttu-id="97c41-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97c41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97c41-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97c41-125">Accept</span></span>|<span data-ttu-id="97c41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97c41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97c41-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97c41-127">Request body</span></span>
<span data-ttu-id="97c41-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97c41-128">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="97c41-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97c41-129">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="97c41-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97c41-130">Property</span></span>|<span data-ttu-id="97c41-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="97c41-131">Type</span></span>|<span data-ttu-id="97c41-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="97c41-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97c41-133">id</span><span class="sxs-lookup"><span data-stu-id="97c41-133">id</span></span>|<span data-ttu-id="97c41-134">String</span><span class="sxs-lookup"><span data-stu-id="97c41-134">String</span></span>|<span data-ttu-id="97c41-135">Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97c41-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="97c41-136">displayName</span><span class="sxs-lookup"><span data-stu-id="97c41-136">displayName</span></span>|<span data-ttu-id="97c41-137">String</span><span class="sxs-lookup"><span data-stu-id="97c41-137">String</span></span>|<span data-ttu-id="97c41-138">O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97c41-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="97c41-139">description</span><span class="sxs-lookup"><span data-stu-id="97c41-139">description</span></span>|<span data-ttu-id="97c41-140">String</span><span class="sxs-lookup"><span data-stu-id="97c41-140">String</span></span>|<span data-ttu-id="97c41-141">A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97c41-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="97c41-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="97c41-142">priority</span></span>|<span data-ttu-id="97c41-143">Int32</span><span class="sxs-lookup"><span data-stu-id="97c41-143">Int32</span></span>|<span data-ttu-id="97c41-144">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="97c41-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="97c41-145">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="97c41-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="97c41-146">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97c41-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="97c41-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97c41-147">createdDateTime</span></span>|<span data-ttu-id="97c41-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97c41-148">DateTimeOffset</span></span>|<span data-ttu-id="97c41-149">Data e hora de criação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97c41-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="97c41-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97c41-150">lastModifiedDateTime</span></span>|<span data-ttu-id="97c41-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97c41-151">DateTimeOffset</span></span>|<span data-ttu-id="97c41-152">Data e hora da última modificação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97c41-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="97c41-153">versão</span><span class="sxs-lookup"><span data-stu-id="97c41-153">version</span></span>|<span data-ttu-id="97c41-154">Int32</span><span class="sxs-lookup"><span data-stu-id="97c41-154">Int32</span></span>|<span data-ttu-id="97c41-155">A versão da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97c41-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="97c41-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="97c41-156">roleScopeTagIds</span></span>|<span data-ttu-id="97c41-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="97c41-157">String collection</span></span>|<span data-ttu-id="97c41-158">Marcas de escopo de função opcional para as restrições de registro.</span><span class="sxs-lookup"><span data-stu-id="97c41-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="97c41-159">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97c41-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="97c41-160">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-160">iosRestriction</span></span>|[<span data-ttu-id="97c41-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="97c41-162">Restrições do IOS com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="97c41-162">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="97c41-163">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-163">windowsRestriction</span></span>|[<span data-ttu-id="97c41-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="97c41-165">Restrições do Windows com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="97c41-165">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="97c41-166">windowsHomeSkuRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-166">windowsHomeSkuRestriction</span></span>|[<span data-ttu-id="97c41-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="97c41-168">Restrições do Windows Home SKU com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="97c41-168">Windows Home Sku restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="97c41-169">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-169">windowsMobileRestriction</span></span>|[<span data-ttu-id="97c41-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="97c41-171">Restrições do Windows Mobile com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="97c41-171">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="97c41-172">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-172">androidRestriction</span></span>|[<span data-ttu-id="97c41-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="97c41-174">Restrições do Android com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="97c41-174">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="97c41-175">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-175">androidForWorkRestriction</span></span>|[<span data-ttu-id="97c41-176">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-176">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="97c41-177">O Android para restrições de trabalho com base na plataforma, na versão do sistema operacional da plataforma e na Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="97c41-177">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="97c41-178">aospRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-178">aospRestriction</span></span>|[<span data-ttu-id="97c41-179">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-179">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="97c41-180">Restrições de AOSP com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="97c41-180">AOSP restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="97c41-181">macRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-181">macRestriction</span></span>|[<span data-ttu-id="97c41-182">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-182">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="97c41-183">Restrições de Mac com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="97c41-183">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="97c41-184">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-184">macOSRestriction</span></span>|[<span data-ttu-id="97c41-185">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="97c41-185">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="97c41-186">Restrições de Mac com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="97c41-186">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="97c41-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="97c41-187">Response</span></span>
<span data-ttu-id="97c41-188">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97c41-188">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97c41-189">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97c41-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="97c41-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97c41-190">Request</span></span>
<span data-ttu-id="97c41-191">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97c41-191">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 4081

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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "aospRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="97c41-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="97c41-192">Response</span></span>
<span data-ttu-id="97c41-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97c41-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4253

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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "aospRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  }
}
```




