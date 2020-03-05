---
title: Criar windowsKioskConfiguration
description: Criar um novo objeto windowsKioskConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ea00cec81315b8b260db4b571c593df0718c3161
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42475758"
---
# <a name="create-windowskioskconfiguration"></a><span data-ttu-id="89376-103">Criar windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="89376-103">Create windowsKioskConfiguration</span></span>

<span data-ttu-id="89376-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="89376-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89376-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="89376-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89376-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89376-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89376-107">Criar um novo objeto [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="89376-107">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89376-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89376-108">Prerequisites</span></span>
<span data-ttu-id="89376-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89376-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89376-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89376-111">Permission type</span></span>|<span data-ttu-id="89376-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="89376-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89376-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89376-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89376-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89376-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89376-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89376-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89376-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89376-116">Not supported.</span></span>|
|<span data-ttu-id="89376-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89376-117">Application</span></span>|<span data-ttu-id="89376-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89376-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89376-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89376-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="89376-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89376-120">Request headers</span></span>
|<span data-ttu-id="89376-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89376-121">Header</span></span>|<span data-ttu-id="89376-122">Valor</span><span class="sxs-lookup"><span data-stu-id="89376-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89376-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="89376-123">Authorization</span></span>|<span data-ttu-id="89376-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89376-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89376-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="89376-125">Accept</span></span>|<span data-ttu-id="89376-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89376-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89376-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89376-127">Request body</span></span>
<span data-ttu-id="89376-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsKioskConfiguration.</span><span class="sxs-lookup"><span data-stu-id="89376-128">In the request body, supply a JSON representation for the windowsKioskConfiguration object.</span></span>

<span data-ttu-id="89376-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsKioskConfiguration.</span><span class="sxs-lookup"><span data-stu-id="89376-129">The following table shows the properties that are required when you create the windowsKioskConfiguration.</span></span>

|<span data-ttu-id="89376-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89376-130">Property</span></span>|<span data-ttu-id="89376-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="89376-131">Type</span></span>|<span data-ttu-id="89376-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="89376-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89376-133">id</span><span class="sxs-lookup"><span data-stu-id="89376-133">id</span></span>|<span data-ttu-id="89376-134">String</span><span class="sxs-lookup"><span data-stu-id="89376-134">String</span></span>|<span data-ttu-id="89376-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="89376-135">Key of the entity.</span></span> <span data-ttu-id="89376-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89376-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89376-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89376-137">lastModifiedDateTime</span></span>|<span data-ttu-id="89376-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89376-138">DateTimeOffset</span></span>|<span data-ttu-id="89376-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="89376-139">DateTime the object was last modified.</span></span> <span data-ttu-id="89376-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89376-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89376-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="89376-141">roleScopeTagIds</span></span>|<span data-ttu-id="89376-142">String collection</span><span class="sxs-lookup"><span data-stu-id="89376-142">String collection</span></span>|<span data-ttu-id="89376-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="89376-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="89376-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89376-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89376-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="89376-145">supportsScopeTags</span></span>|<span data-ttu-id="89376-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="89376-146">Boolean</span></span>|<span data-ttu-id="89376-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="89376-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="89376-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="89376-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="89376-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="89376-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="89376-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="89376-150">This property is read-only.</span></span> <span data-ttu-id="89376-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89376-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89376-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="89376-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="89376-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="89376-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="89376-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="89376-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="89376-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89376-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89376-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="89376-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="89376-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="89376-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="89376-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="89376-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="89376-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89376-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89376-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="89376-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="89376-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="89376-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="89376-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="89376-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="89376-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89376-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89376-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89376-164">createdDateTime</span></span>|<span data-ttu-id="89376-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89376-165">DateTimeOffset</span></span>|<span data-ttu-id="89376-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="89376-166">DateTime the object was created.</span></span> <span data-ttu-id="89376-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89376-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89376-168">description</span><span class="sxs-lookup"><span data-stu-id="89376-168">description</span></span>|<span data-ttu-id="89376-169">String</span><span class="sxs-lookup"><span data-stu-id="89376-169">String</span></span>|<span data-ttu-id="89376-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="89376-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="89376-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89376-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89376-172">displayName</span><span class="sxs-lookup"><span data-stu-id="89376-172">displayName</span></span>|<span data-ttu-id="89376-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89376-173">String</span></span>|<span data-ttu-id="89376-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="89376-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="89376-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89376-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89376-176">versão</span><span class="sxs-lookup"><span data-stu-id="89376-176">version</span></span>|<span data-ttu-id="89376-177">Int32</span><span class="sxs-lookup"><span data-stu-id="89376-177">Int32</span></span>|<span data-ttu-id="89376-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="89376-178">Version of the device configuration.</span></span> <span data-ttu-id="89376-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89376-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89376-180">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="89376-180">kioskProfiles</span></span>|<span data-ttu-id="89376-181">coleção [windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)</span><span class="sxs-lookup"><span data-stu-id="89376-181">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="89376-182">Essa configuração de política permite definir uma lista de perfis de quiosque para uma configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="89376-182">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="89376-183">Essa coleção pode conter um máximo de 3 elementos.</span><span class="sxs-lookup"><span data-stu-id="89376-183">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="89376-184">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="89376-184">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="89376-185">String</span><span class="sxs-lookup"><span data-stu-id="89376-185">String</span></span>|<span data-ttu-id="89376-186">Especifique a URL padrão para a qual o navegador deve navegar na inicialização.</span><span class="sxs-lookup"><span data-stu-id="89376-186">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="89376-187">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="89376-187">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="89376-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="89376-188">Boolean</span></span>|<span data-ttu-id="89376-189">Habilite o botão Home do navegador quiosque.</span><span class="sxs-lookup"><span data-stu-id="89376-189">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="89376-190">Por padrão, o botão página inicial está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="89376-190">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="89376-191">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="89376-191">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="89376-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="89376-192">Boolean</span></span>|<span data-ttu-id="89376-193">Habilite os botões de navegação do navegador quiosque (avançar/voltar).</span><span class="sxs-lookup"><span data-stu-id="89376-193">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="89376-194">Por padrão, os botões de navegação estão desabilitados.</span><span class="sxs-lookup"><span data-stu-id="89376-194">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="89376-195">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="89376-195">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="89376-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="89376-196">Boolean</span></span>|<span data-ttu-id="89376-197">Habilite o botão encerrar sessão do navegador quiosque.</span><span class="sxs-lookup"><span data-stu-id="89376-197">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="89376-198">Por padrão, o botão encerrar sessão está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="89376-198">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="89376-199">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="89376-199">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="89376-200">Int32</span><span class="sxs-lookup"><span data-stu-id="89376-200">Int32</span></span>|<span data-ttu-id="89376-201">Especificar o número de minutos que a sessão ficará ociosa até que o navegador quiosque seja reiniciado em um estado novo.</span><span class="sxs-lookup"><span data-stu-id="89376-201">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="89376-202">Os valores válidos são 1-1440.</span><span class="sxs-lookup"><span data-stu-id="89376-202">Valid values are 1-1440.</span></span> <span data-ttu-id="89376-203">Valores válidos de 1 a 1440</span><span class="sxs-lookup"><span data-stu-id="89376-203">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="89376-204">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="89376-204">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="89376-205">String collection</span><span class="sxs-lookup"><span data-stu-id="89376-205">String collection</span></span>|<span data-ttu-id="89376-206">Especificar URLs às quais os navegadores quiosques não devem navegar</span><span class="sxs-lookup"><span data-stu-id="89376-206">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="89376-207">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="89376-207">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="89376-208">String collection</span><span class="sxs-lookup"><span data-stu-id="89376-208">String collection</span></span>|<span data-ttu-id="89376-209">Especificar URLs às quais o navegador de quiosque pode navegar</span><span class="sxs-lookup"><span data-stu-id="89376-209">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="89376-210">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="89376-210">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="89376-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="89376-211">Boolean</span></span>|<span data-ttu-id="89376-212">Habilitar modo quiosque de navegação pública para o navegador Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="89376-212">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="89376-213">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="89376-213">The Default is false.</span></span>|
|<span data-ttu-id="89376-214">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="89376-214">windowsKioskForceUpdateSchedule</span></span>|[<span data-ttu-id="89376-215">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="89376-215">windowsKioskForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windowskioskforceupdateschedule.md)|<span data-ttu-id="89376-216">forçar agendamento de atualização para dispositivos quiosque.</span><span class="sxs-lookup"><span data-stu-id="89376-216">force update schedule for Kiosk devices.</span></span>|



## <a name="response"></a><span data-ttu-id="89376-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="89376-217">Response</span></span>
<span data-ttu-id="89376-218">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89376-218">If successful, this method returns a `201 Created` response code and a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89376-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89376-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="89376-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89376-220">Request</span></span>
<span data-ttu-id="89376-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89376-221">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="89376-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="89376-222">Response</span></span>
<span data-ttu-id="89376-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89376-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





