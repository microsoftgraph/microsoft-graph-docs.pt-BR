---
title: Criar deviceManagementConfigurationSimpleSettingCollectionDefinition
description: Criar um novo objeto deviceManagementConfigurationSimpleSettingCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 98ab146aeddc8163aa5f27d06a12be76e7ee450f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241330"
---
# <a name="create-devicemanagementconfigurationsimplesettingcollectiondefinition"></a><span data-ttu-id="224fa-103">Criar deviceManagementConfigurationSimpleSettingCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="224fa-103">Create deviceManagementConfigurationSimpleSettingCollectionDefinition</span></span>

<span data-ttu-id="224fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="224fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="224fa-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="224fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="224fa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="224fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="224fa-107">Criar um novo objeto [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="224fa-107">Create a new [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="224fa-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="224fa-108">Prerequisites</span></span>
<span data-ttu-id="224fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="224fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="224fa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="224fa-111">Permission type</span></span>|<span data-ttu-id="224fa-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="224fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="224fa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="224fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="224fa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="224fa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="224fa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="224fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="224fa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="224fa-116">Not supported.</span></span>|
|<span data-ttu-id="224fa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="224fa-117">Application</span></span>|<span data-ttu-id="224fa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="224fa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="224fa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="224fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="224fa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="224fa-120">Request headers</span></span>
|<span data-ttu-id="224fa-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="224fa-121">Header</span></span>|<span data-ttu-id="224fa-122">Valor</span><span class="sxs-lookup"><span data-stu-id="224fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="224fa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="224fa-123">Authorization</span></span>|<span data-ttu-id="224fa-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="224fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="224fa-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="224fa-125">Accept</span></span>|<span data-ttu-id="224fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="224fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="224fa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="224fa-127">Request body</span></span>
<span data-ttu-id="224fa-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementConfigurationSimpleSettingCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="224fa-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSimpleSettingCollectionDefinition object.</span></span>

<span data-ttu-id="224fa-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationSimpleSettingCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="224fa-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSimpleSettingCollectionDefinition.</span></span>

|<span data-ttu-id="224fa-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="224fa-130">Property</span></span>|<span data-ttu-id="224fa-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="224fa-131">Type</span></span>|<span data-ttu-id="224fa-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="224fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="224fa-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="224fa-133">applicability</span></span>|[<span data-ttu-id="224fa-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="224fa-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="224fa-135">Detalhes qual configuração de dispositivo é aplicável no herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="224fa-136">accessTypes</span></span>|[<span data-ttu-id="224fa-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="224fa-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="224fa-138">Modo de acesso de leitura/gravação da configuração herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="224fa-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="224fa-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="224fa-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="224fa-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="224fa-140">keywords</span></span>|<span data-ttu-id="224fa-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="224fa-141">String collection</span></span>|<span data-ttu-id="224fa-142">Tokens que pesquisam configurações em herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="224fa-143">infoUrls</span></span>|<span data-ttu-id="224fa-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="224fa-144">String collection</span></span>|<span data-ttu-id="224fa-145">Lista de links mais informações para a configuração podem ser encontradas em herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-146">ocorrência</span><span class="sxs-lookup"><span data-stu-id="224fa-146">occurrence</span></span>|[<span data-ttu-id="224fa-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="224fa-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="224fa-148">Indica se a configuração é obrigatória ou não herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="224fa-149">baseUri</span></span>|<span data-ttu-id="224fa-150">String</span><span class="sxs-lookup"><span data-stu-id="224fa-150">String</span></span>|<span data-ttu-id="224fa-151">Caminho de CSP base herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="224fa-152">offsetUri</span></span>|<span data-ttu-id="224fa-153">String</span><span class="sxs-lookup"><span data-stu-id="224fa-153">String</span></span>|<span data-ttu-id="224fa-154">Caminho de CSP offset da base herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="224fa-155">rootDefinitionId</span></span>|<span data-ttu-id="224fa-156">String</span><span class="sxs-lookup"><span data-stu-id="224fa-156">String</span></span>|<span data-ttu-id="224fa-157">Definição da configuração raiz se a configuração for uma configuração de filho.</span><span class="sxs-lookup"><span data-stu-id="224fa-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="224fa-158">Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="224fa-159">categoryId</span></span>|<span data-ttu-id="224fa-160">String</span><span class="sxs-lookup"><span data-stu-id="224fa-160">String</span></span>|<span data-ttu-id="224fa-161">Especifica o grupo de área no qual a configuração é configurada em um provedor de serviços de configuração especificado (CSP) herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="224fa-162">settingUsage</span></span>|[<span data-ttu-id="224fa-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="224fa-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="224fa-164">Tipo de configuração, por exemplo, configuração e conformidade herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="224fa-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="224fa-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="224fa-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="224fa-166">id</span><span class="sxs-lookup"><span data-stu-id="224fa-166">id</span></span>|<span data-ttu-id="224fa-167">String</span><span class="sxs-lookup"><span data-stu-id="224fa-167">String</span></span>|<span data-ttu-id="224fa-168">Identificador do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-169">description</span><span class="sxs-lookup"><span data-stu-id="224fa-169">description</span></span>|<span data-ttu-id="224fa-170">String</span><span class="sxs-lookup"><span data-stu-id="224fa-170">String</span></span>|<span data-ttu-id="224fa-171">Descrição do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-172">helpText</span><span class="sxs-lookup"><span data-stu-id="224fa-172">helpText</span></span>|<span data-ttu-id="224fa-173">String</span><span class="sxs-lookup"><span data-stu-id="224fa-173">String</span></span>|<span data-ttu-id="224fa-174">Texto de ajuda do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-175">nome</span><span class="sxs-lookup"><span data-stu-id="224fa-175">name</span></span>|<span data-ttu-id="224fa-176">String</span><span class="sxs-lookup"><span data-stu-id="224fa-176">String</span></span>|<span data-ttu-id="224fa-177">Nome do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-178">displayName</span><span class="sxs-lookup"><span data-stu-id="224fa-178">displayName</span></span>|<span data-ttu-id="224fa-179">String</span><span class="sxs-lookup"><span data-stu-id="224fa-179">String</span></span>|<span data-ttu-id="224fa-180">Nome para exibição do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-181">versão</span><span class="sxs-lookup"><span data-stu-id="224fa-181">version</span></span>|<span data-ttu-id="224fa-182">String</span><span class="sxs-lookup"><span data-stu-id="224fa-182">String</span></span>|<span data-ttu-id="224fa-183">Versão de item herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-184">valueDefinition</span><span class="sxs-lookup"><span data-stu-id="224fa-184">valueDefinition</span></span>|[<span data-ttu-id="224fa-185">deviceManagementConfigurationSettingValueDefinition</span><span class="sxs-lookup"><span data-stu-id="224fa-185">deviceManagementConfigurationSettingValueDefinition</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)|<span data-ttu-id="224fa-186">Definição do valor dessa configuração herdado de [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-186">Definition of the value for this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-187">defaultValue</span><span class="sxs-lookup"><span data-stu-id="224fa-187">defaultValue</span></span>|[<span data-ttu-id="224fa-188">deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="224fa-188">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="224fa-189">Valor de configuração padrão para essa configuração herdada de [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-189">Default setting value for this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-190">dependente</span><span class="sxs-lookup"><span data-stu-id="224fa-190">dependentOn</span></span>|<span data-ttu-id="224fa-191">coleção [deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-191">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="224fa-192">lista de configurações pai essa configuração depende de herdada de [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-192">list of parent settings this setting is dependent on Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-193">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="224fa-193">dependedOnBy</span></span>|<span data-ttu-id="224fa-194">coleção [deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-194">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="224fa-195">lista de configurações filhas que dependem dessa configuração herdada de [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="224fa-195">list of child settings that depend on this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="224fa-196">maximumCount</span><span class="sxs-lookup"><span data-stu-id="224fa-196">maximumCount</span></span>|<span data-ttu-id="224fa-197">Int32</span><span class="sxs-lookup"><span data-stu-id="224fa-197">Int32</span></span>|<span data-ttu-id="224fa-198">Número máximo de configurações simples na coleção.</span><span class="sxs-lookup"><span data-stu-id="224fa-198">Maximum number of simple settings in the collection.</span></span> <span data-ttu-id="224fa-199">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="224fa-199">Valid values 1 to 100</span></span>|
|<span data-ttu-id="224fa-200">minimumCount</span><span class="sxs-lookup"><span data-stu-id="224fa-200">minimumCount</span></span>|<span data-ttu-id="224fa-201">Int32</span><span class="sxs-lookup"><span data-stu-id="224fa-201">Int32</span></span>|<span data-ttu-id="224fa-202">Número mínimo de configurações simples na coleção.</span><span class="sxs-lookup"><span data-stu-id="224fa-202">Minimum number of simple settings in the collection.</span></span> <span data-ttu-id="224fa-203">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="224fa-203">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="224fa-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="224fa-204">Response</span></span>
<span data-ttu-id="224fa-205">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="224fa-205">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="224fa-206">Exemplo</span><span class="sxs-lookup"><span data-stu-id="224fa-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="224fa-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="224fa-207">Request</span></span>
<span data-ttu-id="224fa-208">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="224fa-208">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 9183

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionDefinition",
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
  ],
  "maximumCount": 12,
  "minimumCount": 12
}
```

### <a name="response"></a><span data-ttu-id="224fa-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="224fa-209">Response</span></span>
<span data-ttu-id="224fa-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="224fa-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9232

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionDefinition",
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
  "id": "cb4abda1-bda1-cb4a-a1bd-4acba1bd4acb",
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
  ],
  "maximumCount": 12,
  "minimumCount": 12
}
```




