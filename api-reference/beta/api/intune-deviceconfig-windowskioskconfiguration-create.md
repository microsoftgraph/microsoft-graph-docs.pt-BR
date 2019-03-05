---
title: Criar windowsKioskConfiguration
description: Criar um novo objeto windowsKioskConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd32b23626c027cfc4a9cdac60b5a5a4a6c37973
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160743"
---
# <a name="create-windowskioskconfiguration"></a><span data-ttu-id="aac6f-103">Criar windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="aac6f-103">Create windowsKioskConfiguration</span></span>

> <span data-ttu-id="aac6f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aac6f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aac6f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aac6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aac6f-106">Criar um novo objeto [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="aac6f-106">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aac6f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aac6f-107">Prerequisites</span></span>
<span data-ttu-id="aac6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="aac6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aac6f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aac6f-110">Permission type</span></span>|<span data-ttu-id="aac6f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aac6f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aac6f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aac6f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aac6f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac6f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aac6f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aac6f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aac6f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aac6f-115">Not supported.</span></span>|
|<span data-ttu-id="aac6f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aac6f-116">Application</span></span>|<span data-ttu-id="aac6f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aac6f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aac6f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aac6f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="aac6f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aac6f-119">Request headers</span></span>
|<span data-ttu-id="aac6f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aac6f-120">Header</span></span>|<span data-ttu-id="aac6f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="aac6f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aac6f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="aac6f-122">Authorization</span></span>|<span data-ttu-id="aac6f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aac6f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aac6f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aac6f-124">Accept</span></span>|<span data-ttu-id="aac6f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aac6f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aac6f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aac6f-126">Request body</span></span>
<span data-ttu-id="aac6f-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsKioskConfiguration.</span><span class="sxs-lookup"><span data-stu-id="aac6f-127">In the request body, supply a JSON representation for the windowsKioskConfiguration object.</span></span>

<span data-ttu-id="aac6f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsKioskConfiguration.</span><span class="sxs-lookup"><span data-stu-id="aac6f-128">The following table shows the properties that are required when you create the windowsKioskConfiguration.</span></span>

|<span data-ttu-id="aac6f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aac6f-129">Property</span></span>|<span data-ttu-id="aac6f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="aac6f-130">Type</span></span>|<span data-ttu-id="aac6f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="aac6f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aac6f-132">id</span><span class="sxs-lookup"><span data-stu-id="aac6f-132">id</span></span>|<span data-ttu-id="aac6f-133">String</span><span class="sxs-lookup"><span data-stu-id="aac6f-133">String</span></span>|<span data-ttu-id="aac6f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aac6f-134">Key of the entity.</span></span> <span data-ttu-id="aac6f-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aac6f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aac6f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aac6f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="aac6f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aac6f-137">DateTimeOffset</span></span>|<span data-ttu-id="aac6f-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="aac6f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="aac6f-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aac6f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aac6f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aac6f-140">roleScopeTagIds</span></span>|<span data-ttu-id="aac6f-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aac6f-141">String collection</span></span>|<span data-ttu-id="aac6f-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="aac6f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aac6f-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aac6f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aac6f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="aac6f-144">supportsScopeTags</span></span>|<span data-ttu-id="aac6f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="aac6f-145">Boolean</span></span>|<span data-ttu-id="aac6f-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="aac6f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aac6f-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="aac6f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aac6f-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="aac6f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aac6f-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aac6f-149">This property is read-only.</span></span> <span data-ttu-id="aac6f-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aac6f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aac6f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aac6f-151">createdDateTime</span></span>|<span data-ttu-id="aac6f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aac6f-152">DateTimeOffset</span></span>|<span data-ttu-id="aac6f-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="aac6f-153">DateTime the object was created.</span></span> <span data-ttu-id="aac6f-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aac6f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aac6f-155">description</span><span class="sxs-lookup"><span data-stu-id="aac6f-155">description</span></span>|<span data-ttu-id="aac6f-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aac6f-156">String</span></span>|<span data-ttu-id="aac6f-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aac6f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aac6f-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aac6f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aac6f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="aac6f-159">displayName</span></span>|<span data-ttu-id="aac6f-160">String</span><span class="sxs-lookup"><span data-stu-id="aac6f-160">String</span></span>|<span data-ttu-id="aac6f-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aac6f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aac6f-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aac6f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aac6f-163">version</span><span class="sxs-lookup"><span data-stu-id="aac6f-163">version</span></span>|<span data-ttu-id="aac6f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="aac6f-164">Int32</span></span>|<span data-ttu-id="aac6f-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aac6f-165">Version of the device configuration.</span></span> <span data-ttu-id="aac6f-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aac6f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aac6f-167">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="aac6f-167">kioskProfiles</span></span>|<span data-ttu-id="aac6f-168">coleção [windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)</span><span class="sxs-lookup"><span data-stu-id="aac6f-168">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="aac6f-169">Essa configuração de política permite definir uma lista de perfis de quiosque para uma configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="aac6f-169">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="aac6f-170">Essa coleção pode conter um máximo de 3 elementos.</span><span class="sxs-lookup"><span data-stu-id="aac6f-170">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="aac6f-171">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="aac6f-171">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="aac6f-172">String</span><span class="sxs-lookup"><span data-stu-id="aac6f-172">String</span></span>|<span data-ttu-id="aac6f-173">Especifique a URL padrão para a qual o navegador deve navegar na inicialização.</span><span class="sxs-lookup"><span data-stu-id="aac6f-173">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="aac6f-174">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="aac6f-174">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="aac6f-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="aac6f-175">Boolean</span></span>|<span data-ttu-id="aac6f-176">Habilite o botão Home do navegador quiosque.</span><span class="sxs-lookup"><span data-stu-id="aac6f-176">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="aac6f-177">Por padrão, o botão página inicial está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="aac6f-177">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="aac6f-178">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="aac6f-178">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="aac6f-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="aac6f-179">Boolean</span></span>|<span data-ttu-id="aac6f-180">Habilite os botões de navegação do navegador quiosque (avançar/voltar).</span><span class="sxs-lookup"><span data-stu-id="aac6f-180">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="aac6f-181">Por padrão, os botões de navegação estão desabilitados.</span><span class="sxs-lookup"><span data-stu-id="aac6f-181">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="aac6f-182">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="aac6f-182">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="aac6f-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="aac6f-183">Boolean</span></span>|<span data-ttu-id="aac6f-184">Habilite o botão encerrar sessão do navegador quiosque.</span><span class="sxs-lookup"><span data-stu-id="aac6f-184">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="aac6f-185">Por padrão, o botão encerrar sessão está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="aac6f-185">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="aac6f-186">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="aac6f-186">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="aac6f-187">Int32</span><span class="sxs-lookup"><span data-stu-id="aac6f-187">Int32</span></span>|<span data-ttu-id="aac6f-188">Especificar o número de minutos que a sessão ficará ociosa até que o navegador quiosque seja reiniciado em um estado novo.</span><span class="sxs-lookup"><span data-stu-id="aac6f-188">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="aac6f-189">Os valores válidos são 1-1440.</span><span class="sxs-lookup"><span data-stu-id="aac6f-189">Valid values are 1-1440.</span></span> <span data-ttu-id="aac6f-190">Valores válidos de 1 a 1440</span><span class="sxs-lookup"><span data-stu-id="aac6f-190">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="aac6f-191">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="aac6f-191">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="aac6f-192">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aac6f-192">String collection</span></span>|<span data-ttu-id="aac6f-193">Especificar URLs às quais os navegadores quiosques não devem navegar</span><span class="sxs-lookup"><span data-stu-id="aac6f-193">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="aac6f-194">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="aac6f-194">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="aac6f-195">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aac6f-195">String collection</span></span>|<span data-ttu-id="aac6f-196">Especificar URLs às quais o navegador de quiosque pode navegar</span><span class="sxs-lookup"><span data-stu-id="aac6f-196">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="aac6f-197">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="aac6f-197">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="aac6f-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="aac6f-198">Boolean</span></span>|<span data-ttu-id="aac6f-199">Habilitar modo quiosque de navegação pública para o navegador Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="aac6f-199">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="aac6f-200">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="aac6f-200">The Default is false.</span></span>|
|<span data-ttu-id="aac6f-201">edgeKioskResetAfterIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="aac6f-201">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="aac6f-202">Int32</span><span class="sxs-lookup"><span data-stu-id="aac6f-202">Int32</span></span>|<span data-ttu-id="aac6f-203">Especifica o tempo, em minutos, da última atividade do usuário antes que o Microsoft Edge quiosque seja redefinido.</span><span class="sxs-lookup"><span data-stu-id="aac6f-203">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="aac6f-204">Os valores válidos são 0-1440.</span><span class="sxs-lookup"><span data-stu-id="aac6f-204">Valid values are 0-1440.</span></span> <span data-ttu-id="aac6f-205">O padrão é 5.</span><span class="sxs-lookup"><span data-stu-id="aac6f-205">The default is 5.</span></span> <span data-ttu-id="aac6f-206">0 indica nenhuma redefinição.</span><span class="sxs-lookup"><span data-stu-id="aac6f-206">0 indicates no reset.</span></span> <span data-ttu-id="aac6f-207">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="aac6f-207">Valid values 0 to 1440</span></span>|



## <a name="response"></a><span data-ttu-id="aac6f-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="aac6f-208">Response</span></span>
<span data-ttu-id="aac6f-209">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aac6f-209">If successful, this method returns a `201 Created` response code and a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aac6f-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aac6f-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="aac6f-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aac6f-211">Request</span></span>
<span data-ttu-id="aac6f-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aac6f-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1719

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
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
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
  "edgeKioskResetAfterIdleTimeInMinutes": 4
}
```

### <a name="response"></a><span data-ttu-id="aac6f-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="aac6f-213">Response</span></span>
<span data-ttu-id="aac6f-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aac6f-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1891

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
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
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
  "edgeKioskResetAfterIdleTimeInMinutes": 4
}
```




