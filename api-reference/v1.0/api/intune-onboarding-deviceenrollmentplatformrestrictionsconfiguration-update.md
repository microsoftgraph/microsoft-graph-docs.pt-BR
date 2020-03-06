---
title: Atualizar deviceEnrollmentPlatformRestrictionsConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7428db6ab3bb032b8751b1a2343480d1d43ba418
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512619"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="10f4a-103">Atualizar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="10f4a-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="10f4a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10f4a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10f4a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10f4a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10f4a-106">Atualizar as propriedades de um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10f4a-106">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10f4a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="10f4a-107">Prerequisites</span></span>
<span data-ttu-id="10f4a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10f4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10f4a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10f4a-110">Permission type</span></span>|<span data-ttu-id="10f4a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="10f4a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10f4a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10f4a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10f4a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10f4a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="10f4a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10f4a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10f4a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10f4a-115">Not supported.</span></span>|
|<span data-ttu-id="10f4a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10f4a-116">Application</span></span>|<span data-ttu-id="10f4a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10f4a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10f4a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10f4a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="10f4a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10f4a-119">Request headers</span></span>
|<span data-ttu-id="10f4a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="10f4a-120">Header</span></span>|<span data-ttu-id="10f4a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="10f4a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10f4a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="10f4a-122">Authorization</span></span>|<span data-ttu-id="10f4a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10f4a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10f4a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="10f4a-124">Accept</span></span>|<span data-ttu-id="10f4a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10f4a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10f4a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10f4a-126">Request body</span></span>
<span data-ttu-id="10f4a-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10f4a-127">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="10f4a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10f4a-128">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="10f4a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10f4a-129">Property</span></span>|<span data-ttu-id="10f4a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="10f4a-130">Type</span></span>|<span data-ttu-id="10f4a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="10f4a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10f4a-132">id</span><span class="sxs-lookup"><span data-stu-id="10f4a-132">id</span></span>|<span data-ttu-id="10f4a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10f4a-133">String</span></span>|<span data-ttu-id="10f4a-134">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10f4a-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="10f4a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="10f4a-135">displayName</span></span>|<span data-ttu-id="10f4a-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10f4a-136">String</span></span>|<span data-ttu-id="10f4a-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10f4a-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="10f4a-138">description</span><span class="sxs-lookup"><span data-stu-id="10f4a-138">description</span></span>|<span data-ttu-id="10f4a-139">String</span><span class="sxs-lookup"><span data-stu-id="10f4a-139">String</span></span>|<span data-ttu-id="10f4a-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10f4a-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="10f4a-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="10f4a-141">priority</span></span>|<span data-ttu-id="10f4a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="10f4a-142">Int32</span></span>|<span data-ttu-id="10f4a-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10f4a-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="10f4a-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10f4a-144">createdDateTime</span></span>|<span data-ttu-id="10f4a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10f4a-145">DateTimeOffset</span></span>|<span data-ttu-id="10f4a-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10f4a-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="10f4a-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10f4a-147">lastModifiedDateTime</span></span>|<span data-ttu-id="10f4a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10f4a-148">DateTimeOffset</span></span>|<span data-ttu-id="10f4a-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10f4a-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="10f4a-150">versão</span><span class="sxs-lookup"><span data-stu-id="10f4a-150">version</span></span>|<span data-ttu-id="10f4a-151">Int32</span><span class="sxs-lookup"><span data-stu-id="10f4a-151">Int32</span></span>|<span data-ttu-id="10f4a-152">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10f4a-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="10f4a-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="10f4a-153">iosRestriction</span></span>|[<span data-ttu-id="10f4a-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="10f4a-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="10f4a-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="10f4a-155">Not yet documented</span></span>|
|<span data-ttu-id="10f4a-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="10f4a-156">windowsRestriction</span></span>|[<span data-ttu-id="10f4a-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="10f4a-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="10f4a-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="10f4a-158">Not yet documented</span></span>|
|<span data-ttu-id="10f4a-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="10f4a-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="10f4a-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="10f4a-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="10f4a-161">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="10f4a-161">Not yet documented</span></span>|
|<span data-ttu-id="10f4a-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="10f4a-162">androidRestriction</span></span>|[<span data-ttu-id="10f4a-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="10f4a-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="10f4a-164">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="10f4a-164">Not yet documented</span></span>|
|<span data-ttu-id="10f4a-165">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="10f4a-165">macOSRestriction</span></span>|[<span data-ttu-id="10f4a-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="10f4a-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="10f4a-167">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="10f4a-167">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="10f4a-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="10f4a-168">Response</span></span>
<span data-ttu-id="10f4a-169">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10f4a-169">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10f4a-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10f4a-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="10f4a-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10f4a-171">Request</span></span>
<span data-ttu-id="10f4a-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10f4a-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="10f4a-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="10f4a-173">Response</span></span>
<span data-ttu-id="10f4a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10f4a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




