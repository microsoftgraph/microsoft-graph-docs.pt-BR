---
title: Criar deviceComanagementAuthorityConfiguration
description: Crie um novo objeto deviceComanagementAuthorityConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 726113e94e51bb2eb0dc9b996f87d9a070a3bf6b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135142"
---
# <a name="create-devicecomanagementauthorityconfiguration"></a><span data-ttu-id="cb3be-103">Criar deviceComanagementAuthorityConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb3be-103">Create deviceComanagementAuthorityConfiguration</span></span>

<span data-ttu-id="cb3be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb3be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb3be-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cb3be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb3be-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb3be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb3be-107">Crie um novo [objeto deviceComanagementAuthorityConfiguration.](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb3be-107">Create a new [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb3be-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cb3be-108">Prerequisites</span></span>
<span data-ttu-id="cb3be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb3be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb3be-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb3be-111">Permission type</span></span>|<span data-ttu-id="cb3be-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb3be-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb3be-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb3be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb3be-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb3be-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cb3be-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb3be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb3be-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb3be-116">Not supported.</span></span>|
|<span data-ttu-id="cb3be-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb3be-117">Application</span></span>|<span data-ttu-id="cb3be-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb3be-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb3be-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb3be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cb3be-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb3be-120">Request headers</span></span>
|<span data-ttu-id="cb3be-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb3be-121">Header</span></span>|<span data-ttu-id="cb3be-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cb3be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb3be-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb3be-123">Authorization</span></span>|<span data-ttu-id="cb3be-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb3be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb3be-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cb3be-125">Accept</span></span>|<span data-ttu-id="cb3be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb3be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb3be-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb3be-127">Request body</span></span>
<span data-ttu-id="cb3be-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceComanagementAuthorityConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cb3be-128">In the request body, supply a JSON representation for the deviceComanagementAuthorityConfiguration object.</span></span>

<span data-ttu-id="cb3be-129">A tabela a seguir mostra as propriedades necessárias ao criar deviceComanagementAuthorityConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cb3be-129">The following table shows the properties that are required when you create the deviceComanagementAuthorityConfiguration.</span></span>

|<span data-ttu-id="cb3be-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb3be-130">Property</span></span>|<span data-ttu-id="cb3be-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb3be-131">Type</span></span>|<span data-ttu-id="cb3be-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb3be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb3be-133">id</span><span class="sxs-lookup"><span data-stu-id="cb3be-133">id</span></span>|<span data-ttu-id="cb3be-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb3be-134">String</span></span>|<span data-ttu-id="cb3be-135">Identificador exclusivo da conta Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb3be-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cb3be-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cb3be-136">displayName</span></span>|<span data-ttu-id="cb3be-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb3be-137">String</span></span>|<span data-ttu-id="cb3be-138">O nome de exibição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb3be-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cb3be-139">descrição</span><span class="sxs-lookup"><span data-stu-id="cb3be-139">description</span></span>|<span data-ttu-id="cb3be-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb3be-140">String</span></span>|<span data-ttu-id="cb3be-141">A descrição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb3be-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cb3be-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="cb3be-142">priority</span></span>|<span data-ttu-id="cb3be-143">Int32</span><span class="sxs-lookup"><span data-stu-id="cb3be-143">Int32</span></span>|<span data-ttu-id="cb3be-144">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="cb3be-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="cb3be-145">Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixo.</span><span class="sxs-lookup"><span data-stu-id="cb3be-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="cb3be-146">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb3be-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cb3be-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb3be-147">createdDateTime</span></span>|<span data-ttu-id="cb3be-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb3be-148">DateTimeOffset</span></span>|<span data-ttu-id="cb3be-149">Hora de data criada em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb3be-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cb3be-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb3be-150">lastModifiedDateTime</span></span>|<span data-ttu-id="cb3be-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb3be-151">DateTimeOffset</span></span>|<span data-ttu-id="cb3be-152">Última data de modificação no UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb3be-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cb3be-153">versão</span><span class="sxs-lookup"><span data-stu-id="cb3be-153">version</span></span>|<span data-ttu-id="cb3be-154">Int32</span><span class="sxs-lookup"><span data-stu-id="cb3be-154">Int32</span></span>|<span data-ttu-id="cb3be-155">A versão da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb3be-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cb3be-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cb3be-156">roleScopeTagIds</span></span>|<span data-ttu-id="cb3be-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb3be-157">String collection</span></span>|<span data-ttu-id="cb3be-158">Marcas de escopo de função opcionais para as restrições de registro.</span><span class="sxs-lookup"><span data-stu-id="cb3be-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="cb3be-159">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb3be-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cb3be-160">managedDeviceAuthority</span><span class="sxs-lookup"><span data-stu-id="cb3be-160">managedDeviceAuthority</span></span>|<span data-ttu-id="cb3be-161">Int32</span><span class="sxs-lookup"><span data-stu-id="cb3be-161">Int32</span></span>|<span data-ttu-id="cb3be-162">Configuração da Autoridade de CoManagement ManagedDeviceAuthority</span><span class="sxs-lookup"><span data-stu-id="cb3be-162">CoManagement Authority configuration ManagedDeviceAuthority</span></span>|
|<span data-ttu-id="cb3be-163">installConfigurationManagerAgent</span><span class="sxs-lookup"><span data-stu-id="cb3be-163">installConfigurationManagerAgent</span></span>|<span data-ttu-id="cb3be-164">Booleano</span><span class="sxs-lookup"><span data-stu-id="cb3be-164">Boolean</span></span>|<span data-ttu-id="cb3be-165">Configuração da Autoridade de Gerenciamento de CoManagement InstallConfigurationManagerAgent</span><span class="sxs-lookup"><span data-stu-id="cb3be-165">CoManagement Authority configuration InstallConfigurationManagerAgent</span></span>|
|<span data-ttu-id="cb3be-166">configurationManagerAgentCommandLineArgument</span><span class="sxs-lookup"><span data-stu-id="cb3be-166">configurationManagerAgentCommandLineArgument</span></span>|<span data-ttu-id="cb3be-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb3be-167">String</span></span>|<span data-ttu-id="cb3be-168">Configuração da Autoridade de CoManagement ConfigurationManagerAgentCommandLineArgument</span><span class="sxs-lookup"><span data-stu-id="cb3be-168">CoManagement Authority configuration ConfigurationManagerAgentCommandLineArgument</span></span>|



## <a name="response"></a><span data-ttu-id="cb3be-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb3be-169">Response</span></span>
<span data-ttu-id="cb3be-170">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb3be-170">If successful, this method returns a `201 Created` response code and a [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb3be-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb3be-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb3be-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb3be-172">Request</span></span>
<span data-ttu-id="cb3be-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb3be-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cb3be-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb3be-174">Response</span></span>
<span data-ttu-id="cb3be-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb3be-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




