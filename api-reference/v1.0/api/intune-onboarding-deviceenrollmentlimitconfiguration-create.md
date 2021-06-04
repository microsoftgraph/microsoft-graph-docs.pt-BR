---
title: Criar deviceEnrollmentLimitConfiguration
description: Criar um novo objeto deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f3be4bb3cebe2e8dd08bff5764143d231680dfb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52745069"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="f8bea-103">Criar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8bea-103">Create deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="f8bea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8bea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8bea-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8bea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8bea-106">Criar um novo objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8bea-106">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8bea-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8bea-107">Prerequisites</span></span>
<span data-ttu-id="f8bea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8bea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8bea-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8bea-110">Permission type</span></span>|<span data-ttu-id="f8bea-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8bea-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8bea-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8bea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8bea-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8bea-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f8bea-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8bea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8bea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8bea-115">Not supported.</span></span>|
|<span data-ttu-id="f8bea-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8bea-116">Application</span></span>|<span data-ttu-id="f8bea-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8bea-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8bea-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8bea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f8bea-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8bea-119">Request headers</span></span>
|<span data-ttu-id="f8bea-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8bea-120">Header</span></span>|<span data-ttu-id="f8bea-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f8bea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8bea-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8bea-122">Authorization</span></span>|<span data-ttu-id="f8bea-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8bea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8bea-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8bea-124">Accept</span></span>|<span data-ttu-id="f8bea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8bea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8bea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8bea-126">Request body</span></span>
<span data-ttu-id="f8bea-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f8bea-127">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="f8bea-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f8bea-128">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="f8bea-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8bea-129">Property</span></span>|<span data-ttu-id="f8bea-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8bea-130">Type</span></span>|<span data-ttu-id="f8bea-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8bea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8bea-132">id</span><span class="sxs-lookup"><span data-stu-id="f8bea-132">id</span></span>|<span data-ttu-id="f8bea-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bea-133">String</span></span>|<span data-ttu-id="f8bea-134">Identificador exclusivo da conta Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8bea-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f8bea-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f8bea-135">displayName</span></span>|<span data-ttu-id="f8bea-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bea-136">String</span></span>|<span data-ttu-id="f8bea-137">O nome de exibição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8bea-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f8bea-138">descrição</span><span class="sxs-lookup"><span data-stu-id="f8bea-138">description</span></span>|<span data-ttu-id="f8bea-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8bea-139">String</span></span>|<span data-ttu-id="f8bea-140">A descrição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8bea-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f8bea-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="f8bea-141">priority</span></span>|<span data-ttu-id="f8bea-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f8bea-142">Int32</span></span>|<span data-ttu-id="f8bea-143">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="f8bea-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="f8bea-144">Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixo.</span><span class="sxs-lookup"><span data-stu-id="f8bea-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="f8bea-145">Herdada do [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8bea-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f8bea-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8bea-146">createdDateTime</span></span>|<span data-ttu-id="f8bea-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8bea-147">DateTimeOffset</span></span>|<span data-ttu-id="f8bea-148">Hora de data criada em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8bea-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f8bea-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8bea-149">lastModifiedDateTime</span></span>|<span data-ttu-id="f8bea-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8bea-150">DateTimeOffset</span></span>|<span data-ttu-id="f8bea-151">Última data de modificação no UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8bea-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f8bea-152">versão</span><span class="sxs-lookup"><span data-stu-id="f8bea-152">version</span></span>|<span data-ttu-id="f8bea-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f8bea-153">Int32</span></span>|<span data-ttu-id="f8bea-154">A versão da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8bea-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f8bea-155">limite</span><span class="sxs-lookup"><span data-stu-id="f8bea-155">limit</span></span>|<span data-ttu-id="f8bea-156">Int32</span><span class="sxs-lookup"><span data-stu-id="f8bea-156">Int32</span></span>|<span data-ttu-id="f8bea-157">O número máximo de dispositivos que um usuário pode registrar</span><span class="sxs-lookup"><span data-stu-id="f8bea-157">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="f8bea-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8bea-158">Response</span></span>
<span data-ttu-id="f8bea-159">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8bea-159">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8bea-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8bea-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8bea-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8bea-161">Request</span></span>
<span data-ttu-id="f8bea-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8bea-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f8bea-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8bea-163">Response</span></span>
<span data-ttu-id="f8bea-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8bea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




