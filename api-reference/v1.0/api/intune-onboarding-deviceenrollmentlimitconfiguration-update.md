---
title: Atualizar deviceEnrollmentLimitConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentLimitConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1dfa90f394953e03bf8dfe65fe654dce1fbd32c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512654"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="fd037-103">Atualizar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd037-103">Update deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="fd037-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd037-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd037-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fd037-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd037-106">Atualizar as propriedades de um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd037-106">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd037-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd037-107">Prerequisites</span></span>
<span data-ttu-id="fd037-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd037-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd037-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd037-110">Permission type</span></span>|<span data-ttu-id="fd037-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fd037-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd037-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd037-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd037-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd037-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fd037-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd037-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd037-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd037-115">Not supported.</span></span>|
|<span data-ttu-id="fd037-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd037-116">Application</span></span>|<span data-ttu-id="fd037-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd037-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd037-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd037-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fd037-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd037-119">Request headers</span></span>
|<span data-ttu-id="fd037-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd037-120">Header</span></span>|<span data-ttu-id="fd037-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fd037-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd037-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd037-122">Authorization</span></span>|<span data-ttu-id="fd037-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd037-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd037-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fd037-124">Accept</span></span>|<span data-ttu-id="fd037-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fd037-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd037-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd037-126">Request body</span></span>
<span data-ttu-id="fd037-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd037-127">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="fd037-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd037-128">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="fd037-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd037-129">Property</span></span>|<span data-ttu-id="fd037-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd037-130">Type</span></span>|<span data-ttu-id="fd037-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd037-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd037-132">id</span><span class="sxs-lookup"><span data-stu-id="fd037-132">id</span></span>|<span data-ttu-id="fd037-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd037-133">String</span></span>|<span data-ttu-id="fd037-134">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd037-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fd037-135">displayName</span><span class="sxs-lookup"><span data-stu-id="fd037-135">displayName</span></span>|<span data-ttu-id="fd037-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd037-136">String</span></span>|<span data-ttu-id="fd037-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd037-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fd037-138">description</span><span class="sxs-lookup"><span data-stu-id="fd037-138">description</span></span>|<span data-ttu-id="fd037-139">String</span><span class="sxs-lookup"><span data-stu-id="fd037-139">String</span></span>|<span data-ttu-id="fd037-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd037-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fd037-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="fd037-141">priority</span></span>|<span data-ttu-id="fd037-142">Int32</span><span class="sxs-lookup"><span data-stu-id="fd037-142">Int32</span></span>|<span data-ttu-id="fd037-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd037-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fd037-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd037-144">createdDateTime</span></span>|<span data-ttu-id="fd037-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd037-145">DateTimeOffset</span></span>|<span data-ttu-id="fd037-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd037-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fd037-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd037-147">lastModifiedDateTime</span></span>|<span data-ttu-id="fd037-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd037-148">DateTimeOffset</span></span>|<span data-ttu-id="fd037-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd037-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fd037-150">versão</span><span class="sxs-lookup"><span data-stu-id="fd037-150">version</span></span>|<span data-ttu-id="fd037-151">Int32</span><span class="sxs-lookup"><span data-stu-id="fd037-151">Int32</span></span>|<span data-ttu-id="fd037-152">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd037-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fd037-153">limite</span><span class="sxs-lookup"><span data-stu-id="fd037-153">limit</span></span>|<span data-ttu-id="fd037-154">Int32</span><span class="sxs-lookup"><span data-stu-id="fd037-154">Int32</span></span>|<span data-ttu-id="fd037-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fd037-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fd037-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd037-156">Response</span></span>
<span data-ttu-id="fd037-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd037-157">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd037-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd037-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd037-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd037-159">Request</span></span>
<span data-ttu-id="fd037-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd037-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fd037-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd037-161">Response</span></span>
<span data-ttu-id="fd037-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd037-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




