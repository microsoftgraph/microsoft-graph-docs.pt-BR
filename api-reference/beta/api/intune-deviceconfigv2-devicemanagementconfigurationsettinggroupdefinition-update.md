---
title: Atualizar deviceManagementConfigurationSettingGroupDefinition
description: Atualiza as propriedades de um objeto deviceManagementConfigurationSettingGroupDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3dc8951432f981c6f37183c0c780cf0982b79d33
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241331"
---
# <a name="update-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="af1e3-103">Atualizar deviceManagementConfigurationSettingGroupDefinition</span><span class="sxs-lookup"><span data-stu-id="af1e3-103">Update deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="af1e3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af1e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af1e3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="af1e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af1e3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="af1e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af1e3-107">Atualiza as propriedades de um objeto [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="af1e3-107">Update the properties of a [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af1e3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="af1e3-108">Prerequisites</span></span>
<span data-ttu-id="af1e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af1e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af1e3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af1e3-111">Permission type</span></span>|<span data-ttu-id="af1e3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="af1e3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af1e3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af1e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af1e3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af1e3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af1e3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af1e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af1e3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af1e3-116">Not supported.</span></span>|
|<span data-ttu-id="af1e3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af1e3-117">Application</span></span>|<span data-ttu-id="af1e3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af1e3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af1e3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af1e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="af1e3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af1e3-120">Request headers</span></span>
|<span data-ttu-id="af1e3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af1e3-121">Header</span></span>|<span data-ttu-id="af1e3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="af1e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af1e3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="af1e3-123">Authorization</span></span>|<span data-ttu-id="af1e3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af1e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af1e3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="af1e3-125">Accept</span></span>|<span data-ttu-id="af1e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af1e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af1e3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af1e3-127">Request body</span></span>
<span data-ttu-id="af1e3-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="af1e3-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

<span data-ttu-id="af1e3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="af1e3-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md).</span></span>

