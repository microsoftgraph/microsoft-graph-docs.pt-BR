---
title: Atualizar deviceManagementConfigurationSettingDefinition
description: Atualizar as propriedades de um objeto deviceManagementConfigurationSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1370c49932bb32e3fb96d0a1111b496094f69000
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160050"
---
# <a name="update-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="5dc4b-103">Atualizar deviceManagementConfigurationSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="5dc4b-103">Update deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="5dc4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dc4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5dc4b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5dc4b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dc4b-107">Atualizar as propriedades de um [objeto deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5dc4b-107">Update the properties of a [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5dc4b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5dc4b-108">Prerequisites</span></span>
<span data-ttu-id="5dc4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dc4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dc4b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dc4b-111">Permission type</span></span>|<span data-ttu-id="5dc4b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5dc4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dc4b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dc4b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5dc4b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dc4b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5dc4b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dc4b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dc4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-116">Not supported.</span></span>|
|<span data-ttu-id="5dc4b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dc4b-117">Application</span></span>|<span data-ttu-id="5dc4b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dc4b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dc4b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dc4b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="5dc4b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc4b-120">Request headers</span></span>
|<span data-ttu-id="5dc4b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5dc4b-121">Header</span></span>|<span data-ttu-id="5dc4b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5dc4b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5dc4b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dc4b-123">Authorization</span></span>|<span data-ttu-id="5dc4b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5dc4b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5dc4b-125">Accept</span></span>|<span data-ttu-id="5dc4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5dc4b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dc4b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc4b-127">Request body</span></span>
<span data-ttu-id="5dc4b-128">No corpo da solicitação, fornece uma representação JSON do [objeto deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5dc4b-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

<span data-ttu-id="5dc4b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5dc4b-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span>

|<span data-ttu-id="5dc4b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5dc4b-130">Property</span></span>|<span data-ttu-id="5dc4b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dc4b-131">Type</span></span>|<span data-ttu-id="5dc4b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dc4b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dc4b-133">applicability</span><span class="sxs-lookup"><span data-stu-id="5dc4b-133">applicability</span></span>|[<span data-ttu-id="5dc4b-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="5dc4b-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="5dc4b-135">Detalhes sobre qual configuração de dispositivo é aplicável</span><span class="sxs-lookup"><span data-stu-id="5dc4b-135">Details which device setting is applicable on</span></span>|
|<span data-ttu-id="5dc4b-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="5dc4b-136">accessTypes</span></span>|[<span data-ttu-id="5dc4b-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="5dc4b-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="5dc4b-138">Modo de acesso de leitura/gravação da configuração.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-138">Read/write access mode of the setting.</span></span> <span data-ttu-id="5dc4b-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="5dc4b-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="5dc4b-140">keywords</span></span>|<span data-ttu-id="5dc4b-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dc4b-141">String collection</span></span>|<span data-ttu-id="5dc4b-142">Tokens nos quais pesquisar configurações</span><span class="sxs-lookup"><span data-stu-id="5dc4b-142">Tokens which to search settings on</span></span>|
|<span data-ttu-id="5dc4b-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="5dc4b-143">infoUrls</span></span>|<span data-ttu-id="5dc4b-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dc4b-144">String collection</span></span>|<span data-ttu-id="5dc4b-145">Lista de links em que mais informações sobre a configuração podem ser encontradas em</span><span class="sxs-lookup"><span data-stu-id="5dc4b-145">List of links more info for the setting can be found at</span></span>|
|<span data-ttu-id="5dc4b-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="5dc4b-146">occurrence</span></span>|[<span data-ttu-id="5dc4b-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="5dc4b-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="5dc4b-148">Indica se a configuração é necessária ou não</span><span class="sxs-lookup"><span data-stu-id="5dc4b-148">Indicates whether the setting is required or not</span></span>|
|<span data-ttu-id="5dc4b-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="5dc4b-149">baseUri</span></span>|<span data-ttu-id="5dc4b-150">String</span><span class="sxs-lookup"><span data-stu-id="5dc4b-150">String</span></span>|<span data-ttu-id="5dc4b-151">Caminho CSP Base</span><span class="sxs-lookup"><span data-stu-id="5dc4b-151">Base CSP Path</span></span>|
|<span data-ttu-id="5dc4b-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="5dc4b-152">offsetUri</span></span>|<span data-ttu-id="5dc4b-153">String</span><span class="sxs-lookup"><span data-stu-id="5dc4b-153">String</span></span>|<span data-ttu-id="5dc4b-154">Deslocamento do caminho do CSP da Base</span><span class="sxs-lookup"><span data-stu-id="5dc4b-154">Offset CSP Path from Base</span></span>|
|<span data-ttu-id="5dc4b-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5dc4b-155">rootDefinitionId</span></span>|<span data-ttu-id="5dc4b-156">String</span><span class="sxs-lookup"><span data-stu-id="5dc4b-156">String</span></span>|<span data-ttu-id="5dc4b-157">Definição de configuração raiz se a configuração for uma configuração filha.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-157">Root setting definition if the setting is a child setting.</span></span>|
|<span data-ttu-id="5dc4b-158">categoryId</span><span class="sxs-lookup"><span data-stu-id="5dc4b-158">categoryId</span></span>|<span data-ttu-id="5dc4b-159">String</span><span class="sxs-lookup"><span data-stu-id="5dc4b-159">String</span></span>|<span data-ttu-id="5dc4b-160">Especifica o grupo de área em que a configuração está configurada em um CSP (provedor de serviços de configuração) especificado</span><span class="sxs-lookup"><span data-stu-id="5dc4b-160">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP)</span></span>|
|<span data-ttu-id="5dc4b-161">settingUsage</span><span class="sxs-lookup"><span data-stu-id="5dc4b-161">settingUsage</span></span>|[<span data-ttu-id="5dc4b-162">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="5dc4b-162">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="5dc4b-163">Tipo de configuração, por exemplo, configuração e conformidade.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-163">Setting type, for example, configuration and compliance.</span></span> <span data-ttu-id="5dc4b-164">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-164">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="5dc4b-165">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="5dc4b-165">uxBehavior</span></span>|[<span data-ttu-id="5dc4b-166">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="5dc4b-166">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="5dc4b-167">Representação do tipo de controle de configuração na UX.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-167">Setting control type representation in the UX.</span></span> <span data-ttu-id="5dc4b-168">Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-168">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="5dc4b-169">id</span><span class="sxs-lookup"><span data-stu-id="5dc4b-169">id</span></span>|<span data-ttu-id="5dc4b-170">String</span><span class="sxs-lookup"><span data-stu-id="5dc4b-170">String</span></span>|<span data-ttu-id="5dc4b-171">Identificador do item</span><span class="sxs-lookup"><span data-stu-id="5dc4b-171">Identifier for item</span></span>|
|<span data-ttu-id="5dc4b-172">description</span><span class="sxs-lookup"><span data-stu-id="5dc4b-172">description</span></span>|<span data-ttu-id="5dc4b-173">String</span><span class="sxs-lookup"><span data-stu-id="5dc4b-173">String</span></span>|<span data-ttu-id="5dc4b-174">Descrição do item</span><span class="sxs-lookup"><span data-stu-id="5dc4b-174">Description of the item</span></span>|
|<span data-ttu-id="5dc4b-175">helpText</span><span class="sxs-lookup"><span data-stu-id="5dc4b-175">helpText</span></span>|<span data-ttu-id="5dc4b-176">String</span><span class="sxs-lookup"><span data-stu-id="5dc4b-176">String</span></span>|<span data-ttu-id="5dc4b-177">Texto de ajuda do item</span><span class="sxs-lookup"><span data-stu-id="5dc4b-177">Help text of the item</span></span>|
|<span data-ttu-id="5dc4b-178">name</span><span class="sxs-lookup"><span data-stu-id="5dc4b-178">name</span></span>|<span data-ttu-id="5dc4b-179">String</span><span class="sxs-lookup"><span data-stu-id="5dc4b-179">String</span></span>|<span data-ttu-id="5dc4b-180">Nome do item</span><span class="sxs-lookup"><span data-stu-id="5dc4b-180">Name of the item</span></span>|
|<span data-ttu-id="5dc4b-181">displayName</span><span class="sxs-lookup"><span data-stu-id="5dc4b-181">displayName</span></span>|<span data-ttu-id="5dc4b-182">String</span><span class="sxs-lookup"><span data-stu-id="5dc4b-182">String</span></span>|<span data-ttu-id="5dc4b-183">Nome de exibição do item</span><span class="sxs-lookup"><span data-stu-id="5dc4b-183">Display name of the item</span></span>|
|<span data-ttu-id="5dc4b-184">versão</span><span class="sxs-lookup"><span data-stu-id="5dc4b-184">version</span></span>|<span data-ttu-id="5dc4b-185">String</span><span class="sxs-lookup"><span data-stu-id="5dc4b-185">String</span></span>|<span data-ttu-id="5dc4b-186">Versão do Item</span><span class="sxs-lookup"><span data-stu-id="5dc4b-186">Item Version</span></span>|



## <a name="response"></a><span data-ttu-id="5dc4b-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc4b-187">Response</span></span>
<span data-ttu-id="5dc4b-188">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-188">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dc4b-189">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dc4b-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="5dc4b-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc4b-190">Request</span></span>
<span data-ttu-id="5dc4b-191">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-191">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1006

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
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="5dc4b-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc4b-192">Response</span></span>
<span data-ttu-id="5dc4b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5dc4b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1055

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
  "id": "7af649e5-49e5-7af6-e549-f67ae549f67a",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```




