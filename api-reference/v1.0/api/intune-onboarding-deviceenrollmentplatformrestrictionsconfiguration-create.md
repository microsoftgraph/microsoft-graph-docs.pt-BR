---
title: Criar deviceEnrollmentPlatformRestrictionsConfiguration
description: Criar um novo objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 204b18b654e8cc13e1808d27643cd477d188a0b0
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988949"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="8d3a8-103">Criar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d3a8-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="8d3a8-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8d3a8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d3a8-105">Criar um novo objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d3a8-105">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d3a8-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8d3a8-106">Prerequisites</span></span>
<span data-ttu-id="8d3a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d3a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d3a8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d3a8-109">Permission type</span></span>|<span data-ttu-id="8d3a8-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8d3a8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d3a8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d3a8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8d3a8-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d3a8-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8d3a8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d3a8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d3a8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d3a8-114">Not supported.</span></span>|
|<span data-ttu-id="8d3a8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d3a8-115">Application</span></span>|<span data-ttu-id="8d3a8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d3a8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d3a8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d3a8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8d3a8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d3a8-118">Request headers</span></span>
|<span data-ttu-id="8d3a8-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8d3a8-119">Header</span></span>|<span data-ttu-id="8d3a8-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8d3a8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d3a8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d3a8-121">Authorization</span></span>|<span data-ttu-id="8d3a8-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d3a8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d3a8-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8d3a8-123">Accept</span></span>|<span data-ttu-id="8d3a8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8d3a8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d3a8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d3a8-125">Request body</span></span>
<span data-ttu-id="8d3a8-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8d3a8-126">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="8d3a8-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8d3a8-127">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="8d3a8-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d3a8-128">Property</span></span>|<span data-ttu-id="8d3a8-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d3a8-129">Type</span></span>|<span data-ttu-id="8d3a8-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d3a8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d3a8-131">id</span><span class="sxs-lookup"><span data-stu-id="8d3a8-131">id</span></span>|<span data-ttu-id="8d3a8-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d3a8-132">String</span></span>|<span data-ttu-id="8d3a8-133">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d3a8-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8d3a8-134">displayName</span><span class="sxs-lookup"><span data-stu-id="8d3a8-134">displayName</span></span>|<span data-ttu-id="8d3a8-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d3a8-135">String</span></span>|<span data-ttu-id="8d3a8-136">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d3a8-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8d3a8-137">description</span><span class="sxs-lookup"><span data-stu-id="8d3a8-137">description</span></span>|<span data-ttu-id="8d3a8-138">String</span><span class="sxs-lookup"><span data-stu-id="8d3a8-138">String</span></span>|<span data-ttu-id="8d3a8-139">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d3a8-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8d3a8-140">prioridade</span><span class="sxs-lookup"><span data-stu-id="8d3a8-140">priority</span></span>|<span data-ttu-id="8d3a8-141">Int32</span><span class="sxs-lookup"><span data-stu-id="8d3a8-141">Int32</span></span>|<span data-ttu-id="8d3a8-142">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d3a8-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8d3a8-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d3a8-143">createdDateTime</span></span>|<span data-ttu-id="8d3a8-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d3a8-144">DateTimeOffset</span></span>|<span data-ttu-id="8d3a8-145">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d3a8-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8d3a8-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d3a8-146">lastModifiedDateTime</span></span>|<span data-ttu-id="8d3a8-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d3a8-147">DateTimeOffset</span></span>|<span data-ttu-id="8d3a8-148">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d3a8-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8d3a8-149">versão</span><span class="sxs-lookup"><span data-stu-id="8d3a8-149">version</span></span>|<span data-ttu-id="8d3a8-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8d3a8-150">Int32</span></span>|<span data-ttu-id="8d3a8-151">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d3a8-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8d3a8-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="8d3a8-152">iosRestriction</span></span>|[<span data-ttu-id="8d3a8-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8d3a8-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8d3a8-154">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8d3a8-154">Not yet documented</span></span>|
|<span data-ttu-id="8d3a8-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="8d3a8-155">windowsRestriction</span></span>|[<span data-ttu-id="8d3a8-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8d3a8-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8d3a8-157">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8d3a8-157">Not yet documented</span></span>|
|<span data-ttu-id="8d3a8-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="8d3a8-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="8d3a8-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8d3a8-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8d3a8-160">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8d3a8-160">Not yet documented</span></span>|
|<span data-ttu-id="8d3a8-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="8d3a8-161">androidRestriction</span></span>|[<span data-ttu-id="8d3a8-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8d3a8-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8d3a8-163">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8d3a8-163">Not yet documented</span></span>|
|<span data-ttu-id="8d3a8-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="8d3a8-164">macOSRestriction</span></span>|[<span data-ttu-id="8d3a8-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8d3a8-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8d3a8-166">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8d3a8-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8d3a8-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d3a8-167">Response</span></span>
<span data-ttu-id="8d3a8-168">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d3a8-168">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d3a8-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d3a8-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d3a8-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d3a8-170">Request</span></span>
<span data-ttu-id="8d3a8-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d3a8-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8d3a8-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d3a8-172">Response</span></span>
<span data-ttu-id="8d3a8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d3a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



