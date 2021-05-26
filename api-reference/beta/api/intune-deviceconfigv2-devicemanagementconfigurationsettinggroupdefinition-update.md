---
title: Atualizar deviceManagementConfigurationSettingGroupDefinition
description: Atualize as propriedades de um objeto deviceManagementConfigurationSettingGroupDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 68338b0fe37a9f93911218298f07042e7a879c83
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665438"
---
# <a name="update-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="414ca-103">Atualizar deviceManagementConfigurationSettingGroupDefinition</span><span class="sxs-lookup"><span data-stu-id="414ca-103">Update deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="414ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="414ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="414ca-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="414ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="414ca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="414ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="414ca-107">Atualize as propriedades de [um objeto deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-107">Update the properties of a [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="414ca-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="414ca-108">Prerequisites</span></span>
<span data-ttu-id="414ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="414ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="414ca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="414ca-111">Permission type</span></span>|<span data-ttu-id="414ca-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="414ca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="414ca-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="414ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="414ca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="414ca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="414ca-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="414ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="414ca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="414ca-116">Not supported.</span></span>|
|<span data-ttu-id="414ca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="414ca-117">Application</span></span>|<span data-ttu-id="414ca-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="414ca-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="414ca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="414ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates/{deviceManagementConfigurationSettingTemplateId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="414ca-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="414ca-120">Request headers</span></span>
|<span data-ttu-id="414ca-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="414ca-121">Header</span></span>|<span data-ttu-id="414ca-122">Valor</span><span class="sxs-lookup"><span data-stu-id="414ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="414ca-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="414ca-123">Authorization</span></span>|<span data-ttu-id="414ca-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="414ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="414ca-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="414ca-125">Accept</span></span>|<span data-ttu-id="414ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="414ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="414ca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="414ca-127">Request body</span></span>
<span data-ttu-id="414ca-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

<span data-ttu-id="414ca-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="414ca-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md).</span></span>

