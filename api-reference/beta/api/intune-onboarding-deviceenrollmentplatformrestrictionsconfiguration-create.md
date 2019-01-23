---
title: Criar deviceEnrollmentPlatformRestrictionsConfiguration
description: Criar um novo objeto deviceEnrollmentPlatformRestrictionsConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b2910d8b87535464f449a8649173102aab8b134
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407274"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="cf385-103">Criar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf385-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="cf385-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="cf385-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cf385-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cf385-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf385-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cf385-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf385-107">Criar um novo objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf385-107">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf385-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf385-108">Prerequisites</span></span>
<span data-ttu-id="cf385-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cf385-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cf385-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf385-111">Permission type</span></span>|<span data-ttu-id="cf385-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf385-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf385-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf385-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf385-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf385-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cf385-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf385-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf385-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf385-116">Not supported.</span></span>|
|<span data-ttu-id="cf385-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf385-117">Application</span></span>|<span data-ttu-id="cf385-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf385-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf385-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf385-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cf385-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf385-120">Request headers</span></span>
|<span data-ttu-id="cf385-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf385-121">Header</span></span>|<span data-ttu-id="cf385-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cf385-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf385-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf385-123">Authorization</span></span>|<span data-ttu-id="cf385-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf385-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf385-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf385-125">Accept</span></span>|<span data-ttu-id="cf385-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf385-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf385-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf385-127">Request body</span></span>
<span data-ttu-id="cf385-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cf385-128">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="cf385-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cf385-129">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="cf385-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf385-130">Property</span></span>|<span data-ttu-id="cf385-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf385-131">Type</span></span>|<span data-ttu-id="cf385-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf385-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf385-133">id</span><span class="sxs-lookup"><span data-stu-id="cf385-133">id</span></span>|<span data-ttu-id="cf385-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf385-134">String</span></span>|<span data-ttu-id="cf385-135">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf385-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cf385-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cf385-136">displayName</span></span>|<span data-ttu-id="cf385-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf385-137">String</span></span>|<span data-ttu-id="cf385-138">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf385-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cf385-139">description</span><span class="sxs-lookup"><span data-stu-id="cf385-139">description</span></span>|<span data-ttu-id="cf385-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf385-140">String</span></span>|<span data-ttu-id="cf385-141">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf385-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cf385-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="cf385-142">priority</span></span>|<span data-ttu-id="cf385-143">Int32</span><span class="sxs-lookup"><span data-stu-id="cf385-143">Int32</span></span>|<span data-ttu-id="cf385-144">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf385-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cf385-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf385-145">createdDateTime</span></span>|<span data-ttu-id="cf385-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf385-146">DateTimeOffset</span></span>|<span data-ttu-id="cf385-147">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf385-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cf385-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf385-148">lastModifiedDateTime</span></span>|<span data-ttu-id="cf385-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf385-149">DateTimeOffset</span></span>|<span data-ttu-id="cf385-150">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf385-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cf385-151">version</span><span class="sxs-lookup"><span data-stu-id="cf385-151">version</span></span>|<span data-ttu-id="cf385-152">Int32</span><span class="sxs-lookup"><span data-stu-id="cf385-152">Int32</span></span>|<span data-ttu-id="cf385-153">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf385-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cf385-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="cf385-154">iosRestriction</span></span>|[<span data-ttu-id="cf385-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="cf385-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="cf385-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cf385-156">Not yet documented</span></span>|
|<span data-ttu-id="cf385-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="cf385-157">windowsRestriction</span></span>|[<span data-ttu-id="cf385-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="cf385-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="cf385-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cf385-159">Not yet documented</span></span>|
|<span data-ttu-id="cf385-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="cf385-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="cf385-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="cf385-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="cf385-162">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cf385-162">Not yet documented</span></span>|
|<span data-ttu-id="cf385-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="cf385-163">androidRestriction</span></span>|[<span data-ttu-id="cf385-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="cf385-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="cf385-165">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cf385-165">Not yet documented</span></span>|
|<span data-ttu-id="cf385-166">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="cf385-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="cf385-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="cf385-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="cf385-168">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cf385-168">Not yet documented</span></span>|
|<span data-ttu-id="cf385-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="cf385-169">macRestriction</span></span>|[<span data-ttu-id="cf385-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="cf385-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="cf385-171">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cf385-171">Not yet documented</span></span>|
|<span data-ttu-id="cf385-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="cf385-172">macOSRestriction</span></span>|[<span data-ttu-id="cf385-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="cf385-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="cf385-174">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cf385-174">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cf385-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf385-175">Response</span></span>
<span data-ttu-id="cf385-176">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf385-176">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf385-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf385-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf385-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf385-178">Request</span></span>
<span data-ttu-id="cf385-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf385-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="cf385-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf385-180">Response</span></span>
<span data-ttu-id="cf385-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf385-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




