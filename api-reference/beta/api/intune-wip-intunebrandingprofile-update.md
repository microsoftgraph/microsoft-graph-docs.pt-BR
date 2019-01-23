---
title: Atualizar intuneBrandingProfile
description: Atualize as propriedades de um objeto intuneBrandingProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fa1382101012bb202286f75489532a80a87bb381
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403088"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="e3269-103">Atualizar intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="e3269-103">Update intuneBrandingProfile</span></span>

> <span data-ttu-id="e3269-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e3269-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e3269-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e3269-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3269-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e3269-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3269-107">Atualize as propriedades de um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e3269-107">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3269-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3269-108">Prerequisites</span></span>
<span data-ttu-id="e3269-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e3269-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e3269-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3269-111">Permission type</span></span>|<span data-ttu-id="e3269-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e3269-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3269-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3269-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3269-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3269-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e3269-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3269-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3269-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3269-116">Not supported.</span></span>|
|<span data-ttu-id="e3269-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3269-117">Application</span></span>|<span data-ttu-id="e3269-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3269-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3269-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3269-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="e3269-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3269-120">Request headers</span></span>
|<span data-ttu-id="e3269-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e3269-121">Header</span></span>|<span data-ttu-id="e3269-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e3269-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3269-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3269-123">Authorization</span></span>|<span data-ttu-id="e3269-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3269-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3269-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e3269-125">Accept</span></span>|<span data-ttu-id="e3269-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3269-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3269-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3269-127">Request body</span></span>
<span data-ttu-id="e3269-128">No corpo da solicitação, fornece uma representação JSON para o objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e3269-128">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="e3269-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e3269-129">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="e3269-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3269-130">Property</span></span>|<span data-ttu-id="e3269-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3269-131">Type</span></span>|<span data-ttu-id="e3269-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3269-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3269-133">id</span><span class="sxs-lookup"><span data-stu-id="e3269-133">id</span></span>|<span data-ttu-id="e3269-134">String</span><span class="sxs-lookup"><span data-stu-id="e3269-134">String</span></span>|<span data-ttu-id="e3269-135">Chave de perfil</span><span class="sxs-lookup"><span data-stu-id="e3269-135">Profile Key</span></span>|
|<span data-ttu-id="e3269-136">profileName</span><span class="sxs-lookup"><span data-stu-id="e3269-136">profileName</span></span>|<span data-ttu-id="e3269-137">String</span><span class="sxs-lookup"><span data-stu-id="e3269-137">String</span></span>|<span data-ttu-id="e3269-138">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="e3269-138">Name of the profile</span></span>|
|<span data-ttu-id="e3269-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="e3269-139">profileDescription</span></span>|<span data-ttu-id="e3269-140">String</span><span class="sxs-lookup"><span data-stu-id="e3269-140">String</span></span>|<span data-ttu-id="e3269-141">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="e3269-141">Description of the profile</span></span>|
|<span data-ttu-id="e3269-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="e3269-142">isDefaultProfile</span></span>|<span data-ttu-id="e3269-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3269-143">Boolean</span></span>|<span data-ttu-id="e3269-144">Apresenta se o perfil é usado para padrão.</span><span class="sxs-lookup"><span data-stu-id="e3269-144">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="e3269-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3269-145">createdDateTime</span></span>|<span data-ttu-id="e3269-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3269-146">DateTimeOffset</span></span>|<span data-ttu-id="e3269-147">Quando o BrandingProfile foi criado.</span><span class="sxs-lookup"><span data-stu-id="e3269-147">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="e3269-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3269-148">lastModifiedDateTime</span></span>|<span data-ttu-id="e3269-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3269-149">DateTimeOffset</span></span>|<span data-ttu-id="e3269-150">Quando o BrandingProfile última modificação.</span><span class="sxs-lookup"><span data-stu-id="e3269-150">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="e3269-151">displayName</span><span class="sxs-lookup"><span data-stu-id="e3269-151">displayName</span></span>|<span data-ttu-id="e3269-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3269-152">String</span></span>|<span data-ttu-id="e3269-153">Nome da empresa/organização exibido para usuários finais.</span><span class="sxs-lookup"><span data-stu-id="e3269-153">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="e3269-154">contactITName</span><span class="sxs-lookup"><span data-stu-id="e3269-154">contactITName</span></span>|<span data-ttu-id="e3269-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3269-155">String</span></span>|<span data-ttu-id="e3269-156">Nome da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="e3269-156">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="e3269-157">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="e3269-157">contactITPhoneNumber</span></span>|<span data-ttu-id="e3269-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3269-158">String</span></span>|<span data-ttu-id="e3269-159">Número de telefone da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="e3269-159">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="e3269-160">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e3269-160">contactITEmailAddress</span></span>|<span data-ttu-id="e3269-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3269-161">String</span></span>|<span data-ttu-id="e3269-162">Endereço de email da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="e3269-162">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="e3269-163">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="e3269-163">contactITNotes</span></span>|<span data-ttu-id="e3269-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3269-164">String</span></span>|<span data-ttu-id="e3269-165">Comentários de texto relacionados à pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="e3269-165">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="e3269-166">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="e3269-166">privacyUrl</span></span>|<span data-ttu-id="e3269-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3269-167">String</span></span>|<span data-ttu-id="e3269-168">URL da política de privacidade da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="e3269-168">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="e3269-169">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="e3269-169">onlineSupportSiteUrl</span></span>|<span data-ttu-id="e3269-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3269-170">String</span></span>|<span data-ttu-id="e3269-171">URL do site de assistência técnica de TI da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="e3269-171">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="e3269-172">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="e3269-172">onlineSupportSiteName</span></span>|<span data-ttu-id="e3269-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3269-173">String</span></span>|<span data-ttu-id="e3269-174">Nome de exibição do site de assistência técnica de TI da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="e3269-174">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="e3269-175">themeColor</span><span class="sxs-lookup"><span data-stu-id="e3269-175">themeColor</span></span>|[<span data-ttu-id="e3269-176">rgbColor</span><span class="sxs-lookup"><span data-stu-id="e3269-176">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="e3269-177">Cor de tema principal usado nos aplicativos e no portal da Web do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="e3269-177">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="e3269-178">showLogo</span><span class="sxs-lookup"><span data-stu-id="e3269-178">showLogo</span></span>|<span data-ttu-id="e3269-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="e3269-179">Boolean</span></span>|<span data-ttu-id="e3269-180">Booliano que indica se as imagens de logotipo fornecidas pelo administrador serão exibidas ou não.</span><span class="sxs-lookup"><span data-stu-id="e3269-180">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="e3269-181">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="e3269-181">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="e3269-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="e3269-182">Boolean</span></span>|<span data-ttu-id="e3269-183">Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.</span><span class="sxs-lookup"><span data-stu-id="e3269-183">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="e3269-184">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="e3269-184">themeColorLogo</span></span>|[<span data-ttu-id="e3269-185">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e3269-185">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e3269-186">Imagem de logotipo exibida nos aplicativos de Portal da empresa nos planos de fundo de cores de tema.</span><span class="sxs-lookup"><span data-stu-id="e3269-186">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="e3269-187">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="e3269-187">lightBackgroundLogo</span></span>|[<span data-ttu-id="e3269-188">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e3269-188">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e3269-189">Imagem de logotipo exibida nos aplicativos de Portal da empresa nos planos de fundo claras.</span><span class="sxs-lookup"><span data-stu-id="e3269-189">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="e3269-190">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="e3269-190">landingPageCustomizedImage</span></span>|[<span data-ttu-id="e3269-191">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e3269-191">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e3269-192">Imagem personalizada exibida na página inicial de aplicativos de Portal da empresa</span><span class="sxs-lookup"><span data-stu-id="e3269-192">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="e3269-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3269-193">Response</span></span>
<span data-ttu-id="e3269-194">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3269-194">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3269-195">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3269-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3269-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3269-196">Request</span></span>
<span data-ttu-id="e3269-197">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3269-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
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

### <a name="response"></a><span data-ttu-id="e3269-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3269-198">Response</span></span>
<span data-ttu-id="e3269-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3269-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




