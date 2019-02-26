---
title: Atualizar deviceEnrollmentLimitConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 842c9d6c1cf6e805850317bb804cb8905c189134
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254174"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="943e3-103">Atualizar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="943e3-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="943e3-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="943e3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="943e3-105">Atualizar as propriedades de um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="943e3-105">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="943e3-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="943e3-106">Prerequisites</span></span>
<span data-ttu-id="943e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="943e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="943e3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="943e3-109">Permission type</span></span>|<span data-ttu-id="943e3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="943e3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="943e3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="943e3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="943e3-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="943e3-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="943e3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="943e3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="943e3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="943e3-114">Not supported.</span></span>|
|<span data-ttu-id="943e3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="943e3-115">Application</span></span>|<span data-ttu-id="943e3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="943e3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="943e3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="943e3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="943e3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="943e3-118">Request headers</span></span>
|<span data-ttu-id="943e3-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="943e3-119">Header</span></span>|<span data-ttu-id="943e3-120">Valor</span><span class="sxs-lookup"><span data-stu-id="943e3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="943e3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="943e3-121">Authorization</span></span>|<span data-ttu-id="943e3-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="943e3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="943e3-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="943e3-123">Accept</span></span>|<span data-ttu-id="943e3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="943e3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="943e3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="943e3-125">Request body</span></span>
<span data-ttu-id="943e3-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="943e3-126">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="943e3-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="943e3-127">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="943e3-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="943e3-128">Property</span></span>|<span data-ttu-id="943e3-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="943e3-129">Type</span></span>|<span data-ttu-id="943e3-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="943e3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="943e3-131">id</span><span class="sxs-lookup"><span data-stu-id="943e3-131">id</span></span>|<span data-ttu-id="943e3-132">String</span><span class="sxs-lookup"><span data-stu-id="943e3-132">String</span></span>|<span data-ttu-id="943e3-133">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="943e3-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="943e3-134">displayName</span><span class="sxs-lookup"><span data-stu-id="943e3-134">displayName</span></span>|<span data-ttu-id="943e3-135">String</span><span class="sxs-lookup"><span data-stu-id="943e3-135">String</span></span>|<span data-ttu-id="943e3-136">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="943e3-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="943e3-137">description</span><span class="sxs-lookup"><span data-stu-id="943e3-137">description</span></span>|<span data-ttu-id="943e3-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="943e3-138">String</span></span>|<span data-ttu-id="943e3-139">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="943e3-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="943e3-140">prioridade</span><span class="sxs-lookup"><span data-stu-id="943e3-140">priority</span></span>|<span data-ttu-id="943e3-141">Int32</span><span class="sxs-lookup"><span data-stu-id="943e3-141">Int32</span></span>|<span data-ttu-id="943e3-142">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="943e3-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="943e3-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="943e3-143">createdDateTime</span></span>|<span data-ttu-id="943e3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="943e3-144">DateTimeOffset</span></span>|<span data-ttu-id="943e3-145">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="943e3-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="943e3-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="943e3-146">lastModifiedDateTime</span></span>|<span data-ttu-id="943e3-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="943e3-147">DateTimeOffset</span></span>|<span data-ttu-id="943e3-148">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="943e3-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="943e3-149">version</span><span class="sxs-lookup"><span data-stu-id="943e3-149">version</span></span>|<span data-ttu-id="943e3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="943e3-150">Int32</span></span>|<span data-ttu-id="943e3-151">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="943e3-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="943e3-152">limite</span><span class="sxs-lookup"><span data-stu-id="943e3-152">limit</span></span>|<span data-ttu-id="943e3-153">Int32</span><span class="sxs-lookup"><span data-stu-id="943e3-153">Int32</span></span>|<span data-ttu-id="943e3-154">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="943e3-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="943e3-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="943e3-155">Response</span></span>
<span data-ttu-id="943e3-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="943e3-156">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="943e3-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="943e3-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="943e3-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="943e3-158">Request</span></span>
<span data-ttu-id="943e3-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="943e3-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="943e3-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="943e3-160">Response</span></span>
<span data-ttu-id="943e3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="943e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



