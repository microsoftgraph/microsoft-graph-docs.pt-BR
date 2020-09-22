---
title: Criar deviceEnrollmentPlatformRestrictionsConfiguration
description: Criar um novo objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9bbac90b39141d201792f78dcc9883bc1eb23d2b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033185"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="15f3b-103">Criar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="15f3b-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="15f3b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15f3b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15f3b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15f3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15f3b-106">Criar um novo objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15f3b-106">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15f3b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15f3b-107">Prerequisites</span></span>
<span data-ttu-id="15f3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15f3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15f3b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15f3b-110">Permission type</span></span>|<span data-ttu-id="15f3b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15f3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15f3b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15f3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="15f3b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15f3b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="15f3b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15f3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15f3b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15f3b-115">Not supported.</span></span>|
|<span data-ttu-id="15f3b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15f3b-116">Application</span></span>|<span data-ttu-id="15f3b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15f3b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15f3b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15f3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="15f3b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15f3b-119">Request headers</span></span>
|<span data-ttu-id="15f3b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15f3b-120">Header</span></span>|<span data-ttu-id="15f3b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="15f3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15f3b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="15f3b-122">Authorization</span></span>|<span data-ttu-id="15f3b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15f3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15f3b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15f3b-124">Accept</span></span>|<span data-ttu-id="15f3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="15f3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15f3b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15f3b-126">Request body</span></span>
<span data-ttu-id="15f3b-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="15f3b-127">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="15f3b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="15f3b-128">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="15f3b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15f3b-129">Property</span></span>|<span data-ttu-id="15f3b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="15f3b-130">Type</span></span>|<span data-ttu-id="15f3b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="15f3b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15f3b-132">id</span><span class="sxs-lookup"><span data-stu-id="15f3b-132">id</span></span>|<span data-ttu-id="15f3b-133">String</span><span class="sxs-lookup"><span data-stu-id="15f3b-133">String</span></span>|<span data-ttu-id="15f3b-134">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15f3b-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="15f3b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="15f3b-135">displayName</span></span>|<span data-ttu-id="15f3b-136">String</span><span class="sxs-lookup"><span data-stu-id="15f3b-136">String</span></span>|<span data-ttu-id="15f3b-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15f3b-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="15f3b-138">description</span><span class="sxs-lookup"><span data-stu-id="15f3b-138">description</span></span>|<span data-ttu-id="15f3b-139">String</span><span class="sxs-lookup"><span data-stu-id="15f3b-139">String</span></span>|<span data-ttu-id="15f3b-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15f3b-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="15f3b-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="15f3b-141">priority</span></span>|<span data-ttu-id="15f3b-142">Int32</span><span class="sxs-lookup"><span data-stu-id="15f3b-142">Int32</span></span>|<span data-ttu-id="15f3b-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15f3b-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="15f3b-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15f3b-144">createdDateTime</span></span>|<span data-ttu-id="15f3b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15f3b-145">DateTimeOffset</span></span>|<span data-ttu-id="15f3b-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15f3b-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="15f3b-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15f3b-147">lastModifiedDateTime</span></span>|<span data-ttu-id="15f3b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15f3b-148">DateTimeOffset</span></span>|<span data-ttu-id="15f3b-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15f3b-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="15f3b-150">versão</span><span class="sxs-lookup"><span data-stu-id="15f3b-150">version</span></span>|<span data-ttu-id="15f3b-151">Int32</span><span class="sxs-lookup"><span data-stu-id="15f3b-151">Int32</span></span>|<span data-ttu-id="15f3b-152">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15f3b-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="15f3b-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="15f3b-153">iosRestriction</span></span>|[<span data-ttu-id="15f3b-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="15f3b-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="15f3b-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="15f3b-155">Not yet documented</span></span>|
|<span data-ttu-id="15f3b-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="15f3b-156">windowsRestriction</span></span>|[<span data-ttu-id="15f3b-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="15f3b-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="15f3b-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="15f3b-158">Not yet documented</span></span>|
|<span data-ttu-id="15f3b-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="15f3b-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="15f3b-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="15f3b-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="15f3b-161">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="15f3b-161">Not yet documented</span></span>|
|<span data-ttu-id="15f3b-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="15f3b-162">androidRestriction</span></span>|[<span data-ttu-id="15f3b-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="15f3b-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="15f3b-164">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="15f3b-164">Not yet documented</span></span>|
|<span data-ttu-id="15f3b-165">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="15f3b-165">macOSRestriction</span></span>|[<span data-ttu-id="15f3b-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="15f3b-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="15f3b-167">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="15f3b-167">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="15f3b-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f3b-168">Response</span></span>
<span data-ttu-id="15f3b-169">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15f3b-169">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15f3b-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15f3b-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="15f3b-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15f3b-171">Request</span></span>
<span data-ttu-id="15f3b-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15f3b-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="15f3b-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="15f3b-173">Response</span></span>
<span data-ttu-id="15f3b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15f3b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









