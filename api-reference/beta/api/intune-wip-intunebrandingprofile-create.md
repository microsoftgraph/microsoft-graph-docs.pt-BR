---
title: Criar intuneBrandingProfile
description: Criar um novo objeto intuneBrandingProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2e2a293d4e111e8f6fd578a250ef095c4bd6509e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39938499"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="28da3-103">Criar intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="28da3-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="28da3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="28da3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28da3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28da3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28da3-106">Criar um novo objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="28da3-106">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28da3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="28da3-107">Prerequisites</span></span>
<span data-ttu-id="28da3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28da3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28da3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28da3-110">Permission type</span></span>|<span data-ttu-id="28da3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="28da3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28da3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28da3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28da3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28da3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="28da3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28da3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28da3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28da3-115">Not supported.</span></span>|
|<span data-ttu-id="28da3-116">Application</span><span class="sxs-lookup"><span data-stu-id="28da3-116">Application</span></span>|<span data-ttu-id="28da3-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28da3-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28da3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28da3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="28da3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28da3-119">Request headers</span></span>
|<span data-ttu-id="28da3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28da3-120">Header</span></span>|<span data-ttu-id="28da3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="28da3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28da3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="28da3-122">Authorization</span></span>|<span data-ttu-id="28da3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28da3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28da3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="28da3-124">Accept</span></span>|<span data-ttu-id="28da3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28da3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28da3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28da3-126">Request body</span></span>
<span data-ttu-id="28da3-127">No corpo da solicitação, forneça uma representação JSON do objeto intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="28da3-127">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="28da3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="28da3-128">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="28da3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28da3-129">Property</span></span>|<span data-ttu-id="28da3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="28da3-130">Type</span></span>|<span data-ttu-id="28da3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="28da3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28da3-132">id</span><span class="sxs-lookup"><span data-stu-id="28da3-132">id</span></span>|<span data-ttu-id="28da3-133">String</span><span class="sxs-lookup"><span data-stu-id="28da3-133">String</span></span>|<span data-ttu-id="28da3-134">Chave de perfil</span><span class="sxs-lookup"><span data-stu-id="28da3-134">Profile Key</span></span>|
|<span data-ttu-id="28da3-135">ProfileName</span><span class="sxs-lookup"><span data-stu-id="28da3-135">profileName</span></span>|<span data-ttu-id="28da3-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="28da3-136">String</span></span>|<span data-ttu-id="28da3-137">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="28da3-137">Name of the profile</span></span>|
|<span data-ttu-id="28da3-138">profileDescription</span><span class="sxs-lookup"><span data-stu-id="28da3-138">profileDescription</span></span>|<span data-ttu-id="28da3-139">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="28da3-139">String</span></span>|<span data-ttu-id="28da3-140">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="28da3-140">Description of the profile</span></span>|
|<span data-ttu-id="28da3-141">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="28da3-141">isDefaultProfile</span></span>|<span data-ttu-id="28da3-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="28da3-142">Boolean</span></span>|<span data-ttu-id="28da3-143">Booliano que indica se o perfil é usado como padrão ou não</span><span class="sxs-lookup"><span data-stu-id="28da3-143">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="28da3-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28da3-144">createdDateTime</span></span>|<span data-ttu-id="28da3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28da3-145">DateTimeOffset</span></span>|<span data-ttu-id="28da3-146">Hora em que o BrandingProfile foi criado</span><span class="sxs-lookup"><span data-stu-id="28da3-146">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="28da3-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28da3-147">lastModifiedDateTime</span></span>|<span data-ttu-id="28da3-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28da3-148">DateTimeOffset</span></span>|<span data-ttu-id="28da3-149">Hora em que a BrandingProfile foi modificada pela última vez</span><span class="sxs-lookup"><span data-stu-id="28da3-149">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="28da3-150">displayName</span><span class="sxs-lookup"><span data-stu-id="28da3-150">displayName</span></span>|<span data-ttu-id="28da3-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28da3-151">String</span></span>|<span data-ttu-id="28da3-152">Nome da empresa/organização que é exibido para os usuários finais</span><span class="sxs-lookup"><span data-stu-id="28da3-152">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="28da3-153">themeColor</span><span class="sxs-lookup"><span data-stu-id="28da3-153">themeColor</span></span>|[<span data-ttu-id="28da3-154">rgbColor</span><span class="sxs-lookup"><span data-stu-id="28da3-154">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="28da3-155">Cor do tema principal usada nos aplicativos do portal da empresa e no portal da Web</span><span class="sxs-lookup"><span data-stu-id="28da3-155">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="28da3-156">showLogo</span><span class="sxs-lookup"><span data-stu-id="28da3-156">showLogo</span></span>|<span data-ttu-id="28da3-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="28da3-157">Boolean</span></span>|<span data-ttu-id="28da3-158">Booliano que indica se as imagens de logotipo fornecidas pelo administrador são mostradas ou não</span><span class="sxs-lookup"><span data-stu-id="28da3-158">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="28da3-159">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="28da3-159">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="28da3-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="28da3-160">Boolean</span></span>|<span data-ttu-id="28da3-161">Booliano que indica se o nome de exibição fornecido pelo administrador será mostrado ao lado da imagem de logotipo ou não</span><span class="sxs-lookup"><span data-stu-id="28da3-161">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="28da3-162">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="28da3-162">themeColorLogo</span></span>|[<span data-ttu-id="28da3-163">mimeContent</span><span class="sxs-lookup"><span data-stu-id="28da3-163">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="28da3-164">Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo de cor de tema atrás do logotipo</span><span class="sxs-lookup"><span data-stu-id="28da3-164">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="28da3-165">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="28da3-165">lightBackgroundLogo</span></span>|[<span data-ttu-id="28da3-166">mimeContent</span><span class="sxs-lookup"><span data-stu-id="28da3-166">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="28da3-167">Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo claro atrás do logotipo</span><span class="sxs-lookup"><span data-stu-id="28da3-167">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="28da3-168">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="28da3-168">landingPageCustomizedImage</span></span>|[<span data-ttu-id="28da3-169">mimeContent</span><span class="sxs-lookup"><span data-stu-id="28da3-169">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="28da3-170">Imagem personalizada exibida na página inicial dos aplicativos do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="28da3-170">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="28da3-171">contactITName</span><span class="sxs-lookup"><span data-stu-id="28da3-171">contactITName</span></span>|<span data-ttu-id="28da3-172">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="28da3-172">String</span></span>|<span data-ttu-id="28da3-173">Nome da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="28da3-173">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="28da3-174">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="28da3-174">contactITPhoneNumber</span></span>|<span data-ttu-id="28da3-175">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="28da3-175">String</span></span>|<span data-ttu-id="28da3-176">Número de telefone da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="28da3-176">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="28da3-177">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="28da3-177">contactITEmailAddress</span></span>|<span data-ttu-id="28da3-178">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="28da3-178">String</span></span>|<span data-ttu-id="28da3-179">Endereço de email da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="28da3-179">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="28da3-180">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="28da3-180">contactITNotes</span></span>|<span data-ttu-id="28da3-181">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="28da3-181">String</span></span>|<span data-ttu-id="28da3-182">Comentários de texto sobre a pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="28da3-182">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="28da3-183">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="28da3-183">onlineSupportSiteUrl</span></span>|<span data-ttu-id="28da3-184">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="28da3-184">String</span></span>|<span data-ttu-id="28da3-185">URL para o site de assistência técnica de ti da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="28da3-185">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="28da3-186">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="28da3-186">onlineSupportSiteName</span></span>|<span data-ttu-id="28da3-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28da3-187">String</span></span>|<span data-ttu-id="28da3-188">Nome para exibição do site de assistência técnica de ti da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="28da3-188">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="28da3-189">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="28da3-189">privacyUrl</span></span>|<span data-ttu-id="28da3-190">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="28da3-190">String</span></span>|<span data-ttu-id="28da3-191">URL para a política de privacidade da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="28da3-191">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="28da3-192">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="28da3-192">customPrivacyMessage</span></span>|<span data-ttu-id="28da3-193">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="28da3-193">String</span></span>|<span data-ttu-id="28da3-194">Comentários de texto sobre o que o administrador tem acesso ao no dispositivo</span><span class="sxs-lookup"><span data-stu-id="28da3-194">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="28da3-195">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="28da3-195">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="28da3-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="28da3-196">Boolean</span></span>|<span data-ttu-id="28da3-197">Booliano que indica se o adminsistrator desabilitou a ação "remover dispositivo" em dispositivos corporativos de propriedade.</span><span class="sxs-lookup"><span data-stu-id="28da3-197">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="28da3-198">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="28da3-198">isFactoryResetDisabled</span></span>|<span data-ttu-id="28da3-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="28da3-199">Boolean</span></span>|<span data-ttu-id="28da3-200">Booliano que indica se o adminsistrator desabilitou a ação "redefinição de fábrica" em dispositivos corporativos de propriedade.</span><span class="sxs-lookup"><span data-stu-id="28da3-200">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="28da3-201">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="28da3-201">companyPortalBlockedActions</span></span>|<span data-ttu-id="28da3-202">coleção [companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="28da3-202">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="28da3-203">Conjunto de ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo.</span><span class="sxs-lookup"><span data-stu-id="28da3-203">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="28da3-204">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="28da3-204">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="28da3-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="28da3-205">Boolean</span></span>|<span data-ttu-id="28da3-206">Booliano que indica se os aplicativos empresariais do AzureAD serão mostrados no portal da empresa</span><span class="sxs-lookup"><span data-stu-id="28da3-206">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="28da3-207">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="28da3-207">showOfficeWebApps</span></span>|<span data-ttu-id="28da3-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="28da3-208">Boolean</span></span>|<span data-ttu-id="28da3-209">Booliano que indica se o Office webapps será mostrado no portal da empresa</span><span class="sxs-lookup"><span data-stu-id="28da3-209">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|



## <a name="response"></a><span data-ttu-id="28da3-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="28da3-210">Response</span></span>
<span data-ttu-id="28da3-211">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28da3-211">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28da3-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28da3-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="28da3-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28da3-213">Request</span></span>
<span data-ttu-id="28da3-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28da3-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1620

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "displayName": "Display Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "customPrivacyMessage": "Custom Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "androidForWork",
      "ownerType": "company",
      "action": "remove"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true
}
```

### <a name="response"></a><span data-ttu-id="28da3-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="28da3-215">Response</span></span>
<span data-ttu-id="28da3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28da3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1792

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "customPrivacyMessage": "Custom Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "androidForWork",
      "ownerType": "company",
      "action": "remove"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true
}
```





