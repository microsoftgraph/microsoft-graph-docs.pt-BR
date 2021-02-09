---
title: Atualizar deviceManagementConfigurationSettingGroupDefinition
description: Atualizar as propriedades de um objeto deviceManagementConfigurationSettingGroupDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 61c2d97af46e718d31eace72ac2b19c437410bb4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158916"
---
# <a name="update-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="674e7-103">Atualizar deviceManagementConfigurationSettingGroupDefinition</span><span class="sxs-lookup"><span data-stu-id="674e7-103">Update deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="674e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="674e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="674e7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="674e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="674e7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="674e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="674e7-107">Atualizar as propriedades de um [objeto deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-107">Update the properties of a [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="674e7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="674e7-108">Prerequisites</span></span>
<span data-ttu-id="674e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="674e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="674e7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="674e7-111">Permission type</span></span>|<span data-ttu-id="674e7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="674e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="674e7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="674e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="674e7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="674e7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="674e7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="674e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="674e7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="674e7-116">Not supported.</span></span>|
|<span data-ttu-id="674e7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="674e7-117">Application</span></span>|<span data-ttu-id="674e7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="674e7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="674e7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="674e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="674e7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="674e7-120">Request headers</span></span>
|<span data-ttu-id="674e7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="674e7-121">Header</span></span>|<span data-ttu-id="674e7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="674e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="674e7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="674e7-123">Authorization</span></span>|<span data-ttu-id="674e7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="674e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="674e7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="674e7-125">Accept</span></span>|<span data-ttu-id="674e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="674e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="674e7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="674e7-127">Request body</span></span>
<span data-ttu-id="674e7-128">No corpo da solicitação, fornece uma representação JSON do [objeto deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

<span data-ttu-id="674e7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="674e7-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md).</span></span>

