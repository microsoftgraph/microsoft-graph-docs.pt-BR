---
title: Criar intuneBrandingProfile
description: Criar um novo objeto intuneBrandingProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec5e863d171c952c07acfb0ecf2c312dcd89a366
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990663"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="0a6cf-103">Criar intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="0a6cf-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="0a6cf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0a6cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a6cf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a6cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a6cf-106">Criar um novo objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0a6cf-106">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a6cf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0a6cf-107">Prerequisites</span></span>
<span data-ttu-id="0a6cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a6cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a6cf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a6cf-110">Permission type</span></span>|<span data-ttu-id="0a6cf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0a6cf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a6cf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a6cf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a6cf-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a6cf-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0a6cf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a6cf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a6cf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a6cf-115">Not supported.</span></span>|
|<span data-ttu-id="0a6cf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a6cf-116">Application</span></span>|<span data-ttu-id="0a6cf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a6cf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a6cf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a6cf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="0a6cf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a6cf-119">Request headers</span></span>
|<span data-ttu-id="0a6cf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a6cf-120">Header</span></span>|<span data-ttu-id="0a6cf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0a6cf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a6cf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a6cf-122">Authorization</span></span>|<span data-ttu-id="0a6cf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a6cf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a6cf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0a6cf-124">Accept</span></span>|<span data-ttu-id="0a6cf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a6cf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a6cf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a6cf-126">Request body</span></span>
<span data-ttu-id="0a6cf-127">No corpo da solicitação, forneça uma representação JSON do objeto intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="0a6cf-127">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="0a6cf-128">A tabela a seguir mostra as propriedades que são necessárias ao criar intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="0a6cf-128">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="0a6cf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a6cf-129">Property</span></span>|<span data-ttu-id="0a6cf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a6cf-130">Type</span></span>|<span data-ttu-id="0a6cf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a6cf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a6cf-132">id</span><span class="sxs-lookup"><span data-stu-id="0a6cf-132">id</span></span>|<span data-ttu-id="0a6cf-133">String</span><span class="sxs-lookup"><span data-stu-id="0a6cf-133">String</span></span>|<span data-ttu-id="0a6cf-134">Chave de perfil</span><span class="sxs-lookup"><span data-stu-id="0a6cf-134">Profile Key</span></span>|
|<span data-ttu-id="0a6cf-135">ProfileName</span><span class="sxs-lookup"><span data-stu-id="0a6cf-135">profileName</span></span>|<span data-ttu-id="0a6cf-136">String</span><span class="sxs-lookup"><span data-stu-id="0a6cf-136">String</span></span>|<span data-ttu-id="0a6cf-137">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="0a6cf-137">Name of the profile</span></span>|
|<span data-ttu-id="0a6cf-138">profileDescription</span><span class="sxs-lookup"><span data-stu-id="0a6cf-138">profileDescription</span></span>|<span data-ttu-id="0a6cf-139">String</span><span class="sxs-lookup"><span data-stu-id="0a6cf-139">String</span></span>|<span data-ttu-id="0a6cf-140">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="0a6cf-140">Description of the profile</span></span>|
|<span data-ttu-id="0a6cf-141">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="0a6cf-141">isDefaultProfile</span></span>|<span data-ttu-id="0a6cf-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="0a6cf-142">Boolean</span></span>|<span data-ttu-id="0a6cf-143">Booliano que indica se o perfil é usado como padrão ou não</span><span class="sxs-lookup"><span data-stu-id="0a6cf-143">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="0a6cf-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a6cf-144">createdDateTime</span></span>|<span data-ttu-id="0a6cf-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a6cf-145">DateTimeOffset</span></span>|<span data-ttu-id="0a6cf-146">Hora em que o BrandingProfile foi criado</span><span class="sxs-lookup"><span data-stu-id="0a6cf-146">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="0a6cf-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a6cf-147">lastModifiedDateTime</span></span>|<span data-ttu-id="0a6cf-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a6cf-148">DateTimeOffset</span></span>|<span data-ttu-id="0a6cf-149">Hora em que a BrandingProfile foi modificada pela última vez</span><span class="sxs-lookup"><span data-stu-id="0a6cf-149">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="0a6cf-150">displayName</span><span class="sxs-lookup"><span data-stu-id="0a6cf-150">displayName</span></span>|<span data-ttu-id="0a6cf-151">String</span><span class="sxs-lookup"><span data-stu-id="0a6cf-151">String</span></span>|<span data-ttu-id="0a6cf-152">Nome da empresa/organização que é exibido para os usuários finais</span><span class="sxs-lookup"><span data-stu-id="0a6cf-152">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="0a6cf-153">contactITName</span><span class="sxs-lookup"><span data-stu-id="0a6cf-153">contactITName</span></span>|<span data-ttu-id="0a6cf-154">String</span><span class="sxs-lookup"><span data-stu-id="0a6cf-154">String</span></span>|<span data-ttu-id="0a6cf-155">Nome da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="0a6cf-155">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="0a6cf-156">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="0a6cf-156">contactITPhoneNumber</span></span>|<span data-ttu-id="0a6cf-157">String</span><span class="sxs-lookup"><span data-stu-id="0a6cf-157">String</span></span>|<span data-ttu-id="0a6cf-158">Número de telefone da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="0a6cf-158">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="0a6cf-159">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0a6cf-159">contactITEmailAddress</span></span>|<span data-ttu-id="0a6cf-160">String</span><span class="sxs-lookup"><span data-stu-id="0a6cf-160">String</span></span>|<span data-ttu-id="0a6cf-161">Endereço de email da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="0a6cf-161">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="0a6cf-162">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="0a6cf-162">contactITNotes</span></span>|<span data-ttu-id="0a6cf-163">String</span><span class="sxs-lookup"><span data-stu-id="0a6cf-163">String</span></span>|<span data-ttu-id="0a6cf-164">Comentários de texto sobre a pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="0a6cf-164">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="0a6cf-165">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="0a6cf-165">privacyUrl</span></span>|<span data-ttu-id="0a6cf-166">String</span><span class="sxs-lookup"><span data-stu-id="0a6cf-166">String</span></span>|<span data-ttu-id="0a6cf-167">URL para a política de privacidade da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="0a6cf-167">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="0a6cf-168">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="0a6cf-168">onlineSupportSiteUrl</span></span>|<span data-ttu-id="0a6cf-169">String</span><span class="sxs-lookup"><span data-stu-id="0a6cf-169">String</span></span>|<span data-ttu-id="0a6cf-170">URL para o site de assistência técnica de ti da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="0a6cf-170">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="0a6cf-171">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="0a6cf-171">onlineSupportSiteName</span></span>|<span data-ttu-id="0a6cf-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a6cf-172">String</span></span>|<span data-ttu-id="0a6cf-173">Nome para exibição do site de assistência técnica de ti da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="0a6cf-173">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="0a6cf-174">themeColor</span><span class="sxs-lookup"><span data-stu-id="0a6cf-174">themeColor</span></span>|[<span data-ttu-id="0a6cf-175">rgbColor</span><span class="sxs-lookup"><span data-stu-id="0a6cf-175">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="0a6cf-176">Cor do tema principal usada nos aplicativos do portal da empresa e no portal da Web</span><span class="sxs-lookup"><span data-stu-id="0a6cf-176">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="0a6cf-177">showLogo</span><span class="sxs-lookup"><span data-stu-id="0a6cf-177">showLogo</span></span>|<span data-ttu-id="0a6cf-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="0a6cf-178">Boolean</span></span>|<span data-ttu-id="0a6cf-179">Booliano que indica se as imagens de logotipo fornecidas pelo administrador são mostradas ou não</span><span class="sxs-lookup"><span data-stu-id="0a6cf-179">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="0a6cf-180">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="0a6cf-180">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="0a6cf-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="0a6cf-181">Boolean</span></span>|<span data-ttu-id="0a6cf-182">Booliano que indica se o nome de exibição fornecido pelo administrador será mostrado ao lado da imagem de logotipo ou não</span><span class="sxs-lookup"><span data-stu-id="0a6cf-182">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="0a6cf-183">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="0a6cf-183">themeColorLogo</span></span>|[<span data-ttu-id="0a6cf-184">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0a6cf-184">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0a6cf-185">Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo de cor de tema atrás do logotipo</span><span class="sxs-lookup"><span data-stu-id="0a6cf-185">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="0a6cf-186">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="0a6cf-186">lightBackgroundLogo</span></span>|[<span data-ttu-id="0a6cf-187">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0a6cf-187">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0a6cf-188">Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo claro atrás do logotipo</span><span class="sxs-lookup"><span data-stu-id="0a6cf-188">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="0a6cf-189">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="0a6cf-189">landingPageCustomizedImage</span></span>|[<span data-ttu-id="0a6cf-190">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0a6cf-190">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0a6cf-191">Imagem personalizada exibida na página inicial dos aplicativos do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="0a6cf-191">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="0a6cf-192">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="0a6cf-192">customPrivacyMessage</span></span>|<span data-ttu-id="0a6cf-193">String</span><span class="sxs-lookup"><span data-stu-id="0a6cf-193">String</span></span>|<span data-ttu-id="0a6cf-194">Comentários de texto sobre o que o administrador tem acesso ao no dispositivo</span><span class="sxs-lookup"><span data-stu-id="0a6cf-194">Text comments regarding what the admin has access to on the device</span></span>|



## <a name="response"></a><span data-ttu-id="0a6cf-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a6cf-195">Response</span></span>
<span data-ttu-id="0a6cf-196">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a6cf-196">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a6cf-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a6cf-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a6cf-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a6cf-198">Request</span></span>
<span data-ttu-id="0a6cf-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a6cf-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1264

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
  "customPrivacyMessage": "Custom Privacy Message value"
}
```

### <a name="response"></a><span data-ttu-id="0a6cf-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a6cf-200">Response</span></span>
<span data-ttu-id="0a6cf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a6cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1436

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
  "customPrivacyMessage": "Custom Privacy Message value"
}
```





