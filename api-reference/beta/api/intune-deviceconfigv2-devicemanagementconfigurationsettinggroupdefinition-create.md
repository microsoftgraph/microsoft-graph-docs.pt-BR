---
title: Criar deviceManagementConfigurationSettingGroupDefinition
description: Crie um novo objeto deviceManagementConfigurationSettingGroupDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf8c4d88e032f6a5f388cc62e118791e7cbb8300
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161317"
---
# <a name="create-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="6337a-103">Criar deviceManagementConfigurationSettingGroupDefinition</span><span class="sxs-lookup"><span data-stu-id="6337a-103">Create deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="6337a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6337a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6337a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6337a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6337a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6337a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6337a-107">Crie um novo [objeto deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-107">Create a new [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6337a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6337a-108">Prerequisites</span></span>
<span data-ttu-id="6337a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6337a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6337a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6337a-111">Permission type</span></span>|<span data-ttu-id="6337a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6337a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6337a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6337a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6337a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6337a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6337a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6337a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6337a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6337a-116">Not supported.</span></span>|
|<span data-ttu-id="6337a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6337a-117">Application</span></span>|<span data-ttu-id="6337a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6337a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6337a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6337a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="6337a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6337a-120">Request headers</span></span>
|<span data-ttu-id="6337a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6337a-121">Header</span></span>|<span data-ttu-id="6337a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6337a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6337a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6337a-123">Authorization</span></span>|<span data-ttu-id="6337a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6337a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6337a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6337a-125">Accept</span></span>|<span data-ttu-id="6337a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6337a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6337a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6337a-127">Request body</span></span>
<span data-ttu-id="6337a-128">No corpo da solicitação, fornece uma representação JSON do objeto deviceManagementConfigurationSettingGroupDefinition.</span><span class="sxs-lookup"><span data-stu-id="6337a-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingGroupDefinition object.</span></span>

<span data-ttu-id="6337a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationSettingGroupDefinition.</span><span class="sxs-lookup"><span data-stu-id="6337a-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingGroupDefinition.</span></span>

