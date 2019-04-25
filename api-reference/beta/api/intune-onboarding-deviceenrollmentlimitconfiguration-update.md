---
title: Atualizar deviceEnrollmentLimitConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 775eba06cce66394f448f305d10f80ca9ec16822
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32529286"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="7d20f-103">Atualizar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="7d20f-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="7d20f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7d20f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d20f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d20f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d20f-106">Atualizar as propriedades de um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d20f-106">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d20f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d20f-107">Prerequisites</span></span>
<span data-ttu-id="7d20f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d20f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d20f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d20f-110">Permission type</span></span>|<span data-ttu-id="7d20f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d20f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d20f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d20f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7d20f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d20f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7d20f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d20f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d20f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d20f-115">Not supported.</span></span>|
|<span data-ttu-id="7d20f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d20f-116">Application</span></span>|<span data-ttu-id="7d20f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d20f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d20f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d20f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7d20f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d20f-119">Request headers</span></span>
|<span data-ttu-id="7d20f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d20f-120">Header</span></span>|<span data-ttu-id="7d20f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7d20f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d20f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d20f-122">Authorization</span></span>|<span data-ttu-id="7d20f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d20f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d20f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d20f-124">Accept</span></span>|<span data-ttu-id="7d20f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7d20f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d20f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d20f-126">Request body</span></span>
<span data-ttu-id="7d20f-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d20f-127">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="7d20f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d20f-128">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="7d20f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d20f-129">Property</span></span>|<span data-ttu-id="7d20f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d20f-130">Type</span></span>|<span data-ttu-id="7d20f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d20f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d20f-132">id</span><span class="sxs-lookup"><span data-stu-id="7d20f-132">id</span></span>|<span data-ttu-id="7d20f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d20f-133">String</span></span>|<span data-ttu-id="7d20f-134">ID da configuração da página de status de registro herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d20f-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7d20f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7d20f-135">displayName</span></span>|<span data-ttu-id="7d20f-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d20f-136">String</span></span>|<span data-ttu-id="7d20f-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d20f-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7d20f-138">description</span><span class="sxs-lookup"><span data-stu-id="7d20f-138">description</span></span>|<span data-ttu-id="7d20f-139">String</span><span class="sxs-lookup"><span data-stu-id="7d20f-139">String</span></span>|<span data-ttu-id="7d20f-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d20f-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7d20f-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="7d20f-141">priority</span></span>|<span data-ttu-id="7d20f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7d20f-142">Int32</span></span>|<span data-ttu-id="7d20f-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d20f-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7d20f-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d20f-144">createdDateTime</span></span>|<span data-ttu-id="7d20f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d20f-145">DateTimeOffset</span></span>|<span data-ttu-id="7d20f-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d20f-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7d20f-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d20f-147">lastModifiedDateTime</span></span>|<span data-ttu-id="7d20f-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d20f-148">DateTimeOffset</span></span>|<span data-ttu-id="7d20f-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d20f-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7d20f-150">versão</span><span class="sxs-lookup"><span data-stu-id="7d20f-150">version</span></span>|<span data-ttu-id="7d20f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="7d20f-151">Int32</span></span>|<span data-ttu-id="7d20f-152">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d20f-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7d20f-153">limite</span><span class="sxs-lookup"><span data-stu-id="7d20f-153">limit</span></span>|<span data-ttu-id="7d20f-154">Int32</span><span class="sxs-lookup"><span data-stu-id="7d20f-154">Int32</span></span>|<span data-ttu-id="7d20f-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7d20f-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7d20f-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d20f-156">Response</span></span>
<span data-ttu-id="7d20f-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d20f-157">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d20f-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d20f-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d20f-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d20f-159">Request</span></span>
<span data-ttu-id="7d20f-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d20f-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d20f-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d20f-161">Response</span></span>
<span data-ttu-id="7d20f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d20f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





