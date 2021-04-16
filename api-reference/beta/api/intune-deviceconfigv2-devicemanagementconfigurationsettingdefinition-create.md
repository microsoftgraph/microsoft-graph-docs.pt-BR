---
title: Criar deviceManagementConfigurationSettingDefinition
description: Crie um novo objeto deviceManagementConfigurationSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 90dd6dfc79557ebed69c7359ff3a85d6fd042ee6
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51862783"
---
# <a name="create-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="a8c70-103">Criar deviceManagementConfigurationSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="a8c70-103">Create deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="a8c70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8c70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8c70-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8c70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8c70-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8c70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8c70-107">Crie um novo [objeto deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a8c70-107">Create a new [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8c70-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a8c70-108">Prerequisites</span></span>
<span data-ttu-id="a8c70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8c70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8c70-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8c70-111">Permission type</span></span>|<span data-ttu-id="a8c70-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8c70-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8c70-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8c70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8c70-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8c70-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8c70-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8c70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8c70-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8c70-116">Not supported.</span></span>|
|<span data-ttu-id="a8c70-117">Application</span><span class="sxs-lookup"><span data-stu-id="a8c70-117">Application</span></span>|<span data-ttu-id="a8c70-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8c70-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8c70-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8c70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reusableSettings
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="a8c70-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8c70-120">Request headers</span></span>
|<span data-ttu-id="a8c70-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8c70-121">Header</span></span>|<span data-ttu-id="a8c70-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a8c70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8c70-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8c70-123">Authorization</span></span>|<span data-ttu-id="a8c70-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8c70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8c70-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a8c70-125">Accept</span></span>|<span data-ttu-id="a8c70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8c70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8c70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8c70-127">Request body</span></span>
<span data-ttu-id="a8c70-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementConfigurationSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="a8c70-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingDefinition object.</span></span>

<span data-ttu-id="a8c70-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="a8c70-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingDefinition.</span></span>

