---
title: Criar intuneBrandingProfile
description: Criar um novo objeto intuneBrandingProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 98245e618ef6c821502109164e2c726657477b91
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350178"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="99f5e-103">Criar intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="99f5e-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="99f5e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99f5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99f5e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99f5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99f5e-106">Criar um novo objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="99f5e-106">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99f5e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99f5e-107">Prerequisites</span></span>
<span data-ttu-id="99f5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99f5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99f5e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99f5e-110">Permission type</span></span>|<span data-ttu-id="99f5e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="99f5e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99f5e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99f5e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="99f5e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99f5e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="99f5e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99f5e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99f5e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99f5e-115">Not supported.</span></span>|
|<span data-ttu-id="99f5e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99f5e-116">Application</span></span>|<span data-ttu-id="99f5e-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99f5e-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99f5e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99f5e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="99f5e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99f5e-119">Request headers</span></span>
|<span data-ttu-id="99f5e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99f5e-120">Header</span></span>|<span data-ttu-id="99f5e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="99f5e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99f5e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="99f5e-122">Authorization</span></span>|<span data-ttu-id="99f5e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99f5e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99f5e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="99f5e-124">Accept</span></span>|<span data-ttu-id="99f5e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="99f5e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99f5e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99f5e-126">Request body</span></span>
<span data-ttu-id="99f5e-127">No corpo da solicitação, forneça uma representação JSON do objeto intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="99f5e-127">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="99f5e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="99f5e-128">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="99f5e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99f5e-129">Property</span></span>|<span data-ttu-id="99f5e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="99f5e-130">Type</span></span>|<span data-ttu-id="99f5e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="99f5e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99f5e-132">id</span><span class="sxs-lookup"><span data-stu-id="99f5e-132">id</span></span>|<span data-ttu-id="99f5e-133">String</span><span class="sxs-lookup"><span data-stu-id="99f5e-133">String</span></span>|<span data-ttu-id="99f5e-134">Chave de perfil</span><span class="sxs-lookup"><span data-stu-id="99f5e-134">Profile Key</span></span>|
|<span data-ttu-id="99f5e-135">ProfileName</span><span class="sxs-lookup"><span data-stu-id="99f5e-135">profileName</span></span>|<span data-ttu-id="99f5e-136">String</span><span class="sxs-lookup"><span data-stu-id="99f5e-136">String</span></span>|<span data-ttu-id="99f5e-137">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="99f5e-137">Name of the profile</span></span>|
|<span data-ttu-id="99f5e-138">profileDescription</span><span class="sxs-lookup"><span data-stu-id="99f5e-138">profileDescription</span></span>|<span data-ttu-id="99f5e-139">String</span><span class="sxs-lookup"><span data-stu-id="99f5e-139">String</span></span>|<span data-ttu-id="99f5e-140">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="99f5e-140">Description of the profile</span></span>|
|<span data-ttu-id="99f5e-141">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="99f5e-141">isDefaultProfile</span></span>|<span data-ttu-id="99f5e-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="99f5e-142">Boolean</span></span>|<span data-ttu-id="99f5e-143">Booliano que indica se o perfil é usado como padrão ou não</span><span class="sxs-lookup"><span data-stu-id="99f5e-143">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="99f5e-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99f5e-144">createdDateTime</span></span>|<span data-ttu-id="99f5e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99f5e-145">DateTimeOffset</span></span>|<span data-ttu-id="99f5e-146">Hora em que o BrandingProfile foi criado</span><span class="sxs-lookup"><span data-stu-id="99f5e-146">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="99f5e-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99f5e-147">lastModifiedDateTime</span></span>|<span data-ttu-id="99f5e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99f5e-148">DateTimeOffset</span></span>|<span data-ttu-id="99f5e-149">Hora em que a BrandingProfile foi modificada pela última vez</span><span class="sxs-lookup"><span data-stu-id="99f5e-149">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="99f5e-150">displayName</span><span class="sxs-lookup"><span data-stu-id="99f5e-150">displayName</span></span>|<span data-ttu-id="99f5e-151">String</span><span class="sxs-lookup"><span data-stu-id="99f5e-151">String</span></span>|<span data-ttu-id="99f5e-152">Nome da empresa/organização que é exibido para os usuários finais</span><span class="sxs-lookup"><span data-stu-id="99f5e-152">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="99f5e-153">contactITName</span><span class="sxs-lookup"><span data-stu-id="99f5e-153">contactITName</span></span>|<span data-ttu-id="99f5e-154">String</span><span class="sxs-lookup"><span data-stu-id="99f5e-154">String</span></span>|<span data-ttu-id="99f5e-155">Nome da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="99f5e-155">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="99f5e-156">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="99f5e-156">contactITPhoneNumber</span></span>|<span data-ttu-id="99f5e-157">String</span><span class="sxs-lookup"><span data-stu-id="99f5e-157">String</span></span>|<span data-ttu-id="99f5e-158">Número de telefone da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="99f5e-158">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="99f5e-159">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="99f5e-159">contactITEmailAddress</span></span>|<span data-ttu-id="99f5e-160">String</span><span class="sxs-lookup"><span data-stu-id="99f5e-160">String</span></span>|<span data-ttu-id="99f5e-161">Endereço de email da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="99f5e-161">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="99f5e-162">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="99f5e-162">contactITNotes</span></span>|<span data-ttu-id="99f5e-163">String</span><span class="sxs-lookup"><span data-stu-id="99f5e-163">String</span></span>|<span data-ttu-id="99f5e-164">Comentários de texto sobre a pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="99f5e-164">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="99f5e-165">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="99f5e-165">privacyUrl</span></span>|<span data-ttu-id="99f5e-166">String</span><span class="sxs-lookup"><span data-stu-id="99f5e-166">String</span></span>|<span data-ttu-id="99f5e-167">URL para a política de privacidade da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="99f5e-167">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="99f5e-168">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="99f5e-168">onlineSupportSiteUrl</span></span>|<span data-ttu-id="99f5e-169">String</span><span class="sxs-lookup"><span data-stu-id="99f5e-169">String</span></span>|<span data-ttu-id="99f5e-170">URL para o site de assistência técnica de ti da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="99f5e-170">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="99f5e-171">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="99f5e-171">onlineSupportSiteName</span></span>|<span data-ttu-id="99f5e-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99f5e-172">String</span></span>|<span data-ttu-id="99f5e-173">Nome para exibição do site de assistência técnica de ti da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="99f5e-173">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="99f5e-174">themeColor</span><span class="sxs-lookup"><span data-stu-id="99f5e-174">themeColor</span></span>|[<span data-ttu-id="99f5e-175">rgbColor</span><span class="sxs-lookup"><span data-stu-id="99f5e-175">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="99f5e-176">Cor do tema principal usada nos aplicativos do portal da empresa e no portal da Web</span><span class="sxs-lookup"><span data-stu-id="99f5e-176">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="99f5e-177">showLogo</span><span class="sxs-lookup"><span data-stu-id="99f5e-177">showLogo</span></span>|<span data-ttu-id="99f5e-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="99f5e-178">Boolean</span></span>|<span data-ttu-id="99f5e-179">Booliano que indica se as imagens de logotipo fornecidas pelo administrador são mostradas ou não</span><span class="sxs-lookup"><span data-stu-id="99f5e-179">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="99f5e-180">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="99f5e-180">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="99f5e-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="99f5e-181">Boolean</span></span>|<span data-ttu-id="99f5e-182">Booliano que indica se o nome de exibição fornecido pelo administrador será mostrado ao lado da imagem de logotipo ou não</span><span class="sxs-lookup"><span data-stu-id="99f5e-182">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="99f5e-183">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="99f5e-183">themeColorLogo</span></span>|[<span data-ttu-id="99f5e-184">mimeContent</span><span class="sxs-lookup"><span data-stu-id="99f5e-184">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="99f5e-185">Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo de cor de tema atrás do logotipo</span><span class="sxs-lookup"><span data-stu-id="99f5e-185">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="99f5e-186">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="99f5e-186">lightBackgroundLogo</span></span>|[<span data-ttu-id="99f5e-187">mimeContent</span><span class="sxs-lookup"><span data-stu-id="99f5e-187">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="99f5e-188">Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo claro atrás do logotipo</span><span class="sxs-lookup"><span data-stu-id="99f5e-188">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="99f5e-189">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="99f5e-189">landingPageCustomizedImage</span></span>|[<span data-ttu-id="99f5e-190">mimeContent</span><span class="sxs-lookup"><span data-stu-id="99f5e-190">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="99f5e-191">Imagem personalizada exibida na página inicial dos aplicativos do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="99f5e-191">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="99f5e-192">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="99f5e-192">customPrivacyMessage</span></span>|<span data-ttu-id="99f5e-193">String</span><span class="sxs-lookup"><span data-stu-id="99f5e-193">String</span></span>|<span data-ttu-id="99f5e-194">Comentários de texto sobre o que o administrador tem acesso ao no dispositivo</span><span class="sxs-lookup"><span data-stu-id="99f5e-194">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="99f5e-195">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="99f5e-195">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="99f5e-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="99f5e-196">Boolean</span></span>|<span data-ttu-id="99f5e-197">Booliano que indica se o adminsistrator desabilitou a ação "remover dispositivo" em dispositivos corporativos de propriedade.</span><span class="sxs-lookup"><span data-stu-id="99f5e-197">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="99f5e-198">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="99f5e-198">isFactoryResetDisabled</span></span>|<span data-ttu-id="99f5e-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="99f5e-199">Boolean</span></span>|<span data-ttu-id="99f5e-200">Booliano que indica se o adminsistrator desabilitou a ação "redefinição de fábrica" em dispositivos corporativos de propriedade.</span><span class="sxs-lookup"><span data-stu-id="99f5e-200">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|



## <a name="response"></a><span data-ttu-id="99f5e-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="99f5e-201">Response</span></span>
<span data-ttu-id="99f5e-202">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99f5e-202">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99f5e-203">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99f5e-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="99f5e-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99f5e-204">Request</span></span>
<span data-ttu-id="99f5e-205">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99f5e-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1334

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
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
  "customPrivacyMessage": "Custom Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="99f5e-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="99f5e-206">Response</span></span>
<span data-ttu-id="99f5e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99f5e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1506

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
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
  "customPrivacyMessage": "Custom Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true
}
```






