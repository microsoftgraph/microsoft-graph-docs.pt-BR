---
title: Criar deviceEnrollmentLimitConfiguration
description: Criar um novo objeto deviceEnrollmentLimitConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 858370c77eba655cd0c5a90328396dc6ae40d8ad
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536137"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="ece21-103">Criar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="ece21-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="ece21-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ece21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ece21-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ece21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ece21-106">Criar um novo objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ece21-106">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ece21-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ece21-107">Prerequisites</span></span>
<span data-ttu-id="ece21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ece21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ece21-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ece21-110">Permission type</span></span>|<span data-ttu-id="ece21-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ece21-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ece21-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ece21-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ece21-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ece21-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ece21-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ece21-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ece21-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ece21-115">Not supported.</span></span>|
|<span data-ttu-id="ece21-116">Application</span><span class="sxs-lookup"><span data-stu-id="ece21-116">Application</span></span>|<span data-ttu-id="ece21-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ece21-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ece21-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ece21-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ece21-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ece21-119">Request headers</span></span>
|<span data-ttu-id="ece21-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ece21-120">Header</span></span>|<span data-ttu-id="ece21-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ece21-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ece21-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ece21-122">Authorization</span></span>|<span data-ttu-id="ece21-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ece21-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ece21-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ece21-124">Accept</span></span>|<span data-ttu-id="ece21-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ece21-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ece21-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ece21-126">Request body</span></span>
<span data-ttu-id="ece21-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ece21-127">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="ece21-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ece21-128">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="ece21-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ece21-129">Property</span></span>|<span data-ttu-id="ece21-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ece21-130">Type</span></span>|<span data-ttu-id="ece21-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ece21-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ece21-132">id</span><span class="sxs-lookup"><span data-stu-id="ece21-132">id</span></span>|<span data-ttu-id="ece21-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ece21-133">String</span></span>|<span data-ttu-id="ece21-134">Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ece21-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ece21-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ece21-135">displayName</span></span>|<span data-ttu-id="ece21-136">String</span><span class="sxs-lookup"><span data-stu-id="ece21-136">String</span></span>|<span data-ttu-id="ece21-137">O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ece21-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ece21-138">description</span><span class="sxs-lookup"><span data-stu-id="ece21-138">description</span></span>|<span data-ttu-id="ece21-139">String</span><span class="sxs-lookup"><span data-stu-id="ece21-139">String</span></span>|<span data-ttu-id="ece21-140">A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ece21-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ece21-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="ece21-141">priority</span></span>|<span data-ttu-id="ece21-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ece21-142">Int32</span></span>|<span data-ttu-id="ece21-143">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="ece21-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="ece21-144">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="ece21-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="ece21-145">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ece21-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ece21-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ece21-146">createdDateTime</span></span>|<span data-ttu-id="ece21-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ece21-147">DateTimeOffset</span></span>|<span data-ttu-id="ece21-148">Data e hora de criação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ece21-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ece21-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ece21-149">lastModifiedDateTime</span></span>|<span data-ttu-id="ece21-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ece21-150">DateTimeOffset</span></span>|<span data-ttu-id="ece21-151">Data e hora da última modificação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ece21-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ece21-152">versão</span><span class="sxs-lookup"><span data-stu-id="ece21-152">version</span></span>|<span data-ttu-id="ece21-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ece21-153">Int32</span></span>|<span data-ttu-id="ece21-154">A versão da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ece21-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ece21-155">limite</span><span class="sxs-lookup"><span data-stu-id="ece21-155">limit</span></span>|<span data-ttu-id="ece21-156">Int32</span><span class="sxs-lookup"><span data-stu-id="ece21-156">Int32</span></span>|<span data-ttu-id="ece21-157">O número máximo de dispositivos que um usuário pode registrar</span><span class="sxs-lookup"><span data-stu-id="ece21-157">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="ece21-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="ece21-158">Response</span></span>
<span data-ttu-id="ece21-159">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ece21-159">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ece21-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ece21-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="ece21-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ece21-161">Request</span></span>
<span data-ttu-id="ece21-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ece21-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ece21-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="ece21-163">Response</span></span>
<span data-ttu-id="ece21-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ece21-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






