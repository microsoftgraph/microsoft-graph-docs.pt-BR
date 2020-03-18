---
title: Criar intuneBrandingProfile
description: Criar um novo objeto intuneBrandingProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e67b58af13ec67d157a44b657e019a0bd4c37204
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799735"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="940fb-103">Criar intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="940fb-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="940fb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="940fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="940fb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="940fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="940fb-106">Criar um novo objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="940fb-106">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="940fb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="940fb-107">Prerequisites</span></span>
<span data-ttu-id="940fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="940fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="940fb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="940fb-110">Permission type</span></span>|<span data-ttu-id="940fb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="940fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="940fb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="940fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="940fb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="940fb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="940fb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="940fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="940fb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="940fb-115">Not supported.</span></span>|
|<span data-ttu-id="940fb-116">Application</span><span class="sxs-lookup"><span data-stu-id="940fb-116">Application</span></span>|<span data-ttu-id="940fb-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="940fb-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="940fb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="940fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="940fb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="940fb-119">Request headers</span></span>
|<span data-ttu-id="940fb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="940fb-120">Header</span></span>|<span data-ttu-id="940fb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="940fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="940fb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="940fb-122">Authorization</span></span>|<span data-ttu-id="940fb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="940fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="940fb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="940fb-124">Accept</span></span>|<span data-ttu-id="940fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="940fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="940fb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="940fb-126">Request body</span></span>
<span data-ttu-id="940fb-127">No corpo da solicitação, forneça uma representação JSON do objeto intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="940fb-127">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="940fb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="940fb-128">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="940fb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="940fb-129">Property</span></span>|<span data-ttu-id="940fb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="940fb-130">Type</span></span>|<span data-ttu-id="940fb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="940fb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="940fb-132">id</span><span class="sxs-lookup"><span data-stu-id="940fb-132">id</span></span>|<span data-ttu-id="940fb-133">String</span><span class="sxs-lookup"><span data-stu-id="940fb-133">String</span></span>|<span data-ttu-id="940fb-134">Chave de perfil</span><span class="sxs-lookup"><span data-stu-id="940fb-134">Profile Key</span></span>|
|<span data-ttu-id="940fb-135">ProfileName</span><span class="sxs-lookup"><span data-stu-id="940fb-135">profileName</span></span>|<span data-ttu-id="940fb-136">String</span><span class="sxs-lookup"><span data-stu-id="940fb-136">String</span></span>|<span data-ttu-id="940fb-137">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="940fb-137">Name of the profile</span></span>|
|<span data-ttu-id="940fb-138">profileDescription</span><span class="sxs-lookup"><span data-stu-id="940fb-138">profileDescription</span></span>|<span data-ttu-id="940fb-139">String</span><span class="sxs-lookup"><span data-stu-id="940fb-139">String</span></span>|<span data-ttu-id="940fb-140">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="940fb-140">Description of the profile</span></span>|
|<span data-ttu-id="940fb-141">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="940fb-141">isDefaultProfile</span></span>|<span data-ttu-id="940fb-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="940fb-142">Boolean</span></span>|<span data-ttu-id="940fb-143">Booliano que indica se o perfil é usado como padrão ou não</span><span class="sxs-lookup"><span data-stu-id="940fb-143">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="940fb-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="940fb-144">createdDateTime</span></span>|<span data-ttu-id="940fb-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="940fb-145">DateTimeOffset</span></span>|<span data-ttu-id="940fb-146">Hora em que o BrandingProfile foi criado</span><span class="sxs-lookup"><span data-stu-id="940fb-146">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="940fb-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="940fb-147">lastModifiedDateTime</span></span>|<span data-ttu-id="940fb-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="940fb-148">DateTimeOffset</span></span>|<span data-ttu-id="940fb-149">Hora em que a BrandingProfile foi modificada pela última vez</span><span class="sxs-lookup"><span data-stu-id="940fb-149">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="940fb-150">displayName</span><span class="sxs-lookup"><span data-stu-id="940fb-150">displayName</span></span>|<span data-ttu-id="940fb-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="940fb-151">String</span></span>|<span data-ttu-id="940fb-152">Nome da empresa/organização que é exibido para os usuários finais</span><span class="sxs-lookup"><span data-stu-id="940fb-152">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="940fb-153">themeColor</span><span class="sxs-lookup"><span data-stu-id="940fb-153">themeColor</span></span>|[<span data-ttu-id="940fb-154">rgbColor</span><span class="sxs-lookup"><span data-stu-id="940fb-154">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="940fb-155">Cor do tema principal usada nos aplicativos do portal da empresa e no portal da Web</span><span class="sxs-lookup"><span data-stu-id="940fb-155">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="940fb-156">showLogo</span><span class="sxs-lookup"><span data-stu-id="940fb-156">showLogo</span></span>|<span data-ttu-id="940fb-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="940fb-157">Boolean</span></span>|<span data-ttu-id="940fb-158">Booliano que indica se as imagens de logotipo fornecidas pelo administrador são mostradas ou não</span><span class="sxs-lookup"><span data-stu-id="940fb-158">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="940fb-159">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="940fb-159">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="940fb-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="940fb-160">Boolean</span></span>|<span data-ttu-id="940fb-161">Booliano que indica se o nome de exibição fornecido pelo administrador será mostrado ao lado da imagem de logotipo ou não</span><span class="sxs-lookup"><span data-stu-id="940fb-161">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="940fb-162">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="940fb-162">themeColorLogo</span></span>|[<span data-ttu-id="940fb-163">mimeContent</span><span class="sxs-lookup"><span data-stu-id="940fb-163">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="940fb-164">Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo de cor de tema atrás do logotipo</span><span class="sxs-lookup"><span data-stu-id="940fb-164">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="940fb-165">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="940fb-165">lightBackgroundLogo</span></span>|[<span data-ttu-id="940fb-166">mimeContent</span><span class="sxs-lookup"><span data-stu-id="940fb-166">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="940fb-167">Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo claro atrás do logotipo</span><span class="sxs-lookup"><span data-stu-id="940fb-167">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="940fb-168">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="940fb-168">landingPageCustomizedImage</span></span>|[<span data-ttu-id="940fb-169">mimeContent</span><span class="sxs-lookup"><span data-stu-id="940fb-169">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="940fb-170">Imagem personalizada exibida na página inicial dos aplicativos do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="940fb-170">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="940fb-171">contactITName</span><span class="sxs-lookup"><span data-stu-id="940fb-171">contactITName</span></span>|<span data-ttu-id="940fb-172">String</span><span class="sxs-lookup"><span data-stu-id="940fb-172">String</span></span>|<span data-ttu-id="940fb-173">Nome da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="940fb-173">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="940fb-174">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="940fb-174">contactITPhoneNumber</span></span>|<span data-ttu-id="940fb-175">String</span><span class="sxs-lookup"><span data-stu-id="940fb-175">String</span></span>|<span data-ttu-id="940fb-176">Número de telefone da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="940fb-176">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="940fb-177">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="940fb-177">contactITEmailAddress</span></span>|<span data-ttu-id="940fb-178">String</span><span class="sxs-lookup"><span data-stu-id="940fb-178">String</span></span>|<span data-ttu-id="940fb-179">Endereço de email da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="940fb-179">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="940fb-180">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="940fb-180">contactITNotes</span></span>|<span data-ttu-id="940fb-181">String</span><span class="sxs-lookup"><span data-stu-id="940fb-181">String</span></span>|<span data-ttu-id="940fb-182">Comentários de texto sobre a pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="940fb-182">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="940fb-183">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="940fb-183">onlineSupportSiteUrl</span></span>|<span data-ttu-id="940fb-184">String</span><span class="sxs-lookup"><span data-stu-id="940fb-184">String</span></span>|<span data-ttu-id="940fb-185">URL para o site de assistência técnica de ti da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="940fb-185">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="940fb-186">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="940fb-186">onlineSupportSiteName</span></span>|<span data-ttu-id="940fb-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="940fb-187">String</span></span>|<span data-ttu-id="940fb-188">Nome para exibição do site de assistência técnica de ti da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="940fb-188">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="940fb-189">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="940fb-189">privacyUrl</span></span>|<span data-ttu-id="940fb-190">String</span><span class="sxs-lookup"><span data-stu-id="940fb-190">String</span></span>|<span data-ttu-id="940fb-191">URL para a política de privacidade da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="940fb-191">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="940fb-192">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="940fb-192">customPrivacyMessage</span></span>|<span data-ttu-id="940fb-193">String</span><span class="sxs-lookup"><span data-stu-id="940fb-193">String</span></span>|<span data-ttu-id="940fb-194">Comentários de texto sobre o que o administrador tem acesso ao no dispositivo</span><span class="sxs-lookup"><span data-stu-id="940fb-194">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="940fb-195">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="940fb-195">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="940fb-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="940fb-196">Boolean</span></span>|<span data-ttu-id="940fb-197">Booliano que indica se o adminsistrator desabilitou a ação "remover dispositivo" em dispositivos corporativos de propriedade.</span><span class="sxs-lookup"><span data-stu-id="940fb-197">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="940fb-198">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="940fb-198">isFactoryResetDisabled</span></span>|<span data-ttu-id="940fb-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="940fb-199">Boolean</span></span>|<span data-ttu-id="940fb-200">Booliano que indica se o adminsistrator desabilitou a ação "redefinição de fábrica" em dispositivos corporativos de propriedade.</span><span class="sxs-lookup"><span data-stu-id="940fb-200">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="940fb-201">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="940fb-201">companyPortalBlockedActions</span></span>|<span data-ttu-id="940fb-202">coleção [companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="940fb-202">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="940fb-203">Conjunto de ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo.</span><span class="sxs-lookup"><span data-stu-id="940fb-203">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="940fb-204">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="940fb-204">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="940fb-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="940fb-205">Boolean</span></span>|<span data-ttu-id="940fb-206">Booliano que indica se os aplicativos empresariais do AzureAD serão mostrados no portal da empresa</span><span class="sxs-lookup"><span data-stu-id="940fb-206">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="940fb-207">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="940fb-207">showOfficeWebApps</span></span>|<span data-ttu-id="940fb-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="940fb-208">Boolean</span></span>|<span data-ttu-id="940fb-209">Booliano que indica se o Office webapps será mostrado no portal da empresa</span><span class="sxs-lookup"><span data-stu-id="940fb-209">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="940fb-210">sendDeviceOwnershipChangePushNotification</span><span class="sxs-lookup"><span data-stu-id="940fb-210">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="940fb-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="940fb-211">Boolean</span></span>|<span data-ttu-id="940fb-212">Booliano que indica se uma notificação por push é enviada aos usuários quando o tipo de Propriedade do dispositivo muda de pessoal para corporativo</span><span class="sxs-lookup"><span data-stu-id="940fb-212">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="940fb-213">enrollmentAvailability</span><span class="sxs-lookup"><span data-stu-id="940fb-213">enrollmentAvailability</span></span>|[<span data-ttu-id="940fb-214">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="940fb-214">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="940fb-215">Fluxo de registro de dispositivo personalizado exibido para o usuário final.</span><span class="sxs-lookup"><span data-stu-id="940fb-215">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="940fb-216">Os valores possíveis são: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="940fb-216">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="940fb-217">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="940fb-217">roleScopeTagIds</span></span>|<span data-ttu-id="940fb-218">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="940fb-218">String collection</span></span>|<span data-ttu-id="940fb-219">Lista de marcas de escopo atribuídas ao perfil de identidade visual</span><span class="sxs-lookup"><span data-stu-id="940fb-219">List of scope tags assigned to the branding profile</span></span>|



## <a name="response"></a><span data-ttu-id="940fb-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="940fb-220">Response</span></span>
<span data-ttu-id="940fb-221">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="940fb-221">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="940fb-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="940fb-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="940fb-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="940fb-223">Request</span></span>
<span data-ttu-id="940fb-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="940fb-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1792

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
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "availableWithoutPrompts",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="940fb-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="940fb-225">Response</span></span>
<span data-ttu-id="940fb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="940fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1964

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
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "availableWithoutPrompts",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




