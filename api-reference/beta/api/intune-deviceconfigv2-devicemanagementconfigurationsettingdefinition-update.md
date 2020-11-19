---
title: Atualizar deviceManagementConfigurationSettingDefinition
description: Atualiza as propriedades de um objeto deviceManagementConfigurationSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cb49bbd90b7c952deba932e0bbd1946f7bfc6ede
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241351"
---
# <a name="update-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="c234f-103">Atualizar deviceManagementConfigurationSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="c234f-103">Update deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="c234f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c234f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c234f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c234f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c234f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c234f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c234f-107">Atualiza as propriedades de um objeto [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="c234f-107">Update the properties of a [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c234f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c234f-108">Prerequisites</span></span>
<span data-ttu-id="c234f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c234f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c234f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c234f-111">Permission type</span></span>|<span data-ttu-id="c234f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c234f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c234f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c234f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c234f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c234f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c234f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c234f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c234f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c234f-116">Not supported.</span></span>|
|<span data-ttu-id="c234f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c234f-117">Application</span></span>|<span data-ttu-id="c234f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c234f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c234f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c234f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="c234f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c234f-120">Request headers</span></span>
|<span data-ttu-id="c234f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c234f-121">Header</span></span>|<span data-ttu-id="c234f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c234f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c234f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c234f-123">Authorization</span></span>|<span data-ttu-id="c234f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c234f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c234f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c234f-125">Accept</span></span>|<span data-ttu-id="c234f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c234f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c234f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c234f-127">Request body</span></span>
<span data-ttu-id="c234f-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="c234f-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

<span data-ttu-id="c234f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c234f-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span>

