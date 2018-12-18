---
title: Atualizar deviceEnrollmentPlatformRestrictionsConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
ms.openlocfilehash: dc7ac904df5ae18b0476cfeeb2d1c98a6533a7c3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308201"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="8fe4f-103">Atualizar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="8fe4f-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="8fe4f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8fe4f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fe4f-105">Atualizar as propriedades de um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8fe4f-105">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8fe4f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8fe4f-106">Prerequisites</span></span>
<span data-ttu-id="8fe4f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fe4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fe4f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8fe4f-109">Permission type</span></span>|<span data-ttu-id="8fe4f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8fe4f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fe4f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8fe4f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8fe4f-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fe4f-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8fe4f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8fe4f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fe4f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fe4f-114">Not supported.</span></span>|
|<span data-ttu-id="8fe4f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8fe4f-115">Application</span></span>|<span data-ttu-id="8fe4f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fe4f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fe4f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fe4f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8fe4f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8fe4f-118">Request headers</span></span>
|<span data-ttu-id="8fe4f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8fe4f-119">Header</span></span>|<span data-ttu-id="8fe4f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8fe4f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fe4f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8fe4f-121">Authorization</span></span>|<span data-ttu-id="8fe4f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8fe4f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fe4f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8fe4f-123">Accept</span></span>|<span data-ttu-id="8fe4f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8fe4f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fe4f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8fe4f-125">Request body</span></span>
<span data-ttu-id="8fe4f-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8fe4f-126">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="8fe4f-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8fe4f-127">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="8fe4f-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8fe4f-128">Property</span></span>|<span data-ttu-id="8fe4f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8fe4f-129">Type</span></span>|<span data-ttu-id="8fe4f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fe4f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fe4f-131">id</span><span class="sxs-lookup"><span data-stu-id="8fe4f-131">id</span></span>|<span data-ttu-id="8fe4f-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8fe4f-132">String</span></span>|<span data-ttu-id="8fe4f-133">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe4f-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8fe4f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="8fe4f-134">displayName</span></span>|<span data-ttu-id="8fe4f-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8fe4f-135">String</span></span>|<span data-ttu-id="8fe4f-136">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe4f-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8fe4f-137">description</span><span class="sxs-lookup"><span data-stu-id="8fe4f-137">description</span></span>|<span data-ttu-id="8fe4f-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8fe4f-138">String</span></span>|<span data-ttu-id="8fe4f-139">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe4f-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8fe4f-140">prioridade</span><span class="sxs-lookup"><span data-stu-id="8fe4f-140">priority</span></span>|<span data-ttu-id="8fe4f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe4f-141">Int32</span></span>|<span data-ttu-id="8fe4f-142">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe4f-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8fe4f-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8fe4f-143">createdDateTime</span></span>|<span data-ttu-id="8fe4f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fe4f-144">DateTimeOffset</span></span>|<span data-ttu-id="8fe4f-145">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe4f-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8fe4f-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fe4f-146">lastModifiedDateTime</span></span>|<span data-ttu-id="8fe4f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fe4f-147">DateTimeOffset</span></span>|<span data-ttu-id="8fe4f-148">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe4f-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8fe4f-149">version</span><span class="sxs-lookup"><span data-stu-id="8fe4f-149">version</span></span>|<span data-ttu-id="8fe4f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8fe4f-150">Int32</span></span>|<span data-ttu-id="8fe4f-151">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fe4f-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8fe4f-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="8fe4f-152">iosRestriction</span></span>|[<span data-ttu-id="8fe4f-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8fe4f-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8fe4f-154">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8fe4f-154">Not yet documented</span></span>|
|<span data-ttu-id="8fe4f-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="8fe4f-155">windowsRestriction</span></span>|[<span data-ttu-id="8fe4f-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8fe4f-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8fe4f-157">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8fe4f-157">Not yet documented</span></span>|
|<span data-ttu-id="8fe4f-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="8fe4f-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="8fe4f-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8fe4f-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8fe4f-160">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8fe4f-160">Not yet documented</span></span>|
|<span data-ttu-id="8fe4f-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="8fe4f-161">androidRestriction</span></span>|[<span data-ttu-id="8fe4f-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8fe4f-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8fe4f-163">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8fe4f-163">Not yet documented</span></span>|
|<span data-ttu-id="8fe4f-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="8fe4f-164">macOSRestriction</span></span>|[<span data-ttu-id="8fe4f-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8fe4f-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8fe4f-166">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8fe4f-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8fe4f-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fe4f-167">Response</span></span>
<span data-ttu-id="8fe4f-168">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8fe4f-168">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fe4f-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8fe4f-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="8fe4f-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8fe4f-170">Request</span></span>
<span data-ttu-id="8fe4f-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8fe4f-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8fe4f-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fe4f-172">Response</span></span>
<span data-ttu-id="8fe4f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8fe4f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



