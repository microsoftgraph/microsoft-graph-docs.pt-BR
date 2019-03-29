---
title: Atualizar deviceEnrollmentPlatformRestrictionsConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b7432e9bd253499ac225ba6f033dd6af5b43e266
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967724"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="a1af0-103">Atualizar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1af0-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="a1af0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1af0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1af0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1af0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1af0-106">Atualizar as propriedades de um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1af0-106">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1af0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1af0-107">Prerequisites</span></span>
<span data-ttu-id="a1af0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1af0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1af0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1af0-110">Permission type</span></span>|<span data-ttu-id="a1af0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1af0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1af0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1af0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1af0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1af0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a1af0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1af0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1af0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1af0-115">Not supported.</span></span>|
|<span data-ttu-id="a1af0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1af0-116">Application</span></span>|<span data-ttu-id="a1af0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1af0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1af0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1af0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a1af0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1af0-119">Request headers</span></span>
|<span data-ttu-id="a1af0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1af0-120">Header</span></span>|<span data-ttu-id="a1af0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a1af0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1af0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1af0-122">Authorization</span></span>|<span data-ttu-id="a1af0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1af0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1af0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1af0-124">Accept</span></span>|<span data-ttu-id="a1af0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1af0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1af0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1af0-126">Request body</span></span>
<span data-ttu-id="a1af0-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1af0-127">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="a1af0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1af0-128">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="a1af0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1af0-129">Property</span></span>|<span data-ttu-id="a1af0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1af0-130">Type</span></span>|<span data-ttu-id="a1af0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1af0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1af0-132">id</span><span class="sxs-lookup"><span data-stu-id="a1af0-132">id</span></span>|<span data-ttu-id="a1af0-133">String</span><span class="sxs-lookup"><span data-stu-id="a1af0-133">String</span></span>|<span data-ttu-id="a1af0-134">ID da configuração da página de status de registro herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1af0-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a1af0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a1af0-135">displayName</span></span>|<span data-ttu-id="a1af0-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1af0-136">String</span></span>|<span data-ttu-id="a1af0-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1af0-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a1af0-138">descrição</span><span class="sxs-lookup"><span data-stu-id="a1af0-138">description</span></span>|<span data-ttu-id="a1af0-139">String</span><span class="sxs-lookup"><span data-stu-id="a1af0-139">String</span></span>|<span data-ttu-id="a1af0-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1af0-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a1af0-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="a1af0-141">priority</span></span>|<span data-ttu-id="a1af0-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a1af0-142">Int32</span></span>|<span data-ttu-id="a1af0-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1af0-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a1af0-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1af0-144">createdDateTime</span></span>|<span data-ttu-id="a1af0-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1af0-145">DateTimeOffset</span></span>|<span data-ttu-id="a1af0-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1af0-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a1af0-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1af0-147">lastModifiedDateTime</span></span>|<span data-ttu-id="a1af0-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1af0-148">DateTimeOffset</span></span>|<span data-ttu-id="a1af0-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1af0-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a1af0-150">versão</span><span class="sxs-lookup"><span data-stu-id="a1af0-150">version</span></span>|<span data-ttu-id="a1af0-151">Int32</span><span class="sxs-lookup"><span data-stu-id="a1af0-151">Int32</span></span>|<span data-ttu-id="a1af0-152">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1af0-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a1af0-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="a1af0-153">iosRestriction</span></span>|[<span data-ttu-id="a1af0-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a1af0-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a1af0-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1af0-155">Not yet documented</span></span>|
|<span data-ttu-id="a1af0-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="a1af0-156">windowsRestriction</span></span>|[<span data-ttu-id="a1af0-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a1af0-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a1af0-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1af0-158">Not yet documented</span></span>|
|<span data-ttu-id="a1af0-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="a1af0-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="a1af0-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a1af0-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a1af0-161">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1af0-161">Not yet documented</span></span>|
|<span data-ttu-id="a1af0-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="a1af0-162">androidRestriction</span></span>|[<span data-ttu-id="a1af0-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a1af0-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a1af0-164">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1af0-164">Not yet documented</span></span>|
|<span data-ttu-id="a1af0-165">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="a1af0-165">androidForWorkRestriction</span></span>|[<span data-ttu-id="a1af0-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a1af0-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a1af0-167">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1af0-167">Not yet documented</span></span>|
|<span data-ttu-id="a1af0-168">macRestriction</span><span class="sxs-lookup"><span data-stu-id="a1af0-168">macRestriction</span></span>|[<span data-ttu-id="a1af0-169">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a1af0-169">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a1af0-170">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1af0-170">Not yet documented</span></span>|
|<span data-ttu-id="a1af0-171">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="a1af0-171">macOSRestriction</span></span>|[<span data-ttu-id="a1af0-172">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a1af0-172">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a1af0-173">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1af0-173">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a1af0-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1af0-174">Response</span></span>
<span data-ttu-id="a1af0-175">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1af0-175">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1af0-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1af0-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1af0-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1af0-177">Request</span></span>
<span data-ttu-id="a1af0-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1af0-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a1af0-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1af0-179">Response</span></span>
<span data-ttu-id="a1af0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1af0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




