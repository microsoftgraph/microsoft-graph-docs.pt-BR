---
title: Criar deviceManagementConfigurationSimpleSettingDefinition
description: Crie um novo objeto deviceManagementConfigurationSimpleSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: afba814b56eef8620aa2704c5848671a57b9ff5c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129122"
---
# <a name="create-devicemanagementconfigurationsimplesettingdefinition"></a><span data-ttu-id="3b420-103">Criar deviceManagementConfigurationSimpleSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="3b420-103">Create deviceManagementConfigurationSimpleSettingDefinition</span></span>

<span data-ttu-id="3b420-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b420-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b420-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b420-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b420-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b420-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b420-107">Crie um novo [objeto deviceManagementConfigurationSimpleSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-107">Create a new [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b420-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b420-108">Prerequisites</span></span>
<span data-ttu-id="3b420-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b420-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b420-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b420-111">Permission type</span></span>|<span data-ttu-id="3b420-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b420-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b420-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b420-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b420-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b420-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3b420-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b420-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b420-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b420-116">Not supported.</span></span>|
|<span data-ttu-id="3b420-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b420-117">Application</span></span>|<span data-ttu-id="3b420-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b420-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b420-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b420-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="3b420-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b420-120">Request headers</span></span>
|<span data-ttu-id="3b420-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b420-121">Header</span></span>|<span data-ttu-id="3b420-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3b420-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b420-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b420-123">Authorization</span></span>|<span data-ttu-id="3b420-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b420-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b420-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b420-125">Accept</span></span>|<span data-ttu-id="3b420-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b420-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b420-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b420-127">Request body</span></span>
<span data-ttu-id="3b420-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementConfigurationSimpleSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="3b420-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSimpleSettingDefinition object.</span></span>

<span data-ttu-id="3b420-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationSimpleSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="3b420-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSimpleSettingDefinition.</span></span>

|<span data-ttu-id="3b420-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b420-130">Property</span></span>|<span data-ttu-id="3b420-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b420-131">Type</span></span>|<span data-ttu-id="3b420-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b420-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b420-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="3b420-133">applicability</span></span>|[<span data-ttu-id="3b420-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="3b420-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="3b420-135">Detalhes sobre qual configuração de dispositivo é aplicável em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="3b420-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="3b420-136">accessTypes</span></span>|[<span data-ttu-id="3b420-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="3b420-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="3b420-138">Modo de acesso de leitura/gravação da configuração Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3b420-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="3b420-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="3b420-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="3b420-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="3b420-140">keywords</span></span>|<span data-ttu-id="3b420-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b420-141">String collection</span></span>|<span data-ttu-id="3b420-142">Tokens que para pesquisar configurações em Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="3b420-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="3b420-143">infoUrls</span></span>|<span data-ttu-id="3b420-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b420-144">String collection</span></span>|<span data-ttu-id="3b420-145">Lista de links mais informações para a configuração podem ser encontradas em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="3b420-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="3b420-146">occurrence</span></span>|[<span data-ttu-id="3b420-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="3b420-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="3b420-148">Indica se a configuração é necessária ou não Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="3b420-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="3b420-149">baseUri</span></span>|<span data-ttu-id="3b420-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b420-150">String</span></span>|<span data-ttu-id="3b420-151">Caminho base CSP Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="3b420-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="3b420-152">offsetUri</span></span>|<span data-ttu-id="3b420-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b420-153">String</span></span>|<span data-ttu-id="3b420-154">Caminho de deslocamento CSP da Base Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="3b420-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="3b420-155">rootDefinitionId</span></span>|<span data-ttu-id="3b420-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b420-156">String</span></span>|<span data-ttu-id="3b420-157">Definição de configuração raiz se a configuração for uma configuração filho.</span><span class="sxs-lookup"><span data-stu-id="3b420-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="3b420-158">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="3b420-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="3b420-159">categoryId</span></span>|<span data-ttu-id="3b420-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b420-160">String</span></span>|<span data-ttu-id="3b420-161">Especifica o grupo de área no qual a configuração está configurada em um provedor de serviços de configuração especificado (CSP) Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="3b420-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="3b420-162">settingUsage</span></span>|[<span data-ttu-id="3b420-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="3b420-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="3b420-164">Tipo de configuração, por exemplo, configuração e conformidade Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3b420-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="3b420-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="3b420-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="3b420-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="3b420-166">uxBehavior</span></span>|[<span data-ttu-id="3b420-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="3b420-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="3b420-168">Definindo a representação do tipo de controle no UX Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3b420-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="3b420-169">Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="3b420-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="3b420-170">visibility</span><span class="sxs-lookup"><span data-stu-id="3b420-170">visibility</span></span>|[<span data-ttu-id="3b420-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="3b420-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="3b420-172">Definindo o escopo de visibilidade como UX Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3b420-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="3b420-173">Os valores possíveis são: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="3b420-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="3b420-174">id</span><span class="sxs-lookup"><span data-stu-id="3b420-174">id</span></span>|<span data-ttu-id="3b420-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b420-175">String</span></span>|<span data-ttu-id="3b420-176">Identificador do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-176">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="3b420-177">descrição</span><span class="sxs-lookup"><span data-stu-id="3b420-177">description</span></span>|<span data-ttu-id="3b420-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b420-178">String</span></span>|<span data-ttu-id="3b420-179">Descrição do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-179">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="3b420-180">helpText</span><span class="sxs-lookup"><span data-stu-id="3b420-180">helpText</span></span>|<span data-ttu-id="3b420-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b420-181">String</span></span>|<span data-ttu-id="3b420-182">Texto de ajuda do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-182">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="3b420-183">nome</span><span class="sxs-lookup"><span data-stu-id="3b420-183">name</span></span>|<span data-ttu-id="3b420-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b420-184">String</span></span>|<span data-ttu-id="3b420-185">Nome do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-185">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="3b420-186">displayName</span><span class="sxs-lookup"><span data-stu-id="3b420-186">displayName</span></span>|<span data-ttu-id="3b420-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b420-187">String</span></span>|<span data-ttu-id="3b420-188">Nome de exibição do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-188">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="3b420-189">versão</span><span class="sxs-lookup"><span data-stu-id="3b420-189">version</span></span>|<span data-ttu-id="3b420-190">String</span><span class="sxs-lookup"><span data-stu-id="3b420-190">String</span></span>|<span data-ttu-id="3b420-191">Versão do item Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-191">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="3b420-192">valueDefinition</span><span class="sxs-lookup"><span data-stu-id="3b420-192">valueDefinition</span></span>|[<span data-ttu-id="3b420-193">deviceManagementConfigurationSettingValueDefinition</span><span class="sxs-lookup"><span data-stu-id="3b420-193">deviceManagementConfigurationSettingValueDefinition</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)|<span data-ttu-id="3b420-194">Definição do valor dessa configuração</span><span class="sxs-lookup"><span data-stu-id="3b420-194">Definition of the value for this setting</span></span>|
|<span data-ttu-id="3b420-195">defaultValue</span><span class="sxs-lookup"><span data-stu-id="3b420-195">defaultValue</span></span>|[<span data-ttu-id="3b420-196">deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="3b420-196">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="3b420-197">Valor de configuração padrão para essa configuração</span><span class="sxs-lookup"><span data-stu-id="3b420-197">Default setting value for this setting</span></span>|
|<span data-ttu-id="3b420-198">dependentOn</span><span class="sxs-lookup"><span data-stu-id="3b420-198">dependentOn</span></span>|<span data-ttu-id="3b420-199">[Coleção deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-199">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="3b420-200">lista de configurações pai que essa configuração depende</span><span class="sxs-lookup"><span data-stu-id="3b420-200">list of parent settings this setting is dependent on</span></span>|
|<span data-ttu-id="3b420-201">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="3b420-201">dependedOnBy</span></span>|<span data-ttu-id="3b420-202">[Coleção deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="3b420-202">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="3b420-203">lista de configurações filho que dependem dessa configuração</span><span class="sxs-lookup"><span data-stu-id="3b420-203">list of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="3b420-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b420-204">Response</span></span>
<span data-ttu-id="3b420-205">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b420-205">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b420-206">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b420-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b420-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b420-207">Request</span></span>
<span data-ttu-id="3b420-208">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b420-208">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 9192

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingDefinition",
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
  "version": "Version value",
  "valueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueDefinition"
  },
  "defaultValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValue",
    "children": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
        "settingDefinitionId": "Setting Definition Id value",
        "choiceSettingValue": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
          "value": "Value value",
          "children": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
              "settingDefinitionId": "Setting Definition Id value",
              "choiceSettingValue": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                "value": "Value value",
                "children": [
                  {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                    "settingDefinitionId": "Setting Definition Id value",
                    "choiceSettingValue": {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                      "value": "Value value",
                      "children": [
                        {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                          "settingDefinitionId": "Setting Definition Id value",
                          "choiceSettingValue": {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                            "value": "Value value",
                            "children": [
                              {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                "settingDefinitionId": "Setting Definition Id value",
                                "choiceSettingValue": {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                  "value": "Value value",
                                  "children": [
                                    {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                      "settingDefinitionId": "Setting Definition Id value",
                                      "choiceSettingValue": {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                        "value": "Value value",
                                        "children": [
                                          {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                            "settingDefinitionId": "Setting Definition Id value",
                                            "choiceSettingValue": {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                              "value": "Value value",
                                              "children": [
                                                {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                  "settingDefinitionId": "Setting Definition Id value",
                                                  "choiceSettingValue": {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                    "value": "Value value",
                                                    "children": [
                                                      {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                        "settingDefinitionId": "Setting Definition Id value",
                                                        "choiceSettingValue": {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                          "value": "Value value",
                                                          "children": [
                                                            {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                              "settingDefinitionId": "Setting Definition Id value",
                                                              "choiceSettingValue": {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                "value": "Value value",
                                                                "children": [
                                                                  {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                    "settingDefinitionId": "Setting Definition Id value",
                                                                    "choiceSettingValue": {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                      "value": "Value value",
                                                                      "children": null
                                                                    }
                                                                  }
                                                                ]
                                                              }
                                                            }
                                                          ]
                                                        }
                                                      }
                                                    ]
                                                  }
                                                }
                                              ]
                                            }
                                          }
                                        ]
                                      }
                                    }
                                  ]
                                }
                              }
                            ]
                          }
                        }
                      ]
                    }
                  }
                ]
              }
            }
          ]
        }
      }
    ]
  },
  "dependentOn": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn",
      "dependentOn": "Dependent On value",
      "parentSettingId": "Parent Setting Id value"
    }
  ],
  "dependedOnBy": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
      "dependedOnBy": "Depended On By value",
      "required": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="3b420-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b420-209">Response</span></span>