|<span data-ttu-id="674e7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="674e7-130">Property</span></span>|<span data-ttu-id="674e7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="674e7-131">Type</span></span>|<span data-ttu-id="674e7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="674e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="674e7-133">applicability</span><span class="sxs-lookup"><span data-stu-id="674e7-133">applicability</span></span>|[<span data-ttu-id="674e7-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="674e7-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="674e7-135">Detalhes sobre qual configuração de dispositivo é aplicável. Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="674e7-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="674e7-136">accessTypes</span></span>|[<span data-ttu-id="674e7-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="674e7-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="674e7-138">Modo de acesso de leitura/gravação da configuração Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="674e7-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="674e7-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="674e7-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="674e7-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="674e7-140">keywords</span></span>|<span data-ttu-id="674e7-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="674e7-141">String collection</span></span>|<span data-ttu-id="674e7-142">Tokens que pesquisar configurações em Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="674e7-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="674e7-143">infoUrls</span></span>|<span data-ttu-id="674e7-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="674e7-144">String collection</span></span>|<span data-ttu-id="674e7-145">Lista de links que mais informações sobre a configuração podem ser encontradas Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="674e7-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="674e7-146">occurrence</span></span>|[<span data-ttu-id="674e7-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="674e7-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="674e7-148">Indica se a configuração é necessária ou não Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="674e7-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="674e7-149">baseUri</span></span>|<span data-ttu-id="674e7-150">String</span><span class="sxs-lookup"><span data-stu-id="674e7-150">String</span></span>|<span data-ttu-id="674e7-151">Caminho base do CSP [Herdado de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="674e7-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="674e7-152">offsetUri</span></span>|<span data-ttu-id="674e7-153">String</span><span class="sxs-lookup"><span data-stu-id="674e7-153">String</span></span>|<span data-ttu-id="674e7-154">Deslocamento do caminho do CSP da Base Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="674e7-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="674e7-155">rootDefinitionId</span></span>|<span data-ttu-id="674e7-156">String</span><span class="sxs-lookup"><span data-stu-id="674e7-156">String</span></span>|<span data-ttu-id="674e7-157">Definição de configuração raiz se a configuração for uma configuração filha.</span><span class="sxs-lookup"><span data-stu-id="674e7-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="674e7-158">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="674e7-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="674e7-159">categoryId</span></span>|<span data-ttu-id="674e7-160">String</span><span class="sxs-lookup"><span data-stu-id="674e7-160">String</span></span>|<span data-ttu-id="674e7-161">Especifica o grupo de área sob o qual a configuração é definida em um provedor de serviços de configuração (CSP) especificado. Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="674e7-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="674e7-162">settingUsage</span></span>|[<span data-ttu-id="674e7-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="674e7-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="674e7-164">Tipo de configuração, por exemplo, configuração e conformidade Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="674e7-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="674e7-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="674e7-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="674e7-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="674e7-166">uxBehavior</span></span>|[<span data-ttu-id="674e7-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="674e7-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="674e7-168">Representação do tipo de controle de configuração na UX Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="674e7-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="674e7-169">Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="674e7-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="674e7-170">id</span><span class="sxs-lookup"><span data-stu-id="674e7-170">id</span></span>|<span data-ttu-id="674e7-171">String</span><span class="sxs-lookup"><span data-stu-id="674e7-171">String</span></span>|<span data-ttu-id="674e7-172">Identificador do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-172">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="674e7-173">description</span><span class="sxs-lookup"><span data-stu-id="674e7-173">description</span></span>|<span data-ttu-id="674e7-174">String</span><span class="sxs-lookup"><span data-stu-id="674e7-174">String</span></span>|<span data-ttu-id="674e7-175">Descrição do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-175">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="674e7-176">helpText</span><span class="sxs-lookup"><span data-stu-id="674e7-176">helpText</span></span>|<span data-ttu-id="674e7-177">String</span><span class="sxs-lookup"><span data-stu-id="674e7-177">String</span></span>|<span data-ttu-id="674e7-178">Texto de ajuda do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-178">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="674e7-179">name</span><span class="sxs-lookup"><span data-stu-id="674e7-179">name</span></span>|<span data-ttu-id="674e7-180">String</span><span class="sxs-lookup"><span data-stu-id="674e7-180">String</span></span>|<span data-ttu-id="674e7-181">Nome do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-181">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="674e7-182">displayName</span><span class="sxs-lookup"><span data-stu-id="674e7-182">displayName</span></span>|<span data-ttu-id="674e7-183">String</span><span class="sxs-lookup"><span data-stu-id="674e7-183">String</span></span>|<span data-ttu-id="674e7-184">Nome de exibição do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-184">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="674e7-185">versão</span><span class="sxs-lookup"><span data-stu-id="674e7-185">version</span></span>|<span data-ttu-id="674e7-186">String</span><span class="sxs-lookup"><span data-stu-id="674e7-186">String</span></span>|<span data-ttu-id="674e7-187">Versão do item [Herdado de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-187">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="674e7-188">childIds</span><span class="sxs-lookup"><span data-stu-id="674e7-188">childIds</span></span>|<span data-ttu-id="674e7-189">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="674e7-189">String collection</span></span>|<span data-ttu-id="674e7-190">Configurações de filho dependentes para esse grupo de configurações</span><span class="sxs-lookup"><span data-stu-id="674e7-190">Dependent child settings to this group of settings</span></span>|
|<span data-ttu-id="674e7-191">dependentOn</span><span class="sxs-lookup"><span data-stu-id="674e7-191">dependentOn</span></span>|<span data-ttu-id="674e7-192">[Coleção deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-192">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="674e7-193">Lista de dependências para o grupo de configurações</span><span class="sxs-lookup"><span data-stu-id="674e7-193">List of Dependencies for the setting group</span></span>|
|<span data-ttu-id="674e7-194">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="674e7-194">dependedOnBy</span></span>|<span data-ttu-id="674e7-195">[Coleção deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="674e7-195">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="674e7-196">Lista de configurações filho que dependem dessa configuração</span><span class="sxs-lookup"><span data-stu-id="674e7-196">List of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="674e7-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="674e7-197">Response</span></span>
<span data-ttu-id="674e7-198">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="674e7-198">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="674e7-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="674e7-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="674e7-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="674e7-200">Request</span></span>
<span data-ttu-id="674e7-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="674e7-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1477

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupDefinition",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="674e7-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="674e7-202">Response</span></span>
<span data-ttu-id="674e7-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="674e7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1526

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupDefinition",
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
  "id": "95dc9604-9604-95dc-0496-dc950496dc95",
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
  ]
}
```




