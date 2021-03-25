---
title: Criar iosDeviceFeaturesConfiguration
description: Criar um novo objeto iosDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1a0ecef5d4d7f4dcad9d8f467b6ff14bc9bbd8da
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155285"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="edac1-103">Criar iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="edac1-103">Create iosDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="edac1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edac1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="edac1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="edac1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edac1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="edac1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edac1-107">Criar um novo objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edac1-107">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="edac1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="edac1-108">Prerequisites</span></span>
<span data-ttu-id="edac1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edac1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edac1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="edac1-111">Permission type</span></span>|<span data-ttu-id="edac1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="edac1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edac1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="edac1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="edac1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edac1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="edac1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="edac1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edac1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="edac1-116">Not supported.</span></span>|
|<span data-ttu-id="edac1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="edac1-117">Application</span></span>|<span data-ttu-id="edac1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edac1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="edac1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="edac1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="edac1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="edac1-120">Request headers</span></span>
|<span data-ttu-id="edac1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="edac1-121">Header</span></span>|<span data-ttu-id="edac1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="edac1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edac1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="edac1-123">Authorization</span></span>|<span data-ttu-id="edac1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="edac1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edac1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="edac1-125">Accept</span></span>|<span data-ttu-id="edac1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="edac1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edac1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="edac1-127">Request body</span></span>
<span data-ttu-id="edac1-128">No corpo da solicitação, forneça uma representação JSON do objeto iosDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="edac1-128">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="edac1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="edac1-129">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="edac1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="edac1-130">Property</span></span>|<span data-ttu-id="edac1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="edac1-131">Type</span></span>|<span data-ttu-id="edac1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="edac1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edac1-133">id</span><span class="sxs-lookup"><span data-stu-id="edac1-133">id</span></span>|<span data-ttu-id="edac1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edac1-134">String</span></span>|<span data-ttu-id="edac1-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="edac1-135">Key of the entity.</span></span> <span data-ttu-id="edac1-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edac1-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="edac1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="edac1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edac1-138">DateTimeOffset</span></span>|<span data-ttu-id="edac1-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="edac1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="edac1-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edac1-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="edac1-141">roleScopeTagIds</span></span>|<span data-ttu-id="edac1-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="edac1-142">String collection</span></span>|<span data-ttu-id="edac1-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="edac1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="edac1-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edac1-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="edac1-145">supportsScopeTags</span></span>|<span data-ttu-id="edac1-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="edac1-146">Boolean</span></span>|<span data-ttu-id="edac1-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="edac1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="edac1-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="edac1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="edac1-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="edac1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="edac1-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="edac1-150">This property is read-only.</span></span> <span data-ttu-id="edac1-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edac1-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="edac1-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="edac1-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="edac1-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="edac1-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="edac1-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="edac1-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edac1-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="edac1-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="edac1-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="edac1-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="edac1-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="edac1-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="edac1-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edac1-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="edac1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="edac1-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="edac1-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="edac1-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="edac1-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="edac1-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edac1-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac1-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="edac1-164">createdDateTime</span></span>|<span data-ttu-id="edac1-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edac1-165">DateTimeOffset</span></span>|<span data-ttu-id="edac1-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="edac1-166">DateTime the object was created.</span></span> <span data-ttu-id="edac1-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edac1-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac1-168">descrição</span><span class="sxs-lookup"><span data-stu-id="edac1-168">description</span></span>|<span data-ttu-id="edac1-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edac1-169">String</span></span>|<span data-ttu-id="edac1-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="edac1-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="edac1-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edac1-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac1-172">displayName</span><span class="sxs-lookup"><span data-stu-id="edac1-172">displayName</span></span>|<span data-ttu-id="edac1-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edac1-173">String</span></span>|<span data-ttu-id="edac1-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="edac1-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="edac1-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edac1-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac1-176">versão</span><span class="sxs-lookup"><span data-stu-id="edac1-176">version</span></span>|<span data-ttu-id="edac1-177">Int32</span><span class="sxs-lookup"><span data-stu-id="edac1-177">Int32</span></span>|<span data-ttu-id="edac1-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="edac1-178">Version of the device configuration.</span></span> <span data-ttu-id="edac1-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edac1-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac1-180">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="edac1-180">airPrintDestinations</span></span>|<span data-ttu-id="edac1-181">[Coleção airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="edac1-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="edac1-182">Uma matriz de impressoras AirPrint que sempre devem ser mostradas.</span><span class="sxs-lookup"><span data-stu-id="edac1-182">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="edac1-183">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="edac1-183">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="edac1-184">Herdado [do appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="edac1-184">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="edac1-185">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="edac1-185">assetTagTemplate</span></span>|<span data-ttu-id="edac1-186">String</span><span class="sxs-lookup"><span data-stu-id="edac1-186">String</span></span>|<span data-ttu-id="edac1-187">Informações de marcação de ativos para o dispositivo, exibidas na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="edac1-187">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="edac1-188">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="edac1-188">contentFilterSettings</span></span>|[<span data-ttu-id="edac1-189">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="edac1-189">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="edac1-190">Obtém ou define configurações do Filtro de Conteúdo da Web do iOS, somente modo supervisionado</span><span class="sxs-lookup"><span data-stu-id="edac1-190">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="edac1-191">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="edac1-191">lockScreenFootnote</span></span>|<span data-ttu-id="edac1-192">String</span><span class="sxs-lookup"><span data-stu-id="edac1-192">String</span></span>|<span data-ttu-id="edac1-193">Uma nota de rodapé exibida na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="edac1-193">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="edac1-194">Disponível no iOS 9.3.1 e posterior.</span><span class="sxs-lookup"><span data-stu-id="edac1-194">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="edac1-195">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="edac1-195">homeScreenDockIcons</span></span>|<span data-ttu-id="edac1-196">Coleção [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="edac1-196">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="edac1-197">Uma lista dos aplicativos e pastas exibidos em um dock de tela inicial.</span><span class="sxs-lookup"><span data-stu-id="edac1-197">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="edac1-198">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="edac1-198">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="edac1-199">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="edac1-199">homeScreenPages</span></span>|<span data-ttu-id="edac1-200">Coleção [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="edac1-200">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="edac1-201">Uma lista de páginas na tela inicial.</span><span class="sxs-lookup"><span data-stu-id="edac1-201">A list of pages on the Home Screen.</span></span> <span data-ttu-id="edac1-202">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="edac1-202">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="edac1-203">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="edac1-203">notificationSettings</span></span>|<span data-ttu-id="edac1-204">Coleção [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="edac1-204">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="edac1-205">Configurações de notificação para cada ID de pacote. Aplicáveis apenas a dispositivos no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="edac1-205">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="edac1-206">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="edac1-206">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="edac1-207">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="edac1-207">singleSignOnSettings</span></span>|[<span data-ttu-id="edac1-208">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="edac1-208">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="edac1-209">As configurações de logon Kerberos que permitem que aplicativos em dispositivos de recebimento autentuem suavemente.</span><span class="sxs-lookup"><span data-stu-id="edac1-209">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="edac1-210">wallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="edac1-210">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="edac1-211">iosWallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="edac1-211">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="edac1-212">Um especificador de local de exibição de papel de parede.</span><span class="sxs-lookup"><span data-stu-id="edac1-212">A wallpaper display location specifier.</span></span> <span data-ttu-id="edac1-213">Os valores possíveis são: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span><span class="sxs-lookup"><span data-stu-id="edac1-213">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="edac1-214">wallpaperImage</span><span class="sxs-lookup"><span data-stu-id="edac1-214">wallpaperImage</span></span>|[<span data-ttu-id="edac1-215">mimeContent</span><span class="sxs-lookup"><span data-stu-id="edac1-215">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="edac1-216">Uma imagem de papel de parede deve estar no formato PNG ou JPEG.</span><span class="sxs-lookup"><span data-stu-id="edac1-216">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="edac1-217">Ele requer um dispositivo supervisionado com a versão iOS 8 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="edac1-217">It requires a supervised device with iOS 8 or later version.</span></span>|
|<span data-ttu-id="edac1-218">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="edac1-218">singleSignOnExtension</span></span>|[<span data-ttu-id="edac1-219">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="edac1-219">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="edac1-220">Obtém ou define um único perfil de extensão de entrada.</span><span class="sxs-lookup"><span data-stu-id="edac1-220">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="edac1-221">Preterido: use IOSSingleSignOnExtension.</span><span class="sxs-lookup"><span data-stu-id="edac1-221">Deprecated: use IOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="edac1-222">iosSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="edac1-222">iosSingleSignOnExtension</span></span>|[<span data-ttu-id="edac1-223">iosSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="edac1-223">iosSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-iossinglesignonextension.md)|<span data-ttu-id="edac1-224">Obtém ou define um único perfil de extensão de entrada.</span><span class="sxs-lookup"><span data-stu-id="edac1-224">Gets or sets a single sign-on extension profile.</span></span>|



## <a name="response"></a><span data-ttu-id="edac1-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="edac1-225">Response</span></span>
<span data-ttu-id="edac1-226">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="edac1-226">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edac1-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="edac1-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="edac1-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="edac1-228">Request</span></span>
<span data-ttu-id="edac1-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="edac1-229">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 6830

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
              "bundleID": "Bundle ID value",
              "isWebClip": true
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
                  "bundleID": "Bundle ID value",
                  "isWebClip": true
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
      "soundsEnabled": true,
      "previewVisibility": "alwaysShow"
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
  },
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  },
  "iosSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  }
}
```

### <a name="response"></a><span data-ttu-id="edac1-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="edac1-230">Response</span></span>
<span data-ttu-id="edac1-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="edac1-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7002

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
              "bundleID": "Bundle ID value",
              "isWebClip": true
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
                  "bundleID": "Bundle ID value",
                  "isWebClip": true
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
      "soundsEnabled": true,
      "previewVisibility": "alwaysShow"
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
  },
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  },
  "iosSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  }
}
```




