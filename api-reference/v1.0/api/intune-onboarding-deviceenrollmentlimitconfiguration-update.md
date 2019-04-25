---
title: Atualizar deviceEnrollmentLimitConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c54a7bba58e64fc9f74053cc40e43517bc65a881
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582784"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="4dbba-103">Atualizar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="4dbba-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="4dbba-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4dbba-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dbba-105">Atualizar as propriedades de um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4dbba-105">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4dbba-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4dbba-106">Prerequisites</span></span>
<span data-ttu-id="4dbba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dbba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dbba-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4dbba-109">Permission type</span></span>|<span data-ttu-id="4dbba-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4dbba-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dbba-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4dbba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4dbba-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dbba-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4dbba-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4dbba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dbba-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dbba-114">Not supported.</span></span>|
|<span data-ttu-id="4dbba-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4dbba-115">Application</span></span>|<span data-ttu-id="4dbba-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dbba-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dbba-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4dbba-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4dbba-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4dbba-118">Request headers</span></span>
|<span data-ttu-id="4dbba-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4dbba-119">Header</span></span>|<span data-ttu-id="4dbba-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4dbba-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dbba-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4dbba-121">Authorization</span></span>|<span data-ttu-id="4dbba-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4dbba-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dbba-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4dbba-123">Accept</span></span>|<span data-ttu-id="4dbba-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4dbba-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dbba-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4dbba-125">Request body</span></span>
<span data-ttu-id="4dbba-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4dbba-126">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="4dbba-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4dbba-127">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="4dbba-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4dbba-128">Property</span></span>|<span data-ttu-id="4dbba-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4dbba-129">Type</span></span>|<span data-ttu-id="4dbba-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dbba-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dbba-131">id</span><span class="sxs-lookup"><span data-stu-id="4dbba-131">id</span></span>|<span data-ttu-id="4dbba-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4dbba-132">String</span></span>|<span data-ttu-id="4dbba-133">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4dbba-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4dbba-134">displayName</span><span class="sxs-lookup"><span data-stu-id="4dbba-134">displayName</span></span>|<span data-ttu-id="4dbba-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4dbba-135">String</span></span>|<span data-ttu-id="4dbba-136">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4dbba-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4dbba-137">description</span><span class="sxs-lookup"><span data-stu-id="4dbba-137">description</span></span>|<span data-ttu-id="4dbba-138">String</span><span class="sxs-lookup"><span data-stu-id="4dbba-138">String</span></span>|<span data-ttu-id="4dbba-139">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4dbba-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4dbba-140">prioridade</span><span class="sxs-lookup"><span data-stu-id="4dbba-140">priority</span></span>|<span data-ttu-id="4dbba-141">Int32</span><span class="sxs-lookup"><span data-stu-id="4dbba-141">Int32</span></span>|<span data-ttu-id="4dbba-142">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4dbba-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4dbba-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4dbba-143">createdDateTime</span></span>|<span data-ttu-id="4dbba-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dbba-144">DateTimeOffset</span></span>|<span data-ttu-id="4dbba-145">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4dbba-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4dbba-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4dbba-146">lastModifiedDateTime</span></span>|<span data-ttu-id="4dbba-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dbba-147">DateTimeOffset</span></span>|<span data-ttu-id="4dbba-148">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4dbba-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4dbba-149">versão</span><span class="sxs-lookup"><span data-stu-id="4dbba-149">version</span></span>|<span data-ttu-id="4dbba-150">Int32</span><span class="sxs-lookup"><span data-stu-id="4dbba-150">Int32</span></span>|<span data-ttu-id="4dbba-151">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4dbba-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4dbba-152">limite</span><span class="sxs-lookup"><span data-stu-id="4dbba-152">limit</span></span>|<span data-ttu-id="4dbba-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4dbba-153">Int32</span></span>|<span data-ttu-id="4dbba-154">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4dbba-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4dbba-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dbba-155">Response</span></span>
<span data-ttu-id="4dbba-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4dbba-156">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dbba-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4dbba-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="4dbba-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4dbba-158">Request</span></span>
<span data-ttu-id="4dbba-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4dbba-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4dbba-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dbba-160">Response</span></span>
<span data-ttu-id="4dbba-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4dbba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



