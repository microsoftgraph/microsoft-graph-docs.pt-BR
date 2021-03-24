---
title: Criar windowsKioskConfiguration
description: Crie um novo objeto windowsKioskConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 700ababe5f7e83ad99c09178f4f398961ab90848
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131096"
---
# <a name="create-windowskioskconfiguration"></a><span data-ttu-id="4d396-103">Criar windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="4d396-103">Create windowsKioskConfiguration</span></span>

<span data-ttu-id="4d396-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d396-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d396-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4d396-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d396-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4d396-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d396-107">Crie um novo [objeto windowsKioskConfiguration.](../resources/intune-deviceconfig-windowskioskconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d396-107">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d396-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4d396-108">Prerequisites</span></span>
<span data-ttu-id="4d396-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d396-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d396-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d396-111">Permission type</span></span>|<span data-ttu-id="4d396-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d396-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d396-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d396-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d396-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d396-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d396-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d396-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d396-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d396-116">Not supported.</span></span>|
|<span data-ttu-id="4d396-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d396-117">Application</span></span>|<span data-ttu-id="4d396-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d396-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d396-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d396-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4d396-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d396-120">Request headers</span></span>
|<span data-ttu-id="4d396-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d396-121">Header</span></span>|<span data-ttu-id="4d396-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4d396-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d396-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d396-123">Authorization</span></span>|<span data-ttu-id="4d396-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d396-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d396-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4d396-125">Accept</span></span>|<span data-ttu-id="4d396-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d396-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d396-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d396-127">Request body</span></span>
<span data-ttu-id="4d396-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsKioskConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4d396-128">In the request body, supply a JSON representation for the windowsKioskConfiguration object.</span></span>

<span data-ttu-id="4d396-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o windowsKioskConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4d396-129">The following table shows the properties that are required when you create the windowsKioskConfiguration.</span></span>

|<span data-ttu-id="4d396-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d396-130">Property</span></span>|<span data-ttu-id="4d396-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d396-131">Type</span></span>|<span data-ttu-id="4d396-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d396-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d396-133">id</span><span class="sxs-lookup"><span data-stu-id="4d396-133">id</span></span>|<span data-ttu-id="4d396-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d396-134">String</span></span>|<span data-ttu-id="4d396-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4d396-135">Key of the entity.</span></span> <span data-ttu-id="4d396-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d396-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d396-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d396-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4d396-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d396-138">DateTimeOffset</span></span>|<span data-ttu-id="4d396-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4d396-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4d396-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d396-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d396-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4d396-141">roleScopeTagIds</span></span>|<span data-ttu-id="4d396-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d396-142">String collection</span></span>|<span data-ttu-id="4d396-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="4d396-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4d396-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d396-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d396-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4d396-145">supportsScopeTags</span></span>|<span data-ttu-id="4d396-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="4d396-146">Boolean</span></span>|<span data-ttu-id="4d396-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="4d396-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4d396-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="4d396-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4d396-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="4d396-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4d396-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4d396-150">This property is read-only.</span></span> <span data-ttu-id="4d396-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d396-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d396-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4d396-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4d396-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4d396-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4d396-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="4d396-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4d396-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d396-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d396-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4d396-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4d396-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4d396-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4d396-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="4d396-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4d396-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d396-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d396-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4d396-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4d396-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4d396-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4d396-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="4d396-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4d396-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d396-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d396-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4d396-164">createdDateTime</span></span>|<span data-ttu-id="4d396-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d396-165">DateTimeOffset</span></span>|<span data-ttu-id="4d396-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4d396-166">DateTime the object was created.</span></span> <span data-ttu-id="4d396-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d396-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d396-168">descrição</span><span class="sxs-lookup"><span data-stu-id="4d396-168">description</span></span>|<span data-ttu-id="4d396-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d396-169">String</span></span>|<span data-ttu-id="4d396-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d396-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4d396-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d396-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d396-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4d396-172">displayName</span></span>|<span data-ttu-id="4d396-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d396-173">String</span></span>|<span data-ttu-id="4d396-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d396-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4d396-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d396-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d396-176">versão</span><span class="sxs-lookup"><span data-stu-id="4d396-176">version</span></span>|<span data-ttu-id="4d396-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4d396-177">Int32</span></span>|<span data-ttu-id="4d396-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d396-178">Version of the device configuration.</span></span> <span data-ttu-id="4d396-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d396-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d396-180">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="4d396-180">kioskProfiles</span></span>|<span data-ttu-id="4d396-181">[Coleção windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)</span><span class="sxs-lookup"><span data-stu-id="4d396-181">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="4d396-182">Essa configuração de política permite definir uma lista de perfis de Quiosque para uma configuração de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="4d396-182">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="4d396-183">Essa coleção pode conter no máximo 3 elementos.</span><span class="sxs-lookup"><span data-stu-id="4d396-183">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="4d396-184">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="4d396-184">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="4d396-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d396-185">String</span></span>|<span data-ttu-id="4d396-186">Especifique a URL padrão para a qual o navegador deve navegar ao iniciar.</span><span class="sxs-lookup"><span data-stu-id="4d396-186">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="4d396-187">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="4d396-187">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="4d396-188">Booleano</span><span class="sxs-lookup"><span data-stu-id="4d396-188">Boolean</span></span>|<span data-ttu-id="4d396-189">Habilita o botão home do navegador de quiosque.</span><span class="sxs-lookup"><span data-stu-id="4d396-189">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="4d396-190">Por padrão, o botão home está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="4d396-190">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="4d396-191">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="4d396-191">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="4d396-192">Booleano</span><span class="sxs-lookup"><span data-stu-id="4d396-192">Boolean</span></span>|<span data-ttu-id="4d396-193">Habilita os botões de navegação do navegador de quiosque(forward/back).</span><span class="sxs-lookup"><span data-stu-id="4d396-193">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="4d396-194">Por padrão, os botões de navegação estão desabilitados.</span><span class="sxs-lookup"><span data-stu-id="4d396-194">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="4d396-195">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="4d396-195">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="4d396-196">Booleano</span><span class="sxs-lookup"><span data-stu-id="4d396-196">Boolean</span></span>|<span data-ttu-id="4d396-197">Habilita o botão de sessão final do navegador de quiosque.</span><span class="sxs-lookup"><span data-stu-id="4d396-197">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="4d396-198">Por padrão, o botão de sessão final está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="4d396-198">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="4d396-199">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="4d396-199">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="4d396-200">Int32</span><span class="sxs-lookup"><span data-stu-id="4d396-200">Int32</span></span>|<span data-ttu-id="4d396-201">Especifique o número de minutos em que a sessão fica ociosa até que o navegador de quiosque seja reiniciado em um estado novo.</span><span class="sxs-lookup"><span data-stu-id="4d396-201">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="4d396-202">Os valores válidos são 1-1440.</span><span class="sxs-lookup"><span data-stu-id="4d396-202">Valid values are 1-1440.</span></span> <span data-ttu-id="4d396-203">Valores válidos de 1 a 1440</span><span class="sxs-lookup"><span data-stu-id="4d396-203">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="4d396-204">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="4d396-204">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="4d396-205">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d396-205">String collection</span></span>|<span data-ttu-id="4d396-206">Especificar URLs para as quais os navegadores de quiosque não devem navegar</span><span class="sxs-lookup"><span data-stu-id="4d396-206">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="4d396-207">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="4d396-207">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="4d396-208">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d396-208">String collection</span></span>|<span data-ttu-id="4d396-209">Especificar URLs para as quais o navegador de quiosque pode navegar</span><span class="sxs-lookup"><span data-stu-id="4d396-209">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="4d396-210">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="4d396-210">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="4d396-211">Booleano</span><span class="sxs-lookup"><span data-stu-id="4d396-211">Boolean</span></span>|<span data-ttu-id="4d396-212">Habilita o modo de quiosque de navegação pública para o navegador do Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="4d396-212">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="4d396-213">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="4d396-213">The Default is false.</span></span>|
|<span data-ttu-id="4d396-214">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="4d396-214">windowsKioskForceUpdateSchedule</span></span>|[<span data-ttu-id="4d396-215">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="4d396-215">windowsKioskForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windowskioskforceupdateschedule.md)|<span data-ttu-id="4d396-216">force update schedule for Kiosk devices.</span><span class="sxs-lookup"><span data-stu-id="4d396-216">force update schedule for Kiosk devices.</span></span>|



## <a name="response"></a><span data-ttu-id="4d396-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d396-217">Response</span></span>
<span data-ttu-id="4d396-218">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d396-218">If successful, this method returns a `201 Created` response code and a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d396-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d396-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d396-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d396-220">Request</span></span>
<span data-ttu-id="4d396-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d396-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="4d396-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d396-222">Response</span></span>
<span data-ttu-id="4d396-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d396-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




