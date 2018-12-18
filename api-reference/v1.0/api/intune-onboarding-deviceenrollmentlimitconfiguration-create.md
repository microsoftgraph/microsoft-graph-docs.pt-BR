---
title: Criar deviceEnrollmentLimitConfiguration
description: Criar um novo objeto deviceEnrollmentLimitConfiguration.
author: tfitzmac
ms.openlocfilehash: 4a3f9230b29fbe78e4a3771812bdfa435b1e2c5f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310420"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="f8ebc-103">Criar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8ebc-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="f8ebc-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f8ebc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8ebc-105">Criar um novo objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8ebc-105">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8ebc-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8ebc-106">Prerequisites</span></span>
<span data-ttu-id="f8ebc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8ebc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8ebc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8ebc-109">Permission type</span></span>|<span data-ttu-id="f8ebc-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8ebc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8ebc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8ebc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f8ebc-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8ebc-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f8ebc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8ebc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8ebc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8ebc-114">Not supported.</span></span>|
|<span data-ttu-id="f8ebc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8ebc-115">Application</span></span>|<span data-ttu-id="f8ebc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8ebc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8ebc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8ebc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f8ebc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8ebc-118">Request headers</span></span>
|<span data-ttu-id="f8ebc-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8ebc-119">Header</span></span>|<span data-ttu-id="f8ebc-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f8ebc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8ebc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8ebc-121">Authorization</span></span>|<span data-ttu-id="f8ebc-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8ebc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8ebc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f8ebc-123">Accept</span></span>|<span data-ttu-id="f8ebc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f8ebc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8ebc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8ebc-125">Request body</span></span>
<span data-ttu-id="f8ebc-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f8ebc-126">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="f8ebc-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f8ebc-127">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="f8ebc-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8ebc-128">Property</span></span>|<span data-ttu-id="f8ebc-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8ebc-129">Type</span></span>|<span data-ttu-id="f8ebc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8ebc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8ebc-131">id</span><span class="sxs-lookup"><span data-stu-id="f8ebc-131">id</span></span>|<span data-ttu-id="f8ebc-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8ebc-132">String</span></span>|<span data-ttu-id="f8ebc-133">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8ebc-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f8ebc-134">displayName</span><span class="sxs-lookup"><span data-stu-id="f8ebc-134">displayName</span></span>|<span data-ttu-id="f8ebc-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8ebc-135">String</span></span>|<span data-ttu-id="f8ebc-136">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8ebc-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f8ebc-137">description</span><span class="sxs-lookup"><span data-stu-id="f8ebc-137">description</span></span>|<span data-ttu-id="f8ebc-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8ebc-138">String</span></span>|<span data-ttu-id="f8ebc-139">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8ebc-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f8ebc-140">prioridade</span><span class="sxs-lookup"><span data-stu-id="f8ebc-140">priority</span></span>|<span data-ttu-id="f8ebc-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f8ebc-141">Int32</span></span>|<span data-ttu-id="f8ebc-142">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8ebc-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f8ebc-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8ebc-143">createdDateTime</span></span>|<span data-ttu-id="f8ebc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8ebc-144">DateTimeOffset</span></span>|<span data-ttu-id="f8ebc-145">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8ebc-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f8ebc-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8ebc-146">lastModifiedDateTime</span></span>|<span data-ttu-id="f8ebc-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8ebc-147">DateTimeOffset</span></span>|<span data-ttu-id="f8ebc-148">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8ebc-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f8ebc-149">version</span><span class="sxs-lookup"><span data-stu-id="f8ebc-149">version</span></span>|<span data-ttu-id="f8ebc-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f8ebc-150">Int32</span></span>|<span data-ttu-id="f8ebc-151">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8ebc-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f8ebc-152">limite</span><span class="sxs-lookup"><span data-stu-id="f8ebc-152">limit</span></span>|<span data-ttu-id="f8ebc-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f8ebc-153">Int32</span></span>|<span data-ttu-id="f8ebc-154">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f8ebc-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f8ebc-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8ebc-155">Response</span></span>
<span data-ttu-id="f8ebc-156">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8ebc-156">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8ebc-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8ebc-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8ebc-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8ebc-158">Request</span></span>
<span data-ttu-id="f8ebc-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8ebc-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f8ebc-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8ebc-160">Response</span></span>
<span data-ttu-id="f8ebc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8ebc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