|<span data-ttu-id="6337a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6337a-130">Property</span></span>|<span data-ttu-id="6337a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6337a-131">Type</span></span>|<span data-ttu-id="6337a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6337a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6337a-133">applicability</span><span class="sxs-lookup"><span data-stu-id="6337a-133">applicability</span></span>|[<span data-ttu-id="6337a-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="6337a-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="6337a-135">Detalhes sobre qual configuração de dispositivo é aplicável. Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6337a-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="6337a-136">accessTypes</span></span>|[<span data-ttu-id="6337a-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="6337a-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="6337a-138">Modo de acesso de leitura/gravação da configuração Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6337a-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="6337a-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="6337a-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="6337a-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="6337a-140">keywords</span></span>|<span data-ttu-id="6337a-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6337a-141">String collection</span></span>|<span data-ttu-id="6337a-142">Tokens que pesquisar configurações em Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6337a-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="6337a-143">infoUrls</span></span>|<span data-ttu-id="6337a-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6337a-144">String collection</span></span>|<span data-ttu-id="6337a-145">Lista de links que mais informações sobre a configuração podem ser encontradas Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6337a-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="6337a-146">occurrence</span></span>|[<span data-ttu-id="6337a-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="6337a-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="6337a-148">Indica se a configuração é necessária ou não Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6337a-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="6337a-149">baseUri</span></span>|<span data-ttu-id="6337a-150">String</span><span class="sxs-lookup"><span data-stu-id="6337a-150">String</span></span>|<span data-ttu-id="6337a-151">Caminho base do CSP [Herdado de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6337a-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="6337a-152">offsetUri</span></span>|<span data-ttu-id="6337a-153">String</span><span class="sxs-lookup"><span data-stu-id="6337a-153">String</span></span>|<span data-ttu-id="6337a-154">Deslocamento do caminho do CSP da Base Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6337a-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="6337a-155">rootDefinitionId</span></span>|<span data-ttu-id="6337a-156">String</span><span class="sxs-lookup"><span data-stu-id="6337a-156">String</span></span>|<span data-ttu-id="6337a-157">Definição de configuração raiz se a configuração for uma configuração filha.</span><span class="sxs-lookup"><span data-stu-id="6337a-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="6337a-158">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6337a-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="6337a-159">categoryId</span></span>|<span data-ttu-id="6337a-160">String</span><span class="sxs-lookup"><span data-stu-id="6337a-160">String</span></span>|<span data-ttu-id="6337a-161">Especifica o grupo de área sob o qual a configuração é definida em um provedor de serviços de configuração (CSP) especificado. Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6337a-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="6337a-162">settingUsage</span></span>|[<span data-ttu-id="6337a-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="6337a-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="6337a-164">Tipo de configuração, por exemplo, configuração e conformidade Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6337a-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="6337a-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="6337a-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="6337a-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="6337a-166">uxBehavior</span></span>|[<span data-ttu-id="6337a-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="6337a-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="6337a-168">Representação do tipo de controle de configuração na UX Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6337a-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="6337a-169">Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="6337a-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="6337a-170">id</span><span class="sxs-lookup"><span data-stu-id="6337a-170">id</span></span>|<span data-ttu-id="6337a-171">String</span><span class="sxs-lookup"><span data-stu-id="6337a-171">String</span></span>|<span data-ttu-id="6337a-172">Identificador do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-172">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6337a-173">description</span><span class="sxs-lookup"><span data-stu-id="6337a-173">description</span></span>|<span data-ttu-id="6337a-174">String</span><span class="sxs-lookup"><span data-stu-id="6337a-174">String</span></span>|<span data-ttu-id="6337a-175">Descrição do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-175">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6337a-176">helpText</span><span class="sxs-lookup"><span data-stu-id="6337a-176">helpText</span></span>|<span data-ttu-id="6337a-177">String</span><span class="sxs-lookup"><span data-stu-id="6337a-177">String</span></span>|<span data-ttu-id="6337a-178">Texto de ajuda do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-178">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6337a-179">name</span><span class="sxs-lookup"><span data-stu-id="6337a-179">name</span></span>|<span data-ttu-id="6337a-180">String</span><span class="sxs-lookup"><span data-stu-id="6337a-180">String</span></span>|<span data-ttu-id="6337a-181">Nome do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-181">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6337a-182">displayName</span><span class="sxs-lookup"><span data-stu-id="6337a-182">displayName</span></span>|<span data-ttu-id="6337a-183">String</span><span class="sxs-lookup"><span data-stu-id="6337a-183">String</span></span>|<span data-ttu-id="6337a-184">Nome de exibição do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-184">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6337a-185">versão</span><span class="sxs-lookup"><span data-stu-id="6337a-185">version</span></span>|<span data-ttu-id="6337a-186">String</span><span class="sxs-lookup"><span data-stu-id="6337a-186">String</span></span>|<span data-ttu-id="6337a-187">Versão do item [Herdado de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-187">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6337a-188">childIds</span><span class="sxs-lookup"><span data-stu-id="6337a-188">childIds</span></span>|<span data-ttu-id="6337a-189">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6337a-189">String collection</span></span>|<span data-ttu-id="6337a-190">Configurações de filho dependentes para esse grupo de configurações</span><span class="sxs-lookup"><span data-stu-id="6337a-190">Dependent child settings to this group of settings</span></span>|
|<span data-ttu-id="6337a-191">dependentOn</span><span class="sxs-lookup"><span data-stu-id="6337a-191">dependentOn</span></span>|<span data-ttu-id="6337a-192">[Coleção deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-192">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="6337a-193">Lista de dependências para o grupo de configurações</span><span class="sxs-lookup"><span data-stu-id="6337a-193">List of Dependencies for the setting group</span></span>|
|<span data-ttu-id="6337a-194">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="6337a-194">dependedOnBy</span></span>|<span data-ttu-id="6337a-195">[Coleção deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="6337a-195">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="6337a-196">Lista de configurações filho que dependem dessa configuração</span><span class="sxs-lookup"><span data-stu-id="6337a-196">List of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="6337a-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="6337a-197">Response</span></span>
<span data-ttu-id="6337a-198">Se tiver êxito, este método retornará um código de resposta e um objeto `201 Created` [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6337a-198">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6337a-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6337a-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="6337a-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6337a-200">Request</span></span>
<span data-ttu-id="6337a-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6337a-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
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

### <a name="response"></a><span data-ttu-id="6337a-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="6337a-202">Response</span></span>
<span data-ttu-id="6337a-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6337a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




