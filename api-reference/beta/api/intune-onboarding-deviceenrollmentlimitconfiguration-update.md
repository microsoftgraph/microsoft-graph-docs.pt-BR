---
title: Atualizar deviceEnrollmentLimitConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 651649b36b2aa08c651640caa0f854f2b2ff98fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926509"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="942dc-103">Atualizar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="942dc-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="942dc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="942dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="942dc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="942dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="942dc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="942dc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="942dc-107">Atualizar as propriedades de um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="942dc-107">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="942dc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="942dc-108">Prerequisites</span></span>
<span data-ttu-id="942dc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="942dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="942dc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="942dc-111">Permission type</span></span>|<span data-ttu-id="942dc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="942dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="942dc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="942dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="942dc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="942dc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="942dc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="942dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="942dc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="942dc-116">Not supported.</span></span>|
|<span data-ttu-id="942dc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="942dc-117">Application</span></span>|<span data-ttu-id="942dc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="942dc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="942dc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="942dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="942dc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="942dc-120">Request headers</span></span>
|<span data-ttu-id="942dc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="942dc-121">Header</span></span>|<span data-ttu-id="942dc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="942dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="942dc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="942dc-123">Authorization</span></span>|<span data-ttu-id="942dc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="942dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="942dc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="942dc-125">Accept</span></span>|<span data-ttu-id="942dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="942dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="942dc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="942dc-127">Request body</span></span>
<span data-ttu-id="942dc-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="942dc-128">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="942dc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="942dc-129">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="942dc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="942dc-130">Property</span></span>|<span data-ttu-id="942dc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="942dc-131">Type</span></span>|<span data-ttu-id="942dc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="942dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="942dc-133">id</span><span class="sxs-lookup"><span data-stu-id="942dc-133">id</span></span>|<span data-ttu-id="942dc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="942dc-134">String</span></span>|<span data-ttu-id="942dc-135">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942dc-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="942dc-136">displayName</span><span class="sxs-lookup"><span data-stu-id="942dc-136">displayName</span></span>|<span data-ttu-id="942dc-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="942dc-137">String</span></span>|<span data-ttu-id="942dc-138">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942dc-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="942dc-139">description</span><span class="sxs-lookup"><span data-stu-id="942dc-139">description</span></span>|<span data-ttu-id="942dc-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="942dc-140">String</span></span>|<span data-ttu-id="942dc-141">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942dc-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="942dc-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="942dc-142">priority</span></span>|<span data-ttu-id="942dc-143">Int32</span><span class="sxs-lookup"><span data-stu-id="942dc-143">Int32</span></span>|<span data-ttu-id="942dc-144">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942dc-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="942dc-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="942dc-145">createdDateTime</span></span>|<span data-ttu-id="942dc-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="942dc-146">DateTimeOffset</span></span>|<span data-ttu-id="942dc-147">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942dc-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="942dc-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="942dc-148">lastModifiedDateTime</span></span>|<span data-ttu-id="942dc-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="942dc-149">DateTimeOffset</span></span>|<span data-ttu-id="942dc-150">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942dc-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="942dc-151">version</span><span class="sxs-lookup"><span data-stu-id="942dc-151">version</span></span>|<span data-ttu-id="942dc-152">Int32</span><span class="sxs-lookup"><span data-stu-id="942dc-152">Int32</span></span>|<span data-ttu-id="942dc-153">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942dc-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="942dc-154">limite</span><span class="sxs-lookup"><span data-stu-id="942dc-154">limit</span></span>|<span data-ttu-id="942dc-155">Int32</span><span class="sxs-lookup"><span data-stu-id="942dc-155">Int32</span></span>|<span data-ttu-id="942dc-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="942dc-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="942dc-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="942dc-157">Response</span></span>
<span data-ttu-id="942dc-158">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="942dc-158">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="942dc-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="942dc-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="942dc-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="942dc-160">Request</span></span>
<span data-ttu-id="942dc-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="942dc-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="942dc-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="942dc-162">Response</span></span>
<span data-ttu-id="942dc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="942dc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





