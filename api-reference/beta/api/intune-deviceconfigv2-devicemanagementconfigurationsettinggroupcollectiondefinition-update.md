---
title: Atualizar deviceManagementConfigurationSettingGroupCollectionDefinition
description: Atualize as propriedades de um objeto deviceManagementConfigurationSettingGroupCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 392ae1b5f625502f8f774a52f20ae069182d084a
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665144"
---
# <a name="update-devicemanagementconfigurationsettinggroupcollectiondefinition"></a><span data-ttu-id="9542b-103">Atualizar deviceManagementConfigurationSettingGroupCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="9542b-103">Update deviceManagementConfigurationSettingGroupCollectionDefinition</span></span>

<span data-ttu-id="9542b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9542b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9542b-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9542b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9542b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9542b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9542b-107">Atualize as propriedades de [um objeto deviceManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-107">Update the properties of a [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9542b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9542b-108">Prerequisites</span></span>
<span data-ttu-id="9542b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9542b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9542b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9542b-111">Permission type</span></span>|<span data-ttu-id="9542b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9542b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9542b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9542b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9542b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9542b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9542b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9542b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9542b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9542b-116">Not supported.</span></span>|
|<span data-ttu-id="9542b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9542b-117">Application</span></span>|<span data-ttu-id="9542b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9542b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9542b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9542b-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9542b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9542b-120">Request headers</span></span>
|<span data-ttu-id="9542b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9542b-121">Header</span></span>|<span data-ttu-id="9542b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9542b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9542b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9542b-123">Authorization</span></span>|<span data-ttu-id="9542b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9542b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9542b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9542b-125">Accept</span></span>|<span data-ttu-id="9542b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9542b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9542b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9542b-127">Request body</span></span>
<span data-ttu-id="9542b-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

<span data-ttu-id="9542b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9542b-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md).</span></span>

|<span data-ttu-id="9542b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9542b-130">Property</span></span>|<span data-ttu-id="9542b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9542b-131">Type</span></span>|<span data-ttu-id="9542b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9542b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9542b-133">aplicabilidade</span><span class="sxs-lookup"><span data-stu-id="9542b-133">applicability</span></span>|[<span data-ttu-id="9542b-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="9542b-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="9542b-135">Detalhes sobre qual configuração de dispositivo é aplicável em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9542b-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="9542b-136">accessTypes</span></span>|[<span data-ttu-id="9542b-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="9542b-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="9542b-138">Modo de acesso de leitura/gravação da configuração Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9542b-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="9542b-139">Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="9542b-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="9542b-140">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="9542b-140">keywords</span></span>|<span data-ttu-id="9542b-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9542b-141">String collection</span></span>|<span data-ttu-id="9542b-142">Tokens que para pesquisar configurações em Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9542b-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="9542b-143">infoUrls</span></span>|<span data-ttu-id="9542b-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9542b-144">String collection</span></span>|<span data-ttu-id="9542b-145">Lista de links mais informações para a configuração podem ser encontradas em Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9542b-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="9542b-146">occurrence</span></span>|[<span data-ttu-id="9542b-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="9542b-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="9542b-148">Indica se a configuração é necessária ou não Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9542b-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="9542b-149">baseUri</span></span>|<span data-ttu-id="9542b-150">String</span><span class="sxs-lookup"><span data-stu-id="9542b-150">String</span></span>|<span data-ttu-id="9542b-151">Caminho base CSP Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9542b-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="9542b-152">offsetUri</span></span>|<span data-ttu-id="9542b-153">String</span><span class="sxs-lookup"><span data-stu-id="9542b-153">String</span></span>|<span data-ttu-id="9542b-154">Caminho de deslocamento CSP da Base Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9542b-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="9542b-155">rootDefinitionId</span></span>|<span data-ttu-id="9542b-156">String</span><span class="sxs-lookup"><span data-stu-id="9542b-156">String</span></span>|<span data-ttu-id="9542b-157">Definição de configuração raiz se a configuração for uma configuração filho.</span><span class="sxs-lookup"><span data-stu-id="9542b-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="9542b-158">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9542b-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="9542b-159">categoryId</span></span>|<span data-ttu-id="9542b-160">String</span><span class="sxs-lookup"><span data-stu-id="9542b-160">String</span></span>|<span data-ttu-id="9542b-161">Especifica o grupo de área no qual a configuração está configurada em um provedor de serviços de configuração especificado (CSP) Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9542b-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="9542b-162">settingUsage</span></span>|[<span data-ttu-id="9542b-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="9542b-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="9542b-164">Tipo de configuração, por exemplo, configuração e conformidade Herdada de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9542b-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="9542b-165">Os valores possíveis são: `none` e `configuration`.</span><span class="sxs-lookup"><span data-stu-id="9542b-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="9542b-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="9542b-166">uxBehavior</span></span>|[<span data-ttu-id="9542b-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="9542b-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="9542b-168">Definindo a representação do tipo de controle no UX Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9542b-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="9542b-169">Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="9542b-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="9542b-170">visibility</span><span class="sxs-lookup"><span data-stu-id="9542b-170">visibility</span></span>|[<span data-ttu-id="9542b-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="9542b-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="9542b-172">Definindo o escopo de visibilidade como UX Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9542b-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="9542b-173">Os valores possíveis são: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="9542b-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="9542b-174">referredSettingInformationList</span><span class="sxs-lookup"><span data-stu-id="9542b-174">referredSettingInformationList</span></span>|<span data-ttu-id="9542b-175">[coleção deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-175">[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) collection</span></span>|<span data-ttu-id="9542b-176">Lista de informações de configuração referidas.</span><span class="sxs-lookup"><span data-stu-id="9542b-176">List of referred setting information.</span></span> <span data-ttu-id="9542b-177">Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-177">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9542b-178">id</span><span class="sxs-lookup"><span data-stu-id="9542b-178">id</span></span>|<span data-ttu-id="9542b-179">String</span><span class="sxs-lookup"><span data-stu-id="9542b-179">String</span></span>|<span data-ttu-id="9542b-180">Identificador do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-180">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9542b-181">descrição</span><span class="sxs-lookup"><span data-stu-id="9542b-181">description</span></span>|<span data-ttu-id="9542b-182">String</span><span class="sxs-lookup"><span data-stu-id="9542b-182">String</span></span>|<span data-ttu-id="9542b-183">Descrição do item Herdado [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-183">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9542b-184">helpText</span><span class="sxs-lookup"><span data-stu-id="9542b-184">helpText</span></span>|<span data-ttu-id="9542b-185">String</span><span class="sxs-lookup"><span data-stu-id="9542b-185">String</span></span>|<span data-ttu-id="9542b-186">Texto de ajuda do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-186">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9542b-187">nome</span><span class="sxs-lookup"><span data-stu-id="9542b-187">name</span></span>|<span data-ttu-id="9542b-188">String</span><span class="sxs-lookup"><span data-stu-id="9542b-188">String</span></span>|<span data-ttu-id="9542b-189">Nome do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-189">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9542b-190">displayName</span><span class="sxs-lookup"><span data-stu-id="9542b-190">displayName</span></span>|<span data-ttu-id="9542b-191">String</span><span class="sxs-lookup"><span data-stu-id="9542b-191">String</span></span>|<span data-ttu-id="9542b-192">Nome de exibição do item Herdado de [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-192">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9542b-193">versão</span><span class="sxs-lookup"><span data-stu-id="9542b-193">version</span></span>|<span data-ttu-id="9542b-194">String</span><span class="sxs-lookup"><span data-stu-id="9542b-194">String</span></span>|<span data-ttu-id="9542b-195">Versão do item Herdada [de deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-195">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="9542b-196">childIds</span><span class="sxs-lookup"><span data-stu-id="9542b-196">childIds</span></span>|<span data-ttu-id="9542b-197">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9542b-197">String collection</span></span>|<span data-ttu-id="9542b-198">Configurações filho dependentes para esse grupo de configurações Herdadas de [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-198">Dependent child settings to this group of settings Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="9542b-199">dependentOn</span><span class="sxs-lookup"><span data-stu-id="9542b-199">dependentOn</span></span>|<span data-ttu-id="9542b-200">[Coleção deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-200">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="9542b-201">Lista de dependências do grupo de configurações Herdado de [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-201">List of Dependencies for the setting group Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="9542b-202">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="9542b-202">dependedOnBy</span></span>|<span data-ttu-id="9542b-203">[Coleção deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-203">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="9542b-204">Lista de configurações filho que dependem dessa configuração Herdada de [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9542b-204">List of child settings that depend on this setting Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="9542b-205">maximumCount</span><span class="sxs-lookup"><span data-stu-id="9542b-205">maximumCount</span></span>|<span data-ttu-id="9542b-206">Int32</span><span class="sxs-lookup"><span data-stu-id="9542b-206">Int32</span></span>|<span data-ttu-id="9542b-207">Número máximo de contagem de grupos de configuração na coleção.</span><span class="sxs-lookup"><span data-stu-id="9542b-207">Maximum number of setting group count in the collection.</span></span> <span data-ttu-id="9542b-208">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="9542b-208">Valid values 1 to 100</span></span>|
|<span data-ttu-id="9542b-209">minimumCount</span><span class="sxs-lookup"><span data-stu-id="9542b-209">minimumCount</span></span>|<span data-ttu-id="9542b-210">Int32</span><span class="sxs-lookup"><span data-stu-id="9542b-210">Int32</span></span>|<span data-ttu-id="9542b-211">Número mínimo de contagem de grupos de configuração na coleção.</span><span class="sxs-lookup"><span data-stu-id="9542b-211">Minimum number of setting group count in the collection.</span></span> <span data-ttu-id="9542b-212">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="9542b-212">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="9542b-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="9542b-213">Response</span></span>
<span data-ttu-id="9542b-214">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9542b-214">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9542b-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9542b-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="9542b-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9542b-216">Request</span></span>
<span data-ttu-id="9542b-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9542b-217">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1785

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionDefinition",
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
  ],
  "maximumCount": 12,
  "minimumCount": 12
}
```

### <a name="response"></a><span data-ttu-id="9542b-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="9542b-218">Response</span></span>
<span data-ttu-id="9542b-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9542b-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1834

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionDefinition",
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
  "id": "739da194-a194-739d-94a1-9d7394a19d73",
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
  ],
  "maximumCount": 12,
  "minimumCount": 12
}
```




