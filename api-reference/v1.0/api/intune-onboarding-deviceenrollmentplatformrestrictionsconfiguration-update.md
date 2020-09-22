---
title: Atualizar deviceEnrollmentPlatformRestrictionsConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8911bb53465ceaf8cf1ba344c3f8e6433ae09835
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087275"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="f84b6-103">Atualizar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="f84b6-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="f84b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f84b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f84b6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f84b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f84b6-106">Atualizar as propriedades de um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f84b6-106">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f84b6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f84b6-107">Prerequisites</span></span>
<span data-ttu-id="f84b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f84b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f84b6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f84b6-110">Permission type</span></span>|<span data-ttu-id="f84b6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f84b6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f84b6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f84b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f84b6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f84b6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f84b6-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f84b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f84b6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f84b6-115">Not supported.</span></span>|
|<span data-ttu-id="f84b6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f84b6-116">Application</span></span>|<span data-ttu-id="f84b6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f84b6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f84b6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f84b6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f84b6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f84b6-119">Request headers</span></span>
|<span data-ttu-id="f84b6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f84b6-120">Header</span></span>|<span data-ttu-id="f84b6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f84b6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f84b6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f84b6-122">Authorization</span></span>|<span data-ttu-id="f84b6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f84b6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f84b6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f84b6-124">Accept</span></span>|<span data-ttu-id="f84b6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f84b6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f84b6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f84b6-126">Request body</span></span>
<span data-ttu-id="f84b6-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f84b6-127">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="f84b6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f84b6-128">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="f84b6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f84b6-129">Property</span></span>|<span data-ttu-id="f84b6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f84b6-130">Type</span></span>|<span data-ttu-id="f84b6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f84b6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f84b6-132">id</span><span class="sxs-lookup"><span data-stu-id="f84b6-132">id</span></span>|<span data-ttu-id="f84b6-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f84b6-133">String</span></span>|<span data-ttu-id="f84b6-134">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f84b6-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f84b6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f84b6-135">displayName</span></span>|<span data-ttu-id="f84b6-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f84b6-136">String</span></span>|<span data-ttu-id="f84b6-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f84b6-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f84b6-138">description</span><span class="sxs-lookup"><span data-stu-id="f84b6-138">description</span></span>|<span data-ttu-id="f84b6-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f84b6-139">String</span></span>|<span data-ttu-id="f84b6-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f84b6-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f84b6-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="f84b6-141">priority</span></span>|<span data-ttu-id="f84b6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f84b6-142">Int32</span></span>|<span data-ttu-id="f84b6-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f84b6-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f84b6-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f84b6-144">createdDateTime</span></span>|<span data-ttu-id="f84b6-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f84b6-145">DateTimeOffset</span></span>|<span data-ttu-id="f84b6-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f84b6-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f84b6-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f84b6-147">lastModifiedDateTime</span></span>|<span data-ttu-id="f84b6-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f84b6-148">DateTimeOffset</span></span>|<span data-ttu-id="f84b6-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f84b6-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f84b6-150">versão</span><span class="sxs-lookup"><span data-stu-id="f84b6-150">version</span></span>|<span data-ttu-id="f84b6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f84b6-151">Int32</span></span>|<span data-ttu-id="f84b6-152">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f84b6-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f84b6-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="f84b6-153">iosRestriction</span></span>|[<span data-ttu-id="f84b6-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="f84b6-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="f84b6-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f84b6-155">Not yet documented</span></span>|
|<span data-ttu-id="f84b6-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="f84b6-156">windowsRestriction</span></span>|[<span data-ttu-id="f84b6-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="f84b6-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="f84b6-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f84b6-158">Not yet documented</span></span>|
|<span data-ttu-id="f84b6-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="f84b6-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="f84b6-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="f84b6-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="f84b6-161">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f84b6-161">Not yet documented</span></span>|
|<span data-ttu-id="f84b6-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="f84b6-162">androidRestriction</span></span>|[<span data-ttu-id="f84b6-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="f84b6-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="f84b6-164">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f84b6-164">Not yet documented</span></span>|
|<span data-ttu-id="f84b6-165">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="f84b6-165">macOSRestriction</span></span>|[<span data-ttu-id="f84b6-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="f84b6-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="f84b6-167">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f84b6-167">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f84b6-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="f84b6-168">Response</span></span>
<span data-ttu-id="f84b6-169">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f84b6-169">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f84b6-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f84b6-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="f84b6-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f84b6-171">Request</span></span>
<span data-ttu-id="f84b6-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f84b6-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="f84b6-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="f84b6-173">Response</span></span>
<span data-ttu-id="f84b6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f84b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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