|<span data-ttu-id="c234f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c234f-130">Property</span></span>|<span data-ttu-id="c234f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c234f-131">Type</span></span>|<span data-ttu-id="c234f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c234f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c234f-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="c234f-133">applicability</span></span>|[<span data-ttu-id="c234f-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="c234f-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="c234f-135">Detalhes sobre qual configuração de dispositivo se aplica</span><span class="sxs-lookup"><span data-stu-id="c234f-135">Details which device setting is applicable on</span></span>|
|<span data-ttu-id="c234f-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="c234f-136">accessTypes</span></span>|[<span data-ttu-id="c234f-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="c234f-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="c234f-138">Modo de acesso de leitura/gravação da configuração.</span><span class="sxs-lookup"><span data-stu-id="c234f-138">Read/write access mode of the setting.</span></span> <span data-ttu-id="c234f-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="c234f-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="c234f-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="c234f-140">keywords</span></span>|<span data-ttu-id="c234f-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c234f-141">String collection</span></span>|<span data-ttu-id="c234f-142">Tokens para os quais as configurações de pesquisa</span><span class="sxs-lookup"><span data-stu-id="c234f-142">Tokens which to search settings on</span></span>|
|<span data-ttu-id="c234f-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="c234f-143">infoUrls</span></span>|<span data-ttu-id="c234f-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c234f-144">String collection</span></span>|<span data-ttu-id="c234f-145">Lista de links mais informações para a configuração podem ser encontradas em</span><span class="sxs-lookup"><span data-stu-id="c234f-145">List of links more info for the setting can be found at</span></span>|
|<span data-ttu-id="c234f-146">ocorrência</span><span class="sxs-lookup"><span data-stu-id="c234f-146">occurrence</span></span>|[<span data-ttu-id="c234f-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="c234f-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="c234f-148">Indica se a configuração é obrigatória ou não</span><span class="sxs-lookup"><span data-stu-id="c234f-148">Indicates whether the setting is required or not</span></span>|
|<span data-ttu-id="c234f-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="c234f-149">baseUri</span></span>|<span data-ttu-id="c234f-150">String</span><span class="sxs-lookup"><span data-stu-id="c234f-150">String</span></span>|<span data-ttu-id="c234f-151">Caminho de CSP base</span><span class="sxs-lookup"><span data-stu-id="c234f-151">Base CSP Path</span></span>|
|<span data-ttu-id="c234f-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="c234f-152">offsetUri</span></span>|<span data-ttu-id="c234f-153">String</span><span class="sxs-lookup"><span data-stu-id="c234f-153">String</span></span>|<span data-ttu-id="c234f-154">Caminho de CSP offset da base</span><span class="sxs-lookup"><span data-stu-id="c234f-154">Offset CSP Path from Base</span></span>|
|<span data-ttu-id="c234f-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c234f-155">rootDefinitionId</span></span>|<span data-ttu-id="c234f-156">String</span><span class="sxs-lookup"><span data-stu-id="c234f-156">String</span></span>|<span data-ttu-id="c234f-157">Definição da configuração raiz se a configuração for uma configuração de filho.</span><span class="sxs-lookup"><span data-stu-id="c234f-157">Root setting definition if the setting is a child setting.</span></span>|
|<span data-ttu-id="c234f-158">categoryId</span><span class="sxs-lookup"><span data-stu-id="c234f-158">categoryId</span></span>|<span data-ttu-id="c234f-159">String</span><span class="sxs-lookup"><span data-stu-id="c234f-159">String</span></span>|<span data-ttu-id="c234f-160">Especifica o grupo de área no qual a configuração é configurada em um provedor de serviços de configuração especificado (CSP)</span><span class="sxs-lookup"><span data-stu-id="c234f-160">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP)</span></span>|
|<span data-ttu-id="c234f-161">settingUsage</span><span class="sxs-lookup"><span data-stu-id="c234f-161">settingUsage</span></span>|[<span data-ttu-id="c234f-162">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="c234f-162">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="c234f-163">Tipo de configuração, por exemplo, configuração e conformidade.</span><span class="sxs-lookup"><span data-stu-id="c234f-163">Setting type, for example, configuration and compliance.</span></span> <span data-ttu-id="c234f-164">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="c234f-164">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="c234f-165">id</span><span class="sxs-lookup"><span data-stu-id="c234f-165">id</span></span>|<span data-ttu-id="c234f-166">String</span><span class="sxs-lookup"><span data-stu-id="c234f-166">String</span></span>|<span data-ttu-id="c234f-167">Identificador do item</span><span class="sxs-lookup"><span data-stu-id="c234f-167">Identifier for item</span></span>|
|<span data-ttu-id="c234f-168">description</span><span class="sxs-lookup"><span data-stu-id="c234f-168">description</span></span>|<span data-ttu-id="c234f-169">String</span><span class="sxs-lookup"><span data-stu-id="c234f-169">String</span></span>|<span data-ttu-id="c234f-170">Descrição do item</span><span class="sxs-lookup"><span data-stu-id="c234f-170">Description of the item</span></span>|
|<span data-ttu-id="c234f-171">helpText</span><span class="sxs-lookup"><span data-stu-id="c234f-171">helpText</span></span>|<span data-ttu-id="c234f-172">String</span><span class="sxs-lookup"><span data-stu-id="c234f-172">String</span></span>|<span data-ttu-id="c234f-173">Texto de ajuda do item</span><span class="sxs-lookup"><span data-stu-id="c234f-173">Help text of the item</span></span>|
|<span data-ttu-id="c234f-174">nome</span><span class="sxs-lookup"><span data-stu-id="c234f-174">name</span></span>|<span data-ttu-id="c234f-175">String</span><span class="sxs-lookup"><span data-stu-id="c234f-175">String</span></span>|<span data-ttu-id="c234f-176">Nome do item</span><span class="sxs-lookup"><span data-stu-id="c234f-176">Name of the item</span></span>|
|<span data-ttu-id="c234f-177">displayName</span><span class="sxs-lookup"><span data-stu-id="c234f-177">displayName</span></span>|<span data-ttu-id="c234f-178">String</span><span class="sxs-lookup"><span data-stu-id="c234f-178">String</span></span>|<span data-ttu-id="c234f-179">Nome para exibição do item</span><span class="sxs-lookup"><span data-stu-id="c234f-179">Display name of the item</span></span>|
|<span data-ttu-id="c234f-180">versão</span><span class="sxs-lookup"><span data-stu-id="c234f-180">version</span></span>|<span data-ttu-id="c234f-181">String</span><span class="sxs-lookup"><span data-stu-id="c234f-181">String</span></span>|<span data-ttu-id="c234f-182">Versão do item</span><span class="sxs-lookup"><span data-stu-id="c234f-182">Item Version</span></span>|



## <a name="response"></a><span data-ttu-id="c234f-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="c234f-183">Response</span></span>
<span data-ttu-id="c234f-184">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c234f-184">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c234f-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c234f-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="c234f-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c234f-186">Request</span></span>
<span data-ttu-id="c234f-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c234f-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
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

### <a name="response"></a><span data-ttu-id="c234f-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="c234f-188">Response</span></span>
<span data-ttu-id="c234f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c234f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




