---
title: Criar deviceManagementConfigurationChoiceSettingDefinition
description: Crie um novo objeto deviceManagementConfigurationChoiceSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf82fe5ab01ff4318184dcb7252da0d1e80f7337
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864456"
---
# <a name="create-devicemanagementconfigurationchoicesettingdefinition"></a><span data-ttu-id="b813e-103">Criar deviceManagementConfigurationChoiceSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="b813e-103">Create deviceManagementConfigurationChoiceSettingDefinition</span></span>

<span data-ttu-id="b813e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b813e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b813e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b813e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b813e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b813e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b813e-107">Crie um novo [objeto deviceManagementConfigurationChoiceSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-107">Create a new [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b813e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b813e-108">Prerequisites</span></span>
<span data-ttu-id="b813e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b813e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b813e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b813e-111">Permission type</span></span>|<span data-ttu-id="b813e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b813e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b813e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b813e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b813e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b813e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b813e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b813e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b813e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b813e-116">Not supported.</span></span>|
|<span data-ttu-id="b813e-117">Application</span><span class="sxs-lookup"><span data-stu-id="b813e-117">Application</span></span>|<span data-ttu-id="b813e-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b813e-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b813e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b813e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reusableSettings
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="b813e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b813e-120">Request headers</span></span>
|<span data-ttu-id="b813e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b813e-121">Header</span></span>|<span data-ttu-id="b813e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b813e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b813e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b813e-123">Authorization</span></span>|<span data-ttu-id="b813e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b813e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b813e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b813e-125">Accept</span></span>|<span data-ttu-id="b813e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b813e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b813e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b813e-127">Request body</span></span>
<span data-ttu-id="b813e-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementConfigurationChoiceSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="b813e-128">In the request body, supply a JSON representation for the deviceManagementConfigurationChoiceSettingDefinition object.</span></span>

<span data-ttu-id="b813e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementConfigurationChoiceSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="b813e-129">The following table shows the properties that are required when you create the deviceManagementConfigurationChoiceSettingDefinition.</span></span>

|<span data-ttu-id="b813e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b813e-130">Property</span></span>|<span data-ttu-id="b813e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b813e-131">Type</span></span>|<span data-ttu-id="b813e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b813e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b813e-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="b813e-133">applicability</span></span>|[<span data-ttu-id="b813e-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="b813e-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="b813e-135">Detalhes sobre qual configuração de dispositivo é aplicável em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b813e-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="b813e-136">accessTypes</span></span>|[<span data-ttu-id="b813e-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="b813e-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="b813e-138">Modo de acesso de leitura/gravação da configuração Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b813e-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="b813e-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="b813e-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="b813e-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="b813e-140">keywords</span></span>|<span data-ttu-id="b813e-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b813e-141">String collection</span></span>|<span data-ttu-id="b813e-142">Tokens que para pesquisar configurações em Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b813e-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="b813e-143">infoUrls</span></span>|<span data-ttu-id="b813e-144">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b813e-144">String collection</span></span>|<span data-ttu-id="b813e-145">Lista de links mais informações para a configuração podem ser encontradas em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b813e-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="b813e-146">occurrence</span></span>|[<span data-ttu-id="b813e-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="b813e-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="b813e-148">Indica se a configuração é necessária ou não Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b813e-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="b813e-149">baseUri</span></span>|<span data-ttu-id="b813e-150">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b813e-150">String</span></span>|<span data-ttu-id="b813e-151">Caminho base CSP Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b813e-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="b813e-152">offsetUri</span></span>|<span data-ttu-id="b813e-153">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b813e-153">String</span></span>|<span data-ttu-id="b813e-154">Caminho de deslocamento CSP da Base Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b813e-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b813e-155">rootDefinitionId</span></span>|<span data-ttu-id="b813e-156">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b813e-156">String</span></span>|<span data-ttu-id="b813e-157">Definição de configuração raiz se a configuração for uma configuração filho.</span><span class="sxs-lookup"><span data-stu-id="b813e-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="b813e-158">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b813e-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="b813e-159">categoryId</span></span>|<span data-ttu-id="b813e-160">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b813e-160">String</span></span>|<span data-ttu-id="b813e-161">Especifica o grupo de área no qual a configuração está configurada em um provedor de serviços de configuração especificado (CSP) Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b813e-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="b813e-162">settingUsage</span></span>|[<span data-ttu-id="b813e-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="b813e-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="b813e-164">Tipo de configuração, por exemplo, configuração e conformidade Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b813e-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="b813e-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="b813e-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="b813e-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="b813e-166">uxBehavior</span></span>|[<span data-ttu-id="b813e-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="b813e-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="b813e-168">Definindo a representação do tipo de controle no UX Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b813e-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="b813e-169">Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="b813e-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="b813e-170">visibility</span><span class="sxs-lookup"><span data-stu-id="b813e-170">visibility</span></span>|[<span data-ttu-id="b813e-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="b813e-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="b813e-172">Definindo o escopo de visibilidade como UX Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b813e-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="b813e-173">Os valores possíveis são: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="b813e-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="b813e-174">referredSettingInformationList</span><span class="sxs-lookup"><span data-stu-id="b813e-174">referredSettingInformationList</span></span>|<span data-ttu-id="b813e-175">[coleção deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-175">[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) collection</span></span>|<span data-ttu-id="b813e-176">Lista de informações de configuração referidas.</span><span class="sxs-lookup"><span data-stu-id="b813e-176">List of referred setting information.</span></span> <span data-ttu-id="b813e-177">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-177">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b813e-178">id</span><span class="sxs-lookup"><span data-stu-id="b813e-178">id</span></span>|<span data-ttu-id="b813e-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b813e-179">String</span></span>|<span data-ttu-id="b813e-180">Identificador do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-180">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b813e-181">description</span><span class="sxs-lookup"><span data-stu-id="b813e-181">description</span></span>|<span data-ttu-id="b813e-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b813e-182">String</span></span>|<span data-ttu-id="b813e-183">Descrição do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-183">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b813e-184">helpText</span><span class="sxs-lookup"><span data-stu-id="b813e-184">helpText</span></span>|<span data-ttu-id="b813e-185">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b813e-185">String</span></span>|<span data-ttu-id="b813e-186">Texto de ajuda do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-186">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b813e-187">nome</span><span class="sxs-lookup"><span data-stu-id="b813e-187">name</span></span>|<span data-ttu-id="b813e-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b813e-188">String</span></span>|<span data-ttu-id="b813e-189">Nome do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-189">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b813e-190">displayName</span><span class="sxs-lookup"><span data-stu-id="b813e-190">displayName</span></span>|<span data-ttu-id="b813e-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b813e-191">String</span></span>|<span data-ttu-id="b813e-192">Nome de exibição do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-192">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b813e-193">versão</span><span class="sxs-lookup"><span data-stu-id="b813e-193">version</span></span>|<span data-ttu-id="b813e-194">String</span><span class="sxs-lookup"><span data-stu-id="b813e-194">String</span></span>|<span data-ttu-id="b813e-195">Versão do item Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-195">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b813e-196">options</span><span class="sxs-lookup"><span data-stu-id="b813e-196">options</span></span>|<span data-ttu-id="b813e-197">[Coleção deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b813e-197">[deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md) collection</span></span>|<span data-ttu-id="b813e-198">Opções para a configuração que pode ser selecionada</span><span class="sxs-lookup"><span data-stu-id="b813e-198">Options for the setting that can be selected</span></span>|
|<span data-ttu-id="b813e-199">defaultOptionId</span><span class="sxs-lookup"><span data-stu-id="b813e-199">defaultOptionId</span></span>|<span data-ttu-id="b813e-200">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b813e-200">String</span></span>|<span data-ttu-id="b813e-201">Opção padrão para a configuração de opção</span><span class="sxs-lookup"><span data-stu-id="b813e-201">Default option for choice setting</span></span>|



## <a name="response"></a><span data-ttu-id="b813e-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="b813e-202">Response</span></span>
<span data-ttu-id="b813e-203">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b813e-203">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b813e-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b813e-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="b813e-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b813e-205">Request</span></span>
<span data-ttu-id="b813e-206">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b813e-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reusableSettings
Content-type: application/json
Content-length: 10158

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
  "defaultOptionId": "Default Option Id value"
}
```

### <a name="response"></a><span data-ttu-id="b813e-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="b813e-207">Response</span></span>
<span data-ttu-id="b813e-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b813e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10207

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
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "Setting Definition Id value"
    }
  ],
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




