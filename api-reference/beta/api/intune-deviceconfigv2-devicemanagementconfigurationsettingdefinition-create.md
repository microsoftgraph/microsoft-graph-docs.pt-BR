---
title: Criar deviceManagementConfigurationSettingDefinition
description: Criar um novo objeto deviceManagementConfigurationSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f16ae5a778df7d0398a137f86cda6dfcb3dbdb6d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241357"
---
# <a name="create-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="2ee56-103">Criar deviceManagementConfigurationSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="2ee56-103">Create deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="2ee56-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ee56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ee56-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ee56-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ee56-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ee56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ee56-107">Criar um novo objeto [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="2ee56-107">Create a new [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ee56-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ee56-108">Prerequisites</span></span>
<span data-ttu-id="2ee56-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ee56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ee56-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ee56-111">Permission type</span></span>|<span data-ttu-id="2ee56-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ee56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ee56-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ee56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ee56-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ee56-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2ee56-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ee56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ee56-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ee56-116">Not supported.</span></span>|
|<span data-ttu-id="2ee56-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ee56-117">Application</span></span>|<span data-ttu-id="2ee56-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ee56-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ee56-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ee56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="2ee56-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ee56-120">Request headers</span></span>
|<span data-ttu-id="2ee56-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ee56-121">Header</span></span>|<span data-ttu-id="2ee56-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2ee56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ee56-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ee56-123">Authorization</span></span>|<span data-ttu-id="2ee56-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ee56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ee56-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ee56-125">Accept</span></span>|<span data-ttu-id="2ee56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ee56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ee56-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ee56-127">Request body</span></span>
<span data-ttu-id="2ee56-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementConfigurationSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="2ee56-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingDefinition object.</span></span>

<span data-ttu-id="2ee56-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="2ee56-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingDefinition.</span></span>

