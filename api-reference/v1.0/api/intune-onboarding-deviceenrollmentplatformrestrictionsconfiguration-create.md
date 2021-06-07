---
title: Criar deviceEnrollmentPlatformRestrictionsConfiguration
description: Criar um novo objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cbf7119a6e9819ce392241ae163992c83daec0be
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52744810"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="79126-103">Criar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="79126-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="79126-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79126-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79126-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79126-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79126-106">Criar um novo objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79126-106">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79126-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79126-107">Prerequisites</span></span>
<span data-ttu-id="79126-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79126-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79126-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79126-110">Permission type</span></span>|<span data-ttu-id="79126-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79126-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79126-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79126-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79126-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79126-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="79126-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79126-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79126-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79126-115">Not supported.</span></span>|
|<span data-ttu-id="79126-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79126-116">Application</span></span>|<span data-ttu-id="79126-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79126-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79126-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79126-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="79126-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79126-119">Request headers</span></span>
|<span data-ttu-id="79126-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79126-120">Header</span></span>|<span data-ttu-id="79126-121">Valor</span><span class="sxs-lookup"><span data-stu-id="79126-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79126-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="79126-122">Authorization</span></span>|<span data-ttu-id="79126-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79126-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79126-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79126-124">Accept</span></span>|<span data-ttu-id="79126-125">application/json</span><span class="sxs-lookup"><span data-stu-id="79126-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79126-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79126-126">Request body</span></span>
<span data-ttu-id="79126-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="79126-127">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="79126-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="79126-128">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="79126-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79126-129">Property</span></span>|<span data-ttu-id="79126-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="79126-130">Type</span></span>|<span data-ttu-id="79126-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="79126-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79126-132">id</span><span class="sxs-lookup"><span data-stu-id="79126-132">id</span></span>|<span data-ttu-id="79126-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79126-133">String</span></span>|<span data-ttu-id="79126-134">Identificador exclusivo da conta Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79126-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="79126-135">displayName</span><span class="sxs-lookup"><span data-stu-id="79126-135">displayName</span></span>|<span data-ttu-id="79126-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79126-136">String</span></span>|<span data-ttu-id="79126-137">O nome de exibição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79126-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="79126-138">descrição</span><span class="sxs-lookup"><span data-stu-id="79126-138">description</span></span>|<span data-ttu-id="79126-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79126-139">String</span></span>|<span data-ttu-id="79126-140">A descrição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79126-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="79126-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="79126-141">priority</span></span>|<span data-ttu-id="79126-142">Int32</span><span class="sxs-lookup"><span data-stu-id="79126-142">Int32</span></span>|<span data-ttu-id="79126-143">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="79126-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="79126-144">Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixo.</span><span class="sxs-lookup"><span data-stu-id="79126-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="79126-145">Herdada do [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79126-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="79126-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79126-146">createdDateTime</span></span>|<span data-ttu-id="79126-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79126-147">DateTimeOffset</span></span>|<span data-ttu-id="79126-148">Hora de data criada em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79126-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="79126-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79126-149">lastModifiedDateTime</span></span>|<span data-ttu-id="79126-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79126-150">DateTimeOffset</span></span>|<span data-ttu-id="79126-151">Última data de modificação no UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79126-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="79126-152">versão</span><span class="sxs-lookup"><span data-stu-id="79126-152">version</span></span>|<span data-ttu-id="79126-153">Int32</span><span class="sxs-lookup"><span data-stu-id="79126-153">Int32</span></span>|<span data-ttu-id="79126-154">A versão da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79126-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="79126-155">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="79126-155">iosRestriction</span></span>|[<span data-ttu-id="79126-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="79126-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="79126-157">Restrições de Ios com base na plataforma, versão do sistema operacional da plataforma e propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="79126-157">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="79126-158">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="79126-158">windowsRestriction</span></span>|[<span data-ttu-id="79126-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="79126-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="79126-160">Windows restrições baseadas na plataforma, na versão do sistema operacional da plataforma e na propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="79126-160">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="79126-161">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="79126-161">windowsMobileRestriction</span></span>|[<span data-ttu-id="79126-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="79126-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="79126-163">Windows restrições móveis com base na plataforma, na versão do sistema operacional da plataforma e na propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="79126-163">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="79126-164">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="79126-164">androidRestriction</span></span>|[<span data-ttu-id="79126-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="79126-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="79126-166">Restrições do Android com base na plataforma, na versão do sistema operacional da plataforma e na propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="79126-166">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="79126-167">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="79126-167">macOSRestriction</span></span>|[<span data-ttu-id="79126-168">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="79126-168">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="79126-169">Restrições do Mac com base na plataforma, na versão do sistema operacional da plataforma e na propriedade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="79126-169">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="79126-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="79126-170">Response</span></span>
<span data-ttu-id="79126-171">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79126-171">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79126-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79126-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="79126-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79126-173">Request</span></span>
<span data-ttu-id="79126-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79126-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 1650

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
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="79126-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="79126-175">Response</span></span>
<span data-ttu-id="79126-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79126-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1822

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
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```




