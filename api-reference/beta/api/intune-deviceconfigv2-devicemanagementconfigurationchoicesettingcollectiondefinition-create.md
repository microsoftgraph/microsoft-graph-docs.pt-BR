---
title: Criar deviceManagementConfigurationChoiceSettingCollectionDefinition
description: Crie um novo objeto deviceManagementConfigurationChoiceSettingCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b54eea3409afde9b29fc0f8a80414376ca7533c9
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864050"
---
# <a name="create-devicemanagementconfigurationchoicesettingcollectiondefinition"></a><span data-ttu-id="02b08-103">Criar deviceManagementConfigurationChoiceSettingCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="02b08-103">Create deviceManagementConfigurationChoiceSettingCollectionDefinition</span></span>

<span data-ttu-id="02b08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02b08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02b08-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02b08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02b08-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02b08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02b08-107">Crie um novo [objeto deviceManagementConfigurationChoiceSettingCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-107">Create a new [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02b08-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02b08-108">Prerequisites</span></span>
<span data-ttu-id="02b08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02b08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02b08-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02b08-111">Permission type</span></span>|<span data-ttu-id="02b08-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02b08-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02b08-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02b08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02b08-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02b08-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="02b08-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02b08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02b08-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02b08-116">Not supported.</span></span>|
|<span data-ttu-id="02b08-117">Application</span><span class="sxs-lookup"><span data-stu-id="02b08-117">Application</span></span>|<span data-ttu-id="02b08-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02b08-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02b08-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02b08-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reusableSettings
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="02b08-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02b08-120">Request headers</span></span>
|<span data-ttu-id="02b08-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02b08-121">Header</span></span>|<span data-ttu-id="02b08-122">Valor</span><span class="sxs-lookup"><span data-stu-id="02b08-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02b08-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="02b08-123">Authorization</span></span>|<span data-ttu-id="02b08-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02b08-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02b08-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02b08-125">Accept</span></span>|<span data-ttu-id="02b08-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02b08-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02b08-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02b08-127">Request body</span></span>
<span data-ttu-id="02b08-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementConfigurationChoiceSettingCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="02b08-128">In the request body, supply a JSON representation for the deviceManagementConfigurationChoiceSettingCollectionDefinition object.</span></span>

<span data-ttu-id="02b08-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationChoiceSettingCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="02b08-129">The following table shows the properties that are required when you create the deviceManagementConfigurationChoiceSettingCollectionDefinition.</span></span>

|<span data-ttu-id="02b08-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02b08-130">Property</span></span>|<span data-ttu-id="02b08-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="02b08-131">Type</span></span>|<span data-ttu-id="02b08-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="02b08-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02b08-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="02b08-133">applicability</span></span>|[<span data-ttu-id="02b08-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="02b08-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="02b08-135">Detalhes sobre qual configuração de dispositivo é aplicável em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="02b08-136">accessTypes</span></span>|[<span data-ttu-id="02b08-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="02b08-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="02b08-138">Modo de acesso de leitura/gravação da configuração Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="02b08-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="02b08-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="02b08-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="02b08-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="02b08-140">keywords</span></span>|<span data-ttu-id="02b08-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="02b08-141">String collection</span></span>|<span data-ttu-id="02b08-142">Tokens que para pesquisar configurações em Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="02b08-143">infoUrls</span></span>|<span data-ttu-id="02b08-144">Coleção String</span><span class="sxs-lookup"><span data-stu-id="02b08-144">String collection</span></span>|<span data-ttu-id="02b08-145">Lista de links mais informações para a configuração podem ser encontradas em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="02b08-146">occurrence</span></span>|[<span data-ttu-id="02b08-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="02b08-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="02b08-148">Indica se a configuração é necessária ou não Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="02b08-149">baseUri</span></span>|<span data-ttu-id="02b08-150">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="02b08-150">String</span></span>|<span data-ttu-id="02b08-151">Caminho base CSP Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="02b08-152">offsetUri</span></span>|<span data-ttu-id="02b08-153">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="02b08-153">String</span></span>|<span data-ttu-id="02b08-154">Caminho de deslocamento CSP da Base Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="02b08-155">rootDefinitionId</span></span>|<span data-ttu-id="02b08-156">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="02b08-156">String</span></span>|<span data-ttu-id="02b08-157">Definição de configuração raiz se a configuração for uma configuração filho.</span><span class="sxs-lookup"><span data-stu-id="02b08-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="02b08-158">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="02b08-159">categoryId</span></span>|<span data-ttu-id="02b08-160">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="02b08-160">String</span></span>|<span data-ttu-id="02b08-161">Especifica o grupo de área no qual a configuração está configurada em um provedor de serviços de configuração especificado (CSP) Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="02b08-162">settingUsage</span></span>|[<span data-ttu-id="02b08-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="02b08-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="02b08-164">Tipo de configuração, por exemplo, configuração e conformidade Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="02b08-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="02b08-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="02b08-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="02b08-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="02b08-166">uxBehavior</span></span>|[<span data-ttu-id="02b08-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="02b08-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="02b08-168">Definindo a representação do tipo de controle no UX Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="02b08-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="02b08-169">Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="02b08-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="02b08-170">visibility</span><span class="sxs-lookup"><span data-stu-id="02b08-170">visibility</span></span>|[<span data-ttu-id="02b08-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="02b08-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="02b08-172">Definindo o escopo de visibilidade como UX Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="02b08-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="02b08-173">Os valores possíveis são: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="02b08-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="02b08-174">referredSettingInformationList</span><span class="sxs-lookup"><span data-stu-id="02b08-174">referredSettingInformationList</span></span>|<span data-ttu-id="02b08-175">[coleção deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-175">[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) collection</span></span>|<span data-ttu-id="02b08-176">Lista de informações de configuração referidas.</span><span class="sxs-lookup"><span data-stu-id="02b08-176">List of referred setting information.</span></span> <span data-ttu-id="02b08-177">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-177">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-178">id</span><span class="sxs-lookup"><span data-stu-id="02b08-178">id</span></span>|<span data-ttu-id="02b08-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02b08-179">String</span></span>|<span data-ttu-id="02b08-180">Identificador do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-180">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-181">description</span><span class="sxs-lookup"><span data-stu-id="02b08-181">description</span></span>|<span data-ttu-id="02b08-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02b08-182">String</span></span>|<span data-ttu-id="02b08-183">Descrição do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-183">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-184">helpText</span><span class="sxs-lookup"><span data-stu-id="02b08-184">helpText</span></span>|<span data-ttu-id="02b08-185">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="02b08-185">String</span></span>|<span data-ttu-id="02b08-186">Texto de ajuda do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-186">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-187">nome</span><span class="sxs-lookup"><span data-stu-id="02b08-187">name</span></span>|<span data-ttu-id="02b08-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02b08-188">String</span></span>|<span data-ttu-id="02b08-189">Nome do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-189">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-190">displayName</span><span class="sxs-lookup"><span data-stu-id="02b08-190">displayName</span></span>|<span data-ttu-id="02b08-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02b08-191">String</span></span>|<span data-ttu-id="02b08-192">Nome de exibição do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-192">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-193">versão</span><span class="sxs-lookup"><span data-stu-id="02b08-193">version</span></span>|<span data-ttu-id="02b08-194">String</span><span class="sxs-lookup"><span data-stu-id="02b08-194">String</span></span>|<span data-ttu-id="02b08-195">Versão do item Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-195">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-196">options</span><span class="sxs-lookup"><span data-stu-id="02b08-196">options</span></span>|<span data-ttu-id="02b08-197">[Coleção deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-197">[deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md) collection</span></span>|<span data-ttu-id="02b08-198">Opções para a configuração que pode ser selecionada Herdada de [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-198">Options for the setting that can be selected Inherited from [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-199">defaultOptionId</span><span class="sxs-lookup"><span data-stu-id="02b08-199">defaultOptionId</span></span>|<span data-ttu-id="02b08-200">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="02b08-200">String</span></span>|<span data-ttu-id="02b08-201">Opção padrão para a configuração de opção Herdada [de deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="02b08-201">Default option for choice setting Inherited from [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span></span>|
|<span data-ttu-id="02b08-202">maximumCount</span><span class="sxs-lookup"><span data-stu-id="02b08-202">maximumCount</span></span>|<span data-ttu-id="02b08-203">Int32</span><span class="sxs-lookup"><span data-stu-id="02b08-203">Int32</span></span>|<span data-ttu-id="02b08-204">Número máximo de opções na coleção.</span><span class="sxs-lookup"><span data-stu-id="02b08-204">Maximum number of choices in the collection.</span></span> <span data-ttu-id="02b08-205">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="02b08-205">Valid values 1 to 100</span></span>|
|<span data-ttu-id="02b08-206">minimumCount</span><span class="sxs-lookup"><span data-stu-id="02b08-206">minimumCount</span></span>|<span data-ttu-id="02b08-207">Int32</span><span class="sxs-lookup"><span data-stu-id="02b08-207">Int32</span></span>|<span data-ttu-id="02b08-208">Número mínimo de opções na coleção.</span><span class="sxs-lookup"><span data-stu-id="02b08-208">Minimum number of choices in the collection.</span></span> <span data-ttu-id="02b08-209">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="02b08-209">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="02b08-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="02b08-210">Response</span></span>
<span data-ttu-id="02b08-211">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02b08-211">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02b08-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02b08-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="02b08-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02b08-213">Request</span></span>
<span data-ttu-id="02b08-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02b08-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reusableSettings
Content-type: application/json
Content-length: 10214

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

### <a name="response"></a><span data-ttu-id="02b08-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="02b08-215">Response</span></span>
<span data-ttu-id="02b08-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02b08-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10263

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
  "uxBehavior": "dropdown",
  "visibility": "settingsCatalog",
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "Setting Definition Id value"
    }
  ],
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




