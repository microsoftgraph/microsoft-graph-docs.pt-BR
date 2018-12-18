---
title: Criar deviceEnrollmentLimitConfiguration
description: Criar um novo objeto deviceEnrollmentLimitConfiguration.
author: tfitzmac
ms.openlocfilehash: fdb9fee09f43890280ef0beb79d6d57d9def67f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359665"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="1888d-103">Criar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="1888d-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="1888d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1888d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1888d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1888d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1888d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1888d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1888d-107">Criar um novo objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1888d-107">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1888d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1888d-108">Prerequisites</span></span>
<span data-ttu-id="1888d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1888d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1888d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1888d-111">Permission type</span></span>|<span data-ttu-id="1888d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1888d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1888d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1888d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1888d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1888d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1888d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1888d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1888d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1888d-116">Not supported.</span></span>|
|<span data-ttu-id="1888d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1888d-117">Application</span></span>|<span data-ttu-id="1888d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1888d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1888d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1888d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1888d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1888d-120">Request headers</span></span>
|<span data-ttu-id="1888d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1888d-121">Header</span></span>|<span data-ttu-id="1888d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1888d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1888d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1888d-123">Authorization</span></span>|<span data-ttu-id="1888d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1888d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1888d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1888d-125">Accept</span></span>|<span data-ttu-id="1888d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1888d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1888d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1888d-127">Request body</span></span>
<span data-ttu-id="1888d-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1888d-128">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="1888d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1888d-129">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="1888d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1888d-130">Property</span></span>|<span data-ttu-id="1888d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1888d-131">Type</span></span>|<span data-ttu-id="1888d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1888d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1888d-133">id</span><span class="sxs-lookup"><span data-stu-id="1888d-133">id</span></span>|<span data-ttu-id="1888d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1888d-134">String</span></span>|<span data-ttu-id="1888d-135">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1888d-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1888d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1888d-136">displayName</span></span>|<span data-ttu-id="1888d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1888d-137">String</span></span>|<span data-ttu-id="1888d-138">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1888d-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1888d-139">description</span><span class="sxs-lookup"><span data-stu-id="1888d-139">description</span></span>|<span data-ttu-id="1888d-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1888d-140">String</span></span>|<span data-ttu-id="1888d-141">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1888d-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1888d-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="1888d-142">priority</span></span>|<span data-ttu-id="1888d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1888d-143">Int32</span></span>|<span data-ttu-id="1888d-144">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1888d-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1888d-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1888d-145">createdDateTime</span></span>|<span data-ttu-id="1888d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1888d-146">DateTimeOffset</span></span>|<span data-ttu-id="1888d-147">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1888d-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1888d-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1888d-148">lastModifiedDateTime</span></span>|<span data-ttu-id="1888d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1888d-149">DateTimeOffset</span></span>|<span data-ttu-id="1888d-150">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1888d-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1888d-151">version</span><span class="sxs-lookup"><span data-stu-id="1888d-151">version</span></span>|<span data-ttu-id="1888d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1888d-152">Int32</span></span>|<span data-ttu-id="1888d-153">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1888d-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1888d-154">limite</span><span class="sxs-lookup"><span data-stu-id="1888d-154">limit</span></span>|<span data-ttu-id="1888d-155">Int32</span><span class="sxs-lookup"><span data-stu-id="1888d-155">Int32</span></span>|<span data-ttu-id="1888d-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1888d-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1888d-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="1888d-157">Response</span></span>
<span data-ttu-id="1888d-158">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1888d-158">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1888d-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1888d-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="1888d-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1888d-160">Request</span></span>
<span data-ttu-id="1888d-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1888d-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 269

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="1888d-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="1888d-162">Response</span></span>
<span data-ttu-id="1888d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1888d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





