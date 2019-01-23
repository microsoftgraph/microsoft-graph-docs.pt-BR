---
title: Criar iosDeviceFeaturesConfiguration
description: Criar um novo objeto iosDeviceFeaturesConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6f6a5fe84c5ecd4f95168c027a344237a55961b3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423192"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="03e83-103">Criar iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="03e83-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="03e83-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="03e83-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="03e83-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="03e83-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03e83-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="03e83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03e83-107">Criar um novo objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03e83-107">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03e83-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="03e83-108">Prerequisites</span></span>
<span data-ttu-id="03e83-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="03e83-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="03e83-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03e83-111">Permission type</span></span>|<span data-ttu-id="03e83-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="03e83-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03e83-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03e83-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03e83-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03e83-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03e83-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03e83-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03e83-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03e83-116">Not supported.</span></span>|
|<span data-ttu-id="03e83-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03e83-117">Application</span></span>|<span data-ttu-id="03e83-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03e83-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03e83-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03e83-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="03e83-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03e83-120">Request headers</span></span>
|<span data-ttu-id="03e83-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03e83-121">Header</span></span>|<span data-ttu-id="03e83-122">Valor</span><span class="sxs-lookup"><span data-stu-id="03e83-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03e83-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="03e83-123">Authorization</span></span>|<span data-ttu-id="03e83-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03e83-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03e83-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="03e83-125">Accept</span></span>|<span data-ttu-id="03e83-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03e83-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03e83-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03e83-127">Request body</span></span>
<span data-ttu-id="03e83-128">No corpo da solicitação, forneça uma representação JSON do objeto iosDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="03e83-128">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="03e83-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="03e83-129">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="03e83-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03e83-130">Property</span></span>|<span data-ttu-id="03e83-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="03e83-131">Type</span></span>|<span data-ttu-id="03e83-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="03e83-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03e83-133">id</span><span class="sxs-lookup"><span data-stu-id="03e83-133">id</span></span>|<span data-ttu-id="03e83-134">String</span><span class="sxs-lookup"><span data-stu-id="03e83-134">String</span></span>|<span data-ttu-id="03e83-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="03e83-135">Key of the entity.</span></span> <span data-ttu-id="03e83-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e83-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e83-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03e83-137">lastModifiedDateTime</span></span>|<span data-ttu-id="03e83-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03e83-138">DateTimeOffset</span></span>|<span data-ttu-id="03e83-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="03e83-139">DateTime the object was last modified.</span></span> <span data-ttu-id="03e83-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e83-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e83-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="03e83-141">roleScopeTagIds</span></span>|<span data-ttu-id="03e83-142">String collection</span><span class="sxs-lookup"><span data-stu-id="03e83-142">String collection</span></span>|<span data-ttu-id="03e83-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="03e83-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="03e83-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e83-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e83-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="03e83-145">supportsScopeTags</span></span>|<span data-ttu-id="03e83-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="03e83-146">Boolean</span></span>|<span data-ttu-id="03e83-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="03e83-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="03e83-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="03e83-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="03e83-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="03e83-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="03e83-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03e83-150">This property is read-only.</span></span> <span data-ttu-id="03e83-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e83-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e83-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03e83-152">createdDateTime</span></span>|<span data-ttu-id="03e83-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03e83-153">DateTimeOffset</span></span>|<span data-ttu-id="03e83-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="03e83-154">DateTime the object was created.</span></span> <span data-ttu-id="03e83-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e83-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e83-156">description</span><span class="sxs-lookup"><span data-stu-id="03e83-156">description</span></span>|<span data-ttu-id="03e83-157">String</span><span class="sxs-lookup"><span data-stu-id="03e83-157">String</span></span>|<span data-ttu-id="03e83-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03e83-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="03e83-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e83-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e83-160">displayName</span><span class="sxs-lookup"><span data-stu-id="03e83-160">displayName</span></span>|<span data-ttu-id="03e83-161">String</span><span class="sxs-lookup"><span data-stu-id="03e83-161">String</span></span>|<span data-ttu-id="03e83-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03e83-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="03e83-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e83-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e83-164">version</span><span class="sxs-lookup"><span data-stu-id="03e83-164">version</span></span>|<span data-ttu-id="03e83-165">Int32</span><span class="sxs-lookup"><span data-stu-id="03e83-165">Int32</span></span>|<span data-ttu-id="03e83-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03e83-166">Version of the device configuration.</span></span> <span data-ttu-id="03e83-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e83-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e83-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="03e83-168">airPrintDestinations</span></span>|<span data-ttu-id="03e83-169">coleção [airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="03e83-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="03e83-170">Uma matriz de impressoras AirPrint que sempre devem ser exibidos.</span><span class="sxs-lookup"><span data-stu-id="03e83-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="03e83-171">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="03e83-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="03e83-172">Herdado de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="03e83-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="03e83-173">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="03e83-173">assetTagTemplate</span></span>|<span data-ttu-id="03e83-174">String</span><span class="sxs-lookup"><span data-stu-id="03e83-174">String</span></span>|<span data-ttu-id="03e83-175">Informações de marcação de ativos para o dispositivo, exibidas na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="03e83-175">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="03e83-176">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="03e83-176">contentFilterSettings</span></span>|[<span data-ttu-id="03e83-177">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="03e83-177">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="03e83-178">Obtém ou define o iOS configurações de filtro de conteúdo da Web, somente no modo supervisionada</span><span class="sxs-lookup"><span data-stu-id="03e83-178">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="03e83-179">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="03e83-179">lockScreenFootnote</span></span>|<span data-ttu-id="03e83-180">String</span><span class="sxs-lookup"><span data-stu-id="03e83-180">String</span></span>|<span data-ttu-id="03e83-181">Uma nota de rodapé exibida na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="03e83-181">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="03e83-182">Disponível no iOS 9.3.1 e posterior.</span><span class="sxs-lookup"><span data-stu-id="03e83-182">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="03e83-183">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="03e83-183">homeScreenDockIcons</span></span>|<span data-ttu-id="03e83-184">Coleção [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="03e83-184">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="03e83-185">Uma lista dos aplicativos e pastas exibidos em um dock de tela inicial.</span><span class="sxs-lookup"><span data-stu-id="03e83-185">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="03e83-186">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="03e83-186">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="03e83-187">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="03e83-187">homeScreenPages</span></span>|<span data-ttu-id="03e83-188">Coleção [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="03e83-188">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="03e83-189">Uma lista de páginas na tela inicial.</span><span class="sxs-lookup"><span data-stu-id="03e83-189">A list of pages on the Home Screen.</span></span> <span data-ttu-id="03e83-190">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="03e83-190">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="03e83-191">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="03e83-191">notificationSettings</span></span>|<span data-ttu-id="03e83-192">Coleção [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="03e83-192">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="03e83-193">Configurações de notificação para cada ID de pacote. Aplicáveis apenas a dispositivos no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="03e83-193">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="03e83-194">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="03e83-194">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="03e83-195">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="03e83-195">singleSignOnSettings</span></span>|[<span data-ttu-id="03e83-196">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="03e83-196">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="03e83-197">As configurações de login do Kerberos que permitem que aplicativos no recebimento de dispositivos para autenticar suavemente.</span><span class="sxs-lookup"><span data-stu-id="03e83-197">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="03e83-198">wallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="03e83-198">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="03e83-199">iosWallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="03e83-199">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="03e83-200">Um especificador de local de exibição de parede.</span><span class="sxs-lookup"><span data-stu-id="03e83-200">A wallpaper display location specifier.</span></span> <span data-ttu-id="03e83-201">Os valores possíveis são: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span><span class="sxs-lookup"><span data-stu-id="03e83-201">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="03e83-202">wallpaperImage</span><span class="sxs-lookup"><span data-stu-id="03e83-202">wallpaperImage</span></span>|[<span data-ttu-id="03e83-203">mimeContent</span><span class="sxs-lookup"><span data-stu-id="03e83-203">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="03e83-204">Uma imagem de papel de parede deve estar no formato PNG ou JPEG.</span><span class="sxs-lookup"><span data-stu-id="03e83-204">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="03e83-205">Ele requer um dispositivo supervisionado com iOS 8 ou versão posterior.</span><span class="sxs-lookup"><span data-stu-id="03e83-205">It requires a supervised device with iOS 8 or later version.</span></span>|



## <a name="response"></a><span data-ttu-id="03e83-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="03e83-206">Response</span></span>
<span data-ttu-id="03e83-207">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03e83-207">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03e83-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03e83-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="03e83-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03e83-209">Request</span></span>
<span data-ttu-id="03e83-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03e83-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3656

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="03e83-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="03e83-211">Response</span></span>
<span data-ttu-id="03e83-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03e83-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3828

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




