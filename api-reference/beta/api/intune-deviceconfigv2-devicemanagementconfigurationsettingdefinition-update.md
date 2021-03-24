---
title: Atualizar deviceManagementConfigurationSettingDefinition
description: Atualize as propriedades de um objeto deviceManagementConfigurationSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 99a65dd140e8128e5459517e19c510c2a8114500
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146906"
---
# <a name="update-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="0c0f3-103">Atualizar deviceManagementConfigurationSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="0c0f3-103">Update deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="0c0f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c0f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c0f3-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c0f3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c0f3-107">Atualize as propriedades de [um objeto deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0c0f3-107">Update the properties of a [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c0f3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c0f3-108">Prerequisites</span></span>
<span data-ttu-id="0c0f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c0f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c0f3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c0f3-111">Permission type</span></span>|<span data-ttu-id="0c0f3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c0f3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c0f3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c0f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c0f3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c0f3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c0f3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c0f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c0f3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-116">Not supported.</span></span>|
|<span data-ttu-id="0c0f3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c0f3-117">Application</span></span>|<span data-ttu-id="0c0f3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c0f3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c0f3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c0f3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="0c0f3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c0f3-120">Request headers</span></span>
|<span data-ttu-id="0c0f3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c0f3-121">Header</span></span>|<span data-ttu-id="0c0f3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0c0f3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c0f3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c0f3-123">Authorization</span></span>|<span data-ttu-id="0c0f3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c0f3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c0f3-125">Accept</span></span>|<span data-ttu-id="0c0f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c0f3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c0f3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c0f3-127">Request body</span></span>
<span data-ttu-id="0c0f3-128">No corpo da solicitação, fornece uma representação JSON para [o objeto deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0c0f3-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

<span data-ttu-id="0c0f3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0c0f3-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span>

|<span data-ttu-id="0c0f3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c0f3-130">Property</span></span>|<span data-ttu-id="0c0f3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c0f3-131">Type</span></span>|<span data-ttu-id="0c0f3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c0f3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c0f3-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="0c0f3-133">applicability</span></span>|[<span data-ttu-id="0c0f3-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="0c0f3-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="0c0f3-135">Detalhes em qual configuração de dispositivo é aplicável</span><span class="sxs-lookup"><span data-stu-id="0c0f3-135">Details which device setting is applicable on</span></span>|
|<span data-ttu-id="0c0f3-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="0c0f3-136">accessTypes</span></span>|[<span data-ttu-id="0c0f3-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="0c0f3-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="0c0f3-138">Modo de acesso de leitura/gravação da configuração.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-138">Read/write access mode of the setting.</span></span> <span data-ttu-id="0c0f3-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="0c0f3-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="0c0f3-140">keywords</span></span>|<span data-ttu-id="0c0f3-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c0f3-141">String collection</span></span>|<span data-ttu-id="0c0f3-142">Tokens em que as configurações de pesquisa</span><span class="sxs-lookup"><span data-stu-id="0c0f3-142">Tokens which to search settings on</span></span>|
|<span data-ttu-id="0c0f3-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="0c0f3-143">infoUrls</span></span>|<span data-ttu-id="0c0f3-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c0f3-144">String collection</span></span>|<span data-ttu-id="0c0f3-145">Lista de links mais informações para a configuração podem ser encontradas em</span><span class="sxs-lookup"><span data-stu-id="0c0f3-145">List of links more info for the setting can be found at</span></span>|
|<span data-ttu-id="0c0f3-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="0c0f3-146">occurrence</span></span>|[<span data-ttu-id="0c0f3-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="0c0f3-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="0c0f3-148">Indica se a configuração é necessária ou não</span><span class="sxs-lookup"><span data-stu-id="0c0f3-148">Indicates whether the setting is required or not</span></span>|
|<span data-ttu-id="0c0f3-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="0c0f3-149">baseUri</span></span>|<span data-ttu-id="0c0f3-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c0f3-150">String</span></span>|<span data-ttu-id="0c0f3-151">Caminho CSP Base</span><span class="sxs-lookup"><span data-stu-id="0c0f3-151">Base CSP Path</span></span>|
|<span data-ttu-id="0c0f3-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="0c0f3-152">offsetUri</span></span>|<span data-ttu-id="0c0f3-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c0f3-153">String</span></span>|<span data-ttu-id="0c0f3-154">Deslocamento do caminho do CSP da Base</span><span class="sxs-lookup"><span data-stu-id="0c0f3-154">Offset CSP Path from Base</span></span>|
|<span data-ttu-id="0c0f3-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="0c0f3-155">rootDefinitionId</span></span>|<span data-ttu-id="0c0f3-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c0f3-156">String</span></span>|<span data-ttu-id="0c0f3-157">Definição de configuração raiz se a configuração for uma configuração filho.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-157">Root setting definition if the setting is a child setting.</span></span>|
|<span data-ttu-id="0c0f3-158">categoryId</span><span class="sxs-lookup"><span data-stu-id="0c0f3-158">categoryId</span></span>|<span data-ttu-id="0c0f3-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c0f3-159">String</span></span>|<span data-ttu-id="0c0f3-160">Especifica o grupo de área no qual a configuração está configurada em um provedor de serviços de configuração especificado (CSP)</span><span class="sxs-lookup"><span data-stu-id="0c0f3-160">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP)</span></span>|
|<span data-ttu-id="0c0f3-161">settingUsage</span><span class="sxs-lookup"><span data-stu-id="0c0f3-161">settingUsage</span></span>|[<span data-ttu-id="0c0f3-162">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="0c0f3-162">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="0c0f3-163">Tipo de configuração, por exemplo, configuração e conformidade.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-163">Setting type, for example, configuration and compliance.</span></span> <span data-ttu-id="0c0f3-164">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-164">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="0c0f3-165">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="0c0f3-165">uxBehavior</span></span>|[<span data-ttu-id="0c0f3-166">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="0c0f3-166">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="0c0f3-167">Definindo a representação do tipo de controle no UX.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-167">Setting control type representation in the UX.</span></span> <span data-ttu-id="0c0f3-168">Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-168">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="0c0f3-169">visibility</span><span class="sxs-lookup"><span data-stu-id="0c0f3-169">visibility</span></span>|[<span data-ttu-id="0c0f3-170">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="0c0f3-170">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="0c0f3-171">Definindo o escopo de visibilidade como UX.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-171">Setting visibility scope to UX.</span></span> <span data-ttu-id="0c0f3-172">Os valores possíveis são: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-172">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="0c0f3-173">id</span><span class="sxs-lookup"><span data-stu-id="0c0f3-173">id</span></span>|<span data-ttu-id="0c0f3-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c0f3-174">String</span></span>|<span data-ttu-id="0c0f3-175">Identificador de item</span><span class="sxs-lookup"><span data-stu-id="0c0f3-175">Identifier for item</span></span>|
|<span data-ttu-id="0c0f3-176">descrição</span><span class="sxs-lookup"><span data-stu-id="0c0f3-176">description</span></span>|<span data-ttu-id="0c0f3-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c0f3-177">String</span></span>|<span data-ttu-id="0c0f3-178">Descrição do item</span><span class="sxs-lookup"><span data-stu-id="0c0f3-178">Description of the item</span></span>|
|<span data-ttu-id="0c0f3-179">helpText</span><span class="sxs-lookup"><span data-stu-id="0c0f3-179">helpText</span></span>|<span data-ttu-id="0c0f3-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c0f3-180">String</span></span>|<span data-ttu-id="0c0f3-181">Texto de ajuda do item</span><span class="sxs-lookup"><span data-stu-id="0c0f3-181">Help text of the item</span></span>|
|<span data-ttu-id="0c0f3-182">nome</span><span class="sxs-lookup"><span data-stu-id="0c0f3-182">name</span></span>|<span data-ttu-id="0c0f3-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c0f3-183">String</span></span>|<span data-ttu-id="0c0f3-184">Nome do item</span><span class="sxs-lookup"><span data-stu-id="0c0f3-184">Name of the item</span></span>|
|<span data-ttu-id="0c0f3-185">displayName</span><span class="sxs-lookup"><span data-stu-id="0c0f3-185">displayName</span></span>|<span data-ttu-id="0c0f3-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c0f3-186">String</span></span>|<span data-ttu-id="0c0f3-187">Nome de exibição do item</span><span class="sxs-lookup"><span data-stu-id="0c0f3-187">Display name of the item</span></span>|
|<span data-ttu-id="0c0f3-188">versão</span><span class="sxs-lookup"><span data-stu-id="0c0f3-188">version</span></span>|<span data-ttu-id="0c0f3-189">String</span><span class="sxs-lookup"><span data-stu-id="0c0f3-189">String</span></span>|<span data-ttu-id="0c0f3-190">Versão do item</span><span class="sxs-lookup"><span data-stu-id="0c0f3-190">Item Version</span></span>|



## <a name="response"></a><span data-ttu-id="0c0f3-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c0f3-191">Response</span></span>
<span data-ttu-id="0c0f3-192">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-192">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c0f3-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c0f3-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c0f3-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c0f3-194">Request</span></span>
<span data-ttu-id="0c0f3-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1042

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
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="0c0f3-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c0f3-196">Response</span></span>
<span data-ttu-id="0c0f3-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1091

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
  "id": "7af649e5-49e5-7af6-e549-f67ae549f67a",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```




