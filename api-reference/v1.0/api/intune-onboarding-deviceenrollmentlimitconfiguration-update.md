---
title: Atualizar deviceEnrollmentLimitConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c8173001c86ff5156fa6c382101e10ed54bb9f7f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075235"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="2fee7-103">Atualizar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="2fee7-103">Update deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="2fee7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fee7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2fee7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2fee7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fee7-106">Atualizar as propriedades de um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fee7-106">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2fee7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2fee7-107">Prerequisites</span></span>
<span data-ttu-id="2fee7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fee7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fee7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fee7-110">Permission type</span></span>|<span data-ttu-id="2fee7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2fee7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fee7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fee7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2fee7-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fee7-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2fee7-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fee7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fee7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fee7-115">Not supported.</span></span>|
|<span data-ttu-id="2fee7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fee7-116">Application</span></span>|<span data-ttu-id="2fee7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fee7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fee7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fee7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2fee7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fee7-119">Request headers</span></span>
|<span data-ttu-id="2fee7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2fee7-120">Header</span></span>|<span data-ttu-id="2fee7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2fee7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fee7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fee7-122">Authorization</span></span>|<span data-ttu-id="2fee7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fee7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fee7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2fee7-124">Accept</span></span>|<span data-ttu-id="2fee7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2fee7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fee7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fee7-126">Request body</span></span>
<span data-ttu-id="2fee7-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fee7-127">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="2fee7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fee7-128">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="2fee7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fee7-129">Property</span></span>|<span data-ttu-id="2fee7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fee7-130">Type</span></span>|<span data-ttu-id="2fee7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fee7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fee7-132">id</span><span class="sxs-lookup"><span data-stu-id="2fee7-132">id</span></span>|<span data-ttu-id="2fee7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fee7-133">String</span></span>|<span data-ttu-id="2fee7-134">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fee7-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2fee7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2fee7-135">displayName</span></span>|<span data-ttu-id="2fee7-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fee7-136">String</span></span>|<span data-ttu-id="2fee7-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fee7-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2fee7-138">description</span><span class="sxs-lookup"><span data-stu-id="2fee7-138">description</span></span>|<span data-ttu-id="2fee7-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fee7-139">String</span></span>|<span data-ttu-id="2fee7-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fee7-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2fee7-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="2fee7-141">priority</span></span>|<span data-ttu-id="2fee7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2fee7-142">Int32</span></span>|<span data-ttu-id="2fee7-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fee7-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2fee7-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2fee7-144">createdDateTime</span></span>|<span data-ttu-id="2fee7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fee7-145">DateTimeOffset</span></span>|<span data-ttu-id="2fee7-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fee7-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2fee7-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fee7-147">lastModifiedDateTime</span></span>|<span data-ttu-id="2fee7-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fee7-148">DateTimeOffset</span></span>|<span data-ttu-id="2fee7-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fee7-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2fee7-150">versão</span><span class="sxs-lookup"><span data-stu-id="2fee7-150">version</span></span>|<span data-ttu-id="2fee7-151">Int32</span><span class="sxs-lookup"><span data-stu-id="2fee7-151">Int32</span></span>|<span data-ttu-id="2fee7-152">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fee7-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2fee7-153">limite</span><span class="sxs-lookup"><span data-stu-id="2fee7-153">limit</span></span>|<span data-ttu-id="2fee7-154">Int32</span><span class="sxs-lookup"><span data-stu-id="2fee7-154">Int32</span></span>|<span data-ttu-id="2fee7-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2fee7-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2fee7-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fee7-156">Response</span></span>
<span data-ttu-id="2fee7-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fee7-157">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fee7-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fee7-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="2fee7-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fee7-159">Request</span></span>
<span data-ttu-id="2fee7-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fee7-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2fee7-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fee7-161">Response</span></span>
<span data-ttu-id="2fee7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fee7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









