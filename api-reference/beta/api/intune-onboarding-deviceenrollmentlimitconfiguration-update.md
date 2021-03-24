---
title: Atualizar deviceEnrollmentLimitConfiguration
description: Atualizar as propriedades de um objeto deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ba360475199d47bda3b2c65ee6c7991bbb8fb91
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135016"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="1b8d8-103">Atualizar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="1b8d8-103">Update deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="1b8d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b8d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b8d8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b8d8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b8d8-107">Atualizar as propriedades de um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b8d8-107">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b8d8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1b8d8-108">Prerequisites</span></span>
<span data-ttu-id="1b8d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b8d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b8d8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b8d8-111">Permission type</span></span>|<span data-ttu-id="1b8d8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b8d8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b8d8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b8d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b8d8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b8d8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1b8d8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b8d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b8d8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-116">Not supported.</span></span>|
|<span data-ttu-id="1b8d8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b8d8-117">Application</span></span>|<span data-ttu-id="1b8d8-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b8d8-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b8d8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b8d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1b8d8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b8d8-120">Request headers</span></span>
|<span data-ttu-id="1b8d8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b8d8-121">Header</span></span>|<span data-ttu-id="1b8d8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1b8d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b8d8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b8d8-123">Authorization</span></span>|<span data-ttu-id="1b8d8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b8d8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1b8d8-125">Accept</span></span>|<span data-ttu-id="1b8d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b8d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b8d8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b8d8-127">Request body</span></span>
<span data-ttu-id="1b8d8-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b8d8-128">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="1b8d8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b8d8-129">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="1b8d8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b8d8-130">Property</span></span>|<span data-ttu-id="1b8d8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b8d8-131">Type</span></span>|<span data-ttu-id="1b8d8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b8d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b8d8-133">id</span><span class="sxs-lookup"><span data-stu-id="1b8d8-133">id</span></span>|<span data-ttu-id="1b8d8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b8d8-134">String</span></span>|<span data-ttu-id="1b8d8-135">Identificador exclusivo da conta Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b8d8-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b8d8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1b8d8-136">displayName</span></span>|<span data-ttu-id="1b8d8-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b8d8-137">String</span></span>|<span data-ttu-id="1b8d8-138">O nome de exibição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b8d8-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b8d8-139">descrição</span><span class="sxs-lookup"><span data-stu-id="1b8d8-139">description</span></span>|<span data-ttu-id="1b8d8-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b8d8-140">String</span></span>|<span data-ttu-id="1b8d8-141">A descrição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b8d8-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b8d8-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="1b8d8-142">priority</span></span>|<span data-ttu-id="1b8d8-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1b8d8-143">Int32</span></span>|<span data-ttu-id="1b8d8-144">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="1b8d8-145">Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixo.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="1b8d8-146">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b8d8-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b8d8-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b8d8-147">createdDateTime</span></span>|<span data-ttu-id="1b8d8-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b8d8-148">DateTimeOffset</span></span>|<span data-ttu-id="1b8d8-149">Hora de data criada em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b8d8-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b8d8-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b8d8-150">lastModifiedDateTime</span></span>|<span data-ttu-id="1b8d8-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b8d8-151">DateTimeOffset</span></span>|<span data-ttu-id="1b8d8-152">Última data de modificação no UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b8d8-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b8d8-153">versão</span><span class="sxs-lookup"><span data-stu-id="1b8d8-153">version</span></span>|<span data-ttu-id="1b8d8-154">Int32</span><span class="sxs-lookup"><span data-stu-id="1b8d8-154">Int32</span></span>|<span data-ttu-id="1b8d8-155">A versão da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b8d8-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b8d8-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1b8d8-156">roleScopeTagIds</span></span>|<span data-ttu-id="1b8d8-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b8d8-157">String collection</span></span>|<span data-ttu-id="1b8d8-158">Marcas de escopo de função opcionais para as restrições de registro.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="1b8d8-159">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b8d8-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1b8d8-160">limite</span><span class="sxs-lookup"><span data-stu-id="1b8d8-160">limit</span></span>|<span data-ttu-id="1b8d8-161">Int32</span><span class="sxs-lookup"><span data-stu-id="1b8d8-161">Int32</span></span>|<span data-ttu-id="1b8d8-162">O número máximo de dispositivos que um usuário pode registrar</span><span class="sxs-lookup"><span data-stu-id="1b8d8-162">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="1b8d8-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b8d8-163">Response</span></span>
<span data-ttu-id="1b8d8-164">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-164">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b8d8-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b8d8-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b8d8-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b8d8-166">Request</span></span>
<span data-ttu-id="1b8d8-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 267

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="1b8d8-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b8d8-168">Response</span></span>
<span data-ttu-id="1b8d8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b8d8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "limit": 5
}
```




