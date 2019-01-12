---
title: Criar deviceEnrollmentPlatformRestrictionsConfiguration
description: Criar um novo objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fc6dd6e21388b23146e3378b1e4521f92660d6f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962650"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="38f86-103">Criar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="38f86-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="38f86-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="38f86-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38f86-105">Criar um novo objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38f86-105">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="38f86-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38f86-106">Prerequisites</span></span>
<span data-ttu-id="38f86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38f86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38f86-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38f86-109">Permission type</span></span>|<span data-ttu-id="38f86-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="38f86-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38f86-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38f86-111">Delegated (work or school account)</span></span>|<span data-ttu-id="38f86-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38f86-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="38f86-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38f86-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38f86-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38f86-114">Not supported.</span></span>|
|<span data-ttu-id="38f86-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38f86-115">Application</span></span>|<span data-ttu-id="38f86-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38f86-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38f86-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38f86-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="38f86-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38f86-118">Request headers</span></span>
|<span data-ttu-id="38f86-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38f86-119">Header</span></span>|<span data-ttu-id="38f86-120">Valor</span><span class="sxs-lookup"><span data-stu-id="38f86-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38f86-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="38f86-121">Authorization</span></span>|<span data-ttu-id="38f86-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38f86-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38f86-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="38f86-123">Accept</span></span>|<span data-ttu-id="38f86-124">application/json</span><span class="sxs-lookup"><span data-stu-id="38f86-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38f86-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38f86-125">Request body</span></span>
<span data-ttu-id="38f86-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="38f86-126">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="38f86-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="38f86-127">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="38f86-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38f86-128">Property</span></span>|<span data-ttu-id="38f86-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="38f86-129">Type</span></span>|<span data-ttu-id="38f86-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="38f86-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38f86-131">id</span><span class="sxs-lookup"><span data-stu-id="38f86-131">id</span></span>|<span data-ttu-id="38f86-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38f86-132">String</span></span>|<span data-ttu-id="38f86-133">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38f86-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="38f86-134">displayName</span><span class="sxs-lookup"><span data-stu-id="38f86-134">displayName</span></span>|<span data-ttu-id="38f86-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38f86-135">String</span></span>|<span data-ttu-id="38f86-136">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38f86-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="38f86-137">description</span><span class="sxs-lookup"><span data-stu-id="38f86-137">description</span></span>|<span data-ttu-id="38f86-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38f86-138">String</span></span>|<span data-ttu-id="38f86-139">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38f86-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="38f86-140">prioridade</span><span class="sxs-lookup"><span data-stu-id="38f86-140">priority</span></span>|<span data-ttu-id="38f86-141">Int32</span><span class="sxs-lookup"><span data-stu-id="38f86-141">Int32</span></span>|<span data-ttu-id="38f86-142">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38f86-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="38f86-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38f86-143">createdDateTime</span></span>|<span data-ttu-id="38f86-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38f86-144">DateTimeOffset</span></span>|<span data-ttu-id="38f86-145">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38f86-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="38f86-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38f86-146">lastModifiedDateTime</span></span>|<span data-ttu-id="38f86-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38f86-147">DateTimeOffset</span></span>|<span data-ttu-id="38f86-148">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38f86-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="38f86-149">version</span><span class="sxs-lookup"><span data-stu-id="38f86-149">version</span></span>|<span data-ttu-id="38f86-150">Int32</span><span class="sxs-lookup"><span data-stu-id="38f86-150">Int32</span></span>|<span data-ttu-id="38f86-151">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38f86-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="38f86-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="38f86-152">iosRestriction</span></span>|[<span data-ttu-id="38f86-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="38f86-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="38f86-154">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="38f86-154">Not yet documented</span></span>|
|<span data-ttu-id="38f86-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="38f86-155">windowsRestriction</span></span>|[<span data-ttu-id="38f86-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="38f86-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="38f86-157">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="38f86-157">Not yet documented</span></span>|
|<span data-ttu-id="38f86-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="38f86-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="38f86-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="38f86-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="38f86-160">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="38f86-160">Not yet documented</span></span>|
|<span data-ttu-id="38f86-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="38f86-161">androidRestriction</span></span>|[<span data-ttu-id="38f86-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="38f86-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="38f86-163">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="38f86-163">Not yet documented</span></span>|
|<span data-ttu-id="38f86-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="38f86-164">macOSRestriction</span></span>|[<span data-ttu-id="38f86-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="38f86-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="38f86-166">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="38f86-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="38f86-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="38f86-167">Response</span></span>
<span data-ttu-id="38f86-168">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38f86-168">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38f86-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38f86-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="38f86-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38f86-170">Request</span></span>
<span data-ttu-id="38f86-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38f86-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="38f86-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="38f86-172">Response</span></span>
<span data-ttu-id="38f86-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38f86-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