|<span data-ttu-id="2ee56-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ee56-130">Property</span></span>|<span data-ttu-id="2ee56-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ee56-131">Type</span></span>|<span data-ttu-id="2ee56-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ee56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ee56-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="2ee56-133">applicability</span></span>|[<span data-ttu-id="2ee56-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="2ee56-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="2ee56-135">Detalhes sobre qual configuração de dispositivo se aplica</span><span class="sxs-lookup"><span data-stu-id="2ee56-135">Details which device setting is applicable on</span></span>|
|<span data-ttu-id="2ee56-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="2ee56-136">accessTypes</span></span>|[<span data-ttu-id="2ee56-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="2ee56-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="2ee56-138">Modo de acesso de leitura/gravação da configuração.</span><span class="sxs-lookup"><span data-stu-id="2ee56-138">Read/write access mode of the setting.</span></span> <span data-ttu-id="2ee56-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="2ee56-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="2ee56-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="2ee56-140">keywords</span></span>|<span data-ttu-id="2ee56-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ee56-141">String collection</span></span>|<span data-ttu-id="2ee56-142">Tokens para os quais as configurações de pesquisa</span><span class="sxs-lookup"><span data-stu-id="2ee56-142">Tokens which to search settings on</span></span>|
|<span data-ttu-id="2ee56-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="2ee56-143">infoUrls</span></span>|<span data-ttu-id="2ee56-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ee56-144">String collection</span></span>|<span data-ttu-id="2ee56-145">Lista de links mais informações para a configuração podem ser encontradas em</span><span class="sxs-lookup"><span data-stu-id="2ee56-145">List of links more info for the setting can be found at</span></span>|
|<span data-ttu-id="2ee56-146">ocorrência</span><span class="sxs-lookup"><span data-stu-id="2ee56-146">occurrence</span></span>|[<span data-ttu-id="2ee56-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="2ee56-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="2ee56-148">Indica se a configuração é obrigatória ou não</span><span class="sxs-lookup"><span data-stu-id="2ee56-148">Indicates whether the setting is required or not</span></span>|
|<span data-ttu-id="2ee56-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="2ee56-149">baseUri</span></span>|<span data-ttu-id="2ee56-150">String</span><span class="sxs-lookup"><span data-stu-id="2ee56-150">String</span></span>|<span data-ttu-id="2ee56-151">Caminho de CSP base</span><span class="sxs-lookup"><span data-stu-id="2ee56-151">Base CSP Path</span></span>|
|<span data-ttu-id="2ee56-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="2ee56-152">offsetUri</span></span>|<span data-ttu-id="2ee56-153">String</span><span class="sxs-lookup"><span data-stu-id="2ee56-153">String</span></span>|<span data-ttu-id="2ee56-154">Caminho de CSP offset da base</span><span class="sxs-lookup"><span data-stu-id="2ee56-154">Offset CSP Path from Base</span></span>|
|<span data-ttu-id="2ee56-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2ee56-155">rootDefinitionId</span></span>|<span data-ttu-id="2ee56-156">String</span><span class="sxs-lookup"><span data-stu-id="2ee56-156">String</span></span>|<span data-ttu-id="2ee56-157">Definição da configuração raiz se a configuração for uma configuração de filho.</span><span class="sxs-lookup"><span data-stu-id="2ee56-157">Root setting definition if the setting is a child setting.</span></span>|
|<span data-ttu-id="2ee56-158">categoryId</span><span class="sxs-lookup"><span data-stu-id="2ee56-158">categoryId</span></span>|<span data-ttu-id="2ee56-159">String</span><span class="sxs-lookup"><span data-stu-id="2ee56-159">String</span></span>|<span data-ttu-id="2ee56-160">Especifica o grupo de área no qual a configuração é configurada em um provedor de serviços de configuração especificado (CSP)</span><span class="sxs-lookup"><span data-stu-id="2ee56-160">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP)</span></span>|
|<span data-ttu-id="2ee56-161">settingUsage</span><span class="sxs-lookup"><span data-stu-id="2ee56-161">settingUsage</span></span>|[<span data-ttu-id="2ee56-162">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="2ee56-162">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="2ee56-163">Tipo de configuração, por exemplo, configuração e conformidade.</span><span class="sxs-lookup"><span data-stu-id="2ee56-163">Setting type, for example, configuration and compliance.</span></span> <span data-ttu-id="2ee56-164">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="2ee56-164">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="2ee56-165">id</span><span class="sxs-lookup"><span data-stu-id="2ee56-165">id</span></span>|<span data-ttu-id="2ee56-166">String</span><span class="sxs-lookup"><span data-stu-id="2ee56-166">String</span></span>|<span data-ttu-id="2ee56-167">Identificador do item</span><span class="sxs-lookup"><span data-stu-id="2ee56-167">Identifier for item</span></span>|
|<span data-ttu-id="2ee56-168">description</span><span class="sxs-lookup"><span data-stu-id="2ee56-168">description</span></span>|<span data-ttu-id="2ee56-169">String</span><span class="sxs-lookup"><span data-stu-id="2ee56-169">String</span></span>|<span data-ttu-id="2ee56-170">Descrição do item</span><span class="sxs-lookup"><span data-stu-id="2ee56-170">Description of the item</span></span>|
|<span data-ttu-id="2ee56-171">helpText</span><span class="sxs-lookup"><span data-stu-id="2ee56-171">helpText</span></span>|<span data-ttu-id="2ee56-172">String</span><span class="sxs-lookup"><span data-stu-id="2ee56-172">String</span></span>|<span data-ttu-id="2ee56-173">Texto de ajuda do item</span><span class="sxs-lookup"><span data-stu-id="2ee56-173">Help text of the item</span></span>|
|<span data-ttu-id="2ee56-174">nome</span><span class="sxs-lookup"><span data-stu-id="2ee56-174">name</span></span>|<span data-ttu-id="2ee56-175">String</span><span class="sxs-lookup"><span data-stu-id="2ee56-175">String</span></span>|<span data-ttu-id="2ee56-176">Nome do item</span><span class="sxs-lookup"><span data-stu-id="2ee56-176">Name of the item</span></span>|
|<span data-ttu-id="2ee56-177">displayName</span><span class="sxs-lookup"><span data-stu-id="2ee56-177">displayName</span></span>|<span data-ttu-id="2ee56-178">String</span><span class="sxs-lookup"><span data-stu-id="2ee56-178">String</span></span>|<span data-ttu-id="2ee56-179">Nome para exibição do item</span><span class="sxs-lookup"><span data-stu-id="2ee56-179">Display name of the item</span></span>|
|<span data-ttu-id="2ee56-180">versão</span><span class="sxs-lookup"><span data-stu-id="2ee56-180">version</span></span>|<span data-ttu-id="2ee56-181">String</span><span class="sxs-lookup"><span data-stu-id="2ee56-181">String</span></span>|<span data-ttu-id="2ee56-182">Versão do item</span><span class="sxs-lookup"><span data-stu-id="2ee56-182">Item Version</span></span>|



## <a name="response"></a><span data-ttu-id="2ee56-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ee56-183">Response</span></span>
<span data-ttu-id="2ee56-184">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ee56-184">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ee56-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ee56-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ee56-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ee56-186">Request</span></span>
<span data-ttu-id="2ee56-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ee56-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 977

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingDefinition",
  "applicability": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
    "description": "Description value",
    "platform": "macOS",
    "deviceMode": "kiosk",
    "technologies": "mdm"
  },
  "accessTypes": "add",
  "keywords": [
    "Keywords value"
  ],
  "infoUrls": [
    "Info Urls value"
  ],
  "occurrence": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
    "minDeviceOccurrence": 3,
    "maxDeviceOccurrence": 3
  },
  "baseUri": "Base Uri value",
  "offsetUri": "Offset Uri value",
  "rootDefinitionId": "Root Definition Id value",
  "categoryId": "Category Id value",
  "settingUsage": "configuration",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="2ee56-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ee56-188">Response</span></span>
<span data-ttu-id="2ee56-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ee56-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1026

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingDefinition",
  "applicability": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
    "description": "Description value",
    "platform": "macOS",
    "deviceMode": "kiosk",
    "technologies": "mdm"
  },
  "accessTypes": "add",
  "keywords": [
    "Keywords value"
  ],
  "infoUrls": [
    "Info Urls value"
  ],
  "occurrence": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
    "minDeviceOccurrence": 3,
    "maxDeviceOccurrence": 3
  },
  "baseUri": "Base Uri value",
  "offsetUri": "Offset Uri value",
  "rootDefinitionId": "Root Definition Id value",
  "categoryId": "Category Id value",
  "settingUsage": "configuration",
  "id": "7af649e5-49e5-7af6-e549-f67ae549f67a",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```




