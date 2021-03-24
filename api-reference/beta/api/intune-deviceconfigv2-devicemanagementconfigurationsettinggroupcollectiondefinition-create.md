---
title: Criar deviceManagementConfigurationSettingGroupCollectionDefinition
description: Crie um novo objeto deviceManagementConfigurationSettingGroupCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 687484aac13f66a71abf3988d39960f3acf8e13e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146892"
---
# <a name="create-devicemanagementconfigurationsettinggroupcollectiondefinition"></a><span data-ttu-id="b5ccc-103">Criar deviceManagementConfigurationSettingGroupCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="b5ccc-103">Create deviceManagementConfigurationSettingGroupCollectionDefinition</span></span>

<span data-ttu-id="b5ccc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5ccc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5ccc-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b5ccc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5ccc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b5ccc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5ccc-107">Crie um novo [objeto deviceManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-107">Create a new [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5ccc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b5ccc-108">Prerequisites</span></span>
<span data-ttu-id="b5ccc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5ccc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5ccc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5ccc-111">Permission type</span></span>|<span data-ttu-id="b5ccc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5ccc-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5ccc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5ccc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5ccc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5ccc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5ccc-116">Not supported.</span></span>|
|<span data-ttu-id="b5ccc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5ccc-117">Application</span></span>|<span data-ttu-id="b5ccc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5ccc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5ccc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5ccc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="b5ccc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5ccc-120">Request headers</span></span>
|<span data-ttu-id="b5ccc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b5ccc-121">Header</span></span>|<span data-ttu-id="b5ccc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b5ccc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5ccc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5ccc-123">Authorization</span></span>|<span data-ttu-id="b5ccc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5ccc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5ccc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b5ccc-125">Accept</span></span>|<span data-ttu-id="b5ccc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5ccc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5ccc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5ccc-127">Request body</span></span>
<span data-ttu-id="b5ccc-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementConfigurationSettingGroupCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="b5ccc-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingGroupCollectionDefinition object.</span></span>

<span data-ttu-id="b5ccc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationSettingGroupCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="b5ccc-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingGroupCollectionDefinition.</span></span>

|<span data-ttu-id="b5ccc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5ccc-130">Property</span></span>|<span data-ttu-id="b5ccc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5ccc-131">Type</span></span>|<span data-ttu-id="b5ccc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5ccc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5ccc-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="b5ccc-133">applicability</span></span>|[<span data-ttu-id="b5ccc-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="b5ccc-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="b5ccc-135">Detalhes sobre qual configuração de dispositivo é aplicável em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="b5ccc-136">accessTypes</span></span>|[<span data-ttu-id="b5ccc-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="b5ccc-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="b5ccc-138">Modo de acesso de leitura/gravação da configuração Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b5ccc-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="b5ccc-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="b5ccc-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="b5ccc-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="b5ccc-140">keywords</span></span>|<span data-ttu-id="b5ccc-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ccc-141">String collection</span></span>|<span data-ttu-id="b5ccc-142">Tokens que para pesquisar configurações em Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="b5ccc-143">infoUrls</span></span>|<span data-ttu-id="b5ccc-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ccc-144">String collection</span></span>|<span data-ttu-id="b5ccc-145">Lista de links mais informações para a configuração podem ser encontradas em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="b5ccc-146">occurrence</span></span>|[<span data-ttu-id="b5ccc-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="b5ccc-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="b5ccc-148">Indica se a configuração é necessária ou não Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="b5ccc-149">baseUri</span></span>|<span data-ttu-id="b5ccc-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ccc-150">String</span></span>|<span data-ttu-id="b5ccc-151">Caminho base CSP Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="b5ccc-152">offsetUri</span></span>|<span data-ttu-id="b5ccc-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ccc-153">String</span></span>|<span data-ttu-id="b5ccc-154">Caminho de deslocamento CSP da Base Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b5ccc-155">rootDefinitionId</span></span>|<span data-ttu-id="b5ccc-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ccc-156">String</span></span>|<span data-ttu-id="b5ccc-157">Definição de configuração raiz se a configuração for uma configuração filho.</span><span class="sxs-lookup"><span data-stu-id="b5ccc-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="b5ccc-158">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="b5ccc-159">categoryId</span></span>|<span data-ttu-id="b5ccc-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ccc-160">String</span></span>|<span data-ttu-id="b5ccc-161">Especifica o grupo de área no qual a configuração está configurada em um provedor de serviços de configuração especificado (CSP) Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="b5ccc-162">settingUsage</span></span>|[<span data-ttu-id="b5ccc-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="b5ccc-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="b5ccc-164">Tipo de configuração, por exemplo, configuração e conformidade Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b5ccc-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="b5ccc-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="b5ccc-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="b5ccc-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="b5ccc-166">uxBehavior</span></span>|[<span data-ttu-id="b5ccc-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="b5ccc-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="b5ccc-168">Definindo a representação do tipo de controle no UX Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b5ccc-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="b5ccc-169">Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="b5ccc-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="b5ccc-170">visibility</span><span class="sxs-lookup"><span data-stu-id="b5ccc-170">visibility</span></span>|[<span data-ttu-id="b5ccc-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="b5ccc-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="b5ccc-172">Definindo o escopo de visibilidade como UX Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b5ccc-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="b5ccc-173">Os valores possíveis são: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="b5ccc-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="b5ccc-174">id</span><span class="sxs-lookup"><span data-stu-id="b5ccc-174">id</span></span>|<span data-ttu-id="b5ccc-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ccc-175">String</span></span>|<span data-ttu-id="b5ccc-176">Identificador do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-176">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-177">descrição</span><span class="sxs-lookup"><span data-stu-id="b5ccc-177">description</span></span>|<span data-ttu-id="b5ccc-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ccc-178">String</span></span>|<span data-ttu-id="b5ccc-179">Descrição do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-179">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-180">helpText</span><span class="sxs-lookup"><span data-stu-id="b5ccc-180">helpText</span></span>|<span data-ttu-id="b5ccc-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ccc-181">String</span></span>|<span data-ttu-id="b5ccc-182">Texto de ajuda do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-182">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-183">nome</span><span class="sxs-lookup"><span data-stu-id="b5ccc-183">name</span></span>|<span data-ttu-id="b5ccc-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ccc-184">String</span></span>|<span data-ttu-id="b5ccc-185">Nome do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-185">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-186">displayName</span><span class="sxs-lookup"><span data-stu-id="b5ccc-186">displayName</span></span>|<span data-ttu-id="b5ccc-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ccc-187">String</span></span>|<span data-ttu-id="b5ccc-188">Nome de exibição do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-188">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-189">versão</span><span class="sxs-lookup"><span data-stu-id="b5ccc-189">version</span></span>|<span data-ttu-id="b5ccc-190">String</span><span class="sxs-lookup"><span data-stu-id="b5ccc-190">String</span></span>|<span data-ttu-id="b5ccc-191">Versão do item Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-191">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-192">childIds</span><span class="sxs-lookup"><span data-stu-id="b5ccc-192">childIds</span></span>|<span data-ttu-id="b5ccc-193">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ccc-193">String collection</span></span>|<span data-ttu-id="b5ccc-194">Configurações filho dependentes para esse grupo de configurações Herdadas de [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-194">Dependent child settings to this group of settings Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-195">dependentOn</span><span class="sxs-lookup"><span data-stu-id="b5ccc-195">dependentOn</span></span>|<span data-ttu-id="b5ccc-196">[Coleção deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-196">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="b5ccc-197">Lista de dependências do grupo de configurações Herdado de [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-197">List of Dependencies for the setting group Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-198">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="b5ccc-198">dependedOnBy</span></span>|<span data-ttu-id="b5ccc-199">[Coleção deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-199">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="b5ccc-200">Lista de configurações filho que dependem dessa configuração Herdada de [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b5ccc-200">List of child settings that depend on this setting Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="b5ccc-201">maximumCount</span><span class="sxs-lookup"><span data-stu-id="b5ccc-201">maximumCount</span></span>|<span data-ttu-id="b5ccc-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b5ccc-202">Int32</span></span>|<span data-ttu-id="b5ccc-203">Número máximo de contagem de grupos de configuração na coleção.</span><span class="sxs-lookup"><span data-stu-id="b5ccc-203">Maximum number of setting group count in the collection.</span></span> <span data-ttu-id="b5ccc-204">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="b5ccc-204">Valid values 1 to 100</span></span>|
|<span data-ttu-id="b5ccc-205">minimumCount</span><span class="sxs-lookup"><span data-stu-id="b5ccc-205">minimumCount</span></span>|<span data-ttu-id="b5ccc-206">Int32</span><span class="sxs-lookup"><span data-stu-id="b5ccc-206">Int32</span></span>|<span data-ttu-id="b5ccc-207">Número mínimo de contagem de grupos de configuração na coleção.</span><span class="sxs-lookup"><span data-stu-id="b5ccc-207">Minimum number of setting group count in the collection.</span></span> <span data-ttu-id="b5ccc-208">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="b5ccc-208">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="b5ccc-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5ccc-209">Response</span></span>
<span data-ttu-id="b5ccc-210">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5ccc-210">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5ccc-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5ccc-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5ccc-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5ccc-212">Request</span></span>
<span data-ttu-id="b5ccc-213">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5ccc-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 1569

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionDefinition",
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
  "childIds": [
    "Child Ids value"
  ],
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
  ],
  "maximumCount": 12,
  "minimumCount": 12
}
```

### <a name="response"></a><span data-ttu-id="b5ccc-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5ccc-214">Response</span></span>
<span data-ttu-id="b5ccc-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5ccc-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1618

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionDefinition",
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
  "id": "739da194-a194-739d-94a1-9d7394a19d73",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "childIds": [
    "Child Ids value"
  ],
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
  ],
  "maximumCount": 12,
  "minimumCount": 12
}
```




