---
title: Atualizar deviceManagementConfigurationSimpleSettingCollectionDefinition
description: Atualize as propriedades de um objeto deviceManagementConfigurationSimpleSettingCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 702572c2b71364f4dca1e033abe41e6dc692593c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129150"
---
# <a name="update-devicemanagementconfigurationsimplesettingcollectiondefinition"></a><span data-ttu-id="6aca8-103">Atualizar deviceManagementConfigurationSimpleSettingCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="6aca8-103">Update deviceManagementConfigurationSimpleSettingCollectionDefinition</span></span>

<span data-ttu-id="6aca8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6aca8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6aca8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6aca8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6aca8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6aca8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aca8-107">Atualize as propriedades de [um objeto deviceManagementConfigurationSimpleSettingCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-107">Update the properties of a [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6aca8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6aca8-108">Prerequisites</span></span>
<span data-ttu-id="6aca8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6aca8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aca8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6aca8-111">Permission type</span></span>|<span data-ttu-id="6aca8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6aca8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6aca8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6aca8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6aca8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aca8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6aca8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6aca8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6aca8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6aca8-116">Not supported.</span></span>|
|<span data-ttu-id="6aca8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6aca8-117">Application</span></span>|<span data-ttu-id="6aca8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aca8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6aca8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6aca8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="6aca8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6aca8-120">Request headers</span></span>
|<span data-ttu-id="6aca8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6aca8-121">Header</span></span>|<span data-ttu-id="6aca8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6aca8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6aca8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6aca8-123">Authorization</span></span>|<span data-ttu-id="6aca8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6aca8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6aca8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6aca8-125">Accept</span></span>|<span data-ttu-id="6aca8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6aca8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aca8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6aca8-127">Request body</span></span>
<span data-ttu-id="6aca8-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementConfigurationSimpleSettingCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object.</span></span>

<span data-ttu-id="6aca8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6aca8-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md).</span></span>

|<span data-ttu-id="6aca8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6aca8-130">Property</span></span>|<span data-ttu-id="6aca8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6aca8-131">Type</span></span>|<span data-ttu-id="6aca8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6aca8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6aca8-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="6aca8-133">applicability</span></span>|[<span data-ttu-id="6aca8-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="6aca8-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="6aca8-135">Detalhes sobre qual configuração de dispositivo é aplicável em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="6aca8-136">accessTypes</span></span>|[<span data-ttu-id="6aca8-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="6aca8-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="6aca8-138">Modo de acesso de leitura/gravação da configuração Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6aca8-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="6aca8-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="6aca8-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="6aca8-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="6aca8-140">keywords</span></span>|<span data-ttu-id="6aca8-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6aca8-141">String collection</span></span>|<span data-ttu-id="6aca8-142">Tokens que para pesquisar configurações em Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="6aca8-143">infoUrls</span></span>|<span data-ttu-id="6aca8-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6aca8-144">String collection</span></span>|<span data-ttu-id="6aca8-145">Lista de links mais informações para a configuração podem ser encontradas em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="6aca8-146">occurrence</span></span>|[<span data-ttu-id="6aca8-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="6aca8-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="6aca8-148">Indica se a configuração é necessária ou não Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="6aca8-149">baseUri</span></span>|<span data-ttu-id="6aca8-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6aca8-150">String</span></span>|<span data-ttu-id="6aca8-151">Caminho base CSP Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="6aca8-152">offsetUri</span></span>|<span data-ttu-id="6aca8-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6aca8-153">String</span></span>|<span data-ttu-id="6aca8-154">Caminho de deslocamento CSP da Base Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="6aca8-155">rootDefinitionId</span></span>|<span data-ttu-id="6aca8-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6aca8-156">String</span></span>|<span data-ttu-id="6aca8-157">Definição de configuração raiz se a configuração for uma configuração filho.</span><span class="sxs-lookup"><span data-stu-id="6aca8-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="6aca8-158">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="6aca8-159">categoryId</span></span>|<span data-ttu-id="6aca8-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6aca8-160">String</span></span>|<span data-ttu-id="6aca8-161">Especifica o grupo de área no qual a configuração está configurada em um provedor de serviços de configuração especificado (CSP) Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="6aca8-162">settingUsage</span></span>|[<span data-ttu-id="6aca8-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="6aca8-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="6aca8-164">Tipo de configuração, por exemplo, configuração e conformidade Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6aca8-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="6aca8-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="6aca8-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="6aca8-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="6aca8-166">uxBehavior</span></span>|[<span data-ttu-id="6aca8-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="6aca8-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="6aca8-168">Definindo a representação do tipo de controle no UX Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6aca8-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="6aca8-169">Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="6aca8-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="6aca8-170">visibility</span><span class="sxs-lookup"><span data-stu-id="6aca8-170">visibility</span></span>|[<span data-ttu-id="6aca8-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="6aca8-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="6aca8-172">Definindo o escopo de visibilidade como UX Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6aca8-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="6aca8-173">Os valores possíveis são: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="6aca8-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="6aca8-174">id</span><span class="sxs-lookup"><span data-stu-id="6aca8-174">id</span></span>|<span data-ttu-id="6aca8-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6aca8-175">String</span></span>|<span data-ttu-id="6aca8-176">Identificador do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-176">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-177">descrição</span><span class="sxs-lookup"><span data-stu-id="6aca8-177">description</span></span>|<span data-ttu-id="6aca8-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6aca8-178">String</span></span>|<span data-ttu-id="6aca8-179">Descrição do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-179">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-180">helpText</span><span class="sxs-lookup"><span data-stu-id="6aca8-180">helpText</span></span>|<span data-ttu-id="6aca8-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6aca8-181">String</span></span>|<span data-ttu-id="6aca8-182">Texto de ajuda do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-182">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-183">nome</span><span class="sxs-lookup"><span data-stu-id="6aca8-183">name</span></span>|<span data-ttu-id="6aca8-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6aca8-184">String</span></span>|<span data-ttu-id="6aca8-185">Nome do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-185">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-186">displayName</span><span class="sxs-lookup"><span data-stu-id="6aca8-186">displayName</span></span>|<span data-ttu-id="6aca8-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6aca8-187">String</span></span>|<span data-ttu-id="6aca8-188">Nome de exibição do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-188">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-189">versão</span><span class="sxs-lookup"><span data-stu-id="6aca8-189">version</span></span>|<span data-ttu-id="6aca8-190">String</span><span class="sxs-lookup"><span data-stu-id="6aca8-190">String</span></span>|<span data-ttu-id="6aca8-191">Versão do item Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-191">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-192">valueDefinition</span><span class="sxs-lookup"><span data-stu-id="6aca8-192">valueDefinition</span></span>|[<span data-ttu-id="6aca8-193">deviceManagementConfigurationSettingValueDefinition</span><span class="sxs-lookup"><span data-stu-id="6aca8-193">deviceManagementConfigurationSettingValueDefinition</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)|<span data-ttu-id="6aca8-194">Definição do valor dessa configuração Herdado de [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-194">Definition of the value for this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-195">defaultValue</span><span class="sxs-lookup"><span data-stu-id="6aca8-195">defaultValue</span></span>|[<span data-ttu-id="6aca8-196">deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="6aca8-196">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="6aca8-197">Valor de configuração padrão para essa configuração Herdado de [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-197">Default setting value for this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-198">dependentOn</span><span class="sxs-lookup"><span data-stu-id="6aca8-198">dependentOn</span></span>|<span data-ttu-id="6aca8-199">[Coleção deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-199">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="6aca8-200">lista de configurações pai essa configuração depende de Herdado de [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-200">list of parent settings this setting is dependent on Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-201">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="6aca8-201">dependedOnBy</span></span>|<span data-ttu-id="6aca8-202">[Coleção deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-202">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="6aca8-203">lista de configurações filho que dependem dessa configuração Herdada de [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aca8-203">list of child settings that depend on this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="6aca8-204">maximumCount</span><span class="sxs-lookup"><span data-stu-id="6aca8-204">maximumCount</span></span>|<span data-ttu-id="6aca8-205">Int32</span><span class="sxs-lookup"><span data-stu-id="6aca8-205">Int32</span></span>|<span data-ttu-id="6aca8-206">Número máximo de configurações simples na coleção.</span><span class="sxs-lookup"><span data-stu-id="6aca8-206">Maximum number of simple settings in the collection.</span></span> <span data-ttu-id="6aca8-207">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="6aca8-207">Valid values 1 to 100</span></span>|
|<span data-ttu-id="6aca8-208">minimumCount</span><span class="sxs-lookup"><span data-stu-id="6aca8-208">minimumCount</span></span>|<span data-ttu-id="6aca8-209">Int32</span><span class="sxs-lookup"><span data-stu-id="6aca8-209">Int32</span></span>|<span data-ttu-id="6aca8-210">Número mínimo de configurações simples na coleção.</span><span class="sxs-lookup"><span data-stu-id="6aca8-210">Minimum number of simple settings in the collection.</span></span> <span data-ttu-id="6aca8-211">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="6aca8-211">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="6aca8-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="6aca8-212">Response</span></span>
<span data-ttu-id="6aca8-213">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6aca8-213">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aca8-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6aca8-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="6aca8-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6aca8-215">Request</span></span>
<span data-ttu-id="6aca8-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6aca8-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 9248

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
  "uxBehavior": "dropdown",
  "visibility": "settingsCatalog",
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

### <a name="response"></a><span data-ttu-id="6aca8-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="6aca8-217">Response</span></span>
<span data-ttu-id="6aca8-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6aca8-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9297

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
  "uxBehavior": "dropdown",
  "visibility": "settingsCatalog",
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




