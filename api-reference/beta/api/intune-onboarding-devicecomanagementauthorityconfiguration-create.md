---
title: Criar deviceComanagementAuthorityConfiguration
description: Criar um novo objeto deviceComanagementAuthorityConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 124a60eb471028389546fe41d4a891a6487a5d2f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301454"
---
# <a name="create-devicecomanagementauthorityconfiguration"></a><span data-ttu-id="c0358-103">Criar deviceComanagementAuthorityConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0358-103">Create deviceComanagementAuthorityConfiguration</span></span>

<span data-ttu-id="c0358-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0358-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0358-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0358-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0358-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0358-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0358-107">Criar um novo objeto [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c0358-107">Create a new [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0358-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0358-108">Prerequisites</span></span>
<span data-ttu-id="c0358-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0358-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0358-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0358-111">Permission type</span></span>|<span data-ttu-id="c0358-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c0358-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0358-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0358-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0358-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0358-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c0358-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0358-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0358-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0358-116">Not supported.</span></span>|
|<span data-ttu-id="c0358-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0358-117">Application</span></span>|<span data-ttu-id="c0358-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0358-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0358-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0358-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c0358-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0358-120">Request headers</span></span>
|<span data-ttu-id="c0358-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0358-121">Header</span></span>|<span data-ttu-id="c0358-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c0358-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0358-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0358-123">Authorization</span></span>|<span data-ttu-id="c0358-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0358-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0358-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c0358-125">Accept</span></span>|<span data-ttu-id="c0358-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0358-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0358-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0358-127">Request body</span></span>
<span data-ttu-id="c0358-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceComanagementAuthorityConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c0358-128">In the request body, supply a JSON representation for the deviceComanagementAuthorityConfiguration object.</span></span>

<span data-ttu-id="c0358-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComanagementAuthorityConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c0358-129">The following table shows the properties that are required when you create the deviceComanagementAuthorityConfiguration.</span></span>

|<span data-ttu-id="c0358-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0358-130">Property</span></span>|<span data-ttu-id="c0358-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0358-131">Type</span></span>|<span data-ttu-id="c0358-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0358-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0358-133">id</span><span class="sxs-lookup"><span data-stu-id="c0358-133">id</span></span>|<span data-ttu-id="c0358-134">String</span><span class="sxs-lookup"><span data-stu-id="c0358-134">String</span></span>|<span data-ttu-id="c0358-135">Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0358-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c0358-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c0358-136">displayName</span></span>|<span data-ttu-id="c0358-137">String</span><span class="sxs-lookup"><span data-stu-id="c0358-137">String</span></span>|<span data-ttu-id="c0358-138">O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0358-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c0358-139">description</span><span class="sxs-lookup"><span data-stu-id="c0358-139">description</span></span>|<span data-ttu-id="c0358-140">String</span><span class="sxs-lookup"><span data-stu-id="c0358-140">String</span></span>|<span data-ttu-id="c0358-141">A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0358-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c0358-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="c0358-142">priority</span></span>|<span data-ttu-id="c0358-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c0358-143">Int32</span></span>|<span data-ttu-id="c0358-144">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="c0358-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="c0358-145">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="c0358-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="c0358-146">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0358-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c0358-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0358-147">createdDateTime</span></span>|<span data-ttu-id="c0358-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0358-148">DateTimeOffset</span></span>|<span data-ttu-id="c0358-149">Data e hora de criação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0358-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c0358-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0358-150">lastModifiedDateTime</span></span>|<span data-ttu-id="c0358-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0358-151">DateTimeOffset</span></span>|<span data-ttu-id="c0358-152">Data e hora da última modificação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0358-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c0358-153">versão</span><span class="sxs-lookup"><span data-stu-id="c0358-153">version</span></span>|<span data-ttu-id="c0358-154">Int32</span><span class="sxs-lookup"><span data-stu-id="c0358-154">Int32</span></span>|<span data-ttu-id="c0358-155">A versão da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0358-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c0358-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c0358-156">roleScopeTagIds</span></span>|<span data-ttu-id="c0358-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0358-157">String collection</span></span>|<span data-ttu-id="c0358-158">Marcas de escopo de função opcional para as restrições de registro.</span><span class="sxs-lookup"><span data-stu-id="c0358-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="c0358-159">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0358-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c0358-160">managedDeviceAuthority</span><span class="sxs-lookup"><span data-stu-id="c0358-160">managedDeviceAuthority</span></span>|<span data-ttu-id="c0358-161">Int32</span><span class="sxs-lookup"><span data-stu-id="c0358-161">Int32</span></span>|<span data-ttu-id="c0358-162">ManagedDeviceAuthority de configuração de autoridade de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="c0358-162">CoManagement Authority configuration ManagedDeviceAuthority</span></span>|
|<span data-ttu-id="c0358-163">installConfigurationManagerAgent</span><span class="sxs-lookup"><span data-stu-id="c0358-163">installConfigurationManagerAgent</span></span>|<span data-ttu-id="c0358-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="c0358-164">Boolean</span></span>|<span data-ttu-id="c0358-165">InstallConfigurationManagerAgent de configuração de autoridade de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="c0358-165">CoManagement Authority configuration InstallConfigurationManagerAgent</span></span>|
|<span data-ttu-id="c0358-166">configurationManagerAgentCommandLineArgument</span><span class="sxs-lookup"><span data-stu-id="c0358-166">configurationManagerAgentCommandLineArgument</span></span>|<span data-ttu-id="c0358-167">String</span><span class="sxs-lookup"><span data-stu-id="c0358-167">String</span></span>|<span data-ttu-id="c0358-168">ConfigurationManagerAgentCommandLineArgument de configuração de autoridade de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="c0358-168">CoManagement Authority configuration ConfigurationManagerAgentCommandLineArgument</span></span>|



## <a name="response"></a><span data-ttu-id="c0358-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0358-169">Response</span></span>
<span data-ttu-id="c0358-170">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0358-170">If successful, this method returns a `201 Created` response code and a [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0358-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0358-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0358-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0358-172">Request</span></span>
<span data-ttu-id="c0358-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0358-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.deviceComanagementAuthorityConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "managedDeviceAuthority": 6,
  "installConfigurationManagerAgent": true,
  "configurationManagerAgentCommandLineArgument": "Configuration Manager Agent Command Line Argument value"
}
```

### <a name="response"></a><span data-ttu-id="c0358-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0358-174">Response</span></span>
<span data-ttu-id="c0358-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0358-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 617

{
  "@odata.type": "#microsoft.graph.deviceComanagementAuthorityConfiguration",
  "id": "0ba0057f-057f-0ba0-7f05-a00b7f05a00b",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "managedDeviceAuthority": 6,
  "installConfigurationManagerAgent": true,
  "configurationManagerAgentCommandLineArgument": "Configuration Manager Agent Command Line Argument value"
}
```




