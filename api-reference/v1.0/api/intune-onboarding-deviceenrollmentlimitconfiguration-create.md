---
title: Criar deviceEnrollmentLimitConfiguration
description: Criar um novo objeto deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 010f755a7caa05b6fab294e6d071d6e882449ee8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925382"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="84e55-103">Criar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="84e55-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="84e55-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="84e55-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84e55-105">Criar um novo objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84e55-105">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84e55-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84e55-106">Prerequisites</span></span>
<span data-ttu-id="84e55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84e55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84e55-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84e55-109">Permission type</span></span>|<span data-ttu-id="84e55-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84e55-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84e55-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84e55-111">Delegated (work or school account)</span></span>|<span data-ttu-id="84e55-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84e55-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="84e55-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84e55-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84e55-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84e55-114">Not supported.</span></span>|
|<span data-ttu-id="84e55-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84e55-115">Application</span></span>|<span data-ttu-id="84e55-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84e55-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84e55-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84e55-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="84e55-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84e55-118">Request headers</span></span>
|<span data-ttu-id="84e55-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84e55-119">Header</span></span>|<span data-ttu-id="84e55-120">Valor</span><span class="sxs-lookup"><span data-stu-id="84e55-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84e55-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="84e55-121">Authorization</span></span>|<span data-ttu-id="84e55-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84e55-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84e55-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="84e55-123">Accept</span></span>|<span data-ttu-id="84e55-124">application/json</span><span class="sxs-lookup"><span data-stu-id="84e55-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84e55-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84e55-125">Request body</span></span>
<span data-ttu-id="84e55-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="84e55-126">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="84e55-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="84e55-127">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="84e55-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84e55-128">Property</span></span>|<span data-ttu-id="84e55-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="84e55-129">Type</span></span>|<span data-ttu-id="84e55-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="84e55-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84e55-131">id</span><span class="sxs-lookup"><span data-stu-id="84e55-131">id</span></span>|<span data-ttu-id="84e55-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84e55-132">String</span></span>|<span data-ttu-id="84e55-133">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84e55-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="84e55-134">displayName</span><span class="sxs-lookup"><span data-stu-id="84e55-134">displayName</span></span>|<span data-ttu-id="84e55-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84e55-135">String</span></span>|<span data-ttu-id="84e55-136">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84e55-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="84e55-137">description</span><span class="sxs-lookup"><span data-stu-id="84e55-137">description</span></span>|<span data-ttu-id="84e55-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84e55-138">String</span></span>|<span data-ttu-id="84e55-139">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84e55-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="84e55-140">prioridade</span><span class="sxs-lookup"><span data-stu-id="84e55-140">priority</span></span>|<span data-ttu-id="84e55-141">Int32</span><span class="sxs-lookup"><span data-stu-id="84e55-141">Int32</span></span>|<span data-ttu-id="84e55-142">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84e55-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="84e55-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84e55-143">createdDateTime</span></span>|<span data-ttu-id="84e55-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84e55-144">DateTimeOffset</span></span>|<span data-ttu-id="84e55-145">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84e55-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="84e55-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84e55-146">lastModifiedDateTime</span></span>|<span data-ttu-id="84e55-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84e55-147">DateTimeOffset</span></span>|<span data-ttu-id="84e55-148">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84e55-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="84e55-149">version</span><span class="sxs-lookup"><span data-stu-id="84e55-149">version</span></span>|<span data-ttu-id="84e55-150">Int32</span><span class="sxs-lookup"><span data-stu-id="84e55-150">Int32</span></span>|<span data-ttu-id="84e55-151">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84e55-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="84e55-152">limite</span><span class="sxs-lookup"><span data-stu-id="84e55-152">limit</span></span>|<span data-ttu-id="84e55-153">Int32</span><span class="sxs-lookup"><span data-stu-id="84e55-153">Int32</span></span>|<span data-ttu-id="84e55-154">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="84e55-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="84e55-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="84e55-155">Response</span></span>
<span data-ttu-id="84e55-156">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84e55-156">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84e55-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84e55-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="84e55-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84e55-158">Request</span></span>
<span data-ttu-id="84e55-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84e55-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="84e55-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="84e55-160">Response</span></span>
<span data-ttu-id="84e55-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84e55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



