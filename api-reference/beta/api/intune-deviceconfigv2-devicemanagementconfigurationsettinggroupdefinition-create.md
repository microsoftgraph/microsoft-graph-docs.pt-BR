---
title: Criar deviceManagementConfigurationSettingGroupDefinition
description: Crie um novo objeto deviceManagementConfigurationSettingGroupDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d5d562921ab3376861bc30ace37e1e5f36d4619a
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665466"
---
# <a name="create-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="5c77f-103">Criar deviceManagementConfigurationSettingGroupDefinition</span><span class="sxs-lookup"><span data-stu-id="5c77f-103">Create deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="5c77f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c77f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c77f-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5c77f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c77f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c77f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c77f-107">Crie um novo [objeto deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-107">Create a new [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c77f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5c77f-108">Prerequisites</span></span>
<span data-ttu-id="5c77f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c77f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c77f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c77f-111">Permission type</span></span>|<span data-ttu-id="5c77f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c77f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c77f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c77f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c77f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c77f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c77f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c77f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c77f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c77f-116">Not supported.</span></span>|
|<span data-ttu-id="5c77f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c77f-117">Application</span></span>|<span data-ttu-id="5c77f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c77f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c77f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c77f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reusableSettings
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
POST /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates/{deviceManagementConfigurationSettingTemplateId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="5c77f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c77f-120">Request headers</span></span>
|<span data-ttu-id="5c77f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c77f-121">Header</span></span>|<span data-ttu-id="5c77f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5c77f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c77f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c77f-123">Authorization</span></span>|<span data-ttu-id="5c77f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c77f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c77f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5c77f-125">Accept</span></span>|<span data-ttu-id="5c77f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c77f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c77f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c77f-127">Request body</span></span>
<span data-ttu-id="5c77f-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementConfigurationSettingGroupDefinition.</span><span class="sxs-lookup"><span data-stu-id="5c77f-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingGroupDefinition object.</span></span>

<span data-ttu-id="5c77f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationSettingGroupDefinition.</span><span class="sxs-lookup"><span data-stu-id="5c77f-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingGroupDefinition.</span></span>

|<span data-ttu-id="5c77f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c77f-130">Property</span></span>|<span data-ttu-id="5c77f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c77f-131">Type</span></span>|<span data-ttu-id="5c77f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c77f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c77f-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="5c77f-133">applicability</span></span>|[<span data-ttu-id="5c77f-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="5c77f-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="5c77f-135">Detalhes sobre qual configuração de dispositivo é aplicável em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c77f-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="5c77f-136">accessTypes</span></span>|[<span data-ttu-id="5c77f-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="5c77f-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="5c77f-138">Modo de acesso de leitura/gravação da configuração Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5c77f-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="5c77f-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="5c77f-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="5c77f-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="5c77f-140">keywords</span></span>|<span data-ttu-id="5c77f-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c77f-141">String collection</span></span>|<span data-ttu-id="5c77f-142">Tokens que para pesquisar configurações em Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c77f-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="5c77f-143">infoUrls</span></span>|<span data-ttu-id="5c77f-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c77f-144">String collection</span></span>|<span data-ttu-id="5c77f-145">Lista de links mais informações para a configuração podem ser encontradas em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c77f-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="5c77f-146">occurrence</span></span>|[<span data-ttu-id="5c77f-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="5c77f-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="5c77f-148">Indica se a configuração é necessária ou não Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c77f-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="5c77f-149">baseUri</span></span>|<span data-ttu-id="5c77f-150">String</span><span class="sxs-lookup"><span data-stu-id="5c77f-150">String</span></span>|<span data-ttu-id="5c77f-151">Caminho base CSP Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c77f-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="5c77f-152">offsetUri</span></span>|<span data-ttu-id="5c77f-153">String</span><span class="sxs-lookup"><span data-stu-id="5c77f-153">String</span></span>|<span data-ttu-id="5c77f-154">Caminho de deslocamento CSP da Base Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c77f-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5c77f-155">rootDefinitionId</span></span>|<span data-ttu-id="5c77f-156">String</span><span class="sxs-lookup"><span data-stu-id="5c77f-156">String</span></span>|<span data-ttu-id="5c77f-157">Definição de configuração raiz se a configuração for uma configuração filho.</span><span class="sxs-lookup"><span data-stu-id="5c77f-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="5c77f-158">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c77f-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="5c77f-159">categoryId</span></span>|<span data-ttu-id="5c77f-160">String</span><span class="sxs-lookup"><span data-stu-id="5c77f-160">String</span></span>|<span data-ttu-id="5c77f-161">Especifica o grupo de área no qual a configuração está configurada em um provedor de serviços de configuração especificado (CSP) Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c77f-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="5c77f-162">settingUsage</span></span>|[<span data-ttu-id="5c77f-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="5c77f-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="5c77f-164">Tipo de configuração, por exemplo, configuração e conformidade Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5c77f-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="5c77f-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="5c77f-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="5c77f-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="5c77f-166">uxBehavior</span></span>|[<span data-ttu-id="5c77f-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="5c77f-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="5c77f-168">Definindo a representação do tipo de controle no UX Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5c77f-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="5c77f-169">Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="5c77f-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="5c77f-170">visibility</span><span class="sxs-lookup"><span data-stu-id="5c77f-170">visibility</span></span>|[<span data-ttu-id="5c77f-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="5c77f-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="5c77f-172">Definindo o escopo de visibilidade como UX Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5c77f-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="5c77f-173">Os valores possíveis são: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="5c77f-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="5c77f-174">referredSettingInformationList</span><span class="sxs-lookup"><span data-stu-id="5c77f-174">referredSettingInformationList</span></span>|<span data-ttu-id="5c77f-175">[coleção deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-175">[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) collection</span></span>|<span data-ttu-id="5c77f-176">Lista de informações de configuração referidas.</span><span class="sxs-lookup"><span data-stu-id="5c77f-176">List of referred setting information.</span></span> <span data-ttu-id="5c77f-177">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-177">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c77f-178">id</span><span class="sxs-lookup"><span data-stu-id="5c77f-178">id</span></span>|<span data-ttu-id="5c77f-179">String</span><span class="sxs-lookup"><span data-stu-id="5c77f-179">String</span></span>|<span data-ttu-id="5c77f-180">Identificador do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-180">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c77f-181">descrição</span><span class="sxs-lookup"><span data-stu-id="5c77f-181">description</span></span>|<span data-ttu-id="5c77f-182">String</span><span class="sxs-lookup"><span data-stu-id="5c77f-182">String</span></span>|<span data-ttu-id="5c77f-183">Descrição do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-183">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c77f-184">helpText</span><span class="sxs-lookup"><span data-stu-id="5c77f-184">helpText</span></span>|<span data-ttu-id="5c77f-185">String</span><span class="sxs-lookup"><span data-stu-id="5c77f-185">String</span></span>|<span data-ttu-id="5c77f-186">Texto de ajuda do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-186">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c77f-187">nome</span><span class="sxs-lookup"><span data-stu-id="5c77f-187">name</span></span>|<span data-ttu-id="5c77f-188">String</span><span class="sxs-lookup"><span data-stu-id="5c77f-188">String</span></span>|<span data-ttu-id="5c77f-189">Nome do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-189">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c77f-190">displayName</span><span class="sxs-lookup"><span data-stu-id="5c77f-190">displayName</span></span>|<span data-ttu-id="5c77f-191">String</span><span class="sxs-lookup"><span data-stu-id="5c77f-191">String</span></span>|<span data-ttu-id="5c77f-192">Nome de exibição do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-192">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c77f-193">versão</span><span class="sxs-lookup"><span data-stu-id="5c77f-193">version</span></span>|<span data-ttu-id="5c77f-194">String</span><span class="sxs-lookup"><span data-stu-id="5c77f-194">String</span></span>|<span data-ttu-id="5c77f-195">Versão do item Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-195">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c77f-196">childIds</span><span class="sxs-lookup"><span data-stu-id="5c77f-196">childIds</span></span>|<span data-ttu-id="5c77f-197">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c77f-197">String collection</span></span>|<span data-ttu-id="5c77f-198">Configurações filho dependentes para esse grupo de configurações</span><span class="sxs-lookup"><span data-stu-id="5c77f-198">Dependent child settings to this group of settings</span></span>|
|<span data-ttu-id="5c77f-199">dependentOn</span><span class="sxs-lookup"><span data-stu-id="5c77f-199">dependentOn</span></span>|<span data-ttu-id="5c77f-200">[Coleção deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-200">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="5c77f-201">Lista de dependências para o grupo de configurações</span><span class="sxs-lookup"><span data-stu-id="5c77f-201">List of Dependencies for the setting group</span></span>|
|<span data-ttu-id="5c77f-202">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="5c77f-202">dependedOnBy</span></span>|<span data-ttu-id="5c77f-203">[Coleção deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="5c77f-203">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="5c77f-204">Lista de configurações filho que dependem dessa configuração</span><span class="sxs-lookup"><span data-stu-id="5c77f-204">List of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="5c77f-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c77f-205">Response</span></span>
<span data-ttu-id="5c77f-206">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c77f-206">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c77f-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c77f-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c77f-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c77f-208">Request</span></span>
<span data-ttu-id="5c77f-209">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c77f-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reusableSettings
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

### <a name="response"></a><span data-ttu-id="5c77f-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c77f-210">Response</span></span>
<span data-ttu-id="5c77f-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c77f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