|<span data-ttu-id="414ca-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="414ca-130">Property</span></span>|<span data-ttu-id="414ca-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="414ca-131">Type</span></span>|<span data-ttu-id="414ca-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="414ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="414ca-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="414ca-133">applicability</span></span>|[<span data-ttu-id="414ca-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="414ca-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="414ca-135">Detalhes sobre qual configuração de dispositivo é aplicável em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="414ca-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="414ca-136">accessTypes</span></span>|[<span data-ttu-id="414ca-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="414ca-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="414ca-138">Modo de acesso de leitura/gravação da configuração Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="414ca-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="414ca-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="414ca-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="414ca-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="414ca-140">keywords</span></span>|<span data-ttu-id="414ca-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="414ca-141">String collection</span></span>|<span data-ttu-id="414ca-142">Tokens que para pesquisar configurações em Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="414ca-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="414ca-143">infoUrls</span></span>|<span data-ttu-id="414ca-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="414ca-144">String collection</span></span>|<span data-ttu-id="414ca-145">Lista de links mais informações para a configuração podem ser encontradas em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="414ca-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="414ca-146">occurrence</span></span>|[<span data-ttu-id="414ca-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="414ca-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="414ca-148">Indica se a configuração é necessária ou não Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="414ca-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="414ca-149">baseUri</span></span>|<span data-ttu-id="414ca-150">String</span><span class="sxs-lookup"><span data-stu-id="414ca-150">String</span></span>|<span data-ttu-id="414ca-151">Caminho base CSP Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="414ca-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="414ca-152">offsetUri</span></span>|<span data-ttu-id="414ca-153">String</span><span class="sxs-lookup"><span data-stu-id="414ca-153">String</span></span>|<span data-ttu-id="414ca-154">Caminho de deslocamento CSP da Base Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="414ca-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="414ca-155">rootDefinitionId</span></span>|<span data-ttu-id="414ca-156">String</span><span class="sxs-lookup"><span data-stu-id="414ca-156">String</span></span>|<span data-ttu-id="414ca-157">Definição de configuração raiz se a configuração for uma configuração filho.</span><span class="sxs-lookup"><span data-stu-id="414ca-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="414ca-158">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="414ca-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="414ca-159">categoryId</span></span>|<span data-ttu-id="414ca-160">String</span><span class="sxs-lookup"><span data-stu-id="414ca-160">String</span></span>|<span data-ttu-id="414ca-161">Especifica o grupo de área no qual a configuração está configurada em um provedor de serviços de configuração especificado (CSP) Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="414ca-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="414ca-162">settingUsage</span></span>|[<span data-ttu-id="414ca-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="414ca-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="414ca-164">Tipo de configuração, por exemplo, configuração e conformidade Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="414ca-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="414ca-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="414ca-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="414ca-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="414ca-166">uxBehavior</span></span>|[<span data-ttu-id="414ca-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="414ca-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="414ca-168">Definindo a representação do tipo de controle no UX Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="414ca-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="414ca-169">Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="414ca-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="414ca-170">visibility</span><span class="sxs-lookup"><span data-stu-id="414ca-170">visibility</span></span>|[<span data-ttu-id="414ca-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="414ca-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="414ca-172">Definindo o escopo de visibilidade como UX Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="414ca-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="414ca-173">Os valores possíveis são: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="414ca-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="414ca-174">referredSettingInformationList</span><span class="sxs-lookup"><span data-stu-id="414ca-174">referredSettingInformationList</span></span>|<span data-ttu-id="414ca-175">[coleção deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-175">[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) collection</span></span>|<span data-ttu-id="414ca-176">Lista de informações de configuração referidas.</span><span class="sxs-lookup"><span data-stu-id="414ca-176">List of referred setting information.</span></span> <span data-ttu-id="414ca-177">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-177">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="414ca-178">id</span><span class="sxs-lookup"><span data-stu-id="414ca-178">id</span></span>|<span data-ttu-id="414ca-179">String</span><span class="sxs-lookup"><span data-stu-id="414ca-179">String</span></span>|<span data-ttu-id="414ca-180">Identificador do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-180">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="414ca-181">descrição</span><span class="sxs-lookup"><span data-stu-id="414ca-181">description</span></span>|<span data-ttu-id="414ca-182">String</span><span class="sxs-lookup"><span data-stu-id="414ca-182">String</span></span>|<span data-ttu-id="414ca-183">Descrição do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-183">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="414ca-184">helpText</span><span class="sxs-lookup"><span data-stu-id="414ca-184">helpText</span></span>|<span data-ttu-id="414ca-185">String</span><span class="sxs-lookup"><span data-stu-id="414ca-185">String</span></span>|<span data-ttu-id="414ca-186">Texto de ajuda do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-186">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="414ca-187">nome</span><span class="sxs-lookup"><span data-stu-id="414ca-187">name</span></span>|<span data-ttu-id="414ca-188">String</span><span class="sxs-lookup"><span data-stu-id="414ca-188">String</span></span>|<span data-ttu-id="414ca-189">Nome do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-189">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="414ca-190">displayName</span><span class="sxs-lookup"><span data-stu-id="414ca-190">displayName</span></span>|<span data-ttu-id="414ca-191">String</span><span class="sxs-lookup"><span data-stu-id="414ca-191">String</span></span>|<span data-ttu-id="414ca-192">Nome de exibição do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-192">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="414ca-193">versão</span><span class="sxs-lookup"><span data-stu-id="414ca-193">version</span></span>|<span data-ttu-id="414ca-194">String</span><span class="sxs-lookup"><span data-stu-id="414ca-194">String</span></span>|<span data-ttu-id="414ca-195">Versão do item Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-195">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="414ca-196">childIds</span><span class="sxs-lookup"><span data-stu-id="414ca-196">childIds</span></span>|<span data-ttu-id="414ca-197">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="414ca-197">String collection</span></span>|<span data-ttu-id="414ca-198">Configurações filho dependentes para esse grupo de configurações</span><span class="sxs-lookup"><span data-stu-id="414ca-198">Dependent child settings to this group of settings</span></span>|
|<span data-ttu-id="414ca-199">dependentOn</span><span class="sxs-lookup"><span data-stu-id="414ca-199">dependentOn</span></span>|<span data-ttu-id="414ca-200">[Coleção deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-200">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="414ca-201">Lista de dependências para o grupo de configurações</span><span class="sxs-lookup"><span data-stu-id="414ca-201">List of Dependencies for the setting group</span></span>|
|<span data-ttu-id="414ca-202">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="414ca-202">dependedOnBy</span></span>|<span data-ttu-id="414ca-203">[Coleção deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="414ca-203">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="414ca-204">Lista de configurações filho que dependem dessa configuração</span><span class="sxs-lookup"><span data-stu-id="414ca-204">List of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="414ca-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="414ca-205">Response</span></span>
<span data-ttu-id="414ca-206">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="414ca-206">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="414ca-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="414ca-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="414ca-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="414ca-208">Request</span></span>
<span data-ttu-id="414ca-209">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="414ca-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1729

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
  "visibility": "settingsCatalog",
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "Setting Definition Id value"
    }
  ],
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

### <a name="response"></a><span data-ttu-id="414ca-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="414ca-210">Response</span></span>
<span data-ttu-id="414ca-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="414ca-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1778

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
  "visibility": "settingsCatalog",
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "Setting Definition Id value"
    }
  ],
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




