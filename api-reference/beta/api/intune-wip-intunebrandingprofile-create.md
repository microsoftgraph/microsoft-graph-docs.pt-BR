---
title: Criar intuneBrandingProfile
description: Crie um novo objeto de intuneBrandingProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a613d6d98aee2b17624e7894cafa712c7d6b66ed
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399532"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="17be3-103">Criar intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="17be3-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="17be3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="17be3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="17be3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="17be3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17be3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="17be3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17be3-107">Crie um novo objeto de [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="17be3-107">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17be3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17be3-108">Prerequisites</span></span>
<span data-ttu-id="17be3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="17be3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="17be3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17be3-111">Permission type</span></span>|<span data-ttu-id="17be3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17be3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17be3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17be3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17be3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17be3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="17be3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17be3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17be3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17be3-116">Not supported.</span></span>|
|<span data-ttu-id="17be3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17be3-117">Application</span></span>|<span data-ttu-id="17be3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17be3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17be3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17be3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="17be3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17be3-120">Request headers</span></span>
|<span data-ttu-id="17be3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17be3-121">Header</span></span>|<span data-ttu-id="17be3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="17be3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17be3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="17be3-123">Authorization</span></span>|<span data-ttu-id="17be3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17be3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17be3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17be3-125">Accept</span></span>|<span data-ttu-id="17be3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17be3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17be3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17be3-127">Request body</span></span>
<span data-ttu-id="17be3-128">No corpo da solicitação, fornece uma representação JSON para o objeto intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="17be3-128">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="17be3-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="17be3-129">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="17be3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17be3-130">Property</span></span>|<span data-ttu-id="17be3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="17be3-131">Type</span></span>|<span data-ttu-id="17be3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="17be3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17be3-133">id</span><span class="sxs-lookup"><span data-stu-id="17be3-133">id</span></span>|<span data-ttu-id="17be3-134">String</span><span class="sxs-lookup"><span data-stu-id="17be3-134">String</span></span>|<span data-ttu-id="17be3-135">Chave de perfil</span><span class="sxs-lookup"><span data-stu-id="17be3-135">Profile Key</span></span>|
|<span data-ttu-id="17be3-136">profileName</span><span class="sxs-lookup"><span data-stu-id="17be3-136">profileName</span></span>|<span data-ttu-id="17be3-137">String</span><span class="sxs-lookup"><span data-stu-id="17be3-137">String</span></span>|<span data-ttu-id="17be3-138">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="17be3-138">Name of the profile</span></span>|
|<span data-ttu-id="17be3-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="17be3-139">profileDescription</span></span>|<span data-ttu-id="17be3-140">String</span><span class="sxs-lookup"><span data-stu-id="17be3-140">String</span></span>|<span data-ttu-id="17be3-141">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="17be3-141">Description of the profile</span></span>|
|<span data-ttu-id="17be3-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="17be3-142">isDefaultProfile</span></span>|<span data-ttu-id="17be3-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="17be3-143">Boolean</span></span>|<span data-ttu-id="17be3-144">Apresenta se o perfil é usado para padrão.</span><span class="sxs-lookup"><span data-stu-id="17be3-144">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="17be3-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17be3-145">createdDateTime</span></span>|<span data-ttu-id="17be3-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17be3-146">DateTimeOffset</span></span>|<span data-ttu-id="17be3-147">Quando o BrandingProfile foi criado.</span><span class="sxs-lookup"><span data-stu-id="17be3-147">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="17be3-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17be3-148">lastModifiedDateTime</span></span>|<span data-ttu-id="17be3-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17be3-149">DateTimeOffset</span></span>|<span data-ttu-id="17be3-150">Quando o BrandingProfile última modificação.</span><span class="sxs-lookup"><span data-stu-id="17be3-150">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="17be3-151">displayName</span><span class="sxs-lookup"><span data-stu-id="17be3-151">displayName</span></span>|<span data-ttu-id="17be3-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17be3-152">String</span></span>|<span data-ttu-id="17be3-153">Nome da empresa/organização exibido para usuários finais.</span><span class="sxs-lookup"><span data-stu-id="17be3-153">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="17be3-154">contactITName</span><span class="sxs-lookup"><span data-stu-id="17be3-154">contactITName</span></span>|<span data-ttu-id="17be3-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17be3-155">String</span></span>|<span data-ttu-id="17be3-156">Nome da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="17be3-156">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="17be3-157">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="17be3-157">contactITPhoneNumber</span></span>|<span data-ttu-id="17be3-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17be3-158">String</span></span>|<span data-ttu-id="17be3-159">Número de telefone da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="17be3-159">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="17be3-160">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="17be3-160">contactITEmailAddress</span></span>|<span data-ttu-id="17be3-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17be3-161">String</span></span>|<span data-ttu-id="17be3-162">Endereço de email da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="17be3-162">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="17be3-163">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="17be3-163">contactITNotes</span></span>|<span data-ttu-id="17be3-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17be3-164">String</span></span>|<span data-ttu-id="17be3-165">Comentários de texto relacionados à pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="17be3-165">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="17be3-166">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="17be3-166">privacyUrl</span></span>|<span data-ttu-id="17be3-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17be3-167">String</span></span>|<span data-ttu-id="17be3-168">URL da política de privacidade da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="17be3-168">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="17be3-169">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="17be3-169">onlineSupportSiteUrl</span></span>|<span data-ttu-id="17be3-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17be3-170">String</span></span>|<span data-ttu-id="17be3-171">URL do site de assistência técnica de TI da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="17be3-171">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="17be3-172">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="17be3-172">onlineSupportSiteName</span></span>|<span data-ttu-id="17be3-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17be3-173">String</span></span>|<span data-ttu-id="17be3-174">Nome de exibição do site de assistência técnica de TI da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="17be3-174">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="17be3-175">themeColor</span><span class="sxs-lookup"><span data-stu-id="17be3-175">themeColor</span></span>|[<span data-ttu-id="17be3-176">rgbColor</span><span class="sxs-lookup"><span data-stu-id="17be3-176">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="17be3-177">Cor de tema principal usado nos aplicativos e no portal da Web do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="17be3-177">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="17be3-178">showLogo</span><span class="sxs-lookup"><span data-stu-id="17be3-178">showLogo</span></span>|<span data-ttu-id="17be3-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="17be3-179">Boolean</span></span>|<span data-ttu-id="17be3-180">Booliano que indica se as imagens de logotipo fornecidas pelo administrador serão exibidas ou não.</span><span class="sxs-lookup"><span data-stu-id="17be3-180">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="17be3-181">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="17be3-181">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="17be3-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="17be3-182">Boolean</span></span>|<span data-ttu-id="17be3-183">Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.</span><span class="sxs-lookup"><span data-stu-id="17be3-183">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="17be3-184">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="17be3-184">themeColorLogo</span></span>|[<span data-ttu-id="17be3-185">mimeContent</span><span class="sxs-lookup"><span data-stu-id="17be3-185">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="17be3-186">Imagem de logotipo exibida nos aplicativos de Portal da empresa nos planos de fundo de cores de tema.</span><span class="sxs-lookup"><span data-stu-id="17be3-186">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="17be3-187">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="17be3-187">lightBackgroundLogo</span></span>|[<span data-ttu-id="17be3-188">mimeContent</span><span class="sxs-lookup"><span data-stu-id="17be3-188">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="17be3-189">Imagem de logotipo exibida nos aplicativos de Portal da empresa nos planos de fundo claras.</span><span class="sxs-lookup"><span data-stu-id="17be3-189">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="17be3-190">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="17be3-190">landingPageCustomizedImage</span></span>|[<span data-ttu-id="17be3-191">mimeContent</span><span class="sxs-lookup"><span data-stu-id="17be3-191">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="17be3-192">Imagem personalizada exibida na página inicial de aplicativos de Portal da empresa</span><span class="sxs-lookup"><span data-stu-id="17be3-192">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="17be3-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="17be3-193">Response</span></span>
<span data-ttu-id="17be3-194">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17be3-194">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17be3-195">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17be3-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="17be3-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17be3-196">Request</span></span>
<span data-ttu-id="17be3-197">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17be3-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1205

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
  }
}
```

### <a name="response"></a><span data-ttu-id="17be3-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="17be3-198">Response</span></span>
<span data-ttu-id="17be3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17be3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1377

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
  }
}
```




