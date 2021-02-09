---
title: Criar deviceManagementConfigurationSettingGroupCollectionDefinition
description: Crie um novo objeto deviceManagementConfigurationSettingGroupCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0eb43368c20fda197a6449db31ad29ec7f296b10
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156543"
---
# <a name="create-devicemanagementconfigurationsettinggroupcollectiondefinition"></a><span data-ttu-id="9e0c1-103">Criar deviceManagementConfigurationSettingGroupCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="9e0c1-103">Create deviceManagementConfigurationSettingGroupCollectionDefinition</span></span>

<span data-ttu-id="9e0c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e0c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e0c1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9e0c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e0c1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e0c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e0c1-107">Crie um novo [objeto deviceManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-107">Create a new [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e0c1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e0c1-108">Prerequisites</span></span>
<span data-ttu-id="9e0c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e0c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e0c1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e0c1-111">Permission type</span></span>|<span data-ttu-id="9e0c1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e0c1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e0c1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e0c1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e0c1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e0c1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e0c1-116">Not supported.</span></span>|
|<span data-ttu-id="9e0c1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e0c1-117">Application</span></span>|<span data-ttu-id="9e0c1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e0c1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e0c1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e0c1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="9e0c1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e0c1-120">Request headers</span></span>
|<span data-ttu-id="9e0c1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e0c1-121">Header</span></span>|<span data-ttu-id="9e0c1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9e0c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e0c1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e0c1-123">Authorization</span></span>|<span data-ttu-id="9e0c1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e0c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e0c1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9e0c1-125">Accept</span></span>|<span data-ttu-id="9e0c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e0c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e0c1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e0c1-127">Request body</span></span>
<span data-ttu-id="9e0c1-128">No corpo da solicitação, fornece uma representação JSON do objeto deviceManagementConfigurationSettingGroupCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="9e0c1-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingGroupCollectionDefinition object.</span></span>

<span data-ttu-id="9e0c1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationSettingGroupCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="9e0c1-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingGroupCollectionDefinition.</span></span>

|<span data-ttu-id="9e0c1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e0c1-130">Property</span></span>|<span data-ttu-id="9e0c1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e0c1-131">Type</span></span>|<span data-ttu-id="9e0c1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e0c1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e0c1-133">applicability</span><span class="sxs-lookup"><span data-stu-id="9e0c1-133">applicability</span></span>|[<span data-ttu-id="9e0c1-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="9e0c1-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="9e0c1-135">Detalhes sobre qual configuração de dispositivo é aplicável. Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="9e0c1-136">accessTypes</span></span>|[<span data-ttu-id="9e0c1-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="9e0c1-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="9e0c1-138">Modo de acesso de leitura/gravação da configuração Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9e0c1-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="9e0c1-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="9e0c1-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="9e0c1-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="9e0c1-140">keywords</span></span>|<span data-ttu-id="9e0c1-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e0c1-141">String collection</span></span>|<span data-ttu-id="9e0c1-142">Tokens que pesquisar configurações em Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="9e0c1-143">infoUrls</span></span>|<span data-ttu-id="9e0c1-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e0c1-144">String collection</span></span>|<span data-ttu-id="9e0c1-145">Lista de links que mais informações sobre a configuração podem ser encontradas Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="9e0c1-146">occurrence</span></span>|[<span data-ttu-id="9e0c1-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="9e0c1-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="9e0c1-148">Indica se a configuração é necessária ou não Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="9e0c1-149">baseUri</span></span>|<span data-ttu-id="9e0c1-150">String</span><span class="sxs-lookup"><span data-stu-id="9e0c1-150">String</span></span>|<span data-ttu-id="9e0c1-151">Caminho base do CSP [Herdado de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="9e0c1-152">offsetUri</span></span>|<span data-ttu-id="9e0c1-153">String</span><span class="sxs-lookup"><span data-stu-id="9e0c1-153">String</span></span>|<span data-ttu-id="9e0c1-154">Deslocamento do caminho do CSP da Base Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="9e0c1-155">rootDefinitionId</span></span>|<span data-ttu-id="9e0c1-156">String</span><span class="sxs-lookup"><span data-stu-id="9e0c1-156">String</span></span>|<span data-ttu-id="9e0c1-157">Definição de configuração raiz se a configuração for uma configuração filha.</span><span class="sxs-lookup"><span data-stu-id="9e0c1-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="9e0c1-158">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="9e0c1-159">categoryId</span></span>|<span data-ttu-id="9e0c1-160">String</span><span class="sxs-lookup"><span data-stu-id="9e0c1-160">String</span></span>|<span data-ttu-id="9e0c1-161">Especifica o grupo de área sob o qual a configuração é definida em um provedor de serviços de configuração (CSP) especificado. Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="9e0c1-162">settingUsage</span></span>|[<span data-ttu-id="9e0c1-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="9e0c1-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="9e0c1-164">Tipo de configuração, por exemplo, configuração e conformidade Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9e0c1-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="9e0c1-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="9e0c1-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="9e0c1-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="9e0c1-166">uxBehavior</span></span>|[<span data-ttu-id="9e0c1-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="9e0c1-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="9e0c1-168">Representação do tipo de controle de configuração na UX Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9e0c1-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="9e0c1-169">Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="9e0c1-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="9e0c1-170">id</span><span class="sxs-lookup"><span data-stu-id="9e0c1-170">id</span></span>|<span data-ttu-id="9e0c1-171">String</span><span class="sxs-lookup"><span data-stu-id="9e0c1-171">String</span></span>|<span data-ttu-id="9e0c1-172">Identificador do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-172">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-173">description</span><span class="sxs-lookup"><span data-stu-id="9e0c1-173">description</span></span>|<span data-ttu-id="9e0c1-174">String</span><span class="sxs-lookup"><span data-stu-id="9e0c1-174">String</span></span>|<span data-ttu-id="9e0c1-175">Descrição do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-175">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-176">helpText</span><span class="sxs-lookup"><span data-stu-id="9e0c1-176">helpText</span></span>|<span data-ttu-id="9e0c1-177">String</span><span class="sxs-lookup"><span data-stu-id="9e0c1-177">String</span></span>|<span data-ttu-id="9e0c1-178">Texto de ajuda do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-178">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-179">name</span><span class="sxs-lookup"><span data-stu-id="9e0c1-179">name</span></span>|<span data-ttu-id="9e0c1-180">String</span><span class="sxs-lookup"><span data-stu-id="9e0c1-180">String</span></span>|<span data-ttu-id="9e0c1-181">Nome do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-181">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-182">displayName</span><span class="sxs-lookup"><span data-stu-id="9e0c1-182">displayName</span></span>|<span data-ttu-id="9e0c1-183">String</span><span class="sxs-lookup"><span data-stu-id="9e0c1-183">String</span></span>|<span data-ttu-id="9e0c1-184">Nome de exibição do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-184">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-185">versão</span><span class="sxs-lookup"><span data-stu-id="9e0c1-185">version</span></span>|<span data-ttu-id="9e0c1-186">String</span><span class="sxs-lookup"><span data-stu-id="9e0c1-186">String</span></span>|<span data-ttu-id="9e0c1-187">Versão do item [Herdado de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-187">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-188">childIds</span><span class="sxs-lookup"><span data-stu-id="9e0c1-188">childIds</span></span>|<span data-ttu-id="9e0c1-189">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e0c1-189">String collection</span></span>|<span data-ttu-id="9e0c1-190">Configurações filho dependentes para esse grupo de configurações Herdado de [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-190">Dependent child settings to this group of settings Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-191">dependentOn</span><span class="sxs-lookup"><span data-stu-id="9e0c1-191">dependentOn</span></span>|<span data-ttu-id="9e0c1-192">[Coleção deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-192">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="9e0c1-193">Lista de dependências para o grupo de configurações Herdado [de deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-193">List of Dependencies for the setting group Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-194">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="9e0c1-194">dependedOnBy</span></span>|<span data-ttu-id="9e0c1-195">[Coleção deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-195">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="9e0c1-196">Lista de configurações filho que dependem dessa configuração Herdado de [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9e0c1-196">List of child settings that depend on this setting Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="9e0c1-197">maximumCount</span><span class="sxs-lookup"><span data-stu-id="9e0c1-197">maximumCount</span></span>|<span data-ttu-id="9e0c1-198">Int32</span><span class="sxs-lookup"><span data-stu-id="9e0c1-198">Int32</span></span>|<span data-ttu-id="9e0c1-199">Número máximo de definições de contagem de grupos na coleção.</span><span class="sxs-lookup"><span data-stu-id="9e0c1-199">Maximum number of setting group count in the collection.</span></span> <span data-ttu-id="9e0c1-200">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="9e0c1-200">Valid values 1 to 100</span></span>|
|<span data-ttu-id="9e0c1-201">minimumCount</span><span class="sxs-lookup"><span data-stu-id="9e0c1-201">minimumCount</span></span>|<span data-ttu-id="9e0c1-202">Int32</span><span class="sxs-lookup"><span data-stu-id="9e0c1-202">Int32</span></span>|<span data-ttu-id="9e0c1-203">Número mínimo de contagem de grupos de configuração na coleção.</span><span class="sxs-lookup"><span data-stu-id="9e0c1-203">Minimum number of setting group count in the collection.</span></span> <span data-ttu-id="9e0c1-204">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="9e0c1-204">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="9e0c1-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e0c1-205">Response</span></span>
<span data-ttu-id="9e0c1-206">Se tiver êxito, este método retornará um código de resposta e um objeto `201 Created` [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e0c1-206">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e0c1-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e0c1-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e0c1-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e0c1-208">Request</span></span>
<span data-ttu-id="9e0c1-209">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e0c1-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 1533

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

### <a name="response"></a><span data-ttu-id="9e0c1-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e0c1-210">Response</span></span>
<span data-ttu-id="9e0c1-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e0c1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1582

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




