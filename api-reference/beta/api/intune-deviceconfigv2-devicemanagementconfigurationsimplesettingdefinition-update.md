---
title: Atualizar deviceManagementConfigurationSimpleSettingDefinition
description: Atualiza as propriedades de um objeto deviceManagementConfigurationSimpleSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 46c74c5f8d47ef975e4d533ef825a75ca4cfcd1d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301479"
---
# <a name="update-devicemanagementconfigurationsimplesettingdefinition"></a><span data-ttu-id="46712-103">Atualizar deviceManagementConfigurationSimpleSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="46712-103">Update deviceManagementConfigurationSimpleSettingDefinition</span></span>

<span data-ttu-id="46712-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46712-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46712-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="46712-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46712-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46712-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46712-107">Atualiza as propriedades de um objeto [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="46712-107">Update the properties of a [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46712-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="46712-108">Prerequisites</span></span>
<span data-ttu-id="46712-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46712-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46712-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46712-111">Permission type</span></span>|<span data-ttu-id="46712-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="46712-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46712-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46712-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46712-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46712-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46712-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46712-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46712-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46712-116">Not supported.</span></span>|
|<span data-ttu-id="46712-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46712-117">Application</span></span>|<span data-ttu-id="46712-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46712-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46712-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46712-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="46712-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46712-120">Request headers</span></span>
|<span data-ttu-id="46712-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="46712-121">Header</span></span>|<span data-ttu-id="46712-122">Valor</span><span class="sxs-lookup"><span data-stu-id="46712-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46712-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="46712-123">Authorization</span></span>|<span data-ttu-id="46712-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46712-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46712-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="46712-125">Accept</span></span>|<span data-ttu-id="46712-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46712-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46712-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46712-127">Request body</span></span>
<span data-ttu-id="46712-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="46712-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) object.</span></span>

<span data-ttu-id="46712-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="46712-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md).</span></span>

