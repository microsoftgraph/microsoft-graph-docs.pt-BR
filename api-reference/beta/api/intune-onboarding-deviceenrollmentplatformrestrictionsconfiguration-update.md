---
title: Atualizar deviceEnrollmentPlatformRestrictionsConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2897815a7324f88d4c10c4e5c940bc2d6b078cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528880"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="46175-103">Atualizar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="46175-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="46175-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="46175-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46175-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46175-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46175-106">Atualizar as propriedades de um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46175-106">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46175-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="46175-107">Prerequisites</span></span>
<span data-ttu-id="46175-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46175-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46175-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46175-110">Permission type</span></span>|<span data-ttu-id="46175-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="46175-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46175-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46175-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46175-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46175-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="46175-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46175-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46175-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46175-115">Not supported.</span></span>|
|<span data-ttu-id="46175-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46175-116">Application</span></span>|<span data-ttu-id="46175-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46175-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46175-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46175-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="46175-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46175-119">Request headers</span></span>
|<span data-ttu-id="46175-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="46175-120">Header</span></span>|<span data-ttu-id="46175-121">Valor</span><span class="sxs-lookup"><span data-stu-id="46175-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46175-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="46175-122">Authorization</span></span>|<span data-ttu-id="46175-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46175-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46175-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="46175-124">Accept</span></span>|<span data-ttu-id="46175-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46175-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46175-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46175-126">Request body</span></span>
<span data-ttu-id="46175-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46175-127">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="46175-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46175-128">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="46175-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46175-129">Property</span></span>|<span data-ttu-id="46175-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="46175-130">Type</span></span>|<span data-ttu-id="46175-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="46175-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46175-132">id</span><span class="sxs-lookup"><span data-stu-id="46175-132">id</span></span>|<span data-ttu-id="46175-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46175-133">String</span></span>|<span data-ttu-id="46175-134">ID da configuração da página de status de registro herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46175-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="46175-135">displayName</span><span class="sxs-lookup"><span data-stu-id="46175-135">displayName</span></span>|<span data-ttu-id="46175-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46175-136">String</span></span>|<span data-ttu-id="46175-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46175-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="46175-138">description</span><span class="sxs-lookup"><span data-stu-id="46175-138">description</span></span>|<span data-ttu-id="46175-139">String</span><span class="sxs-lookup"><span data-stu-id="46175-139">String</span></span>|<span data-ttu-id="46175-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46175-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="46175-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="46175-141">priority</span></span>|<span data-ttu-id="46175-142">Int32</span><span class="sxs-lookup"><span data-stu-id="46175-142">Int32</span></span>|<span data-ttu-id="46175-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46175-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="46175-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="46175-144">createdDateTime</span></span>|<span data-ttu-id="46175-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46175-145">DateTimeOffset</span></span>|<span data-ttu-id="46175-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46175-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="46175-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="46175-147">lastModifiedDateTime</span></span>|<span data-ttu-id="46175-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46175-148">DateTimeOffset</span></span>|<span data-ttu-id="46175-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46175-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="46175-150">versão</span><span class="sxs-lookup"><span data-stu-id="46175-150">version</span></span>|<span data-ttu-id="46175-151">Int32</span><span class="sxs-lookup"><span data-stu-id="46175-151">Int32</span></span>|<span data-ttu-id="46175-152">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46175-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="46175-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="46175-153">iosRestriction</span></span>|[<span data-ttu-id="46175-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="46175-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="46175-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="46175-155">Not yet documented</span></span>|
|<span data-ttu-id="46175-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="46175-156">windowsRestriction</span></span>|[<span data-ttu-id="46175-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="46175-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="46175-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="46175-158">Not yet documented</span></span>|
|<span data-ttu-id="46175-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="46175-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="46175-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="46175-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="46175-161">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="46175-161">Not yet documented</span></span>|
|<span data-ttu-id="46175-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="46175-162">androidRestriction</span></span>|[<span data-ttu-id="46175-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="46175-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="46175-164">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="46175-164">Not yet documented</span></span>|
|<span data-ttu-id="46175-165">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="46175-165">androidForWorkRestriction</span></span>|[<span data-ttu-id="46175-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="46175-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="46175-167">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="46175-167">Not yet documented</span></span>|
|<span data-ttu-id="46175-168">macRestriction</span><span class="sxs-lookup"><span data-stu-id="46175-168">macRestriction</span></span>|[<span data-ttu-id="46175-169">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="46175-169">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="46175-170">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="46175-170">Not yet documented</span></span>|
|<span data-ttu-id="46175-171">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="46175-171">macOSRestriction</span></span>|[<span data-ttu-id="46175-172">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="46175-172">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="46175-173">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="46175-173">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="46175-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="46175-174">Response</span></span>
<span data-ttu-id="46175-175">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46175-175">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46175-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46175-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="46175-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46175-177">Request</span></span>
<span data-ttu-id="46175-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46175-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="46175-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="46175-179">Response</span></span>
<span data-ttu-id="46175-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46175-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





