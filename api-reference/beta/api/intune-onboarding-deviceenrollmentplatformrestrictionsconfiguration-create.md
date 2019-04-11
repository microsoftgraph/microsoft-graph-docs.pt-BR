---
title: Criar deviceEnrollmentPlatformRestrictionsConfiguration
description: Criar um novo objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 189a1be56f2f6b444202b1a7e945500e321515d2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778625"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="d9c19-103">Criar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9c19-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="d9c19-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9c19-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9c19-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9c19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9c19-106">Criar um novo objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9c19-106">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9c19-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9c19-107">Prerequisites</span></span>
<span data-ttu-id="d9c19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9c19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9c19-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9c19-110">Permission type</span></span>|<span data-ttu-id="d9c19-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9c19-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9c19-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9c19-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9c19-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9c19-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d9c19-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9c19-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9c19-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9c19-115">Not supported.</span></span>|
|<span data-ttu-id="d9c19-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9c19-116">Application</span></span>|<span data-ttu-id="d9c19-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9c19-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9c19-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9c19-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d9c19-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9c19-119">Request headers</span></span>
|<span data-ttu-id="d9c19-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9c19-120">Header</span></span>|<span data-ttu-id="d9c19-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d9c19-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9c19-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9c19-122">Authorization</span></span>|<span data-ttu-id="d9c19-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9c19-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9c19-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9c19-124">Accept</span></span>|<span data-ttu-id="d9c19-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d9c19-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9c19-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9c19-126">Request body</span></span>
<span data-ttu-id="d9c19-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d9c19-127">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="d9c19-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d9c19-128">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="d9c19-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9c19-129">Property</span></span>|<span data-ttu-id="d9c19-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9c19-130">Type</span></span>|<span data-ttu-id="d9c19-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9c19-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9c19-132">id</span><span class="sxs-lookup"><span data-stu-id="d9c19-132">id</span></span>|<span data-ttu-id="d9c19-133">String</span><span class="sxs-lookup"><span data-stu-id="d9c19-133">String</span></span>|<span data-ttu-id="d9c19-134">ID da configuração da página de status de registro herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9c19-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d9c19-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d9c19-135">displayName</span></span>|<span data-ttu-id="d9c19-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9c19-136">String</span></span>|<span data-ttu-id="d9c19-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9c19-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d9c19-138">description</span><span class="sxs-lookup"><span data-stu-id="d9c19-138">description</span></span>|<span data-ttu-id="d9c19-139">String</span><span class="sxs-lookup"><span data-stu-id="d9c19-139">String</span></span>|<span data-ttu-id="d9c19-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9c19-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d9c19-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="d9c19-141">priority</span></span>|<span data-ttu-id="d9c19-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d9c19-142">Int32</span></span>|<span data-ttu-id="d9c19-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9c19-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d9c19-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9c19-144">createdDateTime</span></span>|<span data-ttu-id="d9c19-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9c19-145">DateTimeOffset</span></span>|<span data-ttu-id="d9c19-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9c19-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d9c19-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9c19-147">lastModifiedDateTime</span></span>|<span data-ttu-id="d9c19-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9c19-148">DateTimeOffset</span></span>|<span data-ttu-id="d9c19-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9c19-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d9c19-150">versão</span><span class="sxs-lookup"><span data-stu-id="d9c19-150">version</span></span>|<span data-ttu-id="d9c19-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d9c19-151">Int32</span></span>|<span data-ttu-id="d9c19-152">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9c19-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d9c19-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="d9c19-153">iosRestriction</span></span>|[<span data-ttu-id="d9c19-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d9c19-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d9c19-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d9c19-155">Not yet documented</span></span>|
|<span data-ttu-id="d9c19-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="d9c19-156">windowsRestriction</span></span>|[<span data-ttu-id="d9c19-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d9c19-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d9c19-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d9c19-158">Not yet documented</span></span>|
|<span data-ttu-id="d9c19-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="d9c19-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="d9c19-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d9c19-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d9c19-161">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d9c19-161">Not yet documented</span></span>|
|<span data-ttu-id="d9c19-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="d9c19-162">androidRestriction</span></span>|[<span data-ttu-id="d9c19-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d9c19-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d9c19-164">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d9c19-164">Not yet documented</span></span>|
|<span data-ttu-id="d9c19-165">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="d9c19-165">androidForWorkRestriction</span></span>|[<span data-ttu-id="d9c19-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d9c19-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d9c19-167">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d9c19-167">Not yet documented</span></span>|
|<span data-ttu-id="d9c19-168">macRestriction</span><span class="sxs-lookup"><span data-stu-id="d9c19-168">macRestriction</span></span>|[<span data-ttu-id="d9c19-169">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d9c19-169">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d9c19-170">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d9c19-170">Not yet documented</span></span>|
|<span data-ttu-id="d9c19-171">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="d9c19-171">macOSRestriction</span></span>|[<span data-ttu-id="d9c19-172">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d9c19-172">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d9c19-173">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d9c19-173">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d9c19-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9c19-174">Response</span></span>
<span data-ttu-id="d9c19-175">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9c19-175">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9c19-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9c19-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9c19-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9c19-177">Request</span></span>
<span data-ttu-id="d9c19-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9c19-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d9c19-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9c19-179">Response</span></span>
<span data-ttu-id="d9c19-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9c19-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