|<span data-ttu-id="46712-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46712-130">Property</span></span>|<span data-ttu-id="46712-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="46712-131">Type</span></span>|<span data-ttu-id="46712-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="46712-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46712-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="46712-133">applicability</span></span>|[<span data-ttu-id="46712-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="46712-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="46712-135">Detalhes qual configuração de dispositivo é aplicável no herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="46712-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="46712-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="46712-136">accessTypes</span></span>|[<span data-ttu-id="46712-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="46712-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="46712-138">Modo de acesso de leitura/gravação da configuração herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="46712-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="46712-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="46712-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="46712-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="46712-140">keywords</span></span>|<span data-ttu-id="46712-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="46712-141">String collection</span></span>|<span data-ttu-id="46712-142">Tokens que pesquisam configurações em herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="46712-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="46712-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="46712-143">infoUrls</span></span>|<span data-ttu-id="46712-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="46712-144">String collection</span></span>|<span data-ttu-id="46712-145">Lista de links mais informações para a configuração podem ser encontradas em herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="46712-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="46712-146">ocorrência</span><span class="sxs-lookup"><span data-stu-id="46712-146">occurrence</span></span>|[<span data-ttu-id="46712-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="46712-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="46712-148">Indica se a configuração é obrigatória ou não herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="46712-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="46712-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="46712-149">baseUri</span></span>|<span data-ttu-id="46712-150">String</span><span class="sxs-lookup"><span data-stu-id="46712-150">String</span></span>|<span data-ttu-id="46712-151">Caminho de CSP base herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="46712-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="46712-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="46712-152">offsetUri</span></span>|<span data-ttu-id="46712-153">String</span><span class="sxs-lookup"><span data-stu-id="46712-153">String</span></span>|<span data-ttu-id="46712-154">Caminho de CSP offset da base herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="46712-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="46712-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="46712-155">rootDefinitionId</span></span>|<span data-ttu-id="46712-156">String</span><span class="sxs-lookup"><span data-stu-id="46712-156">String</span></span>|<span data-ttu-id="46712-157">Definição da configuração raiz se a configuração for uma configuração de filho.</span><span class="sxs-lookup"><span data-stu-id="46712-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="46712-158">Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="46712-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="46712-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="46712-159">categoryId</span></span>|<span data-ttu-id="46712-160">String</span><span class="sxs-lookup"><span data-stu-id="46712-160">String</span></span>|<span data-ttu-id="46712-161">Especifica o grupo de área no qual a configuração é configurada em um provedor de serviços de configuração especificado (CSP) herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="46712-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="46712-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="46712-162">settingUsage</span></span>|[<span data-ttu-id="46712-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="46712-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="46712-164">Tipo de configuração, por exemplo, configuração e conformidade herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="46712-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="46712-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="46712-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="46712-166">id</span><span class="sxs-lookup"><span data-stu-id="46712-166">id</span></span>|<span data-ttu-id="46712-167">String</span><span class="sxs-lookup"><span data-stu-id="46712-167">String</span></span>|<span data-ttu-id="46712-168">Identificador do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="46712-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="46712-169">description</span><span class="sxs-lookup"><span data-stu-id="46712-169">description</span></span>|<span data-ttu-id="46712-170">String</span><span class="sxs-lookup"><span data-stu-id="46712-170">String</span></span>|<span data-ttu-id="46712-171">Descrição do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="46712-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="46712-172">helpText</span><span class="sxs-lookup"><span data-stu-id="46712-172">helpText</span></span>|<span data-ttu-id="46712-173">String</span><span class="sxs-lookup"><span data-stu-id="46712-173">String</span></span>|<span data-ttu-id="46712-174">Texto de ajuda do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="46712-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="46712-175">nome</span><span class="sxs-lookup"><span data-stu-id="46712-175">name</span></span>|<span data-ttu-id="46712-176">String</span><span class="sxs-lookup"><span data-stu-id="46712-176">String</span></span>|<span data-ttu-id="46712-177">Nome do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="46712-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="46712-178">displayName</span><span class="sxs-lookup"><span data-stu-id="46712-178">displayName</span></span>|<span data-ttu-id="46712-179">String</span><span class="sxs-lookup"><span data-stu-id="46712-179">String</span></span>|<span data-ttu-id="46712-180">Nome para exibição do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="46712-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="46712-181">versão</span><span class="sxs-lookup"><span data-stu-id="46712-181">version</span></span>|<span data-ttu-id="46712-182">String</span><span class="sxs-lookup"><span data-stu-id="46712-182">String</span></span>|<span data-ttu-id="46712-183">Versão de item herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="46712-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="46712-184">valueDefinition</span><span class="sxs-lookup"><span data-stu-id="46712-184">valueDefinition</span></span>|[<span data-ttu-id="46712-185">deviceManagementConfigurationSettingValueDefinition</span><span class="sxs-lookup"><span data-stu-id="46712-185">deviceManagementConfigurationSettingValueDefinition</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)|<span data-ttu-id="46712-186">Definição do valor dessa configuração</span><span class="sxs-lookup"><span data-stu-id="46712-186">Definition of the value for this setting</span></span>|
|<span data-ttu-id="46712-187">defaultValue</span><span class="sxs-lookup"><span data-stu-id="46712-187">defaultValue</span></span>|[<span data-ttu-id="46712-188">deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="46712-188">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="46712-189">Valor de configuração padrão para essa configuração</span><span class="sxs-lookup"><span data-stu-id="46712-189">Default setting value for this setting</span></span>|
|<span data-ttu-id="46712-190">dependente</span><span class="sxs-lookup"><span data-stu-id="46712-190">dependentOn</span></span>|<span data-ttu-id="46712-191">coleção [deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="46712-191">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="46712-192">lista de configurações pai de que essa configuração depende</span><span class="sxs-lookup"><span data-stu-id="46712-192">list of parent settings this setting is dependent on</span></span>|
|<span data-ttu-id="46712-193">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="46712-193">dependedOnBy</span></span>|<span data-ttu-id="46712-194">coleção [deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="46712-194">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="46712-195">lista de configurações filhas que dependem dessa configuração</span><span class="sxs-lookup"><span data-stu-id="46712-195">list of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="46712-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="46712-196">Response</span></span>
<span data-ttu-id="46712-197">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46712-197">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46712-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46712-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="46712-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46712-199">Request</span></span>
<span data-ttu-id="46712-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46712-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 9127

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

### <a name="response"></a><span data-ttu-id="46712-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="46712-201">Response</span></span>
<span data-ttu-id="46712-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46712-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9176

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




