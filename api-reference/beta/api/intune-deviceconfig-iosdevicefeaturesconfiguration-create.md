---
title: Criar iosDeviceFeaturesConfiguration
description: Criar um novo objeto iosDeviceFeaturesConfiguration.
author: tfitzmac
ms.openlocfilehash: dcb9819505cf429f6217dc375fcbd0c3366dee89
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310882"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="35d1c-103">Criar iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="35d1c-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="35d1c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="35d1c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35d1c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="35d1c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35d1c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="35d1c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35d1c-107">Criar um novo objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35d1c-107">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35d1c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="35d1c-108">Prerequisites</span></span>
<span data-ttu-id="35d1c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35d1c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35d1c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35d1c-111">Permission type</span></span>|<span data-ttu-id="35d1c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="35d1c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35d1c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35d1c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35d1c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35d1c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="35d1c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35d1c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35d1c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35d1c-116">Not supported.</span></span>|
|<span data-ttu-id="35d1c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35d1c-117">Application</span></span>|<span data-ttu-id="35d1c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35d1c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35d1c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35d1c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="35d1c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35d1c-120">Request headers</span></span>
|<span data-ttu-id="35d1c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="35d1c-121">Header</span></span>|<span data-ttu-id="35d1c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="35d1c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35d1c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="35d1c-123">Authorization</span></span>|<span data-ttu-id="35d1c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35d1c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35d1c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="35d1c-125">Accept</span></span>|<span data-ttu-id="35d1c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35d1c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35d1c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35d1c-127">Request body</span></span>
<span data-ttu-id="35d1c-128">No corpo da solicitação, forneça uma representação JSON do objeto iosDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="35d1c-128">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="35d1c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="35d1c-129">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="35d1c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35d1c-130">Property</span></span>|<span data-ttu-id="35d1c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="35d1c-131">Type</span></span>|<span data-ttu-id="35d1c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="35d1c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35d1c-133">id</span><span class="sxs-lookup"><span data-stu-id="35d1c-133">id</span></span>|<span data-ttu-id="35d1c-134">String</span><span class="sxs-lookup"><span data-stu-id="35d1c-134">String</span></span>|<span data-ttu-id="35d1c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="35d1c-135">Key of the entity.</span></span> <span data-ttu-id="35d1c-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35d1c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35d1c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35d1c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="35d1c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35d1c-138">DateTimeOffset</span></span>|<span data-ttu-id="35d1c-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="35d1c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="35d1c-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35d1c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35d1c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="35d1c-141">roleScopeTagIds</span></span>|<span data-ttu-id="35d1c-142">String collection</span><span class="sxs-lookup"><span data-stu-id="35d1c-142">String collection</span></span>|<span data-ttu-id="35d1c-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="35d1c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="35d1c-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35d1c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35d1c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="35d1c-145">supportsScopeTags</span></span>|<span data-ttu-id="35d1c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="35d1c-146">Boolean</span></span>|<span data-ttu-id="35d1c-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="35d1c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="35d1c-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="35d1c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="35d1c-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="35d1c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="35d1c-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35d1c-150">This property is read-only.</span></span> <span data-ttu-id="35d1c-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35d1c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35d1c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35d1c-152">createdDateTime</span></span>|<span data-ttu-id="35d1c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35d1c-153">DateTimeOffset</span></span>|<span data-ttu-id="35d1c-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="35d1c-154">DateTime the object was created.</span></span> <span data-ttu-id="35d1c-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35d1c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35d1c-156">description</span><span class="sxs-lookup"><span data-stu-id="35d1c-156">description</span></span>|<span data-ttu-id="35d1c-157">String</span><span class="sxs-lookup"><span data-stu-id="35d1c-157">String</span></span>|<span data-ttu-id="35d1c-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35d1c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="35d1c-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35d1c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35d1c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="35d1c-160">displayName</span></span>|<span data-ttu-id="35d1c-161">String</span><span class="sxs-lookup"><span data-stu-id="35d1c-161">String</span></span>|<span data-ttu-id="35d1c-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35d1c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="35d1c-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35d1c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35d1c-164">version</span><span class="sxs-lookup"><span data-stu-id="35d1c-164">version</span></span>|<span data-ttu-id="35d1c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="35d1c-165">Int32</span></span>|<span data-ttu-id="35d1c-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35d1c-166">Version of the device configuration.</span></span> <span data-ttu-id="35d1c-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35d1c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35d1c-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="35d1c-168">airPrintDestinations</span></span>|<span data-ttu-id="35d1c-169">coleção [airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="35d1c-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="35d1c-170">Uma matriz de impressoras AirPrint que sempre devem ser exibidos.</span><span class="sxs-lookup"><span data-stu-id="35d1c-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="35d1c-171">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="35d1c-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="35d1c-172">Herdado de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="35d1c-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="35d1c-173">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="35d1c-173">assetTagTemplate</span></span>|<span data-ttu-id="35d1c-174">String</span><span class="sxs-lookup"><span data-stu-id="35d1c-174">String</span></span>|<span data-ttu-id="35d1c-175">Informações de marcação de ativos para o dispositivo, exibidas na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="35d1c-175">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="35d1c-176">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="35d1c-176">contentFilterSettings</span></span>|[<span data-ttu-id="35d1c-177">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="35d1c-177">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="35d1c-178">Obtém ou define o iOS configurações de filtro de conteúdo da Web, somente no modo supervisionada</span><span class="sxs-lookup"><span data-stu-id="35d1c-178">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="35d1c-179">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="35d1c-179">lockScreenFootnote</span></span>|<span data-ttu-id="35d1c-180">String</span><span class="sxs-lookup"><span data-stu-id="35d1c-180">String</span></span>|<span data-ttu-id="35d1c-181">Uma nota de rodapé exibida na janela de login e na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="35d1c-181">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="35d1c-182">Disponível no iOS 9.3.1 e posterior.</span><span class="sxs-lookup"><span data-stu-id="35d1c-182">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="35d1c-183">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="35d1c-183">homeScreenDockIcons</span></span>|<span data-ttu-id="35d1c-184">Coleção [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="35d1c-184">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="35d1c-185">Uma lista dos aplicativos e pastas exibidos em um dock de tela inicial.</span><span class="sxs-lookup"><span data-stu-id="35d1c-185">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="35d1c-186">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="35d1c-186">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="35d1c-187">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="35d1c-187">homeScreenPages</span></span>|<span data-ttu-id="35d1c-188">Coleção [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="35d1c-188">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="35d1c-189">Uma lista de páginas na tela inicial.</span><span class="sxs-lookup"><span data-stu-id="35d1c-189">A list of pages on the Home Screen.</span></span> <span data-ttu-id="35d1c-190">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="35d1c-190">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="35d1c-191">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="35d1c-191">notificationSettings</span></span>|<span data-ttu-id="35d1c-192">Coleção [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="35d1c-192">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="35d1c-193">Configurações de notificação para cada ID de pacote. Aplicáveis apenas a dispositivos no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="35d1c-193">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="35d1c-194">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="35d1c-194">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="35d1c-195">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="35d1c-195">singleSignOnSettings</span></span>|[<span data-ttu-id="35d1c-196">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="35d1c-196">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="35d1c-197">As configurações de login do Kerberos que permitem que aplicativos no recebimento de dispositivos para autenticar suavemente.</span><span class="sxs-lookup"><span data-stu-id="35d1c-197">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|



## <a name="response"></a><span data-ttu-id="35d1c-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="35d1c-198">Response</span></span>
<span data-ttu-id="35d1c-199">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35d1c-199">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35d1c-200">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35d1c-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="35d1c-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35d1c-201">Request</span></span>
<span data-ttu-id="35d1c-202">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35d1c-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3543

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="35d1c-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="35d1c-203">Response</span></span>
<span data-ttu-id="35d1c-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35d1c-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3651

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
  }
}
```





