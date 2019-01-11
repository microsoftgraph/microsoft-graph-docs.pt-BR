---
title: Atualizar deviceEnrollmentLimitConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f41238c42159f40821b2913f51e0b46a1f21725d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804910"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="ca2fa-103">Atualizar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca2fa-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="ca2fa-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ca2fa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca2fa-105">Atualizar as propriedades de um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca2fa-105">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca2fa-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca2fa-106">Prerequisites</span></span>
<span data-ttu-id="ca2fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca2fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca2fa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca2fa-109">Permission type</span></span>|<span data-ttu-id="ca2fa-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ca2fa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca2fa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca2fa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ca2fa-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca2fa-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ca2fa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca2fa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca2fa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca2fa-114">Not supported.</span></span>|
|<span data-ttu-id="ca2fa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca2fa-115">Application</span></span>|<span data-ttu-id="ca2fa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca2fa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca2fa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca2fa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ca2fa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca2fa-118">Request headers</span></span>
|<span data-ttu-id="ca2fa-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca2fa-119">Header</span></span>|<span data-ttu-id="ca2fa-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ca2fa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca2fa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca2fa-121">Authorization</span></span>|<span data-ttu-id="ca2fa-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca2fa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca2fa-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca2fa-123">Accept</span></span>|<span data-ttu-id="ca2fa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ca2fa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca2fa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca2fa-125">Request body</span></span>
<span data-ttu-id="ca2fa-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca2fa-126">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="ca2fa-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca2fa-127">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="ca2fa-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca2fa-128">Property</span></span>|<span data-ttu-id="ca2fa-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca2fa-129">Type</span></span>|<span data-ttu-id="ca2fa-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca2fa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca2fa-131">id</span><span class="sxs-lookup"><span data-stu-id="ca2fa-131">id</span></span>|<span data-ttu-id="ca2fa-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca2fa-132">String</span></span>|<span data-ttu-id="ca2fa-133">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca2fa-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ca2fa-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ca2fa-134">displayName</span></span>|<span data-ttu-id="ca2fa-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca2fa-135">String</span></span>|<span data-ttu-id="ca2fa-136">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca2fa-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ca2fa-137">description</span><span class="sxs-lookup"><span data-stu-id="ca2fa-137">description</span></span>|<span data-ttu-id="ca2fa-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca2fa-138">String</span></span>|<span data-ttu-id="ca2fa-139">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca2fa-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ca2fa-140">prioridade</span><span class="sxs-lookup"><span data-stu-id="ca2fa-140">priority</span></span>|<span data-ttu-id="ca2fa-141">Int32</span><span class="sxs-lookup"><span data-stu-id="ca2fa-141">Int32</span></span>|<span data-ttu-id="ca2fa-142">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca2fa-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ca2fa-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca2fa-143">createdDateTime</span></span>|<span data-ttu-id="ca2fa-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca2fa-144">DateTimeOffset</span></span>|<span data-ttu-id="ca2fa-145">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca2fa-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ca2fa-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca2fa-146">lastModifiedDateTime</span></span>|<span data-ttu-id="ca2fa-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca2fa-147">DateTimeOffset</span></span>|<span data-ttu-id="ca2fa-148">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca2fa-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ca2fa-149">version</span><span class="sxs-lookup"><span data-stu-id="ca2fa-149">version</span></span>|<span data-ttu-id="ca2fa-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ca2fa-150">Int32</span></span>|<span data-ttu-id="ca2fa-151">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca2fa-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ca2fa-152">limite</span><span class="sxs-lookup"><span data-stu-id="ca2fa-152">limit</span></span>|<span data-ttu-id="ca2fa-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ca2fa-153">Int32</span></span>|<span data-ttu-id="ca2fa-154">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ca2fa-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ca2fa-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca2fa-155">Response</span></span>
<span data-ttu-id="ca2fa-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca2fa-156">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca2fa-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca2fa-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="ca2fa-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca2fa-158">Request</span></span>
<span data-ttu-id="ca2fa-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca2fa-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 205

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="ca2fa-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca2fa-160">Response</span></span>
<span data-ttu-id="ca2fa-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca2fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 377

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```