<span data-ttu-id="3b420-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b420-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9241

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingDefinition",
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
  "id": "30dc0613-0613-30dc-1306-dc301306dc30",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "valueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueDefinition"
  },
  "defaultValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValue",
    "children": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
        "settingDefinitionId": "Setting Definition Id value",
        "choiceSettingValue": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
          "value": "Value value",
          "children": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
              "settingDefinitionId": "Setting Definition Id value",
              "choiceSettingValue": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                "value": "Value value",
                "children": [
                  {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                    "settingDefinitionId": "Setting Definition Id value",
                    "choiceSettingValue": {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                      "value": "Value value",
                      "children": [
                        {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                          "settingDefinitionId": "Setting Definition Id value",
                          "choiceSettingValue": {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                            "value": "Value value",
                            "children": [
                              {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                "settingDefinitionId": "Setting Definition Id value",
                                "choiceSettingValue": {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                  "value": "Value value",
                                  "children": [
                                    {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                      "settingDefinitionId": "Setting Definition Id value",
                                      "choiceSettingValue": {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                        "value": "Value value",
                                        "children": [
                                          {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                            "settingDefinitionId": "Setting Definition Id value",
                                            "choiceSettingValue": {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                              "value": "Value value",
                                              "children": [
                                                {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                  "settingDefinitionId": "Setting Definition Id value",
                                                  "choiceSettingValue": {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                    "value": "Value value",
                                                    "children": [
                                                      {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                        "settingDefinitionId": "Setting Definition Id value",
                                                        "choiceSettingValue": {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                          "value": "Value value",
                                                          "children": [
                                                            {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                              "settingDefinitionId": "Setting Definition Id value",
                                                              "choiceSettingValue": {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                "value": "Value value",
                                                                "children": [
                                                                  {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                    "settingDefinitionId": "Setting Definition Id value",
                                                                    "choiceSettingValue": {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                      "value": "Value value",
                                                                      "children": null
                                                                    }
                                                                  }
                                                                ]
                                                              }
                                                            }
                                                          ]
                                                        }
                                                      }
                                                    ]
                                                  }
                                                }
                                              ]
                                            }
                                          }
                                        ]
                                      }
                                    }
                                  ]
                                }
                              }
                            ]
                          }
                        }
                      ]
                    }
                  }
                ]
              }
            }
          ]
        }
      }
    ]
  },
  "dependentOn": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn",
      "dependentOn": "Dependent On value",
      "parentSettingId": "Parent Setting Id value"
    }
  ],
  "dependedOnBy": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
      "dependedOnBy": "Depended On By value",
      "required": true
    }
  ]
}
```




