---
title: Atualizar deviceManagementConfigurationChoiceSettingCollectionDefinition
description: Atualiza as propriedades de um objeto deviceManagementConfigurationChoiceSettingCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c65ad896fd14e0661d1b11f3f2a6d326e998ff7a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301480"
---
# <a name="update-devicemanagementconfigurationchoicesettingcollectiondefinition"></a><span data-ttu-id="ad1ee-103">Atualizar deviceManagementConfigurationChoiceSettingCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="ad1ee-103">Update deviceManagementConfigurationChoiceSettingCollectionDefinition</span></span>

<span data-ttu-id="ad1ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad1ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad1ee-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad1ee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad1ee-107">Atualiza as propriedades de um objeto [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="ad1ee-107">Update the properties of a [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad1ee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ad1ee-108">Prerequisites</span></span>
<span data-ttu-id="ad1ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad1ee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad1ee-111">Permission type</span></span>|<span data-ttu-id="ad1ee-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad1ee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad1ee-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad1ee-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ad1ee-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad1ee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-116">Not supported.</span></span>|
|<span data-ttu-id="ad1ee-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad1ee-117">Application</span></span>|<span data-ttu-id="ad1ee-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad1ee-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad1ee-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad1ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="ad1ee-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad1ee-120">Request headers</span></span>
|<span data-ttu-id="ad1ee-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad1ee-121">Header</span></span>|<span data-ttu-id="ad1ee-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ad1ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad1ee-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad1ee-123">Authorization</span></span>|<span data-ttu-id="ad1ee-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad1ee-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ad1ee-125">Accept</span></span>|<span data-ttu-id="ad1ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad1ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad1ee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad1ee-127">Request body</span></span>
<span data-ttu-id="ad1ee-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="ad1ee-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) object.</span></span>

<span data-ttu-id="ad1ee-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md).</span></span>

|<span data-ttu-id="ad1ee-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad1ee-130">Property</span></span>|<span data-ttu-id="ad1ee-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad1ee-131">Type</span></span>|<span data-ttu-id="ad1ee-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad1ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad1ee-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="ad1ee-133">applicability</span></span>|[<span data-ttu-id="ad1ee-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="ad1ee-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="ad1ee-135">Detalhes qual configuração de dispositivo é aplicável no herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ad1ee-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="ad1ee-136">accessTypes</span></span>|[<span data-ttu-id="ad1ee-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="ad1ee-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="ad1ee-138">Modo de acesso de leitura/gravação da configuração herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="ad1ee-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="ad1ee-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="ad1ee-140">keywords</span></span>|<span data-ttu-id="ad1ee-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad1ee-141">String collection</span></span>|<span data-ttu-id="ad1ee-142">Tokens que pesquisam configurações em herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ad1ee-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="ad1ee-143">infoUrls</span></span>|<span data-ttu-id="ad1ee-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad1ee-144">String collection</span></span>|<span data-ttu-id="ad1ee-145">Lista de links mais informações para a configuração podem ser encontradas em herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ad1ee-146">ocorrência</span><span class="sxs-lookup"><span data-stu-id="ad1ee-146">occurrence</span></span>|[<span data-ttu-id="ad1ee-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="ad1ee-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="ad1ee-148">Indica se a configuração é obrigatória ou não herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ad1ee-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="ad1ee-149">baseUri</span></span>|<span data-ttu-id="ad1ee-150">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-150">String</span></span>|<span data-ttu-id="ad1ee-151">Caminho de CSP base herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ad1ee-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="ad1ee-152">offsetUri</span></span>|<span data-ttu-id="ad1ee-153">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-153">String</span></span>|<span data-ttu-id="ad1ee-154">Caminho de CSP offset da base herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ad1ee-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ad1ee-155">rootDefinitionId</span></span>|<span data-ttu-id="ad1ee-156">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-156">String</span></span>|<span data-ttu-id="ad1ee-157">Definição da configuração raiz se a configuração for uma configuração de filho.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="ad1ee-158">Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ad1ee-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="ad1ee-159">categoryId</span></span>|<span data-ttu-id="ad1ee-160">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-160">String</span></span>|<span data-ttu-id="ad1ee-161">Especifica o grupo de área no qual a configuração é configurada em um provedor de serviços de configuração especificado (CSP) herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ad1ee-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="ad1ee-162">settingUsage</span></span>|[<span data-ttu-id="ad1ee-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="ad1ee-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="ad1ee-164">Tipo de configuração, por exemplo, configuração e conformidade herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="ad1ee-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="ad1ee-166">id</span><span class="sxs-lookup"><span data-stu-id="ad1ee-166">id</span></span>|<span data-ttu-id="ad1ee-167">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-167">String</span></span>|<span data-ttu-id="ad1ee-168">Identificador do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ad1ee-169">description</span><span class="sxs-lookup"><span data-stu-id="ad1ee-169">description</span></span>|<span data-ttu-id="ad1ee-170">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-170">String</span></span>|<span data-ttu-id="ad1ee-171">Descrição do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ad1ee-172">helpText</span><span class="sxs-lookup"><span data-stu-id="ad1ee-172">helpText</span></span>|<span data-ttu-id="ad1ee-173">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-173">String</span></span>|<span data-ttu-id="ad1ee-174">Texto de ajuda do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ad1ee-175">nome</span><span class="sxs-lookup"><span data-stu-id="ad1ee-175">name</span></span>|<span data-ttu-id="ad1ee-176">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-176">String</span></span>|<span data-ttu-id="ad1ee-177">Nome do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ad1ee-178">displayName</span><span class="sxs-lookup"><span data-stu-id="ad1ee-178">displayName</span></span>|<span data-ttu-id="ad1ee-179">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-179">String</span></span>|<span data-ttu-id="ad1ee-180">Nome para exibição do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ad1ee-181">versão</span><span class="sxs-lookup"><span data-stu-id="ad1ee-181">version</span></span>|<span data-ttu-id="ad1ee-182">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-182">String</span></span>|<span data-ttu-id="ad1ee-183">Versão de item herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="ad1ee-184">options</span><span class="sxs-lookup"><span data-stu-id="ad1ee-184">options</span></span>|<span data-ttu-id="ad1ee-185">coleção [deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-185">[deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md) collection</span></span>|<span data-ttu-id="ad1ee-186">Opções para a configuração que pode ser selecionada herdada de [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-186">Options for the setting that can be selected Inherited from [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span></span>|
|<span data-ttu-id="ad1ee-187">defaultoptionid</span><span class="sxs-lookup"><span data-stu-id="ad1ee-187">defaultOptionId</span></span>|<span data-ttu-id="ad1ee-188">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-188">String</span></span>|<span data-ttu-id="ad1ee-189">Opção padrão para a configuração de opção herdada de [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-189">Default option for choice setting Inherited from [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span></span>|
|<span data-ttu-id="ad1ee-190">maximumCount</span><span class="sxs-lookup"><span data-stu-id="ad1ee-190">maximumCount</span></span>|<span data-ttu-id="ad1ee-191">Int32</span><span class="sxs-lookup"><span data-stu-id="ad1ee-191">Int32</span></span>|<span data-ttu-id="ad1ee-192">Número máximo de opções na coleção.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-192">Maximum number of choices in the collection.</span></span> <span data-ttu-id="ad1ee-193">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="ad1ee-193">Valid values 1 to 100</span></span>|
|<span data-ttu-id="ad1ee-194">minimumCount</span><span class="sxs-lookup"><span data-stu-id="ad1ee-194">minimumCount</span></span>|<span data-ttu-id="ad1ee-195">Int32</span><span class="sxs-lookup"><span data-stu-id="ad1ee-195">Int32</span></span>|<span data-ttu-id="ad1ee-196">Número mínimo de opções na coleção.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-196">Minimum number of choices in the collection.</span></span> <span data-ttu-id="ad1ee-197">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="ad1ee-197">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="ad1ee-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad1ee-198">Response</span></span>
<span data-ttu-id="ad1ee-199">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-199">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad1ee-200">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad1ee-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad1ee-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad1ee-201">Request</span></span>
<span data-ttu-id="ad1ee-202">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 9933

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionDefinition",
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
  "options": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinition",
      "optionValue": {
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
      "itemId": "Item Id value",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value"
    }
  ],
  "defaultOptionId": "Default Option Id value",
  "maximumCount": 12,
  "minimumCount": 12
}
```

### <a name="response"></a><span data-ttu-id="ad1ee-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad1ee-203">Response</span></span>
<span data-ttu-id="ad1ee-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9982

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionDefinition",
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
  "id": "eb03fdca-fdca-eb03-cafd-03ebcafd03eb",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "options": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinition",
      "optionValue": {
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
      "itemId": "Item Id value",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value"
    }
  ],
  "defaultOptionId": "Default Option Id value",
  "maximumCount": 12,
  "minimumCount": 12
}
```




