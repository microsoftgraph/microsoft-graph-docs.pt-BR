---
title: Atualizar deviceEnrollmentPlatformRestrictionsConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentPlatformRestrictionsConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 970462a8f993e8ef01f5c1359e865b625bfec611
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402297"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="1b2e6-103">Atualizar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="1b2e6-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="1b2e6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="1b2e6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1b2e6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1b2e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b2e6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="1b2e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b2e6-107">Atualizar as propriedades de um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b2e6-107">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b2e6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1b2e6-108">Prerequisites</span></span>
<span data-ttu-id="1b2e6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1b2e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1b2e6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b2e6-111">Permission type</span></span>|<span data-ttu-id="1b2e6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1b2e6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b2e6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b2e6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b2e6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b2e6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1b2e6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b2e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b2e6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b2e6-116">Not supported.</span></span>|
|<span data-ttu-id="1b2e6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b2e6-117">Application</span></span>|<span data-ttu-id="1b2e6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b2e6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b2e6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b2e6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1b2e6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b2e6-120">Request headers</span></span>
|<span data-ttu-id="1b2e6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b2e6-121">Header</span></span>|<span data-ttu-id="1b2e6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1b2e6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b2e6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b2e6-123">Authorization</span></span>|<span data-ttu-id="1b2e6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b2e6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b2e6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1b2e6-125">Accept</span></span>|<span data-ttu-id="1b2e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b2e6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b2e6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b2e6-127">Request body</span></span>
<span data-ttu-id="1b2e6-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b2e6-128">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="1b2e6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b2e6-129">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="1b2e6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b2e6-130">Property</span></span>|<span data-ttu-id="1b2e6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b2e6-131">Type</span></span>|<span data-ttu-id="1b2e6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b2e6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b2e6-133">id</span><span class="sxs-lookup"><span data-stu-id="1b2e6-133">id</span></span>|<span data-ttu-id="1b2e6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b2e6-134">String</span></span>|<span data-ttu-id="1b2e6-135">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b2e6-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b2e6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1b2e6-136">displayName</span></span>|<span data-ttu-id="1b2e6-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b2e6-137">String</span></span>|<span data-ttu-id="1b2e6-138">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b2e6-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b2e6-139">description</span><span class="sxs-lookup"><span data-stu-id="1b2e6-139">description</span></span>|<span data-ttu-id="1b2e6-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b2e6-140">String</span></span>|<span data-ttu-id="1b2e6-141">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b2e6-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b2e6-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="1b2e6-142">priority</span></span>|<span data-ttu-id="1b2e6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1b2e6-143">Int32</span></span>|<span data-ttu-id="1b2e6-144">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b2e6-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b2e6-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b2e6-145">createdDateTime</span></span>|<span data-ttu-id="1b2e6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b2e6-146">DateTimeOffset</span></span>|<span data-ttu-id="1b2e6-147">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b2e6-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b2e6-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b2e6-148">lastModifiedDateTime</span></span>|<span data-ttu-id="1b2e6-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b2e6-149">DateTimeOffset</span></span>|<span data-ttu-id="1b2e6-150">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b2e6-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b2e6-151">version</span><span class="sxs-lookup"><span data-stu-id="1b2e6-151">version</span></span>|<span data-ttu-id="1b2e6-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1b2e6-152">Int32</span></span>|<span data-ttu-id="1b2e6-153">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b2e6-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b2e6-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="1b2e6-154">iosRestriction</span></span>|[<span data-ttu-id="1b2e6-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1b2e6-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1b2e6-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1b2e6-156">Not yet documented</span></span>|
|<span data-ttu-id="1b2e6-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="1b2e6-157">windowsRestriction</span></span>|[<span data-ttu-id="1b2e6-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1b2e6-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1b2e6-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1b2e6-159">Not yet documented</span></span>|
|<span data-ttu-id="1b2e6-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="1b2e6-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="1b2e6-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1b2e6-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1b2e6-162">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1b2e6-162">Not yet documented</span></span>|
|<span data-ttu-id="1b2e6-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="1b2e6-163">androidRestriction</span></span>|[<span data-ttu-id="1b2e6-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1b2e6-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1b2e6-165">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1b2e6-165">Not yet documented</span></span>|
|<span data-ttu-id="1b2e6-166">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="1b2e6-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="1b2e6-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1b2e6-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1b2e6-168">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1b2e6-168">Not yet documented</span></span>|
|<span data-ttu-id="1b2e6-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="1b2e6-169">macRestriction</span></span>|[<span data-ttu-id="1b2e6-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1b2e6-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1b2e6-171">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1b2e6-171">Not yet documented</span></span>|
|<span data-ttu-id="1b2e6-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="1b2e6-172">macOSRestriction</span></span>|[<span data-ttu-id="1b2e6-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1b2e6-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1b2e6-174">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1b2e6-174">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1b2e6-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b2e6-175">Response</span></span>
<span data-ttu-id="1b2e6-176">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b2e6-176">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b2e6-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b2e6-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b2e6-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b2e6-178">Request</span></span>
<span data-ttu-id="1b2e6-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b2e6-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 2231

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
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macRestriction": {
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

### <a name="response"></a><span data-ttu-id="1b2e6-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b2e6-180">Response</span></span>
<span data-ttu-id="1b2e6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b2e6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2403

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
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macRestriction": {
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




