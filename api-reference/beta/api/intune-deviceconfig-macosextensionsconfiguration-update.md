---
title: Atualizar macOSExtensionsConfiguration
description: Atualize as propriedades de um objeto macOSExtensionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6deff87a77cff0c3c5581223b5f85b10d93b9856
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151148"
---
# <a name="update-macosextensionsconfiguration"></a><span data-ttu-id="01e9a-103">Atualizar macOSExtensionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="01e9a-103">Update macOSExtensionsConfiguration</span></span>

<span data-ttu-id="01e9a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01e9a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01e9a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="01e9a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01e9a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01e9a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01e9a-107">Atualize as propriedades de [um objeto macOSExtensionsConfiguration.](../resources/intune-deviceconfig-macosextensionsconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01e9a-107">Update the properties of a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01e9a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01e9a-108">Prerequisites</span></span>
<span data-ttu-id="01e9a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01e9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01e9a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01e9a-111">Permission type</span></span>|<span data-ttu-id="01e9a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01e9a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01e9a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01e9a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01e9a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01e9a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01e9a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01e9a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01e9a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01e9a-116">Not supported.</span></span>|
|<span data-ttu-id="01e9a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01e9a-117">Application</span></span>|<span data-ttu-id="01e9a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01e9a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01e9a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01e9a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="01e9a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01e9a-120">Request headers</span></span>
|<span data-ttu-id="01e9a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01e9a-121">Header</span></span>|<span data-ttu-id="01e9a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="01e9a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01e9a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="01e9a-123">Authorization</span></span>|<span data-ttu-id="01e9a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01e9a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01e9a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="01e9a-125">Accept</span></span>|<span data-ttu-id="01e9a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01e9a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01e9a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01e9a-127">Request body</span></span>
<span data-ttu-id="01e9a-128">No corpo da solicitação, fornece uma representação JSON para o [objeto macOSExtensionsConfiguration.](../resources/intune-deviceconfig-macosextensionsconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01e9a-128">In the request body, supply a JSON representation for the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

<span data-ttu-id="01e9a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01e9a-129">The following table shows the properties that are required when you create the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span></span>

|<span data-ttu-id="01e9a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01e9a-130">Property</span></span>|<span data-ttu-id="01e9a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="01e9a-131">Type</span></span>|<span data-ttu-id="01e9a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="01e9a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01e9a-133">id</span><span class="sxs-lookup"><span data-stu-id="01e9a-133">id</span></span>|<span data-ttu-id="01e9a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01e9a-134">String</span></span>|<span data-ttu-id="01e9a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="01e9a-135">Key of the entity.</span></span> <span data-ttu-id="01e9a-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01e9a-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01e9a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01e9a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="01e9a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01e9a-138">DateTimeOffset</span></span>|<span data-ttu-id="01e9a-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="01e9a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="01e9a-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01e9a-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01e9a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="01e9a-141">roleScopeTagIds</span></span>|<span data-ttu-id="01e9a-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="01e9a-142">String collection</span></span>|<span data-ttu-id="01e9a-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="01e9a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="01e9a-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01e9a-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01e9a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="01e9a-145">supportsScopeTags</span></span>|<span data-ttu-id="01e9a-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="01e9a-146">Boolean</span></span>|<span data-ttu-id="01e9a-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="01e9a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="01e9a-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="01e9a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="01e9a-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="01e9a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="01e9a-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="01e9a-150">This property is read-only.</span></span> <span data-ttu-id="01e9a-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01e9a-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01e9a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="01e9a-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="01e9a-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="01e9a-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="01e9a-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="01e9a-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="01e9a-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01e9a-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01e9a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="01e9a-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="01e9a-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="01e9a-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="01e9a-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="01e9a-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="01e9a-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01e9a-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01e9a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="01e9a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="01e9a-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="01e9a-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="01e9a-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="01e9a-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="01e9a-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01e9a-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01e9a-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01e9a-164">createdDateTime</span></span>|<span data-ttu-id="01e9a-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01e9a-165">DateTimeOffset</span></span>|<span data-ttu-id="01e9a-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="01e9a-166">DateTime the object was created.</span></span> <span data-ttu-id="01e9a-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01e9a-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01e9a-168">descrição</span><span class="sxs-lookup"><span data-stu-id="01e9a-168">description</span></span>|<span data-ttu-id="01e9a-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01e9a-169">String</span></span>|<span data-ttu-id="01e9a-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="01e9a-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="01e9a-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01e9a-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01e9a-172">displayName</span><span class="sxs-lookup"><span data-stu-id="01e9a-172">displayName</span></span>|<span data-ttu-id="01e9a-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01e9a-173">String</span></span>|<span data-ttu-id="01e9a-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="01e9a-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="01e9a-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01e9a-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01e9a-176">versão</span><span class="sxs-lookup"><span data-stu-id="01e9a-176">version</span></span>|<span data-ttu-id="01e9a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="01e9a-177">Int32</span></span>|<span data-ttu-id="01e9a-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="01e9a-178">Version of the device configuration.</span></span> <span data-ttu-id="01e9a-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01e9a-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01e9a-180">kernelExtensionOverridesAllowed</span><span class="sxs-lookup"><span data-stu-id="01e9a-180">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="01e9a-181">Booleano</span><span class="sxs-lookup"><span data-stu-id="01e9a-181">Boolean</span></span>|<span data-ttu-id="01e9a-182">Se definido como true, os usuários podem aprovar extensões de kernel adicionais não explicitamente permitidas pelos perfis de configurações.</span><span class="sxs-lookup"><span data-stu-id="01e9a-182">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="01e9a-183">kernelExtensionAllowedTeamIdentifiers</span><span class="sxs-lookup"><span data-stu-id="01e9a-183">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="01e9a-184">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="01e9a-184">String collection</span></span>|<span data-ttu-id="01e9a-185">Todas as extensões de kernel assinadas pelos identificadores de equipe nesta lista terão permissão para carregar.</span><span class="sxs-lookup"><span data-stu-id="01e9a-185">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="01e9a-186">kernelExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="01e9a-186">kernelExtensionsAllowed</span></span>|<span data-ttu-id="01e9a-187">[Coleção macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md)</span><span class="sxs-lookup"><span data-stu-id="01e9a-187">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="01e9a-188">Uma lista de extensões de kernel que poderão ser carregadas.</span><span class="sxs-lookup"><span data-stu-id="01e9a-188">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="01e9a-189">.</span><span class="sxs-lookup"><span data-stu-id="01e9a-189">.</span></span> <span data-ttu-id="01e9a-190">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="01e9a-190">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="01e9a-191">systemExtensionsBlockOverride</span><span class="sxs-lookup"><span data-stu-id="01e9a-191">systemExtensionsBlockOverride</span></span>|<span data-ttu-id="01e9a-192">Booleano</span><span class="sxs-lookup"><span data-stu-id="01e9a-192">Boolean</span></span>|<span data-ttu-id="01e9a-193">Obtém ou define se o usuário deve permitir que o usuário aprove extensões adicionais do sistema não explicitamente permitidas pelos perfis de configuração.</span><span class="sxs-lookup"><span data-stu-id="01e9a-193">Gets or sets whether to allow the user to approve additional system extensions not explicitly allowed by configuration profiles.</span></span>|
|<span data-ttu-id="01e9a-194">systemExtensionsAllowedTeamIdentifiers</span><span class="sxs-lookup"><span data-stu-id="01e9a-194">systemExtensionsAllowedTeamIdentifiers</span></span>|<span data-ttu-id="01e9a-195">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="01e9a-195">String collection</span></span>|<span data-ttu-id="01e9a-196">Obtém ou define uma lista de identificadores de equipe permitidos.</span><span class="sxs-lookup"><span data-stu-id="01e9a-196">Gets or sets a list of allowed team identifiers.</span></span> <span data-ttu-id="01e9a-197">Qualquer extensão do sistema assinada com qualquer um dos identificadores de equipe especificados será aprovada.</span><span class="sxs-lookup"><span data-stu-id="01e9a-197">Any system extension signed with any of the specified team identifiers will be approved.</span></span>|
|<span data-ttu-id="01e9a-198">systemExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="01e9a-198">systemExtensionsAllowed</span></span>|<span data-ttu-id="01e9a-199">[Coleção macOSSystemExtension](../resources/intune-deviceconfig-macossystemextension.md)</span><span class="sxs-lookup"><span data-stu-id="01e9a-199">[macOSSystemExtension](../resources/intune-deviceconfig-macossystemextension.md) collection</span></span>|<span data-ttu-id="01e9a-200">Obtém ou define uma lista de extensões de sistema macOS permitidas.</span><span class="sxs-lookup"><span data-stu-id="01e9a-200">Gets or sets a list of allowed macOS system extensions.</span></span> <span data-ttu-id="01e9a-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="01e9a-201">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="01e9a-202">systemExtensionsAllowedTypes</span><span class="sxs-lookup"><span data-stu-id="01e9a-202">systemExtensionsAllowedTypes</span></span>|<span data-ttu-id="01e9a-203">[Coleção macOSSystemExtensionTypeMapping](../resources/intune-deviceconfig-macossystemextensiontypemapping.md)</span><span class="sxs-lookup"><span data-stu-id="01e9a-203">[macOSSystemExtensionTypeMapping](../resources/intune-deviceconfig-macossystemextensiontypemapping.md) collection</span></span>|<span data-ttu-id="01e9a-204">Obtém ou define uma lista de tipos de extensão do sistema macOS permitidos.</span><span class="sxs-lookup"><span data-stu-id="01e9a-204">Gets or sets a list of allowed macOS system extension types.</span></span> <span data-ttu-id="01e9a-205">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="01e9a-205">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="01e9a-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="01e9a-206">Response</span></span>
<span data-ttu-id="01e9a-207">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01e9a-207">If successful, this method returns a `200 OK` response code and an updated [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01e9a-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01e9a-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="01e9a-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01e9a-209">Request</span></span>
<span data-ttu-id="01e9a-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01e9a-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1965

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "Kernel Extension Allowed Team Identifiers value"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ],
  "systemExtensionsBlockOverride": true,
  "systemExtensionsAllowedTeamIdentifiers": [
    "System Extensions Allowed Team Identifiers value"
  ],
  "systemExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ],
  "systemExtensionsAllowedTypes": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping",
      "teamIdentifier": "Team Identifier value",
      "allowedTypes": "networkExtensionsAllowed"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="01e9a-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="01e9a-211">Response</span></span>
<span data-ttu-id="01e9a-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01e9a-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2137

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "id": "c273f4f6-f4f6-c273-f6f4-73c2f6f473c2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "Kernel Extension Allowed Team Identifiers value"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ],
  "systemExtensionsBlockOverride": true,
  "systemExtensionsAllowedTeamIdentifiers": [
    "System Extensions Allowed Team Identifiers value"
  ],
  "systemExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ],
  "systemExtensionsAllowedTypes": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping",
      "teamIdentifier": "Team Identifier value",
      "allowedTypes": "networkExtensionsAllowed"
    }
  ]
}
```




