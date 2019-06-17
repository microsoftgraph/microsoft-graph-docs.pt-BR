---
title: Atualizar iosDeviceFeaturesConfiguration
description: Atualizar as propriedades de um objeto iosDeviceFeaturesConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ecc28e52e8e359332d104cd6de8f6aad4223edc8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34967059"
---
# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="b2293-103">Atualizar iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="b2293-103">Update iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="b2293-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2293-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2293-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2293-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2293-106">Atualizar as propriedades de um objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2293-106">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2293-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2293-107">Prerequisites</span></span>
<span data-ttu-id="b2293-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2293-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2293-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2293-110">Permission type</span></span>|<span data-ttu-id="b2293-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2293-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2293-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2293-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2293-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2293-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2293-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2293-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2293-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2293-115">Not supported.</span></span>|
|<span data-ttu-id="b2293-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2293-116">Application</span></span>|<span data-ttu-id="b2293-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2293-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2293-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2293-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b2293-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2293-119">Request headers</span></span>
|<span data-ttu-id="b2293-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2293-120">Header</span></span>|<span data-ttu-id="b2293-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b2293-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2293-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2293-122">Authorization</span></span>|<span data-ttu-id="b2293-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2293-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2293-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2293-124">Accept</span></span>|<span data-ttu-id="b2293-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2293-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2293-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2293-126">Request body</span></span>
<span data-ttu-id="b2293-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2293-127">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="b2293-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2293-128">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="b2293-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2293-129">Property</span></span>|<span data-ttu-id="b2293-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2293-130">Type</span></span>|<span data-ttu-id="b2293-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2293-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2293-132">id</span><span class="sxs-lookup"><span data-stu-id="b2293-132">id</span></span>|<span data-ttu-id="b2293-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2293-133">String</span></span>|<span data-ttu-id="b2293-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b2293-134">Key of the entity.</span></span> <span data-ttu-id="b2293-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2293-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2293-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2293-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b2293-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2293-137">DateTimeOffset</span></span>|<span data-ttu-id="b2293-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b2293-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b2293-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2293-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2293-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b2293-140">roleScopeTagIds</span></span>|<span data-ttu-id="b2293-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2293-141">String collection</span></span>|<span data-ttu-id="b2293-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b2293-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b2293-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2293-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2293-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b2293-144">supportsScopeTags</span></span>|<span data-ttu-id="b2293-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2293-145">Boolean</span></span>|<span data-ttu-id="b2293-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b2293-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b2293-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b2293-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b2293-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b2293-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b2293-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2293-149">This property is read-only.</span></span> <span data-ttu-id="b2293-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2293-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2293-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b2293-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b2293-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b2293-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b2293-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="b2293-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b2293-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2293-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2293-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b2293-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b2293-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b2293-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b2293-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="b2293-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b2293-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2293-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2293-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b2293-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b2293-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b2293-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b2293-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="b2293-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b2293-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2293-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2293-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2293-163">createdDateTime</span></span>|<span data-ttu-id="b2293-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2293-164">DateTimeOffset</span></span>|<span data-ttu-id="b2293-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b2293-165">DateTime the object was created.</span></span> <span data-ttu-id="b2293-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2293-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2293-167">descrição</span><span class="sxs-lookup"><span data-stu-id="b2293-167">description</span></span>|<span data-ttu-id="b2293-168">String</span><span class="sxs-lookup"><span data-stu-id="b2293-168">String</span></span>|<span data-ttu-id="b2293-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2293-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b2293-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2293-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2293-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b2293-171">displayName</span></span>|<span data-ttu-id="b2293-172">String</span><span class="sxs-lookup"><span data-stu-id="b2293-172">String</span></span>|<span data-ttu-id="b2293-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2293-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b2293-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2293-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2293-175">versão</span><span class="sxs-lookup"><span data-stu-id="b2293-175">version</span></span>|<span data-ttu-id="b2293-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b2293-176">Int32</span></span>|<span data-ttu-id="b2293-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2293-177">Version of the device configuration.</span></span> <span data-ttu-id="b2293-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2293-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2293-179">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="b2293-179">airPrintDestinations</span></span>|<span data-ttu-id="b2293-180">coleção [airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="b2293-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="b2293-181">Uma matriz de impressoras de impressão que sempre devem ser mostradas.</span><span class="sxs-lookup"><span data-stu-id="b2293-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="b2293-182">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b2293-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b2293-183">Herdado de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="b2293-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="b2293-184">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="b2293-184">assetTagTemplate</span></span>|<span data-ttu-id="b2293-185">String</span><span class="sxs-lookup"><span data-stu-id="b2293-185">String</span></span>|<span data-ttu-id="b2293-186">Informações de marcação de ativos para o dispositivo, exibidas na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="b2293-186">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="b2293-187">Contentfiltersettings à</span><span class="sxs-lookup"><span data-stu-id="b2293-187">contentFilterSettings</span></span>|[<span data-ttu-id="b2293-188">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="b2293-188">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="b2293-189">Obtém ou define as configurações de filtro de conteúdo da Web iOS, modo supervisionado somente</span><span class="sxs-lookup"><span data-stu-id="b2293-189">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="b2293-190">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="b2293-190">lockScreenFootnote</span></span>|<span data-ttu-id="b2293-191">String</span><span class="sxs-lookup"><span data-stu-id="b2293-191">String</span></span>|<span data-ttu-id="b2293-192">Uma nota de rodapé exibida na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="b2293-192">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="b2293-193">Disponível no iOS 9.3.1 e posterior.</span><span class="sxs-lookup"><span data-stu-id="b2293-193">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="b2293-194">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="b2293-194">homeScreenDockIcons</span></span>|<span data-ttu-id="b2293-195">Coleção [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="b2293-195">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="b2293-196">Uma lista dos aplicativos e pastas exibidos em um dock de tela inicial.</span><span class="sxs-lookup"><span data-stu-id="b2293-196">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="b2293-197">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b2293-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b2293-198">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="b2293-198">homeScreenPages</span></span>|<span data-ttu-id="b2293-199">Coleção [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="b2293-199">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="b2293-200">Uma lista de páginas na tela inicial.</span><span class="sxs-lookup"><span data-stu-id="b2293-200">A list of pages on the Home Screen.</span></span> <span data-ttu-id="b2293-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b2293-201">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b2293-202">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="b2293-202">notificationSettings</span></span>|<span data-ttu-id="b2293-203">Coleção [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="b2293-203">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="b2293-204">Configurações de notificação para cada ID de pacote. Aplicáveis apenas a dispositivos no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="b2293-204">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="b2293-205">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b2293-205">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b2293-206">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="b2293-206">singleSignOnSettings</span></span>|[<span data-ttu-id="b2293-207">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="b2293-207">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="b2293-208">As configurações de logon Kerberos que permitem que os aplicativos de recebimento de dispositivos sejam autenticados sem problemas.</span><span class="sxs-lookup"><span data-stu-id="b2293-208">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="b2293-209">wallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="b2293-209">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="b2293-210">iosWallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="b2293-210">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="b2293-211">Um especificador de local de exibição de papel de parede.</span><span class="sxs-lookup"><span data-stu-id="b2293-211">A wallpaper display location specifier.</span></span> <span data-ttu-id="b2293-212">Os valores possíveis são: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span><span class="sxs-lookup"><span data-stu-id="b2293-212">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="b2293-213">wallpaperImage</span><span class="sxs-lookup"><span data-stu-id="b2293-213">wallpaperImage</span></span>|[<span data-ttu-id="b2293-214">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b2293-214">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b2293-215">Uma imagem de papel de parede deve estar no formato PNG ou JPEG.</span><span class="sxs-lookup"><span data-stu-id="b2293-215">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="b2293-216">Requer um dispositivo supervisionado com o iOS 8 ou versão posterior.</span><span class="sxs-lookup"><span data-stu-id="b2293-216">It requires a supervised device with iOS 8 or later version.</span></span>|



## <a name="response"></a><span data-ttu-id="b2293-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2293-217">Response</span></span>
<span data-ttu-id="b2293-218">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2293-218">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2293-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2293-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2293-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2293-220">Request</span></span>
<span data-ttu-id="b2293-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2293-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4429

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "assetTagTemplate": "Asset Tag Template value",
  "contentFilterSettings": {
    "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
    "specificWebsitesOnly": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ],
    "websiteList": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ]
  },
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ],
  "singleSignOnSettings": {
    "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
    "allowedAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "allowedUrls": [
      "Allowed Urls value"
    ],
    "displayName": "Display Name value",
    "kerberosPrincipalName": "Kerberos Principal Name value",
    "kerberosRealm": "Kerberos Realm value"
  },
  "wallpaperDisplayLocation": "lockScreen",
  "wallpaperImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="b2293-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2293-222">Response</span></span>
<span data-ttu-id="b2293-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2293-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4601

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "assetTagTemplate": "Asset Tag Template value",
  "contentFilterSettings": {
    "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
    "specificWebsitesOnly": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ],
    "websiteList": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ]
  },
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ],
  "singleSignOnSettings": {
    "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
    "allowedAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "allowedUrls": [
      "Allowed Urls value"
    ],
    "displayName": "Display Name value",
    "kerberosPrincipalName": "Kerberos Principal Name value",
    "kerberosRealm": "Kerberos Realm value"
  },
  "wallpaperDisplayLocation": "lockScreen",
  "wallpaperImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```





