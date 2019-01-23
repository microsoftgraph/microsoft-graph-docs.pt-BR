---
title: Atualizar windowsKioskConfiguration
description: Atualize as propriedades de um objeto windowsKioskConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 767acd4136226e2687977cf09d2c08f6c413fcb8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414883"
---
# <a name="update-windowskioskconfiguration"></a><span data-ttu-id="f4567-103">Atualizar windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4567-103">Update windowsKioskConfiguration</span></span>

> <span data-ttu-id="f4567-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f4567-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f4567-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f4567-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4567-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f4567-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4567-107">Atualize as propriedades de um objeto [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f4567-107">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4567-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4567-108">Prerequisites</span></span>
<span data-ttu-id="f4567-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f4567-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f4567-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4567-111">Permission type</span></span>|<span data-ttu-id="f4567-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f4567-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4567-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4567-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4567-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4567-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4567-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4567-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4567-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4567-116">Not supported.</span></span>|
|<span data-ttu-id="f4567-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4567-117">Application</span></span>|<span data-ttu-id="f4567-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4567-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4567-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4567-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f4567-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4567-120">Request headers</span></span>
|<span data-ttu-id="f4567-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4567-121">Header</span></span>|<span data-ttu-id="f4567-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f4567-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4567-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4567-123">Authorization</span></span>|<span data-ttu-id="f4567-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4567-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4567-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4567-125">Accept</span></span>|<span data-ttu-id="f4567-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4567-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4567-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4567-127">Request body</span></span>
<span data-ttu-id="f4567-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f4567-128">In the request body, supply a JSON representation for the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

<span data-ttu-id="f4567-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4567-129">The following table shows the properties that are required when you create the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>

|<span data-ttu-id="f4567-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4567-130">Property</span></span>|<span data-ttu-id="f4567-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4567-131">Type</span></span>|<span data-ttu-id="f4567-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4567-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4567-133">id</span><span class="sxs-lookup"><span data-stu-id="f4567-133">id</span></span>|<span data-ttu-id="f4567-134">String</span><span class="sxs-lookup"><span data-stu-id="f4567-134">String</span></span>|<span data-ttu-id="f4567-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f4567-135">Key of the entity.</span></span> <span data-ttu-id="f4567-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4567-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4567-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4567-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f4567-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4567-138">DateTimeOffset</span></span>|<span data-ttu-id="f4567-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f4567-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f4567-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4567-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4567-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4567-141">roleScopeTagIds</span></span>|<span data-ttu-id="f4567-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f4567-142">String collection</span></span>|<span data-ttu-id="f4567-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="f4567-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f4567-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4567-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4567-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f4567-145">supportsScopeTags</span></span>|<span data-ttu-id="f4567-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4567-146">Boolean</span></span>|<span data-ttu-id="f4567-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f4567-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f4567-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f4567-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f4567-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="f4567-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f4567-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4567-150">This property is read-only.</span></span> <span data-ttu-id="f4567-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4567-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4567-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4567-152">createdDateTime</span></span>|<span data-ttu-id="f4567-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4567-153">DateTimeOffset</span></span>|<span data-ttu-id="f4567-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f4567-154">DateTime the object was created.</span></span> <span data-ttu-id="f4567-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4567-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4567-156">description</span><span class="sxs-lookup"><span data-stu-id="f4567-156">description</span></span>|<span data-ttu-id="f4567-157">String</span><span class="sxs-lookup"><span data-stu-id="f4567-157">String</span></span>|<span data-ttu-id="f4567-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4567-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f4567-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4567-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4567-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f4567-160">displayName</span></span>|<span data-ttu-id="f4567-161">String</span><span class="sxs-lookup"><span data-stu-id="f4567-161">String</span></span>|<span data-ttu-id="f4567-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4567-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f4567-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4567-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4567-164">version</span><span class="sxs-lookup"><span data-stu-id="f4567-164">version</span></span>|<span data-ttu-id="f4567-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f4567-165">Int32</span></span>|<span data-ttu-id="f4567-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4567-166">Version of the device configuration.</span></span> <span data-ttu-id="f4567-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4567-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4567-168">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="f4567-168">kioskProfiles</span></span>|<span data-ttu-id="f4567-169">coleção [windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4567-169">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="f4567-170">Essa configuração de política permite definir uma lista de perfis de quiosque de uma configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="f4567-170">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="f4567-171">Essa coleção pode conter um máximo de 3 elementos.</span><span class="sxs-lookup"><span data-stu-id="f4567-171">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="f4567-172">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="f4567-172">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="f4567-173">String</span><span class="sxs-lookup"><span data-stu-id="f4567-173">String</span></span>|<span data-ttu-id="f4567-174">Especifique a URL de padrão deve navegar o navegador no lançamento.</span><span class="sxs-lookup"><span data-stu-id="f4567-174">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="f4567-175">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="f4567-175">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="f4567-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4567-176">Boolean</span></span>|<span data-ttu-id="f4567-177">Habilite o botão de página inicial do navegador quiosque.</span><span class="sxs-lookup"><span data-stu-id="f4567-177">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="f4567-178">Por padrão, o botão página inicial está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="f4567-178">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="f4567-179">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="f4567-179">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="f4567-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4567-180">Boolean</span></span>|<span data-ttu-id="f4567-181">Habilite buttons(forward/back) de navegação do navegador quiosque.</span><span class="sxs-lookup"><span data-stu-id="f4567-181">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="f4567-182">Por padrão, os botões de navegação são desabilitados.</span><span class="sxs-lookup"><span data-stu-id="f4567-182">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="f4567-183">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="f4567-183">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="f4567-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4567-184">Boolean</span></span>|<span data-ttu-id="f4567-185">Habilite o botão de sessão do navegador quiosque encerrar.</span><span class="sxs-lookup"><span data-stu-id="f4567-185">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="f4567-186">Por padrão, o botão de sessão encerrar está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="f4567-186">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="f4567-187">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="f4567-187">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="f4567-188">Int32</span><span class="sxs-lookup"><span data-stu-id="f4567-188">Int32</span></span>|<span data-ttu-id="f4567-189">Especifique o número de minutos que a sessão está ociosa até que o navegador de quiosque reinicia em um estado atualizado.</span><span class="sxs-lookup"><span data-stu-id="f4567-189">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="f4567-190">Valores válidos são 1-1440.</span><span class="sxs-lookup"><span data-stu-id="f4567-190">Valid values are 1-1440.</span></span> <span data-ttu-id="f4567-191">Valores válidos 1 a 1440</span><span class="sxs-lookup"><span data-stu-id="f4567-191">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="f4567-192">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="f4567-192">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="f4567-193">String collection</span><span class="sxs-lookup"><span data-stu-id="f4567-193">String collection</span></span>|<span data-ttu-id="f4567-194">Especifique as URLs que os navegadores de quiosque não devem navegar</span><span class="sxs-lookup"><span data-stu-id="f4567-194">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="f4567-195">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="f4567-195">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="f4567-196">String collection</span><span class="sxs-lookup"><span data-stu-id="f4567-196">String collection</span></span>|<span data-ttu-id="f4567-197">Especifique as URLs que o navegador de quiosque é permitido para navegar até</span><span class="sxs-lookup"><span data-stu-id="f4567-197">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="f4567-198">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="f4567-198">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="f4567-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4567-199">Boolean</span></span>|<span data-ttu-id="f4567-200">Habilite o modo de quiosque navegação pública para o navegador do Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="f4567-200">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="f4567-201">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="f4567-201">The Default is false.</span></span>|
|<span data-ttu-id="f4567-202">edgeKioskResetAfterIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="f4567-202">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="f4567-203">Int32</span><span class="sxs-lookup"><span data-stu-id="f4567-203">Int32</span></span>|<span data-ttu-id="f4567-204">Especifica o tempo em minutos a partir da última atividade do usuário antes de quiosque Microsoft Edge redefine.</span><span class="sxs-lookup"><span data-stu-id="f4567-204">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="f4567-205">Valores válidos são 0-1440.</span><span class="sxs-lookup"><span data-stu-id="f4567-205">Valid values are 0-1440.</span></span> <span data-ttu-id="f4567-206">O padrão é 5.</span><span class="sxs-lookup"><span data-stu-id="f4567-206">The default is 5.</span></span> <span data-ttu-id="f4567-207">0 não indica que nenhuma reset.</span><span class="sxs-lookup"><span data-stu-id="f4567-207">0 indicates no reset.</span></span> <span data-ttu-id="f4567-208">Valores válidos 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="f4567-208">Valid values 0 to 1440</span></span>|



## <a name="response"></a><span data-ttu-id="f4567-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4567-209">Response</span></span>
<span data-ttu-id="f4567-210">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4567-210">If successful, this method returns a `200 OK` response code and an updated [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4567-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4567-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4567-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4567-212">Request</span></span>
<span data-ttu-id="f4567-213">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4567-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="f4567-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4567-214">Response</span></span>
<span data-ttu-id="f4567-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4567-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




