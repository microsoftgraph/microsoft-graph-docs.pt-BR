---
title: Atualizar deviceManagementConfigurationSimpleSettingCollectionDefinition
description: Atualiza as propriedades de um objeto deviceManagementConfigurationSimpleSettingCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9f55e7a6437da546d0b762ed6fd329d833efeae4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241326"
---
# <a name="update-devicemanagementconfigurationsimplesettingcollectiondefinition"></a><span data-ttu-id="8b5cb-103">Atualizar deviceManagementConfigurationSimpleSettingCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="8b5cb-103">Update deviceManagementConfigurationSimpleSettingCollectionDefinition</span></span>

<span data-ttu-id="8b5cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b5cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b5cb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8b5cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b5cb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8b5cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b5cb-107">Atualiza as propriedades de um objeto [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="8b5cb-107">Update the properties of a [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b5cb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8b5cb-108">Prerequisites</span></span>
<span data-ttu-id="8b5cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b5cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b5cb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b5cb-111">Permission type</span></span>|<span data-ttu-id="8b5cb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b5cb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8b5cb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b5cb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8b5cb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b5cb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b5cb-116">Not supported.</span></span>|
|<span data-ttu-id="8b5cb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b5cb-117">Application</span></span>|<span data-ttu-id="8b5cb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b5cb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b5cb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b5cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="8b5cb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b5cb-120">Request headers</span></span>
|<span data-ttu-id="8b5cb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8b5cb-121">Header</span></span>|<span data-ttu-id="8b5cb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8b5cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b5cb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b5cb-123">Authorization</span></span>|<span data-ttu-id="8b5cb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b5cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b5cb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8b5cb-125">Accept</span></span>|<span data-ttu-id="8b5cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b5cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b5cb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b5cb-127">Request body</span></span>
<span data-ttu-id="8b5cb-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="8b5cb-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object.</span></span>

<span data-ttu-id="8b5cb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8b5cb-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md).</span></span>

|<span data-ttu-id="8b5cb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b5cb-130">Property</span></span>|<span data-ttu-id="8b5cb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b5cb-131">Type</span></span>|<span data-ttu-id="8b5cb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b5cb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b5cb-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="8b5cb-133">applicability</span></span>|[<span data-ttu-id="8b5cb-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="8b5cb-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="8b5cb-135">Detalhes qual configuração de dispositivo é aplicável no herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="8b5cb-136">accessTypes</span></span>|[<span data-ttu-id="8b5cb-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="8b5cb-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="8b5cb-138">Modo de acesso de leitura/gravação da configuração herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8b5cb-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="8b5cb-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="8b5cb-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="8b5cb-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="8b5cb-140">keywords</span></span>|<span data-ttu-id="8b5cb-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b5cb-141">String collection</span></span>|<span data-ttu-id="8b5cb-142">Tokens que pesquisam configurações em herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="8b5cb-143">infoUrls</span></span>|<span data-ttu-id="8b5cb-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b5cb-144">String collection</span></span>|<span data-ttu-id="8b5cb-145">Lista de links mais informações para a configuração podem ser encontradas em herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-146">ocorrência</span><span class="sxs-lookup"><span data-stu-id="8b5cb-146">occurrence</span></span>|[<span data-ttu-id="8b5cb-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="8b5cb-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="8b5cb-148">Indica se a configuração é obrigatória ou não herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="8b5cb-149">baseUri</span></span>|<span data-ttu-id="8b5cb-150">String</span><span class="sxs-lookup"><span data-stu-id="8b5cb-150">String</span></span>|<span data-ttu-id="8b5cb-151">Caminho de CSP base herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="8b5cb-152">offsetUri</span></span>|<span data-ttu-id="8b5cb-153">String</span><span class="sxs-lookup"><span data-stu-id="8b5cb-153">String</span></span>|<span data-ttu-id="8b5cb-154">Caminho de CSP offset da base herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8b5cb-155">rootDefinitionId</span></span>|<span data-ttu-id="8b5cb-156">String</span><span class="sxs-lookup"><span data-stu-id="8b5cb-156">String</span></span>|<span data-ttu-id="8b5cb-157">Definição da configuração raiz se a configuração for uma configuração de filho.</span><span class="sxs-lookup"><span data-stu-id="8b5cb-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="8b5cb-158">Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="8b5cb-159">categoryId</span></span>|<span data-ttu-id="8b5cb-160">String</span><span class="sxs-lookup"><span data-stu-id="8b5cb-160">String</span></span>|<span data-ttu-id="8b5cb-161">Especifica o grupo de área no qual a configuração é configurada em um provedor de serviços de configuração especificado (CSP) herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="8b5cb-162">settingUsage</span></span>|[<span data-ttu-id="8b5cb-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="8b5cb-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="8b5cb-164">Tipo de configuração, por exemplo, configuração e conformidade herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8b5cb-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="8b5cb-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="8b5cb-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="8b5cb-166">id</span><span class="sxs-lookup"><span data-stu-id="8b5cb-166">id</span></span>|<span data-ttu-id="8b5cb-167">String</span><span class="sxs-lookup"><span data-stu-id="8b5cb-167">String</span></span>|<span data-ttu-id="8b5cb-168">Identificador do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-169">description</span><span class="sxs-lookup"><span data-stu-id="8b5cb-169">description</span></span>|<span data-ttu-id="8b5cb-170">String</span><span class="sxs-lookup"><span data-stu-id="8b5cb-170">String</span></span>|<span data-ttu-id="8b5cb-171">Descrição do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-172">helpText</span><span class="sxs-lookup"><span data-stu-id="8b5cb-172">helpText</span></span>|<span data-ttu-id="8b5cb-173">String</span><span class="sxs-lookup"><span data-stu-id="8b5cb-173">String</span></span>|<span data-ttu-id="8b5cb-174">Texto de ajuda do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-175">nome</span><span class="sxs-lookup"><span data-stu-id="8b5cb-175">name</span></span>|<span data-ttu-id="8b5cb-176">String</span><span class="sxs-lookup"><span data-stu-id="8b5cb-176">String</span></span>|<span data-ttu-id="8b5cb-177">Nome do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-178">displayName</span><span class="sxs-lookup"><span data-stu-id="8b5cb-178">displayName</span></span>|<span data-ttu-id="8b5cb-179">String</span><span class="sxs-lookup"><span data-stu-id="8b5cb-179">String</span></span>|<span data-ttu-id="8b5cb-180">Nome para exibição do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-181">versão</span><span class="sxs-lookup"><span data-stu-id="8b5cb-181">version</span></span>|<span data-ttu-id="8b5cb-182">String</span><span class="sxs-lookup"><span data-stu-id="8b5cb-182">String</span></span>|<span data-ttu-id="8b5cb-183">Versão de item herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-184">valueDefinition</span><span class="sxs-lookup"><span data-stu-id="8b5cb-184">valueDefinition</span></span>|[<span data-ttu-id="8b5cb-185">deviceManagementConfigurationSettingValueDefinition</span><span class="sxs-lookup"><span data-stu-id="8b5cb-185">deviceManagementConfigurationSettingValueDefinition</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)|<span data-ttu-id="8b5cb-186">Definição do valor dessa configuração herdado de [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-186">Definition of the value for this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-187">defaultValue</span><span class="sxs-lookup"><span data-stu-id="8b5cb-187">defaultValue</span></span>|[<span data-ttu-id="8b5cb-188">deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="8b5cb-188">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="8b5cb-189">Valor de configuração padrão para essa configuração herdada de [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-189">Default setting value for this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-190">dependente</span><span class="sxs-lookup"><span data-stu-id="8b5cb-190">dependentOn</span></span>|<span data-ttu-id="8b5cb-191">coleção [deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-191">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="8b5cb-192">lista de configurações pai essa configuração depende de herdada de [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-192">list of parent settings this setting is dependent on Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-193">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="8b5cb-193">dependedOnBy</span></span>|<span data-ttu-id="8b5cb-194">coleção [deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-194">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="8b5cb-195">lista de configurações filhas que dependem dessa configuração herdada de [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b5cb-195">list of child settings that depend on this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="8b5cb-196">maximumCount</span><span class="sxs-lookup"><span data-stu-id="8b5cb-196">maximumCount</span></span>|<span data-ttu-id="8b5cb-197">Int32</span><span class="sxs-lookup"><span data-stu-id="8b5cb-197">Int32</span></span>|<span data-ttu-id="8b5cb-198">Número máximo de configurações simples na coleção.</span><span class="sxs-lookup"><span data-stu-id="8b5cb-198">Maximum number of simple settings in the collection.</span></span> <span data-ttu-id="8b5cb-199">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="8b5cb-199">Valid values 1 to 100</span></span>|
|<span data-ttu-id="8b5cb-200">minimumCount</span><span class="sxs-lookup"><span data-stu-id="8b5cb-200">minimumCount</span></span>|<span data-ttu-id="8b5cb-201">Int32</span><span class="sxs-lookup"><span data-stu-id="8b5cb-201">Int32</span></span>|<span data-ttu-id="8b5cb-202">Número mínimo de configurações simples na coleção.</span><span class="sxs-lookup"><span data-stu-id="8b5cb-202">Minimum number of simple settings in the collection.</span></span> <span data-ttu-id="8b5cb-203">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="8b5cb-203">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="8b5cb-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b5cb-204">Response</span></span>
<span data-ttu-id="8b5cb-205">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b5cb-205">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b5cb-206">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b5cb-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b5cb-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b5cb-207">Request</span></span>
<span data-ttu-id="8b5cb-208">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b5cb-208">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
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

### <a name="response"></a><span data-ttu-id="8b5cb-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b5cb-209">Response</span></span>
<span data-ttu-id="8b5cb-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8b5cb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




