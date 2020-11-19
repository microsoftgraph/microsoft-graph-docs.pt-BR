---
title: Criar deviceManagementConfigurationSettingGroupCollectionDefinition
description: Criar um novo objeto deviceManagementConfigurationSettingGroupCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 863a4e9573cf83afb1f2b91334cc771c0036c383
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241350"
---
# <a name="create-devicemanagementconfigurationsettinggroupcollectiondefinition"></a><span data-ttu-id="6a09f-103">Criar deviceManagementConfigurationSettingGroupCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="6a09f-103">Create deviceManagementConfigurationSettingGroupCollectionDefinition</span></span>

<span data-ttu-id="6a09f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a09f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a09f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a09f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a09f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a09f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a09f-107">Criar um novo objeto [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="6a09f-107">Create a new [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a09f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a09f-108">Prerequisites</span></span>
<span data-ttu-id="6a09f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a09f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a09f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a09f-111">Permission type</span></span>|<span data-ttu-id="6a09f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6a09f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a09f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a09f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a09f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a09f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6a09f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a09f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a09f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a09f-116">Not supported.</span></span>|
|<span data-ttu-id="6a09f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a09f-117">Application</span></span>|<span data-ttu-id="6a09f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a09f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a09f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a09f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="6a09f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a09f-120">Request headers</span></span>
|<span data-ttu-id="6a09f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a09f-121">Header</span></span>|<span data-ttu-id="6a09f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6a09f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a09f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a09f-123">Authorization</span></span>|<span data-ttu-id="6a09f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a09f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a09f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a09f-125">Accept</span></span>|<span data-ttu-id="6a09f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a09f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a09f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a09f-127">Request body</span></span>
<span data-ttu-id="6a09f-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementConfigurationSettingGroupCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="6a09f-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingGroupCollectionDefinition object.</span></span>

<span data-ttu-id="6a09f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationSettingGroupCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="6a09f-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingGroupCollectionDefinition.</span></span>

|<span data-ttu-id="6a09f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a09f-130">Property</span></span>|<span data-ttu-id="6a09f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a09f-131">Type</span></span>|<span data-ttu-id="6a09f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a09f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a09f-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="6a09f-133">applicability</span></span>|[<span data-ttu-id="6a09f-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="6a09f-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="6a09f-135">Detalhes qual configuração de dispositivo é aplicável no herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="6a09f-136">accessTypes</span></span>|[<span data-ttu-id="6a09f-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="6a09f-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="6a09f-138">Modo de acesso de leitura/gravação da configuração herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6a09f-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="6a09f-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="6a09f-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="6a09f-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="6a09f-140">keywords</span></span>|<span data-ttu-id="6a09f-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a09f-141">String collection</span></span>|<span data-ttu-id="6a09f-142">Tokens que pesquisam configurações em herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="6a09f-143">infoUrls</span></span>|<span data-ttu-id="6a09f-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a09f-144">String collection</span></span>|<span data-ttu-id="6a09f-145">Lista de links mais informações para a configuração podem ser encontradas em herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-146">ocorrência</span><span class="sxs-lookup"><span data-stu-id="6a09f-146">occurrence</span></span>|[<span data-ttu-id="6a09f-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="6a09f-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="6a09f-148">Indica se a configuração é obrigatória ou não herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="6a09f-149">baseUri</span></span>|<span data-ttu-id="6a09f-150">String</span><span class="sxs-lookup"><span data-stu-id="6a09f-150">String</span></span>|<span data-ttu-id="6a09f-151">Caminho de CSP base herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="6a09f-152">offsetUri</span></span>|<span data-ttu-id="6a09f-153">String</span><span class="sxs-lookup"><span data-stu-id="6a09f-153">String</span></span>|<span data-ttu-id="6a09f-154">Caminho de CSP offset da base herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="6a09f-155">rootDefinitionId</span></span>|<span data-ttu-id="6a09f-156">String</span><span class="sxs-lookup"><span data-stu-id="6a09f-156">String</span></span>|<span data-ttu-id="6a09f-157">Definição da configuração raiz se a configuração for uma configuração de filho.</span><span class="sxs-lookup"><span data-stu-id="6a09f-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="6a09f-158">Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="6a09f-159">categoryId</span></span>|<span data-ttu-id="6a09f-160">String</span><span class="sxs-lookup"><span data-stu-id="6a09f-160">String</span></span>|<span data-ttu-id="6a09f-161">Especifica o grupo de área no qual a configuração é configurada em um provedor de serviços de configuração especificado (CSP) herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="6a09f-162">settingUsage</span></span>|[<span data-ttu-id="6a09f-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="6a09f-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="6a09f-164">Tipo de configuração, por exemplo, configuração e conformidade herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6a09f-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="6a09f-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="6a09f-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="6a09f-166">id</span><span class="sxs-lookup"><span data-stu-id="6a09f-166">id</span></span>|<span data-ttu-id="6a09f-167">String</span><span class="sxs-lookup"><span data-stu-id="6a09f-167">String</span></span>|<span data-ttu-id="6a09f-168">Identificador do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-169">description</span><span class="sxs-lookup"><span data-stu-id="6a09f-169">description</span></span>|<span data-ttu-id="6a09f-170">String</span><span class="sxs-lookup"><span data-stu-id="6a09f-170">String</span></span>|<span data-ttu-id="6a09f-171">Descrição do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-172">helpText</span><span class="sxs-lookup"><span data-stu-id="6a09f-172">helpText</span></span>|<span data-ttu-id="6a09f-173">String</span><span class="sxs-lookup"><span data-stu-id="6a09f-173">String</span></span>|<span data-ttu-id="6a09f-174">Texto de ajuda do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-175">nome</span><span class="sxs-lookup"><span data-stu-id="6a09f-175">name</span></span>|<span data-ttu-id="6a09f-176">String</span><span class="sxs-lookup"><span data-stu-id="6a09f-176">String</span></span>|<span data-ttu-id="6a09f-177">Nome do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-178">displayName</span><span class="sxs-lookup"><span data-stu-id="6a09f-178">displayName</span></span>|<span data-ttu-id="6a09f-179">String</span><span class="sxs-lookup"><span data-stu-id="6a09f-179">String</span></span>|<span data-ttu-id="6a09f-180">Nome para exibição do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-181">versão</span><span class="sxs-lookup"><span data-stu-id="6a09f-181">version</span></span>|<span data-ttu-id="6a09f-182">String</span><span class="sxs-lookup"><span data-stu-id="6a09f-182">String</span></span>|<span data-ttu-id="6a09f-183">Versão de item herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-184">childIds</span><span class="sxs-lookup"><span data-stu-id="6a09f-184">childIds</span></span>|<span data-ttu-id="6a09f-185">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a09f-185">String collection</span></span>|<span data-ttu-id="6a09f-186">Configurações filhas dependentes para este grupo de configurações herdadas de [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-186">Dependent child settings to this group of settings Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-187">dependente</span><span class="sxs-lookup"><span data-stu-id="6a09f-187">dependentOn</span></span>|<span data-ttu-id="6a09f-188">coleção [deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-188">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="6a09f-189">Lista de dependências para o grupo de configurações herdado de [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-189">List of Dependencies for the setting group Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-190">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="6a09f-190">dependedOnBy</span></span>|<span data-ttu-id="6a09f-191">coleção [deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-191">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="6a09f-192">Lista de configurações filhas que dependem dessa configuração herdada de [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a09f-192">List of child settings that depend on this setting Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="6a09f-193">maximumCount</span><span class="sxs-lookup"><span data-stu-id="6a09f-193">maximumCount</span></span>|<span data-ttu-id="6a09f-194">Int32</span><span class="sxs-lookup"><span data-stu-id="6a09f-194">Int32</span></span>|<span data-ttu-id="6a09f-195">Número máximo de contagem de grupo de configuração na coleção.</span><span class="sxs-lookup"><span data-stu-id="6a09f-195">Maximum number of setting group count in the collection.</span></span> <span data-ttu-id="6a09f-196">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="6a09f-196">Valid values 1 to 100</span></span>|
|<span data-ttu-id="6a09f-197">minimumCount</span><span class="sxs-lookup"><span data-stu-id="6a09f-197">minimumCount</span></span>|<span data-ttu-id="6a09f-198">Int32</span><span class="sxs-lookup"><span data-stu-id="6a09f-198">Int32</span></span>|<span data-ttu-id="6a09f-199">Número mínimo de configuração de contagem de grupo na coleção.</span><span class="sxs-lookup"><span data-stu-id="6a09f-199">Minimum number of setting group count in the collection.</span></span> <span data-ttu-id="6a09f-200">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="6a09f-200">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="6a09f-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a09f-201">Response</span></span>
<span data-ttu-id="6a09f-202">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a09f-202">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a09f-203">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a09f-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a09f-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a09f-204">Request</span></span>
<span data-ttu-id="6a09f-205">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a09f-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 1504

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

### <a name="response"></a><span data-ttu-id="6a09f-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a09f-206">Response</span></span>
<span data-ttu-id="6a09f-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a09f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1553

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




