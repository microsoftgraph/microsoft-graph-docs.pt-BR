---
title: Atualizar deviceEnrollmentLimitConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentLimitConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c0010d5bdba68cd1ac94aa8c474dedc9213a585
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352970"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="c5908-103">Atualizar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5908-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="c5908-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c5908-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5908-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5908-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5908-106">Atualizar as propriedades de um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5908-106">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5908-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5908-107">Prerequisites</span></span>
<span data-ttu-id="c5908-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5908-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5908-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5908-110">Permission type</span></span>|<span data-ttu-id="c5908-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c5908-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5908-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5908-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5908-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5908-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c5908-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5908-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5908-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5908-115">Not supported.</span></span>|
|<span data-ttu-id="c5908-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5908-116">Application</span></span>|<span data-ttu-id="c5908-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5908-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5908-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5908-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c5908-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5908-119">Request headers</span></span>
|<span data-ttu-id="c5908-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5908-120">Header</span></span>|<span data-ttu-id="c5908-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c5908-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5908-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5908-122">Authorization</span></span>|<span data-ttu-id="c5908-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5908-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5908-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c5908-124">Accept</span></span>|<span data-ttu-id="c5908-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5908-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5908-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5908-126">Request body</span></span>
<span data-ttu-id="c5908-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5908-127">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="c5908-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5908-128">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="c5908-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5908-129">Property</span></span>|<span data-ttu-id="c5908-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5908-130">Type</span></span>|<span data-ttu-id="c5908-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5908-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5908-132">id</span><span class="sxs-lookup"><span data-stu-id="c5908-132">id</span></span>|<span data-ttu-id="c5908-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5908-133">String</span></span>|<span data-ttu-id="c5908-134">Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5908-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c5908-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c5908-135">displayName</span></span>|<span data-ttu-id="c5908-136">String</span><span class="sxs-lookup"><span data-stu-id="c5908-136">String</span></span>|<span data-ttu-id="c5908-137">O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5908-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c5908-138">descrição</span><span class="sxs-lookup"><span data-stu-id="c5908-138">description</span></span>|<span data-ttu-id="c5908-139">String</span><span class="sxs-lookup"><span data-stu-id="c5908-139">String</span></span>|<span data-ttu-id="c5908-140">A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5908-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c5908-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="c5908-141">priority</span></span>|<span data-ttu-id="c5908-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c5908-142">Int32</span></span>|<span data-ttu-id="c5908-143">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="c5908-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="c5908-144">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="c5908-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="c5908-145">Herdada do [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5908-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c5908-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5908-146">createdDateTime</span></span>|<span data-ttu-id="c5908-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5908-147">DateTimeOffset</span></span>|<span data-ttu-id="c5908-148">Data e hora de criação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5908-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c5908-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5908-149">lastModifiedDateTime</span></span>|<span data-ttu-id="c5908-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5908-150">DateTimeOffset</span></span>|<span data-ttu-id="c5908-151">Data e hora da última modificação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5908-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c5908-152">versão</span><span class="sxs-lookup"><span data-stu-id="c5908-152">version</span></span>|<span data-ttu-id="c5908-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c5908-153">Int32</span></span>|<span data-ttu-id="c5908-154">A versão da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5908-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c5908-155">limite</span><span class="sxs-lookup"><span data-stu-id="c5908-155">limit</span></span>|<span data-ttu-id="c5908-156">Int32</span><span class="sxs-lookup"><span data-stu-id="c5908-156">Int32</span></span>|<span data-ttu-id="c5908-157">O número máximo de dispositivos que um usuário pode registrar</span><span class="sxs-lookup"><span data-stu-id="c5908-157">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="c5908-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5908-158">Response</span></span>
<span data-ttu-id="c5908-159">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5908-159">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5908-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5908-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5908-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5908-161">Request</span></span>
<span data-ttu-id="c5908-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5908-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c5908-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5908-163">Response</span></span>
<span data-ttu-id="c5908-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5908-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






