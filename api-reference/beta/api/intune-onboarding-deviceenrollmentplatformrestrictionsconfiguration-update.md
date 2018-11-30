---
title: Atualizar deviceEnrollmentPlatformRestrictionsConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentPlatformRestrictionsConfiguration.
ms.openlocfilehash: 840f67c25eb0e0cc34e951be12a1dd5cddca17c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039680"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="736dc-103">Atualizar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="736dc-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="736dc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="736dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="736dc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="736dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="736dc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="736dc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="736dc-107">Atualizar as propriedades de um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="736dc-107">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="736dc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="736dc-108">Prerequisites</span></span>
<span data-ttu-id="736dc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="736dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="736dc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="736dc-111">Permission type</span></span>|<span data-ttu-id="736dc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="736dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="736dc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="736dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="736dc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="736dc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="736dc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="736dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="736dc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="736dc-116">Not supported.</span></span>|
|<span data-ttu-id="736dc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="736dc-117">Application</span></span>|<span data-ttu-id="736dc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="736dc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="736dc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="736dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="736dc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="736dc-120">Request headers</span></span>
|<span data-ttu-id="736dc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="736dc-121">Header</span></span>|<span data-ttu-id="736dc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="736dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="736dc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="736dc-123">Authorization</span></span>|<span data-ttu-id="736dc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="736dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="736dc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="736dc-125">Accept</span></span>|<span data-ttu-id="736dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="736dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="736dc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="736dc-127">Request body</span></span>
<span data-ttu-id="736dc-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="736dc-128">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="736dc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="736dc-129">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="736dc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="736dc-130">Property</span></span>|<span data-ttu-id="736dc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="736dc-131">Type</span></span>|<span data-ttu-id="736dc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="736dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="736dc-133">id</span><span class="sxs-lookup"><span data-stu-id="736dc-133">id</span></span>|<span data-ttu-id="736dc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="736dc-134">String</span></span>|<span data-ttu-id="736dc-135">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="736dc-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="736dc-136">displayName</span><span class="sxs-lookup"><span data-stu-id="736dc-136">displayName</span></span>|<span data-ttu-id="736dc-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="736dc-137">String</span></span>|<span data-ttu-id="736dc-138">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="736dc-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="736dc-139">description</span><span class="sxs-lookup"><span data-stu-id="736dc-139">description</span></span>|<span data-ttu-id="736dc-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="736dc-140">String</span></span>|<span data-ttu-id="736dc-141">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="736dc-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="736dc-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="736dc-142">priority</span></span>|<span data-ttu-id="736dc-143">Int32</span><span class="sxs-lookup"><span data-stu-id="736dc-143">Int32</span></span>|<span data-ttu-id="736dc-144">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="736dc-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="736dc-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="736dc-145">createdDateTime</span></span>|<span data-ttu-id="736dc-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="736dc-146">DateTimeOffset</span></span>|<span data-ttu-id="736dc-147">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="736dc-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="736dc-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="736dc-148">lastModifiedDateTime</span></span>|<span data-ttu-id="736dc-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="736dc-149">DateTimeOffset</span></span>|<span data-ttu-id="736dc-150">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="736dc-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="736dc-151">version</span><span class="sxs-lookup"><span data-stu-id="736dc-151">version</span></span>|<span data-ttu-id="736dc-152">Int32</span><span class="sxs-lookup"><span data-stu-id="736dc-152">Int32</span></span>|<span data-ttu-id="736dc-153">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="736dc-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="736dc-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="736dc-154">iosRestriction</span></span>|[<span data-ttu-id="736dc-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="736dc-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="736dc-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="736dc-156">Not yet documented</span></span>|
|<span data-ttu-id="736dc-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="736dc-157">windowsRestriction</span></span>|[<span data-ttu-id="736dc-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="736dc-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="736dc-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="736dc-159">Not yet documented</span></span>|
|<span data-ttu-id="736dc-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="736dc-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="736dc-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="736dc-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="736dc-162">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="736dc-162">Not yet documented</span></span>|
|<span data-ttu-id="736dc-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="736dc-163">androidRestriction</span></span>|[<span data-ttu-id="736dc-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="736dc-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="736dc-165">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="736dc-165">Not yet documented</span></span>|
|<span data-ttu-id="736dc-166">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="736dc-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="736dc-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="736dc-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="736dc-168">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="736dc-168">Not yet documented</span></span>|
|<span data-ttu-id="736dc-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="736dc-169">macRestriction</span></span>|[<span data-ttu-id="736dc-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="736dc-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="736dc-171">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="736dc-171">Not yet documented</span></span>|
|<span data-ttu-id="736dc-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="736dc-172">macOSRestriction</span></span>|[<span data-ttu-id="736dc-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="736dc-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="736dc-174">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="736dc-174">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="736dc-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="736dc-175">Response</span></span>
<span data-ttu-id="736dc-176">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="736dc-176">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="736dc-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="736dc-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="736dc-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="736dc-178">Request</span></span>
<span data-ttu-id="736dc-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="736dc-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 2207

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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

### <a name="response"></a><span data-ttu-id="736dc-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="736dc-180">Response</span></span>
<span data-ttu-id="736dc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="736dc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