|<span data-ttu-id="a8c70-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8c70-130">Property</span></span>|<span data-ttu-id="a8c70-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8c70-131">Type</span></span>|<span data-ttu-id="a8c70-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8c70-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8c70-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="a8c70-133">applicability</span></span>|[<span data-ttu-id="a8c70-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="a8c70-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="a8c70-135">Detalhes em qual configuração de dispositivo é aplicável</span><span class="sxs-lookup"><span data-stu-id="a8c70-135">Details which device setting is applicable on</span></span>|
|<span data-ttu-id="a8c70-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="a8c70-136">accessTypes</span></span>|[<span data-ttu-id="a8c70-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="a8c70-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="a8c70-138">Modo de acesso de leitura/gravação da configuração.</span><span class="sxs-lookup"><span data-stu-id="a8c70-138">Read/write access mode of the setting.</span></span> <span data-ttu-id="a8c70-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="a8c70-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="a8c70-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="a8c70-140">keywords</span></span>|<span data-ttu-id="a8c70-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="a8c70-141">String collection</span></span>|<span data-ttu-id="a8c70-142">Tokens em que as configurações de pesquisa</span><span class="sxs-lookup"><span data-stu-id="a8c70-142">Tokens which to search settings on</span></span>|
|<span data-ttu-id="a8c70-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="a8c70-143">infoUrls</span></span>|<span data-ttu-id="a8c70-144">Coleção String</span><span class="sxs-lookup"><span data-stu-id="a8c70-144">String collection</span></span>|<span data-ttu-id="a8c70-145">Lista de links mais informações para a configuração podem ser encontradas em</span><span class="sxs-lookup"><span data-stu-id="a8c70-145">List of links more info for the setting can be found at</span></span>|
|<span data-ttu-id="a8c70-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="a8c70-146">occurrence</span></span>|[<span data-ttu-id="a8c70-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="a8c70-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="a8c70-148">Indica se a configuração é necessária ou não</span><span class="sxs-lookup"><span data-stu-id="a8c70-148">Indicates whether the setting is required or not</span></span>|
|<span data-ttu-id="a8c70-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="a8c70-149">baseUri</span></span>|<span data-ttu-id="a8c70-150">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a8c70-150">String</span></span>|<span data-ttu-id="a8c70-151">Caminho CSP Base</span><span class="sxs-lookup"><span data-stu-id="a8c70-151">Base CSP Path</span></span>|
|<span data-ttu-id="a8c70-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="a8c70-152">offsetUri</span></span>|<span data-ttu-id="a8c70-153">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a8c70-153">String</span></span>|<span data-ttu-id="a8c70-154">Deslocamento do caminho do CSP da Base</span><span class="sxs-lookup"><span data-stu-id="a8c70-154">Offset CSP Path from Base</span></span>|
|<span data-ttu-id="a8c70-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a8c70-155">rootDefinitionId</span></span>|<span data-ttu-id="a8c70-156">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a8c70-156">String</span></span>|<span data-ttu-id="a8c70-157">Definição de configuração raiz se a configuração for uma configuração filho.</span><span class="sxs-lookup"><span data-stu-id="a8c70-157">Root setting definition if the setting is a child setting.</span></span>|
|<span data-ttu-id="a8c70-158">categoryId</span><span class="sxs-lookup"><span data-stu-id="a8c70-158">categoryId</span></span>|<span data-ttu-id="a8c70-159">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a8c70-159">String</span></span>|<span data-ttu-id="a8c70-160">Especifica o grupo de área no qual a configuração está configurada em um provedor de serviços de configuração especificado (CSP)</span><span class="sxs-lookup"><span data-stu-id="a8c70-160">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP)</span></span>|
|<span data-ttu-id="a8c70-161">settingUsage</span><span class="sxs-lookup"><span data-stu-id="a8c70-161">settingUsage</span></span>|[<span data-ttu-id="a8c70-162">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="a8c70-162">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="a8c70-163">Tipo de configuração, por exemplo, configuração e conformidade.</span><span class="sxs-lookup"><span data-stu-id="a8c70-163">Setting type, for example, configuration and compliance.</span></span> <span data-ttu-id="a8c70-164">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="a8c70-164">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="a8c70-165">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="a8c70-165">uxBehavior</span></span>|[<span data-ttu-id="a8c70-166">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="a8c70-166">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="a8c70-167">Definindo a representação do tipo de controle no UX.</span><span class="sxs-lookup"><span data-stu-id="a8c70-167">Setting control type representation in the UX.</span></span> <span data-ttu-id="a8c70-168">Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="a8c70-168">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="a8c70-169">visibility</span><span class="sxs-lookup"><span data-stu-id="a8c70-169">visibility</span></span>|[<span data-ttu-id="a8c70-170">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="a8c70-170">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="a8c70-171">Definindo o escopo de visibilidade como UX.</span><span class="sxs-lookup"><span data-stu-id="a8c70-171">Setting visibility scope to UX.</span></span> <span data-ttu-id="a8c70-172">Os valores possíveis são: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="a8c70-172">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="a8c70-173">referredSettingInformationList</span><span class="sxs-lookup"><span data-stu-id="a8c70-173">referredSettingInformationList</span></span>|<span data-ttu-id="a8c70-174">[coleção deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md)</span><span class="sxs-lookup"><span data-stu-id="a8c70-174">[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) collection</span></span>|<span data-ttu-id="a8c70-175">Lista de informações de configuração referidas.</span><span class="sxs-lookup"><span data-stu-id="a8c70-175">List of referred setting information.</span></span>|
|<span data-ttu-id="a8c70-176">id</span><span class="sxs-lookup"><span data-stu-id="a8c70-176">id</span></span>|<span data-ttu-id="a8c70-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8c70-177">String</span></span>|<span data-ttu-id="a8c70-178">Identificador de item</span><span class="sxs-lookup"><span data-stu-id="a8c70-178">Identifier for item</span></span>|
|<span data-ttu-id="a8c70-179">description</span><span class="sxs-lookup"><span data-stu-id="a8c70-179">description</span></span>|<span data-ttu-id="a8c70-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8c70-180">String</span></span>|<span data-ttu-id="a8c70-181">Descrição do item</span><span class="sxs-lookup"><span data-stu-id="a8c70-181">Description of the item</span></span>|
|<span data-ttu-id="a8c70-182">helpText</span><span class="sxs-lookup"><span data-stu-id="a8c70-182">helpText</span></span>|<span data-ttu-id="a8c70-183">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a8c70-183">String</span></span>|<span data-ttu-id="a8c70-184">Texto de ajuda do item</span><span class="sxs-lookup"><span data-stu-id="a8c70-184">Help text of the item</span></span>|
|<span data-ttu-id="a8c70-185">nome</span><span class="sxs-lookup"><span data-stu-id="a8c70-185">name</span></span>|<span data-ttu-id="a8c70-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8c70-186">String</span></span>|<span data-ttu-id="a8c70-187">Nome do item</span><span class="sxs-lookup"><span data-stu-id="a8c70-187">Name of the item</span></span>|
|<span data-ttu-id="a8c70-188">displayName</span><span class="sxs-lookup"><span data-stu-id="a8c70-188">displayName</span></span>|<span data-ttu-id="a8c70-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8c70-189">String</span></span>|<span data-ttu-id="a8c70-190">Nome de exibição do item</span><span class="sxs-lookup"><span data-stu-id="a8c70-190">Display name of the item</span></span>|
|<span data-ttu-id="a8c70-191">versão</span><span class="sxs-lookup"><span data-stu-id="a8c70-191">version</span></span>|<span data-ttu-id="a8c70-192">String</span><span class="sxs-lookup"><span data-stu-id="a8c70-192">String</span></span>|<span data-ttu-id="a8c70-193">Versão do item</span><span class="sxs-lookup"><span data-stu-id="a8c70-193">Item Version</span></span>|



## <a name="response"></a><span data-ttu-id="a8c70-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8c70-194">Response</span></span>
<span data-ttu-id="a8c70-195">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8c70-195">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8c70-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8c70-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8c70-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8c70-197">Request</span></span>
<span data-ttu-id="a8c70-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8c70-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reusableSettings
Content-type: application/json
Content-length: 1258

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
  "uxBehavior": "dropdown",
  "visibility": "settingsCatalog",
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "Setting Definition Id value"
    }
  ],
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="a8c70-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8c70-199">Response</span></span>
<span data-ttu-id="a8c70-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8c70-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1307

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
  "uxBehavior": "dropdown",
  "visibility": "settingsCatalog",
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "Setting Definition Id value"
    }
  ],
  "id": "7af649e5-49e5-7af6-e549-f67ae549f67a",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```