|<span data-ttu-id="af1e3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af1e3-130">Property</span></span>|<span data-ttu-id="af1e3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="af1e3-131">Type</span></span>|<span data-ttu-id="af1e3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="af1e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af1e3-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="af1e3-133">applicability</span></span>|[<span data-ttu-id="af1e3-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="af1e3-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="af1e3-135">Detalhes qual configuração de dispositivo é aplicável no herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="af1e3-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="af1e3-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="af1e3-136">accessTypes</span></span>|[<span data-ttu-id="af1e3-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="af1e3-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="af1e3-138">Modo de acesso de leitura/gravação da configuração herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="af1e3-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="af1e3-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="af1e3-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="af1e3-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="af1e3-140">keywords</span></span>|<span data-ttu-id="af1e3-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="af1e3-141">String collection</span></span>|<span data-ttu-id="af1e3-142">Tokens que pesquisam configurações em herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="af1e3-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="af1e3-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="af1e3-143">infoUrls</span></span>|<span data-ttu-id="af1e3-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="af1e3-144">String collection</span></span>|<span data-ttu-id="af1e3-145">Lista de links mais informações para a configuração podem ser encontradas em herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="af1e3-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="af1e3-146">ocorrência</span><span class="sxs-lookup"><span data-stu-id="af1e3-146">occurrence</span></span>|[<span data-ttu-id="af1e3-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="af1e3-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="af1e3-148">Indica se a configuração é obrigatória ou não herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="af1e3-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="af1e3-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="af1e3-149">baseUri</span></span>|<span data-ttu-id="af1e3-150">String</span><span class="sxs-lookup"><span data-stu-id="af1e3-150">String</span></span>|<span data-ttu-id="af1e3-151">Caminho de CSP base herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="af1e3-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="af1e3-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="af1e3-152">offsetUri</span></span>|<span data-ttu-id="af1e3-153">String</span><span class="sxs-lookup"><span data-stu-id="af1e3-153">String</span></span>|<span data-ttu-id="af1e3-154">Caminho de CSP offset da base herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="af1e3-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="af1e3-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="af1e3-155">rootDefinitionId</span></span>|<span data-ttu-id="af1e3-156">String</span><span class="sxs-lookup"><span data-stu-id="af1e3-156">String</span></span>|<span data-ttu-id="af1e3-157">Definição da configuração raiz se a configuração for uma configuração de filho.</span><span class="sxs-lookup"><span data-stu-id="af1e3-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="af1e3-158">Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="af1e3-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="af1e3-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="af1e3-159">categoryId</span></span>|<span data-ttu-id="af1e3-160">String</span><span class="sxs-lookup"><span data-stu-id="af1e3-160">String</span></span>|<span data-ttu-id="af1e3-161">Especifica o grupo de área no qual a configuração é configurada em um provedor de serviços de configuração especificado (CSP) herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="af1e3-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="af1e3-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="af1e3-162">settingUsage</span></span>|[<span data-ttu-id="af1e3-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="af1e3-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="af1e3-164">Tipo de configuração, por exemplo, configuração e conformidade herdadas de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="af1e3-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="af1e3-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="af1e3-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="af1e3-166">id</span><span class="sxs-lookup"><span data-stu-id="af1e3-166">id</span></span>|<span data-ttu-id="af1e3-167">String</span><span class="sxs-lookup"><span data-stu-id="af1e3-167">String</span></span>|<span data-ttu-id="af1e3-168">Identificador do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="af1e3-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="af1e3-169">description</span><span class="sxs-lookup"><span data-stu-id="af1e3-169">description</span></span>|<span data-ttu-id="af1e3-170">String</span><span class="sxs-lookup"><span data-stu-id="af1e3-170">String</span></span>|<span data-ttu-id="af1e3-171">Descrição do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="af1e3-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="af1e3-172">helpText</span><span class="sxs-lookup"><span data-stu-id="af1e3-172">helpText</span></span>|<span data-ttu-id="af1e3-173">String</span><span class="sxs-lookup"><span data-stu-id="af1e3-173">String</span></span>|<span data-ttu-id="af1e3-174">Texto de ajuda do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="af1e3-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="af1e3-175">nome</span><span class="sxs-lookup"><span data-stu-id="af1e3-175">name</span></span>|<span data-ttu-id="af1e3-176">String</span><span class="sxs-lookup"><span data-stu-id="af1e3-176">String</span></span>|<span data-ttu-id="af1e3-177">Nome do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="af1e3-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="af1e3-178">displayName</span><span class="sxs-lookup"><span data-stu-id="af1e3-178">displayName</span></span>|<span data-ttu-id="af1e3-179">String</span><span class="sxs-lookup"><span data-stu-id="af1e3-179">String</span></span>|<span data-ttu-id="af1e3-180">Nome para exibição do item herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="af1e3-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="af1e3-181">versão</span><span class="sxs-lookup"><span data-stu-id="af1e3-181">version</span></span>|<span data-ttu-id="af1e3-182">String</span><span class="sxs-lookup"><span data-stu-id="af1e3-182">String</span></span>|<span data-ttu-id="af1e3-183">Versão de item herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="af1e3-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="af1e3-184">childIds</span><span class="sxs-lookup"><span data-stu-id="af1e3-184">childIds</span></span>|<span data-ttu-id="af1e3-185">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="af1e3-185">String collection</span></span>|<span data-ttu-id="af1e3-186">Configurações filhas dependentes para este grupo de configurações</span><span class="sxs-lookup"><span data-stu-id="af1e3-186">Dependent child settings to this group of settings</span></span>|
|<span data-ttu-id="af1e3-187">dependente</span><span class="sxs-lookup"><span data-stu-id="af1e3-187">dependentOn</span></span>|<span data-ttu-id="af1e3-188">coleção [deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="af1e3-188">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="af1e3-189">Lista de dependências para o grupo de configurações</span><span class="sxs-lookup"><span data-stu-id="af1e3-189">List of Dependencies for the setting group</span></span>|
|<span data-ttu-id="af1e3-190">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="af1e3-190">dependedOnBy</span></span>|<span data-ttu-id="af1e3-191">coleção [deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="af1e3-191">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="af1e3-192">Lista de configurações filhas que dependem dessa configuração</span><span class="sxs-lookup"><span data-stu-id="af1e3-192">List of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="af1e3-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="af1e3-193">Response</span></span>
<span data-ttu-id="af1e3-194">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af1e3-194">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af1e3-195">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af1e3-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="af1e3-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af1e3-196">Request</span></span>
<span data-ttu-id="af1e3-197">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af1e3-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1448

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

### <a name="response"></a><span data-ttu-id="af1e3-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="af1e3-198">Response</span></span>
<span data-ttu-id="af1e3-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af1e3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1497

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




