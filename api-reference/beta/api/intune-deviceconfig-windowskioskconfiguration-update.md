---
title: Atualizar windowsKioskConfiguration
description: Atualiza as propriedades de um objeto windowsKioskConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8898a7fa356ffbce429d031fbc2f3ababab2bc65
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42734866"
---
# <a name="update-windowskioskconfiguration"></a><span data-ttu-id="88cfb-103">Atualizar windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="88cfb-103">Update windowsKioskConfiguration</span></span>

> <span data-ttu-id="88cfb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88cfb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88cfb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88cfb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88cfb-106">Atualiza as propriedades de um objeto [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="88cfb-106">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88cfb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88cfb-107">Prerequisites</span></span>
<span data-ttu-id="88cfb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88cfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88cfb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88cfb-110">Permission type</span></span>|<span data-ttu-id="88cfb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="88cfb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88cfb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88cfb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88cfb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88cfb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88cfb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88cfb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88cfb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88cfb-115">Not supported.</span></span>|
|<span data-ttu-id="88cfb-116">Application</span><span class="sxs-lookup"><span data-stu-id="88cfb-116">Application</span></span>|<span data-ttu-id="88cfb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88cfb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88cfb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88cfb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="88cfb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88cfb-119">Request headers</span></span>
|<span data-ttu-id="88cfb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88cfb-120">Header</span></span>|<span data-ttu-id="88cfb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="88cfb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88cfb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="88cfb-122">Authorization</span></span>|<span data-ttu-id="88cfb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88cfb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88cfb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88cfb-124">Accept</span></span>|<span data-ttu-id="88cfb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="88cfb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88cfb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88cfb-126">Request body</span></span>
<span data-ttu-id="88cfb-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="88cfb-127">In the request body, supply a JSON representation for the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

<span data-ttu-id="88cfb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="88cfb-128">The following table shows the properties that are required when you create the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>

|<span data-ttu-id="88cfb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88cfb-129">Property</span></span>|<span data-ttu-id="88cfb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="88cfb-130">Type</span></span>|<span data-ttu-id="88cfb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="88cfb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88cfb-132">id</span><span class="sxs-lookup"><span data-stu-id="88cfb-132">id</span></span>|<span data-ttu-id="88cfb-133">String</span><span class="sxs-lookup"><span data-stu-id="88cfb-133">String</span></span>|<span data-ttu-id="88cfb-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="88cfb-134">Key of the entity.</span></span> <span data-ttu-id="88cfb-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88cfb-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88cfb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88cfb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="88cfb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88cfb-137">DateTimeOffset</span></span>|<span data-ttu-id="88cfb-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="88cfb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="88cfb-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88cfb-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88cfb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="88cfb-140">roleScopeTagIds</span></span>|<span data-ttu-id="88cfb-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="88cfb-141">String collection</span></span>|<span data-ttu-id="88cfb-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="88cfb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="88cfb-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88cfb-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88cfb-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="88cfb-144">supportsScopeTags</span></span>|<span data-ttu-id="88cfb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="88cfb-145">Boolean</span></span>|<span data-ttu-id="88cfb-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="88cfb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="88cfb-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="88cfb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="88cfb-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="88cfb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="88cfb-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="88cfb-149">This property is read-only.</span></span> <span data-ttu-id="88cfb-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88cfb-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88cfb-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="88cfb-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="88cfb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="88cfb-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="88cfb-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="88cfb-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="88cfb-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88cfb-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88cfb-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="88cfb-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="88cfb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="88cfb-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="88cfb-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="88cfb-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="88cfb-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88cfb-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88cfb-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="88cfb-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="88cfb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="88cfb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="88cfb-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="88cfb-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="88cfb-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88cfb-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88cfb-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88cfb-163">createdDateTime</span></span>|<span data-ttu-id="88cfb-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88cfb-164">DateTimeOffset</span></span>|<span data-ttu-id="88cfb-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="88cfb-165">DateTime the object was created.</span></span> <span data-ttu-id="88cfb-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88cfb-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88cfb-167">description</span><span class="sxs-lookup"><span data-stu-id="88cfb-167">description</span></span>|<span data-ttu-id="88cfb-168">String</span><span class="sxs-lookup"><span data-stu-id="88cfb-168">String</span></span>|<span data-ttu-id="88cfb-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="88cfb-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="88cfb-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88cfb-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88cfb-171">displayName</span><span class="sxs-lookup"><span data-stu-id="88cfb-171">displayName</span></span>|<span data-ttu-id="88cfb-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88cfb-172">String</span></span>|<span data-ttu-id="88cfb-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="88cfb-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="88cfb-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88cfb-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88cfb-175">versão</span><span class="sxs-lookup"><span data-stu-id="88cfb-175">version</span></span>|<span data-ttu-id="88cfb-176">Int32</span><span class="sxs-lookup"><span data-stu-id="88cfb-176">Int32</span></span>|<span data-ttu-id="88cfb-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="88cfb-177">Version of the device configuration.</span></span> <span data-ttu-id="88cfb-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88cfb-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88cfb-179">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="88cfb-179">kioskProfiles</span></span>|<span data-ttu-id="88cfb-180">coleção [windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)</span><span class="sxs-lookup"><span data-stu-id="88cfb-180">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="88cfb-181">Essa configuração de política permite definir uma lista de perfis de quiosque para uma configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="88cfb-181">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="88cfb-182">Essa coleção pode conter um máximo de 3 elementos.</span><span class="sxs-lookup"><span data-stu-id="88cfb-182">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="88cfb-183">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="88cfb-183">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="88cfb-184">String</span><span class="sxs-lookup"><span data-stu-id="88cfb-184">String</span></span>|<span data-ttu-id="88cfb-185">Especifique a URL padrão para a qual o navegador deve navegar na inicialização.</span><span class="sxs-lookup"><span data-stu-id="88cfb-185">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="88cfb-186">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="88cfb-186">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="88cfb-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="88cfb-187">Boolean</span></span>|<span data-ttu-id="88cfb-188">Habilite o botão Home do navegador quiosque.</span><span class="sxs-lookup"><span data-stu-id="88cfb-188">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="88cfb-189">Por padrão, o botão página inicial está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="88cfb-189">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="88cfb-190">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="88cfb-190">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="88cfb-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="88cfb-191">Boolean</span></span>|<span data-ttu-id="88cfb-192">Habilite os botões de navegação do navegador quiosque (avançar/voltar).</span><span class="sxs-lookup"><span data-stu-id="88cfb-192">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="88cfb-193">Por padrão, os botões de navegação estão desabilitados.</span><span class="sxs-lookup"><span data-stu-id="88cfb-193">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="88cfb-194">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="88cfb-194">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="88cfb-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="88cfb-195">Boolean</span></span>|<span data-ttu-id="88cfb-196">Habilite o botão encerrar sessão do navegador quiosque.</span><span class="sxs-lookup"><span data-stu-id="88cfb-196">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="88cfb-197">Por padrão, o botão encerrar sessão está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="88cfb-197">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="88cfb-198">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="88cfb-198">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="88cfb-199">Int32</span><span class="sxs-lookup"><span data-stu-id="88cfb-199">Int32</span></span>|<span data-ttu-id="88cfb-200">Especificar o número de minutos que a sessão ficará ociosa até que o navegador quiosque seja reiniciado em um estado novo.</span><span class="sxs-lookup"><span data-stu-id="88cfb-200">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="88cfb-201">Os valores válidos são 1-1440.</span><span class="sxs-lookup"><span data-stu-id="88cfb-201">Valid values are 1-1440.</span></span> <span data-ttu-id="88cfb-202">Valores válidos de 1 a 1440</span><span class="sxs-lookup"><span data-stu-id="88cfb-202">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="88cfb-203">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="88cfb-203">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="88cfb-204">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="88cfb-204">String collection</span></span>|<span data-ttu-id="88cfb-205">Especificar URLs às quais os navegadores quiosques não devem navegar</span><span class="sxs-lookup"><span data-stu-id="88cfb-205">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="88cfb-206">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="88cfb-206">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="88cfb-207">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="88cfb-207">String collection</span></span>|<span data-ttu-id="88cfb-208">Especificar URLs às quais o navegador de quiosque pode navegar</span><span class="sxs-lookup"><span data-stu-id="88cfb-208">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="88cfb-209">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="88cfb-209">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="88cfb-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="88cfb-210">Boolean</span></span>|<span data-ttu-id="88cfb-211">Habilitar modo quiosque de navegação pública para o navegador Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="88cfb-211">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="88cfb-212">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="88cfb-212">The Default is false.</span></span>|
|<span data-ttu-id="88cfb-213">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="88cfb-213">windowsKioskForceUpdateSchedule</span></span>|[<span data-ttu-id="88cfb-214">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="88cfb-214">windowsKioskForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windowskioskforceupdateschedule.md)|<span data-ttu-id="88cfb-215">forçar agendamento de atualização para dispositivos quiosque.</span><span class="sxs-lookup"><span data-stu-id="88cfb-215">force update schedule for Kiosk devices.</span></span>|



## <a name="response"></a><span data-ttu-id="88cfb-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="88cfb-216">Response</span></span>
<span data-ttu-id="88cfb-217">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88cfb-217">If successful, this method returns a `200 OK` response code and an updated [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88cfb-218">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88cfb-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="88cfb-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88cfb-219">Request</span></span>
<span data-ttu-id="88cfb-220">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88cfb-220">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2829

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
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
  "kioskProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsKioskProfile",
      "profileId": "Profile Id value",
      "profileName": "Profile Name value",
      "appConfiguration": {
        "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
        "apps": [
          {
            "@odata.type": "microsoft.graph.windowsKioskUWPApp",
            "startLayoutTileSize": "small",
            "name": "Name value",
            "appType": "store",
            "autoLaunch": true,
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
        "allowAccessToDownloadsFolder": true,
        "disallowDesktopApps": true,
        "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
      },
      "userAccountsConfiguration": [
        {
          "@odata.type": "microsoft.graph.windowsKioskVisitor"
        }
      ]
    }
  ],
  "kioskBrowserDefaultUrl": "https://example.com/kioskBrowserDefaultUrl/",
  "kioskBrowserEnableHomeButton": true,
  "kioskBrowserEnableNavigationButtons": true,
  "kioskBrowserEnableEndSessionButton": true,
  "kioskBrowserRestartOnIdleTimeInMinutes": 6,
  "kioskBrowserBlockedURLs": [
    "Kiosk Browser Blocked URLs value"
  ],
  "kioskBrowserBlockedUrlExceptions": [
    "Kiosk Browser Blocked Url Exceptions value"
  ],
  "edgeKioskEnablePublicBrowsing": true,
  "windowsKioskForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "dayofWeek": "monday",
    "dayofMonth": 10,
    "runImmediatelyIfAfterStartDateTime": true
  }
}
```

### <a name="response"></a><span data-ttu-id="88cfb-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="88cfb-221">Response</span></span>
<span data-ttu-id="88cfb-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88cfb-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3001

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "id": "146a990b-990b-146a-0b99-6a140b996a14",
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
  "kioskProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsKioskProfile",
      "profileId": "Profile Id value",
      "profileName": "Profile Name value",
      "appConfiguration": {
        "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
        "apps": [
          {
            "@odata.type": "microsoft.graph.windowsKioskUWPApp",
            "startLayoutTileSize": "small",
            "name": "Name value",
            "appType": "store",
            "autoLaunch": true,
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
        "allowAccessToDownloadsFolder": true,
        "disallowDesktopApps": true,
        "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
      },
      "userAccountsConfiguration": [
        {
          "@odata.type": "microsoft.graph.windowsKioskVisitor"
        }
      ]
    }
  ],
  "kioskBrowserDefaultUrl": "https://example.com/kioskBrowserDefaultUrl/",
  "kioskBrowserEnableHomeButton": true,
  "kioskBrowserEnableNavigationButtons": true,
  "kioskBrowserEnableEndSessionButton": true,
  "kioskBrowserRestartOnIdleTimeInMinutes": 6,
  "kioskBrowserBlockedURLs": [
    "Kiosk Browser Blocked URLs value"
  ],
  "kioskBrowserBlockedUrlExceptions": [
    "Kiosk Browser Blocked Url Exceptions value"
  ],
  "edgeKioskEnablePublicBrowsing": true,
  "windowsKioskForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "dayofWeek": "monday",
    "dayofMonth": 10,
    "runImmediatelyIfAfterStartDateTime": true
  }
}
```




