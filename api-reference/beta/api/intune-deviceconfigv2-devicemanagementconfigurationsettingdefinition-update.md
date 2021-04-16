---
title: Atualizar deviceManagementConfigurationSettingDefinition
description: Atualize as propriedades de um objeto deviceManagementConfigurationSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e3840e07382cc13a587460466f09d84dd7e64452
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867949"
---
# <a name="update-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="c582b-103">Atualizar deviceManagementConfigurationSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="c582b-103">Update deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="c582b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c582b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c582b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c582b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c582b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c582b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c582b-107">Atualize as propriedades de [um objeto deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c582b-107">Update the properties of a [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c582b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c582b-108">Prerequisites</span></span>
<span data-ttu-id="c582b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c582b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c582b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c582b-111">Permission type</span></span>|<span data-ttu-id="c582b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c582b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c582b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c582b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c582b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c582b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c582b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c582b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c582b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c582b-116">Not supported.</span></span>|
|<span data-ttu-id="c582b-117">Application</span><span class="sxs-lookup"><span data-stu-id="c582b-117">Application</span></span>|<span data-ttu-id="c582b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c582b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c582b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c582b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="c582b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c582b-120">Request headers</span></span>
|<span data-ttu-id="c582b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c582b-121">Header</span></span>|<span data-ttu-id="c582b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c582b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c582b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c582b-123">Authorization</span></span>|<span data-ttu-id="c582b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c582b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c582b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c582b-125">Accept</span></span>|<span data-ttu-id="c582b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c582b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c582b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c582b-127">Request body</span></span>
<span data-ttu-id="c582b-128">No corpo da solicitação, fornece uma representação JSON para [o objeto deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c582b-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

<span data-ttu-id="c582b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c582b-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span>

|<span data-ttu-id="c582b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c582b-130">Property</span></span>|<span data-ttu-id="c582b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c582b-131">Type</span></span>|<span data-ttu-id="c582b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c582b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c582b-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="c582b-133">applicability</span></span>|[<span data-ttu-id="c582b-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="c582b-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="c582b-135">Detalhes em qual configuração de dispositivo é aplicável</span><span class="sxs-lookup"><span data-stu-id="c582b-135">Details which device setting is applicable on</span></span>|
|<span data-ttu-id="c582b-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="c582b-136">accessTypes</span></span>|[<span data-ttu-id="c582b-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="c582b-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="c582b-138">Modo de acesso de leitura/gravação da configuração.</span><span class="sxs-lookup"><span data-stu-id="c582b-138">Read/write access mode of the setting.</span></span> <span data-ttu-id="c582b-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="c582b-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="c582b-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="c582b-140">keywords</span></span>|<span data-ttu-id="c582b-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="c582b-141">String collection</span></span>|<span data-ttu-id="c582b-142">Tokens em que as configurações de pesquisa</span><span class="sxs-lookup"><span data-stu-id="c582b-142">Tokens which to search settings on</span></span>|
|<span data-ttu-id="c582b-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="c582b-143">infoUrls</span></span>|<span data-ttu-id="c582b-144">Coleção String</span><span class="sxs-lookup"><span data-stu-id="c582b-144">String collection</span></span>|<span data-ttu-id="c582b-145">Lista de links mais informações para a configuração podem ser encontradas em</span><span class="sxs-lookup"><span data-stu-id="c582b-145">List of links more info for the setting can be found at</span></span>|
|<span data-ttu-id="c582b-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="c582b-146">occurrence</span></span>|[<span data-ttu-id="c582b-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="c582b-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="c582b-148">Indica se a configuração é necessária ou não</span><span class="sxs-lookup"><span data-stu-id="c582b-148">Indicates whether the setting is required or not</span></span>|
|<span data-ttu-id="c582b-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="c582b-149">baseUri</span></span>|<span data-ttu-id="c582b-150">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="c582b-150">String</span></span>|<span data-ttu-id="c582b-151">Caminho CSP Base</span><span class="sxs-lookup"><span data-stu-id="c582b-151">Base CSP Path</span></span>|
|<span data-ttu-id="c582b-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="c582b-152">offsetUri</span></span>|<span data-ttu-id="c582b-153">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="c582b-153">String</span></span>|<span data-ttu-id="c582b-154">Deslocamento do caminho do CSP da Base</span><span class="sxs-lookup"><span data-stu-id="c582b-154">Offset CSP Path from Base</span></span>|
|<span data-ttu-id="c582b-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c582b-155">rootDefinitionId</span></span>|<span data-ttu-id="c582b-156">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="c582b-156">String</span></span>|<span data-ttu-id="c582b-157">Definição de configuração raiz se a configuração for uma configuração filho.</span><span class="sxs-lookup"><span data-stu-id="c582b-157">Root setting definition if the setting is a child setting.</span></span>|
|<span data-ttu-id="c582b-158">categoryId</span><span class="sxs-lookup"><span data-stu-id="c582b-158">categoryId</span></span>|<span data-ttu-id="c582b-159">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="c582b-159">String</span></span>|<span data-ttu-id="c582b-160">Especifica o grupo de área no qual a configuração está configurada em um provedor de serviços de configuração especificado (CSP)</span><span class="sxs-lookup"><span data-stu-id="c582b-160">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP)</span></span>|
|<span data-ttu-id="c582b-161">settingUsage</span><span class="sxs-lookup"><span data-stu-id="c582b-161">settingUsage</span></span>|[<span data-ttu-id="c582b-162">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="c582b-162">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="c582b-163">Tipo de configuração, por exemplo, configuração e conformidade.</span><span class="sxs-lookup"><span data-stu-id="c582b-163">Setting type, for example, configuration and compliance.</span></span> <span data-ttu-id="c582b-164">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="c582b-164">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="c582b-165">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="c582b-165">uxBehavior</span></span>|[<span data-ttu-id="c582b-166">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="c582b-166">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="c582b-167">Definindo a representação do tipo de controle no UX.</span><span class="sxs-lookup"><span data-stu-id="c582b-167">Setting control type representation in the UX.</span></span> <span data-ttu-id="c582b-168">Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="c582b-168">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="c582b-169">visibility</span><span class="sxs-lookup"><span data-stu-id="c582b-169">visibility</span></span>|[<span data-ttu-id="c582b-170">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="c582b-170">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="c582b-171">Definindo o escopo de visibilidade como UX.</span><span class="sxs-lookup"><span data-stu-id="c582b-171">Setting visibility scope to UX.</span></span> <span data-ttu-id="c582b-172">Os valores possíveis são: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="c582b-172">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="c582b-173">referredSettingInformationList</span><span class="sxs-lookup"><span data-stu-id="c582b-173">referredSettingInformationList</span></span>|<span data-ttu-id="c582b-174">[coleção deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md)</span><span class="sxs-lookup"><span data-stu-id="c582b-174">[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) collection</span></span>|<span data-ttu-id="c582b-175">Lista de informações de configuração referidas.</span><span class="sxs-lookup"><span data-stu-id="c582b-175">List of referred setting information.</span></span>|
|<span data-ttu-id="c582b-176">id</span><span class="sxs-lookup"><span data-stu-id="c582b-176">id</span></span>|<span data-ttu-id="c582b-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c582b-177">String</span></span>|<span data-ttu-id="c582b-178">Identificador de item</span><span class="sxs-lookup"><span data-stu-id="c582b-178">Identifier for item</span></span>|
|<span data-ttu-id="c582b-179">description</span><span class="sxs-lookup"><span data-stu-id="c582b-179">description</span></span>|<span data-ttu-id="c582b-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c582b-180">String</span></span>|<span data-ttu-id="c582b-181">Descrição do item</span><span class="sxs-lookup"><span data-stu-id="c582b-181">Description of the item</span></span>|
|<span data-ttu-id="c582b-182">helpText</span><span class="sxs-lookup"><span data-stu-id="c582b-182">helpText</span></span>|<span data-ttu-id="c582b-183">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="c582b-183">String</span></span>|<span data-ttu-id="c582b-184">Texto de ajuda do item</span><span class="sxs-lookup"><span data-stu-id="c582b-184">Help text of the item</span></span>|
|<span data-ttu-id="c582b-185">nome</span><span class="sxs-lookup"><span data-stu-id="c582b-185">name</span></span>|<span data-ttu-id="c582b-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c582b-186">String</span></span>|<span data-ttu-id="c582b-187">Nome do item</span><span class="sxs-lookup"><span data-stu-id="c582b-187">Name of the item</span></span>|
|<span data-ttu-id="c582b-188">displayName</span><span class="sxs-lookup"><span data-stu-id="c582b-188">displayName</span></span>|<span data-ttu-id="c582b-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c582b-189">String</span></span>|<span data-ttu-id="c582b-190">Nome de exibição do item</span><span class="sxs-lookup"><span data-stu-id="c582b-190">Display name of the item</span></span>|
|<span data-ttu-id="c582b-191">versão</span><span class="sxs-lookup"><span data-stu-id="c582b-191">version</span></span>|<span data-ttu-id="c582b-192">String</span><span class="sxs-lookup"><span data-stu-id="c582b-192">String</span></span>|<span data-ttu-id="c582b-193">Versão do item</span><span class="sxs-lookup"><span data-stu-id="c582b-193">Item Version</span></span>|



## <a name="response"></a><span data-ttu-id="c582b-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="c582b-194">Response</span></span>
<span data-ttu-id="c582b-195">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c582b-195">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c582b-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c582b-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="c582b-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c582b-197">Request</span></span>
<span data-ttu-id="c582b-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c582b-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
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

### <a name="response"></a><span data-ttu-id="c582b-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="c582b-199">Response</span></span>
<span data-ttu-id="c582b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c582b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




