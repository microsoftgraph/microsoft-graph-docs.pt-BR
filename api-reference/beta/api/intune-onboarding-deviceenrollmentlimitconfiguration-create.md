---
title: Criar deviceEnrollmentLimitConfiguration
description: Criar um novo objeto deviceEnrollmentLimitConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cc7ab67dc44eec17a6e7a516967d3f3b0bc644ae
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401128"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="d7c08-103">Criar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="d7c08-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="d7c08-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="d7c08-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d7c08-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d7c08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7c08-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="d7c08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7c08-107">Criar um novo objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7c08-107">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7c08-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d7c08-108">Prerequisites</span></span>
<span data-ttu-id="d7c08-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d7c08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d7c08-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7c08-111">Permission type</span></span>|<span data-ttu-id="d7c08-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d7c08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7c08-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7c08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7c08-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7c08-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d7c08-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7c08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7c08-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7c08-116">Not supported.</span></span>|
|<span data-ttu-id="d7c08-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7c08-117">Application</span></span>|<span data-ttu-id="d7c08-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7c08-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7c08-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7c08-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d7c08-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7c08-120">Request headers</span></span>
|<span data-ttu-id="d7c08-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d7c08-121">Header</span></span>|<span data-ttu-id="d7c08-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d7c08-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7c08-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7c08-123">Authorization</span></span>|<span data-ttu-id="d7c08-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7c08-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7c08-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d7c08-125">Accept</span></span>|<span data-ttu-id="d7c08-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7c08-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7c08-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7c08-127">Request body</span></span>
<span data-ttu-id="d7c08-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d7c08-128">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="d7c08-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d7c08-129">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="d7c08-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7c08-130">Property</span></span>|<span data-ttu-id="d7c08-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7c08-131">Type</span></span>|<span data-ttu-id="d7c08-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7c08-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7c08-133">id</span><span class="sxs-lookup"><span data-stu-id="d7c08-133">id</span></span>|<span data-ttu-id="d7c08-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7c08-134">String</span></span>|<span data-ttu-id="d7c08-135">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7c08-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d7c08-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d7c08-136">displayName</span></span>|<span data-ttu-id="d7c08-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7c08-137">String</span></span>|<span data-ttu-id="d7c08-138">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7c08-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d7c08-139">description</span><span class="sxs-lookup"><span data-stu-id="d7c08-139">description</span></span>|<span data-ttu-id="d7c08-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7c08-140">String</span></span>|<span data-ttu-id="d7c08-141">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7c08-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d7c08-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="d7c08-142">priority</span></span>|<span data-ttu-id="d7c08-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d7c08-143">Int32</span></span>|<span data-ttu-id="d7c08-144">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7c08-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d7c08-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7c08-145">createdDateTime</span></span>|<span data-ttu-id="d7c08-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7c08-146">DateTimeOffset</span></span>|<span data-ttu-id="d7c08-147">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7c08-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d7c08-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7c08-148">lastModifiedDateTime</span></span>|<span data-ttu-id="d7c08-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7c08-149">DateTimeOffset</span></span>|<span data-ttu-id="d7c08-150">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7c08-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d7c08-151">version</span><span class="sxs-lookup"><span data-stu-id="d7c08-151">version</span></span>|<span data-ttu-id="d7c08-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d7c08-152">Int32</span></span>|<span data-ttu-id="d7c08-153">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7c08-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d7c08-154">limite</span><span class="sxs-lookup"><span data-stu-id="d7c08-154">limit</span></span>|<span data-ttu-id="d7c08-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d7c08-155">Int32</span></span>|<span data-ttu-id="d7c08-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d7c08-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d7c08-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7c08-157">Response</span></span>
<span data-ttu-id="d7c08-158">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7c08-158">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7c08-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7c08-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7c08-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7c08-160">Request</span></span>
<span data-ttu-id="d7c08-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7c08-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="d7c08-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7c08-162">Response</span></span>
<span data-ttu-id="d7c08-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7c08-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




