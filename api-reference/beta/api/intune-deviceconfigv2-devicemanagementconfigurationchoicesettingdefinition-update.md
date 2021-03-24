---
title: Atualizar deviceManagementConfigurationChoiceSettingDefinition
description: Atualize as propriedades de um objeto deviceManagementConfigurationChoiceSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 56dd2a5f74eed2bceceb4d0e1b6becd8b8b9a389
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129288"
---
# <a name="update-devicemanagementconfigurationchoicesettingdefinition"></a><span data-ttu-id="7ac6d-103">Atualizar deviceManagementConfigurationChoiceSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="7ac6d-103">Update deviceManagementConfigurationChoiceSettingDefinition</span></span>

<span data-ttu-id="7ac6d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ac6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ac6d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ac6d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ac6d-107">Atualize as propriedades de [um objeto deviceManagementConfigurationChoiceSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-107">Update the properties of a [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ac6d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7ac6d-108">Prerequisites</span></span>
<span data-ttu-id="7ac6d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ac6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ac6d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ac6d-111">Permission type</span></span>|<span data-ttu-id="7ac6d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ac6d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ac6d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ac6d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ac6d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ac6d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-116">Not supported.</span></span>|
|<span data-ttu-id="7ac6d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ac6d-117">Application</span></span>|<span data-ttu-id="7ac6d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ac6d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ac6d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ac6d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="7ac6d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ac6d-120">Request headers</span></span>
|<span data-ttu-id="7ac6d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ac6d-121">Header</span></span>|<span data-ttu-id="7ac6d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7ac6d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ac6d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ac6d-123">Authorization</span></span>|<span data-ttu-id="7ac6d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ac6d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7ac6d-125">Accept</span></span>|<span data-ttu-id="7ac6d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ac6d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ac6d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ac6d-127">Request body</span></span>
<span data-ttu-id="7ac6d-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementConfigurationChoiceSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object.</span></span>

<span data-ttu-id="7ac6d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7ac6d-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md).</span></span>

|<span data-ttu-id="7ac6d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ac6d-130">Property</span></span>|<span data-ttu-id="7ac6d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ac6d-131">Type</span></span>|<span data-ttu-id="7ac6d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ac6d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ac6d-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="7ac6d-133">applicability</span></span>|[<span data-ttu-id="7ac6d-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="7ac6d-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="7ac6d-135">Detalhes sobre qual configuração de dispositivo é aplicável em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7ac6d-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="7ac6d-136">accessTypes</span></span>|[<span data-ttu-id="7ac6d-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="7ac6d-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="7ac6d-138">Modo de acesso de leitura/gravação da configuração Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7ac6d-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="7ac6d-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="7ac6d-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="7ac6d-140">keywords</span></span>|<span data-ttu-id="7ac6d-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac6d-141">String collection</span></span>|<span data-ttu-id="7ac6d-142">Tokens que para pesquisar configurações em Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7ac6d-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="7ac6d-143">infoUrls</span></span>|<span data-ttu-id="7ac6d-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac6d-144">String collection</span></span>|<span data-ttu-id="7ac6d-145">Lista de links mais informações para a configuração podem ser encontradas em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7ac6d-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="7ac6d-146">occurrence</span></span>|[<span data-ttu-id="7ac6d-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="7ac6d-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="7ac6d-148">Indica se a configuração é necessária ou não Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7ac6d-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="7ac6d-149">baseUri</span></span>|<span data-ttu-id="7ac6d-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac6d-150">String</span></span>|<span data-ttu-id="7ac6d-151">Caminho base CSP Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7ac6d-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="7ac6d-152">offsetUri</span></span>|<span data-ttu-id="7ac6d-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac6d-153">String</span></span>|<span data-ttu-id="7ac6d-154">Caminho de deslocamento CSP da Base Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7ac6d-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7ac6d-155">rootDefinitionId</span></span>|<span data-ttu-id="7ac6d-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac6d-156">String</span></span>|<span data-ttu-id="7ac6d-157">Definição de configuração raiz se a configuração for uma configuração filho.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="7ac6d-158">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7ac6d-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="7ac6d-159">categoryId</span></span>|<span data-ttu-id="7ac6d-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac6d-160">String</span></span>|<span data-ttu-id="7ac6d-161">Especifica o grupo de área no qual a configuração está configurada em um provedor de serviços de configuração especificado (CSP) Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7ac6d-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="7ac6d-162">settingUsage</span></span>|[<span data-ttu-id="7ac6d-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="7ac6d-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="7ac6d-164">Tipo de configuração, por exemplo, configuração e conformidade Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7ac6d-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="7ac6d-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="7ac6d-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="7ac6d-166">uxBehavior</span></span>|[<span data-ttu-id="7ac6d-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="7ac6d-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="7ac6d-168">Definindo a representação do tipo de controle no UX Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7ac6d-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="7ac6d-169">Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="7ac6d-170">visibility</span><span class="sxs-lookup"><span data-stu-id="7ac6d-170">visibility</span></span>|[<span data-ttu-id="7ac6d-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="7ac6d-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="7ac6d-172">Definindo o escopo de visibilidade como UX Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7ac6d-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="7ac6d-173">Os valores possíveis são: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="7ac6d-174">id</span><span class="sxs-lookup"><span data-stu-id="7ac6d-174">id</span></span>|<span data-ttu-id="7ac6d-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac6d-175">String</span></span>|<span data-ttu-id="7ac6d-176">Identificador do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-176">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7ac6d-177">descrição</span><span class="sxs-lookup"><span data-stu-id="7ac6d-177">description</span></span>|<span data-ttu-id="7ac6d-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac6d-178">String</span></span>|<span data-ttu-id="7ac6d-179">Descrição do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-179">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7ac6d-180">helpText</span><span class="sxs-lookup"><span data-stu-id="7ac6d-180">helpText</span></span>|<span data-ttu-id="7ac6d-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac6d-181">String</span></span>|<span data-ttu-id="7ac6d-182">Texto de ajuda do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-182">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7ac6d-183">nome</span><span class="sxs-lookup"><span data-stu-id="7ac6d-183">name</span></span>|<span data-ttu-id="7ac6d-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac6d-184">String</span></span>|<span data-ttu-id="7ac6d-185">Nome do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-185">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7ac6d-186">displayName</span><span class="sxs-lookup"><span data-stu-id="7ac6d-186">displayName</span></span>|<span data-ttu-id="7ac6d-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac6d-187">String</span></span>|<span data-ttu-id="7ac6d-188">Nome de exibição do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-188">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7ac6d-189">versão</span><span class="sxs-lookup"><span data-stu-id="7ac6d-189">version</span></span>|<span data-ttu-id="7ac6d-190">String</span><span class="sxs-lookup"><span data-stu-id="7ac6d-190">String</span></span>|<span data-ttu-id="7ac6d-191">Versão do item Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-191">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7ac6d-192">options</span><span class="sxs-lookup"><span data-stu-id="7ac6d-192">options</span></span>|<span data-ttu-id="7ac6d-193">[Coleção deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ac6d-193">[deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md) collection</span></span>|<span data-ttu-id="7ac6d-194">Opções para a configuração que pode ser selecionada</span><span class="sxs-lookup"><span data-stu-id="7ac6d-194">Options for the setting that can be selected</span></span>|
|<span data-ttu-id="7ac6d-195">defaultOptionId</span><span class="sxs-lookup"><span data-stu-id="7ac6d-195">defaultOptionId</span></span>|<span data-ttu-id="7ac6d-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac6d-196">String</span></span>|<span data-ttu-id="7ac6d-197">Opção padrão para a configuração de opção</span><span class="sxs-lookup"><span data-stu-id="7ac6d-197">Default option for choice setting</span></span>|



## <a name="response"></a><span data-ttu-id="7ac6d-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ac6d-198">Response</span></span>
<span data-ttu-id="7ac6d-199">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-199">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ac6d-200">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ac6d-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ac6d-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ac6d-201">Request</span></span>
<span data-ttu-id="7ac6d-202">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 9942

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingDefinition",
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
  "defaultOptionId": "Default Option Id value"
}
```

### <a name="response"></a><span data-ttu-id="7ac6d-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ac6d-203">Response</span></span>
<span data-ttu-id="7ac6d-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ac6d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9991

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingDefinition",
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
  "id": "30b2258a-258a-30b2-8a25-b2308a25b230",
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
  "defaultOptionId": "Default Option Id value"
}
```




