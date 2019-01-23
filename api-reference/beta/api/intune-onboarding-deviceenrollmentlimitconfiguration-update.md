---
title: Atualizar deviceEnrollmentLimitConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentLimitConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: afcd7a866275d8178dc1ab929bdde614e3d519a6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416486"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="6e183-103">Atualizar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e183-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="6e183-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="6e183-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6e183-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6e183-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e183-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="6e183-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e183-107">Atualizar as propriedades de um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e183-107">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e183-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e183-108">Prerequisites</span></span>
<span data-ttu-id="6e183-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6e183-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6e183-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e183-111">Permission type</span></span>|<span data-ttu-id="6e183-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6e183-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e183-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e183-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e183-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e183-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6e183-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e183-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e183-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e183-116">Not supported.</span></span>|
|<span data-ttu-id="6e183-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e183-117">Application</span></span>|<span data-ttu-id="6e183-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e183-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e183-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e183-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6e183-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e183-120">Request headers</span></span>
|<span data-ttu-id="6e183-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e183-121">Header</span></span>|<span data-ttu-id="6e183-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6e183-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e183-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e183-123">Authorization</span></span>|<span data-ttu-id="6e183-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e183-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e183-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6e183-125">Accept</span></span>|<span data-ttu-id="6e183-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e183-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e183-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e183-127">Request body</span></span>
<span data-ttu-id="6e183-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e183-128">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="6e183-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e183-129">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="6e183-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e183-130">Property</span></span>|<span data-ttu-id="6e183-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e183-131">Type</span></span>|<span data-ttu-id="6e183-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e183-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e183-133">id</span><span class="sxs-lookup"><span data-stu-id="6e183-133">id</span></span>|<span data-ttu-id="6e183-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e183-134">String</span></span>|<span data-ttu-id="6e183-135">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e183-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6e183-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6e183-136">displayName</span></span>|<span data-ttu-id="6e183-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e183-137">String</span></span>|<span data-ttu-id="6e183-138">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e183-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6e183-139">description</span><span class="sxs-lookup"><span data-stu-id="6e183-139">description</span></span>|<span data-ttu-id="6e183-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e183-140">String</span></span>|<span data-ttu-id="6e183-141">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e183-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6e183-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="6e183-142">priority</span></span>|<span data-ttu-id="6e183-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6e183-143">Int32</span></span>|<span data-ttu-id="6e183-144">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e183-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6e183-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e183-145">createdDateTime</span></span>|<span data-ttu-id="6e183-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e183-146">DateTimeOffset</span></span>|<span data-ttu-id="6e183-147">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e183-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6e183-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e183-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6e183-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e183-149">DateTimeOffset</span></span>|<span data-ttu-id="6e183-150">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e183-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6e183-151">version</span><span class="sxs-lookup"><span data-stu-id="6e183-151">version</span></span>|<span data-ttu-id="6e183-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6e183-152">Int32</span></span>|<span data-ttu-id="6e183-153">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e183-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6e183-154">limite</span><span class="sxs-lookup"><span data-stu-id="6e183-154">limit</span></span>|<span data-ttu-id="6e183-155">Int32</span><span class="sxs-lookup"><span data-stu-id="6e183-155">Int32</span></span>|<span data-ttu-id="6e183-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6e183-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6e183-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e183-157">Response</span></span>
<span data-ttu-id="6e183-158">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e183-158">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e183-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e183-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e183-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e183-160">Request</span></span>
<span data-ttu-id="6e183-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e183-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="6e183-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e183-162">Response</span></span>
<span data-ttu-id="6e183-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e183-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




