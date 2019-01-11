---
title: Atualizar deviceEnrollmentLimitConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bd4b1c581260a7cd1438ddad6bc2e486af1ac679
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832883"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="54f9b-103">Atualizar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="54f9b-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="54f9b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="54f9b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54f9b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="54f9b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54f9b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="54f9b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54f9b-107">Atualizar as propriedades de um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54f9b-107">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="54f9b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54f9b-108">Prerequisites</span></span>
<span data-ttu-id="54f9b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54f9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54f9b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54f9b-111">Permission type</span></span>|<span data-ttu-id="54f9b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="54f9b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54f9b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54f9b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54f9b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54f9b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="54f9b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54f9b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54f9b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54f9b-116">Not supported.</span></span>|
|<span data-ttu-id="54f9b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54f9b-117">Application</span></span>|<span data-ttu-id="54f9b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54f9b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54f9b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54f9b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="54f9b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54f9b-120">Request headers</span></span>
|<span data-ttu-id="54f9b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54f9b-121">Header</span></span>|<span data-ttu-id="54f9b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="54f9b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54f9b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="54f9b-123">Authorization</span></span>|<span data-ttu-id="54f9b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54f9b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54f9b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="54f9b-125">Accept</span></span>|<span data-ttu-id="54f9b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54f9b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54f9b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54f9b-127">Request body</span></span>
<span data-ttu-id="54f9b-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54f9b-128">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="54f9b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54f9b-129">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="54f9b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54f9b-130">Property</span></span>|<span data-ttu-id="54f9b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="54f9b-131">Type</span></span>|<span data-ttu-id="54f9b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="54f9b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54f9b-133">id</span><span class="sxs-lookup"><span data-stu-id="54f9b-133">id</span></span>|<span data-ttu-id="54f9b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54f9b-134">String</span></span>|<span data-ttu-id="54f9b-135">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f9b-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="54f9b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="54f9b-136">displayName</span></span>|<span data-ttu-id="54f9b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54f9b-137">String</span></span>|<span data-ttu-id="54f9b-138">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f9b-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="54f9b-139">description</span><span class="sxs-lookup"><span data-stu-id="54f9b-139">description</span></span>|<span data-ttu-id="54f9b-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54f9b-140">String</span></span>|<span data-ttu-id="54f9b-141">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f9b-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="54f9b-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="54f9b-142">priority</span></span>|<span data-ttu-id="54f9b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="54f9b-143">Int32</span></span>|<span data-ttu-id="54f9b-144">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f9b-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="54f9b-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54f9b-145">createdDateTime</span></span>|<span data-ttu-id="54f9b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54f9b-146">DateTimeOffset</span></span>|<span data-ttu-id="54f9b-147">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f9b-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="54f9b-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54f9b-148">lastModifiedDateTime</span></span>|<span data-ttu-id="54f9b-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54f9b-149">DateTimeOffset</span></span>|<span data-ttu-id="54f9b-150">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f9b-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="54f9b-151">version</span><span class="sxs-lookup"><span data-stu-id="54f9b-151">version</span></span>|<span data-ttu-id="54f9b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="54f9b-152">Int32</span></span>|<span data-ttu-id="54f9b-153">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f9b-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="54f9b-154">limite</span><span class="sxs-lookup"><span data-stu-id="54f9b-154">limit</span></span>|<span data-ttu-id="54f9b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="54f9b-155">Int32</span></span>|<span data-ttu-id="54f9b-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="54f9b-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="54f9b-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="54f9b-157">Response</span></span>
<span data-ttu-id="54f9b-158">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54f9b-158">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54f9b-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54f9b-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="54f9b-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54f9b-160">Request</span></span>
<span data-ttu-id="54f9b-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54f9b-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 196

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="54f9b-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="54f9b-162">Response</span></span>
<span data-ttu-id="54f9b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54f9b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





