---
title: Atualizar deviceEnrollmentLimitConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc479345fa9083976c937ec8bf71630e2205a0c6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758028"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="dfa38-103">Atualizar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="dfa38-103">Update deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="dfa38-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfa38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dfa38-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dfa38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfa38-106">Atualizar as propriedades de um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dfa38-106">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfa38-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dfa38-107">Prerequisites</span></span>
<span data-ttu-id="dfa38-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfa38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfa38-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfa38-110">Permission type</span></span>|<span data-ttu-id="dfa38-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfa38-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfa38-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfa38-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dfa38-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfa38-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dfa38-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfa38-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfa38-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfa38-115">Not supported.</span></span>|
|<span data-ttu-id="dfa38-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfa38-116">Application</span></span>|<span data-ttu-id="dfa38-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfa38-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfa38-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfa38-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dfa38-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfa38-119">Request headers</span></span>
|<span data-ttu-id="dfa38-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dfa38-120">Header</span></span>|<span data-ttu-id="dfa38-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dfa38-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfa38-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfa38-122">Authorization</span></span>|<span data-ttu-id="dfa38-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfa38-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfa38-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dfa38-124">Accept</span></span>|<span data-ttu-id="dfa38-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dfa38-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfa38-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfa38-126">Request body</span></span>
<span data-ttu-id="dfa38-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dfa38-127">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="dfa38-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dfa38-128">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="dfa38-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dfa38-129">Property</span></span>|<span data-ttu-id="dfa38-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfa38-130">Type</span></span>|<span data-ttu-id="dfa38-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfa38-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfa38-132">id</span><span class="sxs-lookup"><span data-stu-id="dfa38-132">id</span></span>|<span data-ttu-id="dfa38-133">String</span><span class="sxs-lookup"><span data-stu-id="dfa38-133">String</span></span>|<span data-ttu-id="dfa38-134">Identificador exclusivo da conta Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfa38-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dfa38-135">displayName</span><span class="sxs-lookup"><span data-stu-id="dfa38-135">displayName</span></span>|<span data-ttu-id="dfa38-136">String</span><span class="sxs-lookup"><span data-stu-id="dfa38-136">String</span></span>|<span data-ttu-id="dfa38-137">O nome de exibição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfa38-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dfa38-138">description</span><span class="sxs-lookup"><span data-stu-id="dfa38-138">description</span></span>|<span data-ttu-id="dfa38-139">String</span><span class="sxs-lookup"><span data-stu-id="dfa38-139">String</span></span>|<span data-ttu-id="dfa38-140">A descrição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfa38-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dfa38-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="dfa38-141">priority</span></span>|<span data-ttu-id="dfa38-142">Int32</span><span class="sxs-lookup"><span data-stu-id="dfa38-142">Int32</span></span>|<span data-ttu-id="dfa38-143">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="dfa38-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="dfa38-144">Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixo.</span><span class="sxs-lookup"><span data-stu-id="dfa38-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="dfa38-145">Herdada do [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfa38-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dfa38-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dfa38-146">createdDateTime</span></span>|<span data-ttu-id="dfa38-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfa38-147">DateTimeOffset</span></span>|<span data-ttu-id="dfa38-148">Hora de data criada em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfa38-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dfa38-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dfa38-149">lastModifiedDateTime</span></span>|<span data-ttu-id="dfa38-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfa38-150">DateTimeOffset</span></span>|<span data-ttu-id="dfa38-151">Última data de modificação no UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfa38-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dfa38-152">versão</span><span class="sxs-lookup"><span data-stu-id="dfa38-152">version</span></span>|<span data-ttu-id="dfa38-153">Int32</span><span class="sxs-lookup"><span data-stu-id="dfa38-153">Int32</span></span>|<span data-ttu-id="dfa38-154">A versão da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfa38-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dfa38-155">limite</span><span class="sxs-lookup"><span data-stu-id="dfa38-155">limit</span></span>|<span data-ttu-id="dfa38-156">Int32</span><span class="sxs-lookup"><span data-stu-id="dfa38-156">Int32</span></span>|<span data-ttu-id="dfa38-157">O número máximo de dispositivos que um usuário pode registrar</span><span class="sxs-lookup"><span data-stu-id="dfa38-157">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="dfa38-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfa38-158">Response</span></span>
<span data-ttu-id="dfa38-159">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfa38-159">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfa38-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfa38-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfa38-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfa38-161">Request</span></span>
<span data-ttu-id="dfa38-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfa38-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dfa38-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfa38-163">Response</span></span>
<span data-ttu-id="dfa38-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfa38-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




