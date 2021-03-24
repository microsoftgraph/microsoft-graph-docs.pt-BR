---
title: Atualizar deviceComanagementAuthorityConfiguration
description: Atualize as propriedades de um objeto deviceComanagementAuthorityConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ab03be505736eb358e784d68ce97fd924526a9a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135086"
---
# <a name="update-devicecomanagementauthorityconfiguration"></a><span data-ttu-id="c5f0c-103">Atualizar deviceComanagementAuthorityConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5f0c-103">Update deviceComanagementAuthorityConfiguration</span></span>

<span data-ttu-id="c5f0c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5f0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5f0c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c5f0c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5f0c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5f0c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5f0c-107">Atualize as propriedades de [um objeto deviceComanagementAuthorityConfiguration.](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5f0c-107">Update the properties of a [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5f0c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5f0c-108">Prerequisites</span></span>
<span data-ttu-id="c5f0c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5f0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5f0c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5f0c-111">Permission type</span></span>|<span data-ttu-id="c5f0c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5f0c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5f0c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5f0c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5f0c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5f0c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c5f0c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5f0c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5f0c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5f0c-116">Not supported.</span></span>|
|<span data-ttu-id="c5f0c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5f0c-117">Application</span></span>|<span data-ttu-id="c5f0c-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5f0c-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5f0c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5f0c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c5f0c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5f0c-120">Request headers</span></span>
|<span data-ttu-id="c5f0c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5f0c-121">Header</span></span>|<span data-ttu-id="c5f0c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c5f0c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5f0c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5f0c-123">Authorization</span></span>|<span data-ttu-id="c5f0c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5f0c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5f0c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c5f0c-125">Accept</span></span>|<span data-ttu-id="c5f0c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5f0c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5f0c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5f0c-127">Request body</span></span>
<span data-ttu-id="c5f0c-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceComanagementAuthorityConfiguration.](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5f0c-128">In the request body, supply a JSON representation for the [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object.</span></span>

<span data-ttu-id="c5f0c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5f0c-129">The following table shows the properties that are required when you create the [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md).</span></span>

|<span data-ttu-id="c5f0c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5f0c-130">Property</span></span>|<span data-ttu-id="c5f0c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5f0c-131">Type</span></span>|<span data-ttu-id="c5f0c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5f0c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5f0c-133">id</span><span class="sxs-lookup"><span data-stu-id="c5f0c-133">id</span></span>|<span data-ttu-id="c5f0c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5f0c-134">String</span></span>|<span data-ttu-id="c5f0c-135">Identificador exclusivo da conta Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5f0c-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c5f0c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c5f0c-136">displayName</span></span>|<span data-ttu-id="c5f0c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5f0c-137">String</span></span>|<span data-ttu-id="c5f0c-138">O nome de exibição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5f0c-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c5f0c-139">descrição</span><span class="sxs-lookup"><span data-stu-id="c5f0c-139">description</span></span>|<span data-ttu-id="c5f0c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5f0c-140">String</span></span>|<span data-ttu-id="c5f0c-141">A descrição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5f0c-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c5f0c-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="c5f0c-142">priority</span></span>|<span data-ttu-id="c5f0c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c5f0c-143">Int32</span></span>|<span data-ttu-id="c5f0c-144">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="c5f0c-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="c5f0c-145">Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixo.</span><span class="sxs-lookup"><span data-stu-id="c5f0c-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="c5f0c-146">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5f0c-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c5f0c-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5f0c-147">createdDateTime</span></span>|<span data-ttu-id="c5f0c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5f0c-148">DateTimeOffset</span></span>|<span data-ttu-id="c5f0c-149">Hora de data criada em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5f0c-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c5f0c-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5f0c-150">lastModifiedDateTime</span></span>|<span data-ttu-id="c5f0c-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5f0c-151">DateTimeOffset</span></span>|<span data-ttu-id="c5f0c-152">Última data de modificação no UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5f0c-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c5f0c-153">versão</span><span class="sxs-lookup"><span data-stu-id="c5f0c-153">version</span></span>|<span data-ttu-id="c5f0c-154">Int32</span><span class="sxs-lookup"><span data-stu-id="c5f0c-154">Int32</span></span>|<span data-ttu-id="c5f0c-155">A versão da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5f0c-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c5f0c-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c5f0c-156">roleScopeTagIds</span></span>|<span data-ttu-id="c5f0c-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5f0c-157">String collection</span></span>|<span data-ttu-id="c5f0c-158">Marcas de escopo de função opcionais para as restrições de registro.</span><span class="sxs-lookup"><span data-stu-id="c5f0c-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="c5f0c-159">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5f0c-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c5f0c-160">managedDeviceAuthority</span><span class="sxs-lookup"><span data-stu-id="c5f0c-160">managedDeviceAuthority</span></span>|<span data-ttu-id="c5f0c-161">Int32</span><span class="sxs-lookup"><span data-stu-id="c5f0c-161">Int32</span></span>|<span data-ttu-id="c5f0c-162">Configuração da Autoridade de CoManagement ManagedDeviceAuthority</span><span class="sxs-lookup"><span data-stu-id="c5f0c-162">CoManagement Authority configuration ManagedDeviceAuthority</span></span>|
|<span data-ttu-id="c5f0c-163">installConfigurationManagerAgent</span><span class="sxs-lookup"><span data-stu-id="c5f0c-163">installConfigurationManagerAgent</span></span>|<span data-ttu-id="c5f0c-164">Booleano</span><span class="sxs-lookup"><span data-stu-id="c5f0c-164">Boolean</span></span>|<span data-ttu-id="c5f0c-165">Configuração da Autoridade de Gerenciamento de CoManagement InstallConfigurationManagerAgent</span><span class="sxs-lookup"><span data-stu-id="c5f0c-165">CoManagement Authority configuration InstallConfigurationManagerAgent</span></span>|
|<span data-ttu-id="c5f0c-166">configurationManagerAgentCommandLineArgument</span><span class="sxs-lookup"><span data-stu-id="c5f0c-166">configurationManagerAgentCommandLineArgument</span></span>|<span data-ttu-id="c5f0c-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5f0c-167">String</span></span>|<span data-ttu-id="c5f0c-168">Configuração da Autoridade de CoManagement ConfigurationManagerAgentCommandLineArgument</span><span class="sxs-lookup"><span data-stu-id="c5f0c-168">CoManagement Authority configuration ConfigurationManagerAgentCommandLineArgument</span></span>|



## <a name="response"></a><span data-ttu-id="c5f0c-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5f0c-169">Response</span></span>
<span data-ttu-id="c5f0c-170">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5f0c-170">If successful, this method returns a `200 OK` response code and an updated [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5f0c-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5f0c-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5f0c-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5f0c-172">Request</span></span>
<span data-ttu-id="c5f0c-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5f0c-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="c5f0c-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5f0c-174">Response</span></span>
<span data-ttu-id="c5f0c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5f0c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




