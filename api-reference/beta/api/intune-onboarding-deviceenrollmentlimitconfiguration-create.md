---
title: Criar deviceEnrollmentLimitConfiguration
description: Criar um novo objeto deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7509be622b9e89ba35d65730018b8158a3444d6b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135079"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="0c595-103">Criar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c595-103">Create deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="0c595-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c595-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c595-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0c595-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c595-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c595-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c595-107">Criar um novo objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c595-107">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c595-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c595-108">Prerequisites</span></span>
<span data-ttu-id="0c595-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c595-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c595-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c595-111">Permission type</span></span>|<span data-ttu-id="0c595-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c595-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c595-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c595-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c595-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c595-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0c595-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c595-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c595-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c595-116">Not supported.</span></span>|
|<span data-ttu-id="0c595-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c595-117">Application</span></span>|<span data-ttu-id="0c595-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c595-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c595-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c595-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0c595-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c595-120">Request headers</span></span>
|<span data-ttu-id="0c595-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c595-121">Header</span></span>|<span data-ttu-id="0c595-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0c595-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c595-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c595-123">Authorization</span></span>|<span data-ttu-id="0c595-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c595-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c595-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c595-125">Accept</span></span>|<span data-ttu-id="0c595-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c595-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c595-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c595-127">Request body</span></span>
<span data-ttu-id="0c595-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0c595-128">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="0c595-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0c595-129">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="0c595-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c595-130">Property</span></span>|<span data-ttu-id="0c595-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c595-131">Type</span></span>|<span data-ttu-id="0c595-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c595-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c595-133">id</span><span class="sxs-lookup"><span data-stu-id="0c595-133">id</span></span>|<span data-ttu-id="0c595-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c595-134">String</span></span>|<span data-ttu-id="0c595-135">Identificador exclusivo da conta Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c595-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0c595-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0c595-136">displayName</span></span>|<span data-ttu-id="0c595-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c595-137">String</span></span>|<span data-ttu-id="0c595-138">O nome de exibição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c595-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0c595-139">descrição</span><span class="sxs-lookup"><span data-stu-id="0c595-139">description</span></span>|<span data-ttu-id="0c595-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c595-140">String</span></span>|<span data-ttu-id="0c595-141">A descrição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c595-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0c595-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="0c595-142">priority</span></span>|<span data-ttu-id="0c595-143">Int32</span><span class="sxs-lookup"><span data-stu-id="0c595-143">Int32</span></span>|<span data-ttu-id="0c595-144">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="0c595-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="0c595-145">Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixo.</span><span class="sxs-lookup"><span data-stu-id="0c595-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="0c595-146">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c595-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0c595-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c595-147">createdDateTime</span></span>|<span data-ttu-id="0c595-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c595-148">DateTimeOffset</span></span>|<span data-ttu-id="0c595-149">Hora de data criada em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c595-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0c595-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c595-150">lastModifiedDateTime</span></span>|<span data-ttu-id="0c595-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c595-151">DateTimeOffset</span></span>|<span data-ttu-id="0c595-152">Última data de modificação no UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c595-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0c595-153">versão</span><span class="sxs-lookup"><span data-stu-id="0c595-153">version</span></span>|<span data-ttu-id="0c595-154">Int32</span><span class="sxs-lookup"><span data-stu-id="0c595-154">Int32</span></span>|<span data-ttu-id="0c595-155">A versão da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c595-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0c595-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0c595-156">roleScopeTagIds</span></span>|<span data-ttu-id="0c595-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c595-157">String collection</span></span>|<span data-ttu-id="0c595-158">Marcas de escopo de função opcionais para as restrições de registro.</span><span class="sxs-lookup"><span data-stu-id="0c595-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="0c595-159">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c595-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0c595-160">limite</span><span class="sxs-lookup"><span data-stu-id="0c595-160">limit</span></span>|<span data-ttu-id="0c595-161">Int32</span><span class="sxs-lookup"><span data-stu-id="0c595-161">Int32</span></span>|<span data-ttu-id="0c595-162">O número máximo de dispositivos que um usuário pode registrar</span><span class="sxs-lookup"><span data-stu-id="0c595-162">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="0c595-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c595-163">Response</span></span>
<span data-ttu-id="0c595-164">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c595-164">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c595-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c595-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c595-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c595-166">Request</span></span>
<span data-ttu-id="0c595-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c595-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="0c595-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c595-168">Response</span></span>
<span data-ttu-id="0c595-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c595-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




