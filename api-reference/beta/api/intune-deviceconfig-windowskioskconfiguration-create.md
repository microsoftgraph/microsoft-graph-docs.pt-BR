---
title: Criar windowsKioskConfiguration
description: Criar um novo objeto windowsKioskConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 237bf64f2ccb90304bb03f0e7ab9b7b5ed9197c0
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30572149"
---
# <a name="create-windowskioskconfiguration"></a><span data-ttu-id="a39f4-103">Criar windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="a39f4-103">Create windowsKioskConfiguration</span></span>

> <span data-ttu-id="a39f4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a39f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a39f4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a39f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a39f4-106">Criar um novo objeto [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a39f4-106">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a39f4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a39f4-107">Prerequisites</span></span>
<span data-ttu-id="a39f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a39f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a39f4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a39f4-110">Permission type</span></span>|<span data-ttu-id="a39f4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a39f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a39f4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a39f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a39f4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a39f4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a39f4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a39f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a39f4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a39f4-115">Not supported.</span></span>|
|<span data-ttu-id="a39f4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a39f4-116">Application</span></span>|<span data-ttu-id="a39f4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a39f4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a39f4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a39f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a39f4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a39f4-119">Request headers</span></span>
|<span data-ttu-id="a39f4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a39f4-120">Header</span></span>|<span data-ttu-id="a39f4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a39f4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a39f4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a39f4-122">Authorization</span></span>|<span data-ttu-id="a39f4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a39f4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a39f4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a39f4-124">Accept</span></span>|<span data-ttu-id="a39f4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a39f4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a39f4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a39f4-126">Request body</span></span>
<span data-ttu-id="a39f4-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsKioskConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a39f4-127">In the request body, supply a JSON representation for the windowsKioskConfiguration object.</span></span>

<span data-ttu-id="a39f4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsKioskConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a39f4-128">The following table shows the properties that are required when you create the windowsKioskConfiguration.</span></span>

|<span data-ttu-id="a39f4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a39f4-129">Property</span></span>|<span data-ttu-id="a39f4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a39f4-130">Type</span></span>|<span data-ttu-id="a39f4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a39f4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a39f4-132">id</span><span class="sxs-lookup"><span data-stu-id="a39f4-132">id</span></span>|<span data-ttu-id="a39f4-133">String</span><span class="sxs-lookup"><span data-stu-id="a39f4-133">String</span></span>|<span data-ttu-id="a39f4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a39f4-134">Key of the entity.</span></span> <span data-ttu-id="a39f4-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a39f4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a39f4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a39f4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a39f4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a39f4-137">DateTimeOffset</span></span>|<span data-ttu-id="a39f4-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a39f4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a39f4-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a39f4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a39f4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a39f4-140">roleScopeTagIds</span></span>|<span data-ttu-id="a39f4-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a39f4-141">String collection</span></span>|<span data-ttu-id="a39f4-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a39f4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a39f4-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a39f4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a39f4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a39f4-144">supportsScopeTags</span></span>|<span data-ttu-id="a39f4-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a39f4-145">Boolean</span></span>|<span data-ttu-id="a39f4-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a39f4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a39f4-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a39f4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a39f4-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a39f4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a39f4-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a39f4-149">This property is read-only.</span></span> <span data-ttu-id="a39f4-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a39f4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a39f4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a39f4-151">createdDateTime</span></span>|<span data-ttu-id="a39f4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a39f4-152">DateTimeOffset</span></span>|<span data-ttu-id="a39f4-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a39f4-153">DateTime the object was created.</span></span> <span data-ttu-id="a39f4-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a39f4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a39f4-155">descrição</span><span class="sxs-lookup"><span data-stu-id="a39f4-155">description</span></span>|<span data-ttu-id="a39f4-156">String</span><span class="sxs-lookup"><span data-stu-id="a39f4-156">String</span></span>|<span data-ttu-id="a39f4-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a39f4-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a39f4-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a39f4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a39f4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a39f4-159">displayName</span></span>|<span data-ttu-id="a39f4-160">String</span><span class="sxs-lookup"><span data-stu-id="a39f4-160">String</span></span>|<span data-ttu-id="a39f4-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a39f4-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a39f4-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a39f4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a39f4-163">versão</span><span class="sxs-lookup"><span data-stu-id="a39f4-163">version</span></span>|<span data-ttu-id="a39f4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a39f4-164">Int32</span></span>|<span data-ttu-id="a39f4-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a39f4-165">Version of the device configuration.</span></span> <span data-ttu-id="a39f4-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a39f4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a39f4-167">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="a39f4-167">kioskProfiles</span></span>|<span data-ttu-id="a39f4-168">coleção [windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a39f4-168">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="a39f4-169">Essa configuração de política permite definir uma lista de perfis de quiosque para uma configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="a39f4-169">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="a39f4-170">Essa coleção pode conter um máximo de 3 elementos.</span><span class="sxs-lookup"><span data-stu-id="a39f4-170">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="a39f4-171">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="a39f4-171">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="a39f4-172">String</span><span class="sxs-lookup"><span data-stu-id="a39f4-172">String</span></span>|<span data-ttu-id="a39f4-173">Especifique a URL padrão para a qual o navegador deve navegar na inicialização.</span><span class="sxs-lookup"><span data-stu-id="a39f4-173">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="a39f4-174">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="a39f4-174">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="a39f4-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="a39f4-175">Boolean</span></span>|<span data-ttu-id="a39f4-176">Habilite o botão Home do navegador quiosque.</span><span class="sxs-lookup"><span data-stu-id="a39f4-176">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="a39f4-177">Por padrão, o botão página inicial está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="a39f4-177">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="a39f4-178">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="a39f4-178">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="a39f4-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="a39f4-179">Boolean</span></span>|<span data-ttu-id="a39f4-180">Habilite os botões de navegação do navegador quiosque (avançar/voltar).</span><span class="sxs-lookup"><span data-stu-id="a39f4-180">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="a39f4-181">Por padrão, os botões de navegação estão desabilitados.</span><span class="sxs-lookup"><span data-stu-id="a39f4-181">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="a39f4-182">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="a39f4-182">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="a39f4-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="a39f4-183">Boolean</span></span>|<span data-ttu-id="a39f4-184">Habilite o botão encerrar sessão do navegador quiosque.</span><span class="sxs-lookup"><span data-stu-id="a39f4-184">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="a39f4-185">Por padrão, o botão encerrar sessão está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="a39f4-185">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="a39f4-186">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="a39f4-186">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="a39f4-187">Int32</span><span class="sxs-lookup"><span data-stu-id="a39f4-187">Int32</span></span>|<span data-ttu-id="a39f4-188">Especificar o número de minutos que a sessão ficará ociosa até que o navegador quiosque seja reiniciado em um estado novo.</span><span class="sxs-lookup"><span data-stu-id="a39f4-188">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="a39f4-189">Os valores válidos são 1-1440.</span><span class="sxs-lookup"><span data-stu-id="a39f4-189">Valid values are 1-1440.</span></span> <span data-ttu-id="a39f4-190">Valores válidos de 1 a 1440</span><span class="sxs-lookup"><span data-stu-id="a39f4-190">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="a39f4-191">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="a39f4-191">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="a39f4-192">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a39f4-192">String collection</span></span>|<span data-ttu-id="a39f4-193">Especificar URLs às quais os navegadores quiosques não devem navegar</span><span class="sxs-lookup"><span data-stu-id="a39f4-193">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="a39f4-194">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="a39f4-194">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="a39f4-195">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a39f4-195">String collection</span></span>|<span data-ttu-id="a39f4-196">Especificar URLs às quais o navegador de quiosque pode navegar</span><span class="sxs-lookup"><span data-stu-id="a39f4-196">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="a39f4-197">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="a39f4-197">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="a39f4-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="a39f4-198">Boolean</span></span>|<span data-ttu-id="a39f4-199">Habilitar modo quiosque de navegação pública para o navegador Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="a39f4-199">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="a39f4-200">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="a39f4-200">The Default is false.</span></span>|



## <a name="response"></a><span data-ttu-id="a39f4-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="a39f4-201">Response</span></span>
<span data-ttu-id="a39f4-202">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a39f4-202">If successful, this method returns a `201 Created` response code and a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a39f4-203">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a39f4-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="a39f4-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a39f4-204">Request</span></span>
<span data-ttu-id="a39f4-205">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a39f4-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1753

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "edgeKioskEnablePublicBrowsing": true
}
```

### <a name="response"></a><span data-ttu-id="a39f4-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="a39f4-206">Response</span></span>
<span data-ttu-id="a39f4-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a39f4-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1925

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "id": "146a990b-990b-146a-0b99-6a140b996a14",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "edgeKioskEnablePublicBrowsing": true
}
```




