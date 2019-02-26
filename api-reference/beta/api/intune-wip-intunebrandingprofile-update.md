---
title: Atualizar intuneBrandingProfile
description: Atualiza as propriedades de um objeto intuneBrandingProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a66589e4be7d5cc175c792935e2f309c8f28e33
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162339"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="b946e-103">Atualizar intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="b946e-103">Update intuneBrandingProfile</span></span>

> <span data-ttu-id="b946e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b946e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b946e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b946e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b946e-106">Atualiza as propriedades de um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b946e-106">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b946e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b946e-107">Prerequisites</span></span>
<span data-ttu-id="b946e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b946e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b946e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b946e-110">Permission type</span></span>|<span data-ttu-id="b946e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b946e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b946e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b946e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b946e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b946e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b946e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b946e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b946e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b946e-115">Not supported.</span></span>|
|<span data-ttu-id="b946e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b946e-116">Application</span></span>|<span data-ttu-id="b946e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b946e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b946e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b946e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="b946e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b946e-119">Request headers</span></span>
|<span data-ttu-id="b946e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b946e-120">Header</span></span>|<span data-ttu-id="b946e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b946e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b946e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b946e-122">Authorization</span></span>|<span data-ttu-id="b946e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b946e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b946e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b946e-124">Accept</span></span>|<span data-ttu-id="b946e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b946e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b946e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b946e-126">Request body</span></span>
<span data-ttu-id="b946e-127">No corpo da solicitação, forneça uma representação JSON do objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b946e-127">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="b946e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span><span class="sxs-lookup"><span data-stu-id="b946e-128">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="b946e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b946e-129">Property</span></span>|<span data-ttu-id="b946e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b946e-130">Type</span></span>|<span data-ttu-id="b946e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b946e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b946e-132">id</span><span class="sxs-lookup"><span data-stu-id="b946e-132">id</span></span>|<span data-ttu-id="b946e-133">String</span><span class="sxs-lookup"><span data-stu-id="b946e-133">String</span></span>|<span data-ttu-id="b946e-134">Chave de perfil</span><span class="sxs-lookup"><span data-stu-id="b946e-134">Profile Key</span></span>|
|<span data-ttu-id="b946e-135">ProfileName</span><span class="sxs-lookup"><span data-stu-id="b946e-135">profileName</span></span>|<span data-ttu-id="b946e-136">String</span><span class="sxs-lookup"><span data-stu-id="b946e-136">String</span></span>|<span data-ttu-id="b946e-137">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="b946e-137">Name of the profile</span></span>|
|<span data-ttu-id="b946e-138">profileDescription</span><span class="sxs-lookup"><span data-stu-id="b946e-138">profileDescription</span></span>|<span data-ttu-id="b946e-139">String</span><span class="sxs-lookup"><span data-stu-id="b946e-139">String</span></span>|<span data-ttu-id="b946e-140">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="b946e-140">Description of the profile</span></span>|
|<span data-ttu-id="b946e-141">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="b946e-141">isDefaultProfile</span></span>|<span data-ttu-id="b946e-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="b946e-142">Boolean</span></span>|<span data-ttu-id="b946e-143">Apresenta se o perfil é usado para o padrão.</span><span class="sxs-lookup"><span data-stu-id="b946e-143">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="b946e-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b946e-144">createdDateTime</span></span>|<span data-ttu-id="b946e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b946e-145">DateTimeOffset</span></span>|<span data-ttu-id="b946e-146">Quando o BrandingProfile foi criado.</span><span class="sxs-lookup"><span data-stu-id="b946e-146">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="b946e-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b946e-147">lastModifiedDateTime</span></span>|<span data-ttu-id="b946e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b946e-148">DateTimeOffset</span></span>|<span data-ttu-id="b946e-149">Quando o BrandingProfile foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b946e-149">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="b946e-150">displayName</span><span class="sxs-lookup"><span data-stu-id="b946e-150">displayName</span></span>|<span data-ttu-id="b946e-151">String</span><span class="sxs-lookup"><span data-stu-id="b946e-151">String</span></span>|<span data-ttu-id="b946e-152">Nome da empresa/organização exibido para usuários finais.</span><span class="sxs-lookup"><span data-stu-id="b946e-152">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="b946e-153">contactITName</span><span class="sxs-lookup"><span data-stu-id="b946e-153">contactITName</span></span>|<span data-ttu-id="b946e-154">String</span><span class="sxs-lookup"><span data-stu-id="b946e-154">String</span></span>|<span data-ttu-id="b946e-155">Nome da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="b946e-155">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="b946e-156">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="b946e-156">contactITPhoneNumber</span></span>|<span data-ttu-id="b946e-157">String</span><span class="sxs-lookup"><span data-stu-id="b946e-157">String</span></span>|<span data-ttu-id="b946e-158">Número de telefone da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="b946e-158">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="b946e-159">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="b946e-159">contactITEmailAddress</span></span>|<span data-ttu-id="b946e-160">String</span><span class="sxs-lookup"><span data-stu-id="b946e-160">String</span></span>|<span data-ttu-id="b946e-161">Endereço de email da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="b946e-161">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="b946e-162">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="b946e-162">contactITNotes</span></span>|<span data-ttu-id="b946e-163">String</span><span class="sxs-lookup"><span data-stu-id="b946e-163">String</span></span>|<span data-ttu-id="b946e-164">Comentários de texto relacionados à pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="b946e-164">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="b946e-165">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="b946e-165">privacyUrl</span></span>|<span data-ttu-id="b946e-166">String</span><span class="sxs-lookup"><span data-stu-id="b946e-166">String</span></span>|<span data-ttu-id="b946e-167">URL da política de privacidade da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="b946e-167">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="b946e-168">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="b946e-168">onlineSupportSiteUrl</span></span>|<span data-ttu-id="b946e-169">String</span><span class="sxs-lookup"><span data-stu-id="b946e-169">String</span></span>|<span data-ttu-id="b946e-170">URL do site de assistência técnica de TI da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="b946e-170">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="b946e-171">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="b946e-171">onlineSupportSiteName</span></span>|<span data-ttu-id="b946e-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b946e-172">String</span></span>|<span data-ttu-id="b946e-173">Nome de exibição do site de assistência técnica de TI da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="b946e-173">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="b946e-174">themeColor</span><span class="sxs-lookup"><span data-stu-id="b946e-174">themeColor</span></span>|[<span data-ttu-id="b946e-175">rgbColor</span><span class="sxs-lookup"><span data-stu-id="b946e-175">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="b946e-176">Cor de tema principal usado nos aplicativos e no portal da Web do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="b946e-176">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="b946e-177">showLogo</span><span class="sxs-lookup"><span data-stu-id="b946e-177">showLogo</span></span>|<span data-ttu-id="b946e-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="b946e-178">Boolean</span></span>|<span data-ttu-id="b946e-179">Booliano que indica se as imagens de logotipo fornecidas pelo administrador serão exibidas ou não.</span><span class="sxs-lookup"><span data-stu-id="b946e-179">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="b946e-180">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="b946e-180">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="b946e-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="b946e-181">Boolean</span></span>|<span data-ttu-id="b946e-182">Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.</span><span class="sxs-lookup"><span data-stu-id="b946e-182">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="b946e-183">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="b946e-183">themeColorLogo</span></span>|[<span data-ttu-id="b946e-184">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b946e-184">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b946e-185">Imagem do logotipo exibida nos aplicativos do portal da empresa em planos de fundo de cores de tema.</span><span class="sxs-lookup"><span data-stu-id="b946e-185">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="b946e-186">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="b946e-186">lightBackgroundLogo</span></span>|[<span data-ttu-id="b946e-187">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b946e-187">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b946e-188">Imagem do logotipo exibida nos aplicativos do portal da empresa em planos de fundo claros.</span><span class="sxs-lookup"><span data-stu-id="b946e-188">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="b946e-189">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="b946e-189">landingPageCustomizedImage</span></span>|[<span data-ttu-id="b946e-190">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b946e-190">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b946e-191">Imagem personalizada exibida na página inicial dos aplicativos do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="b946e-191">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="b946e-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="b946e-192">Response</span></span>
<span data-ttu-id="b946e-193">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b946e-193">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b946e-194">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b946e-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="b946e-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b946e-195">Request</span></span>
<span data-ttu-id="b946e-196">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b946e-196">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b946e-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="b946e-197">Response</span></span>
<span data-ttu-id="b946e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b946e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




