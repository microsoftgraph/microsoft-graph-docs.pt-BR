---
title: Criar deviceEnrollmentLimitConfiguration
description: Criar um novo objeto deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a331e49ea65450012d5f632b88579044382c9a1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986373"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="0a1aa-103">Criar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="0a1aa-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="0a1aa-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a1aa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a1aa-105">Criar um novo objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a1aa-105">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a1aa-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0a1aa-106">Prerequisites</span></span>
<span data-ttu-id="0a1aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a1aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a1aa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a1aa-109">Permission type</span></span>|<span data-ttu-id="0a1aa-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0a1aa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a1aa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a1aa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0a1aa-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a1aa-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0a1aa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a1aa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a1aa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a1aa-114">Not supported.</span></span>|
|<span data-ttu-id="0a1aa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a1aa-115">Application</span></span>|<span data-ttu-id="0a1aa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a1aa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a1aa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a1aa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0a1aa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1aa-118">Request headers</span></span>
|<span data-ttu-id="0a1aa-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a1aa-119">Header</span></span>|<span data-ttu-id="0a1aa-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0a1aa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a1aa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a1aa-121">Authorization</span></span>|<span data-ttu-id="0a1aa-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a1aa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a1aa-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0a1aa-123">Accept</span></span>|<span data-ttu-id="0a1aa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0a1aa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a1aa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1aa-125">Request body</span></span>
<span data-ttu-id="0a1aa-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0a1aa-126">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="0a1aa-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0a1aa-127">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="0a1aa-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a1aa-128">Property</span></span>|<span data-ttu-id="0a1aa-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a1aa-129">Type</span></span>|<span data-ttu-id="0a1aa-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a1aa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a1aa-131">id</span><span class="sxs-lookup"><span data-stu-id="0a1aa-131">id</span></span>|<span data-ttu-id="0a1aa-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a1aa-132">String</span></span>|<span data-ttu-id="0a1aa-133">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a1aa-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0a1aa-134">displayName</span><span class="sxs-lookup"><span data-stu-id="0a1aa-134">displayName</span></span>|<span data-ttu-id="0a1aa-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a1aa-135">String</span></span>|<span data-ttu-id="0a1aa-136">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a1aa-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0a1aa-137">description</span><span class="sxs-lookup"><span data-stu-id="0a1aa-137">description</span></span>|<span data-ttu-id="0a1aa-138">String</span><span class="sxs-lookup"><span data-stu-id="0a1aa-138">String</span></span>|<span data-ttu-id="0a1aa-139">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a1aa-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0a1aa-140">prioridade</span><span class="sxs-lookup"><span data-stu-id="0a1aa-140">priority</span></span>|<span data-ttu-id="0a1aa-141">Int32</span><span class="sxs-lookup"><span data-stu-id="0a1aa-141">Int32</span></span>|<span data-ttu-id="0a1aa-142">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a1aa-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0a1aa-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a1aa-143">createdDateTime</span></span>|<span data-ttu-id="0a1aa-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a1aa-144">DateTimeOffset</span></span>|<span data-ttu-id="0a1aa-145">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a1aa-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0a1aa-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a1aa-146">lastModifiedDateTime</span></span>|<span data-ttu-id="0a1aa-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a1aa-147">DateTimeOffset</span></span>|<span data-ttu-id="0a1aa-148">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a1aa-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0a1aa-149">versão</span><span class="sxs-lookup"><span data-stu-id="0a1aa-149">version</span></span>|<span data-ttu-id="0a1aa-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0a1aa-150">Int32</span></span>|<span data-ttu-id="0a1aa-151">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a1aa-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0a1aa-152">limite</span><span class="sxs-lookup"><span data-stu-id="0a1aa-152">limit</span></span>|<span data-ttu-id="0a1aa-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0a1aa-153">Int32</span></span>|<span data-ttu-id="0a1aa-154">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0a1aa-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0a1aa-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a1aa-155">Response</span></span>
<span data-ttu-id="0a1aa-156">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a1aa-156">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a1aa-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a1aa-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a1aa-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1aa-158">Request</span></span>
<span data-ttu-id="0a1aa-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a1aa-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0a1aa-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a1aa-160">Response</span></span>
<span data-ttu-id="0a1aa-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a1aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



