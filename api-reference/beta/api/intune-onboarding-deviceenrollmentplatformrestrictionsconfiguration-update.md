---
title: Atualizar deviceEnrollmentPlatformRestrictionsConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: de385a33863c746ba2f3cbc30ef7093dcca8190e
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44174486"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="1e540-103">Atualizar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="1e540-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="1e540-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e540-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e540-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e540-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e540-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e540-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e540-107">Atualizar as propriedades de um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e540-107">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e540-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e540-108">Prerequisites</span></span>
<span data-ttu-id="1e540-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e540-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e540-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e540-111">Permission type</span></span>|<span data-ttu-id="1e540-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e540-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e540-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e540-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e540-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e540-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1e540-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e540-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e540-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e540-116">Not supported.</span></span>|
|<span data-ttu-id="1e540-117">Application</span><span class="sxs-lookup"><span data-stu-id="1e540-117">Application</span></span>|<span data-ttu-id="1e540-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e540-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e540-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e540-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1e540-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e540-120">Request headers</span></span>
|<span data-ttu-id="1e540-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e540-121">Header</span></span>|<span data-ttu-id="1e540-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1e540-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e540-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e540-123">Authorization</span></span>|<span data-ttu-id="1e540-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e540-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e540-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e540-125">Accept</span></span>|<span data-ttu-id="1e540-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e540-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e540-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e540-127">Request body</span></span>
<span data-ttu-id="1e540-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e540-128">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="1e540-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e540-129">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="1e540-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e540-130">Property</span></span>|<span data-ttu-id="1e540-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e540-131">Type</span></span>|<span data-ttu-id="1e540-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e540-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e540-133">id</span><span class="sxs-lookup"><span data-stu-id="1e540-133">id</span></span>|<span data-ttu-id="1e540-134">String</span><span class="sxs-lookup"><span data-stu-id="1e540-134">String</span></span>|<span data-ttu-id="1e540-135">Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e540-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1e540-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1e540-136">displayName</span></span>|<span data-ttu-id="1e540-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e540-137">String</span></span>|<span data-ttu-id="1e540-138">O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e540-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1e540-139">description</span><span class="sxs-lookup"><span data-stu-id="1e540-139">description</span></span>|<span data-ttu-id="1e540-140">String</span><span class="sxs-lookup"><span data-stu-id="1e540-140">String</span></span>|<span data-ttu-id="1e540-141">A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e540-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1e540-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="1e540-142">priority</span></span>|<span data-ttu-id="1e540-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1e540-143">Int32</span></span>|<span data-ttu-id="1e540-144">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="1e540-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="1e540-145">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="1e540-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="1e540-146">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e540-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1e540-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e540-147">createdDateTime</span></span>|<span data-ttu-id="1e540-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e540-148">DateTimeOffset</span></span>|<span data-ttu-id="1e540-149">Data e hora de criação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e540-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1e540-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e540-150">lastModifiedDateTime</span></span>|<span data-ttu-id="1e540-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e540-151">DateTimeOffset</span></span>|<span data-ttu-id="1e540-152">Data e hora da última modificação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e540-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1e540-153">versão</span><span class="sxs-lookup"><span data-stu-id="1e540-153">version</span></span>|<span data-ttu-id="1e540-154">Int32</span><span class="sxs-lookup"><span data-stu-id="1e540-154">Int32</span></span>|<span data-ttu-id="1e540-155">A versão da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e540-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1e540-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1e540-156">roleScopeTagIds</span></span>|<span data-ttu-id="1e540-157">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e540-157">String collection</span></span>|<span data-ttu-id="1e540-158">Marcas de escopo de função opcional para as restrições de registro.</span><span class="sxs-lookup"><span data-stu-id="1e540-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="1e540-159">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e540-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1e540-160">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="1e540-160">iosRestriction</span></span>|[<span data-ttu-id="1e540-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1e540-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1e540-162">Restrições do IOS com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1e540-162">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="1e540-163">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="1e540-163">windowsRestriction</span></span>|[<span data-ttu-id="1e540-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1e540-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1e540-165">Restrições do Windows com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1e540-165">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="1e540-166">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="1e540-166">windowsMobileRestriction</span></span>|[<span data-ttu-id="1e540-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1e540-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1e540-168">Restrições do Windows Mobile com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1e540-168">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="1e540-169">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="1e540-169">androidRestriction</span></span>|[<span data-ttu-id="1e540-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1e540-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1e540-171">Restrições do Android com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1e540-171">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="1e540-172">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="1e540-172">androidForWorkRestriction</span></span>|[<span data-ttu-id="1e540-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1e540-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1e540-174">O Android para restrições de trabalho com base na plataforma, na versão do sistema operacional da plataforma e na Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1e540-174">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="1e540-175">macRestriction</span><span class="sxs-lookup"><span data-stu-id="1e540-175">macRestriction</span></span>|[<span data-ttu-id="1e540-176">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1e540-176">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1e540-177">Restrições de Mac com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1e540-177">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="1e540-178">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="1e540-178">macOSRestriction</span></span>|[<span data-ttu-id="1e540-179">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1e540-179">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1e540-180">Restrições de Mac com base na plataforma, versão do sistema operacional da plataforma e Propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1e540-180">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="1e540-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e540-181">Response</span></span>
<span data-ttu-id="1e540-182">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e540-182">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e540-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e540-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e540-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e540-184">Request</span></span>
<span data-ttu-id="1e540-185">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e540-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 2825

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

### <a name="response"></a><span data-ttu-id="1e540-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e540-186">Response</span></span>
<span data-ttu-id="1e540-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e540-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2997

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



