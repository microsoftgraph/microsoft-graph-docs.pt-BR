---
title: Criar deviceEnrollmentLimitConfiguration
description: Criar um novo objeto deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db0985a06eb6f83faa57757b84e1d1f41ba52ce9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43403454"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="49f46-103">Criar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="49f46-103">Create deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="49f46-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49f46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49f46-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49f46-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49f46-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49f46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49f46-107">Criar um novo objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49f46-107">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49f46-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49f46-108">Prerequisites</span></span>
<span data-ttu-id="49f46-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49f46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49f46-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49f46-111">Permission type</span></span>|<span data-ttu-id="49f46-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49f46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49f46-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49f46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49f46-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49f46-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="49f46-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49f46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49f46-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49f46-116">Not supported.</span></span>|
|<span data-ttu-id="49f46-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49f46-117">Application</span></span>|<span data-ttu-id="49f46-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49f46-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49f46-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49f46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="49f46-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49f46-120">Request headers</span></span>
|<span data-ttu-id="49f46-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49f46-121">Header</span></span>|<span data-ttu-id="49f46-122">Valor</span><span class="sxs-lookup"><span data-stu-id="49f46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49f46-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="49f46-123">Authorization</span></span>|<span data-ttu-id="49f46-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49f46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49f46-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49f46-125">Accept</span></span>|<span data-ttu-id="49f46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49f46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49f46-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49f46-127">Request body</span></span>
<span data-ttu-id="49f46-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="49f46-128">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="49f46-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="49f46-129">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="49f46-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49f46-130">Property</span></span>|<span data-ttu-id="49f46-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="49f46-131">Type</span></span>|<span data-ttu-id="49f46-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="49f46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49f46-133">id</span><span class="sxs-lookup"><span data-stu-id="49f46-133">id</span></span>|<span data-ttu-id="49f46-134">String</span><span class="sxs-lookup"><span data-stu-id="49f46-134">String</span></span>|<span data-ttu-id="49f46-135">Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49f46-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49f46-136">displayName</span><span class="sxs-lookup"><span data-stu-id="49f46-136">displayName</span></span>|<span data-ttu-id="49f46-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49f46-137">String</span></span>|<span data-ttu-id="49f46-138">O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49f46-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49f46-139">description</span><span class="sxs-lookup"><span data-stu-id="49f46-139">description</span></span>|<span data-ttu-id="49f46-140">String</span><span class="sxs-lookup"><span data-stu-id="49f46-140">String</span></span>|<span data-ttu-id="49f46-141">A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49f46-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49f46-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="49f46-142">priority</span></span>|<span data-ttu-id="49f46-143">Int32</span><span class="sxs-lookup"><span data-stu-id="49f46-143">Int32</span></span>|<span data-ttu-id="49f46-144">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="49f46-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="49f46-145">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="49f46-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="49f46-146">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49f46-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49f46-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49f46-147">createdDateTime</span></span>|<span data-ttu-id="49f46-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49f46-148">DateTimeOffset</span></span>|<span data-ttu-id="49f46-149">Data e hora de criação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49f46-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49f46-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49f46-150">lastModifiedDateTime</span></span>|<span data-ttu-id="49f46-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49f46-151">DateTimeOffset</span></span>|<span data-ttu-id="49f46-152">Data e hora da última modificação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49f46-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49f46-153">versão</span><span class="sxs-lookup"><span data-stu-id="49f46-153">version</span></span>|<span data-ttu-id="49f46-154">Int32</span><span class="sxs-lookup"><span data-stu-id="49f46-154">Int32</span></span>|<span data-ttu-id="49f46-155">A versão da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49f46-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49f46-156">limite</span><span class="sxs-lookup"><span data-stu-id="49f46-156">limit</span></span>|<span data-ttu-id="49f46-157">Int32</span><span class="sxs-lookup"><span data-stu-id="49f46-157">Int32</span></span>|<span data-ttu-id="49f46-158">O número máximo de dispositivos que um usuário pode registrar</span><span class="sxs-lookup"><span data-stu-id="49f46-158">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="49f46-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="49f46-159">Response</span></span>
<span data-ttu-id="49f46-160">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49f46-160">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49f46-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49f46-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="49f46-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49f46-162">Request</span></span>
<span data-ttu-id="49f46-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49f46-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="49f46-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="49f46-164">Response</span></span>
<span data-ttu-id="49f46-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49f46-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



