---
title: Atualizar intuneBrandingProfile
description: Atualiza as propriedades de um objeto intuneBrandingProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1a2bb95404c3976b8702e752b5d9d17ad3872191
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457423"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="83b90-103">Atualizar intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="83b90-103">Update intuneBrandingProfile</span></span>

<span data-ttu-id="83b90-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="83b90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83b90-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83b90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83b90-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83b90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83b90-107">Atualiza as propriedades de um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="83b90-107">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83b90-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="83b90-108">Prerequisites</span></span>
<span data-ttu-id="83b90-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83b90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83b90-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83b90-111">Permission type</span></span>|<span data-ttu-id="83b90-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="83b90-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83b90-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83b90-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83b90-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b90-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="83b90-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83b90-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83b90-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83b90-116">Not supported.</span></span>|
|<span data-ttu-id="83b90-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83b90-117">Application</span></span>|<span data-ttu-id="83b90-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b90-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83b90-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83b90-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="83b90-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83b90-120">Request headers</span></span>
|<span data-ttu-id="83b90-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83b90-121">Header</span></span>|<span data-ttu-id="83b90-122">Valor</span><span class="sxs-lookup"><span data-stu-id="83b90-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83b90-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="83b90-123">Authorization</span></span>|<span data-ttu-id="83b90-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83b90-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83b90-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="83b90-125">Accept</span></span>|<span data-ttu-id="83b90-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83b90-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83b90-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83b90-127">Request body</span></span>
<span data-ttu-id="83b90-128">No corpo da solicitação, forneça uma representação JSON do objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="83b90-128">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="83b90-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span><span class="sxs-lookup"><span data-stu-id="83b90-129">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="83b90-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83b90-130">Property</span></span>|<span data-ttu-id="83b90-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="83b90-131">Type</span></span>|<span data-ttu-id="83b90-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="83b90-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83b90-133">id</span><span class="sxs-lookup"><span data-stu-id="83b90-133">id</span></span>|<span data-ttu-id="83b90-134">String</span><span class="sxs-lookup"><span data-stu-id="83b90-134">String</span></span>|<span data-ttu-id="83b90-135">Chave de perfil</span><span class="sxs-lookup"><span data-stu-id="83b90-135">Profile Key</span></span>|
|<span data-ttu-id="83b90-136">ProfileName</span><span class="sxs-lookup"><span data-stu-id="83b90-136">profileName</span></span>|<span data-ttu-id="83b90-137">String</span><span class="sxs-lookup"><span data-stu-id="83b90-137">String</span></span>|<span data-ttu-id="83b90-138">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="83b90-138">Name of the profile</span></span>|
|<span data-ttu-id="83b90-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="83b90-139">profileDescription</span></span>|<span data-ttu-id="83b90-140">String</span><span class="sxs-lookup"><span data-stu-id="83b90-140">String</span></span>|<span data-ttu-id="83b90-141">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="83b90-141">Description of the profile</span></span>|
|<span data-ttu-id="83b90-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="83b90-142">isDefaultProfile</span></span>|<span data-ttu-id="83b90-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b90-143">Boolean</span></span>|<span data-ttu-id="83b90-144">Booliano que indica se o perfil é usado como padrão ou não</span><span class="sxs-lookup"><span data-stu-id="83b90-144">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="83b90-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83b90-145">createdDateTime</span></span>|<span data-ttu-id="83b90-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83b90-146">DateTimeOffset</span></span>|<span data-ttu-id="83b90-147">Hora em que o BrandingProfile foi criado</span><span class="sxs-lookup"><span data-stu-id="83b90-147">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="83b90-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83b90-148">lastModifiedDateTime</span></span>|<span data-ttu-id="83b90-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83b90-149">DateTimeOffset</span></span>|<span data-ttu-id="83b90-150">Hora em que a BrandingProfile foi modificada pela última vez</span><span class="sxs-lookup"><span data-stu-id="83b90-150">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="83b90-151">displayName</span><span class="sxs-lookup"><span data-stu-id="83b90-151">displayName</span></span>|<span data-ttu-id="83b90-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83b90-152">String</span></span>|<span data-ttu-id="83b90-153">Nome da empresa/organização que é exibido para os usuários finais</span><span class="sxs-lookup"><span data-stu-id="83b90-153">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="83b90-154">themeColor</span><span class="sxs-lookup"><span data-stu-id="83b90-154">themeColor</span></span>|[<span data-ttu-id="83b90-155">rgbColor</span><span class="sxs-lookup"><span data-stu-id="83b90-155">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="83b90-156">Cor do tema principal usada nos aplicativos do portal da empresa e no portal da Web</span><span class="sxs-lookup"><span data-stu-id="83b90-156">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="83b90-157">showLogo</span><span class="sxs-lookup"><span data-stu-id="83b90-157">showLogo</span></span>|<span data-ttu-id="83b90-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b90-158">Boolean</span></span>|<span data-ttu-id="83b90-159">Booliano que indica se as imagens de logotipo fornecidas pelo administrador são mostradas ou não</span><span class="sxs-lookup"><span data-stu-id="83b90-159">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="83b90-160">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="83b90-160">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="83b90-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="83b90-161">Boolean</span></span>|<span data-ttu-id="83b90-162">Booliano que indica se o nome de exibição fornecido pelo administrador será mostrado ao lado da imagem de logotipo ou não</span><span class="sxs-lookup"><span data-stu-id="83b90-162">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="83b90-163">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="83b90-163">themeColorLogo</span></span>|[<span data-ttu-id="83b90-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="83b90-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="83b90-165">Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo de cor de tema atrás do logotipo</span><span class="sxs-lookup"><span data-stu-id="83b90-165">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="83b90-166">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="83b90-166">lightBackgroundLogo</span></span>|[<span data-ttu-id="83b90-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="83b90-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="83b90-168">Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo claro atrás do logotipo</span><span class="sxs-lookup"><span data-stu-id="83b90-168">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="83b90-169">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="83b90-169">landingPageCustomizedImage</span></span>|[<span data-ttu-id="83b90-170">mimeContent</span><span class="sxs-lookup"><span data-stu-id="83b90-170">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="83b90-171">Imagem personalizada exibida na página inicial dos aplicativos do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="83b90-171">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="83b90-172">contactITName</span><span class="sxs-lookup"><span data-stu-id="83b90-172">contactITName</span></span>|<span data-ttu-id="83b90-173">String</span><span class="sxs-lookup"><span data-stu-id="83b90-173">String</span></span>|<span data-ttu-id="83b90-174">Nome da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="83b90-174">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="83b90-175">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="83b90-175">contactITPhoneNumber</span></span>|<span data-ttu-id="83b90-176">String</span><span class="sxs-lookup"><span data-stu-id="83b90-176">String</span></span>|<span data-ttu-id="83b90-177">Número de telefone da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="83b90-177">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="83b90-178">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="83b90-178">contactITEmailAddress</span></span>|<span data-ttu-id="83b90-179">String</span><span class="sxs-lookup"><span data-stu-id="83b90-179">String</span></span>|<span data-ttu-id="83b90-180">Endereço de email da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="83b90-180">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="83b90-181">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="83b90-181">contactITNotes</span></span>|<span data-ttu-id="83b90-182">String</span><span class="sxs-lookup"><span data-stu-id="83b90-182">String</span></span>|<span data-ttu-id="83b90-183">Comentários de texto sobre a pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="83b90-183">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="83b90-184">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="83b90-184">onlineSupportSiteUrl</span></span>|<span data-ttu-id="83b90-185">String</span><span class="sxs-lookup"><span data-stu-id="83b90-185">String</span></span>|<span data-ttu-id="83b90-186">URL para o site de assistência técnica de ti da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="83b90-186">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="83b90-187">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="83b90-187">onlineSupportSiteName</span></span>|<span data-ttu-id="83b90-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83b90-188">String</span></span>|<span data-ttu-id="83b90-189">Nome para exibição do site de assistência técnica de ti da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="83b90-189">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="83b90-190">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="83b90-190">privacyUrl</span></span>|<span data-ttu-id="83b90-191">String</span><span class="sxs-lookup"><span data-stu-id="83b90-191">String</span></span>|<span data-ttu-id="83b90-192">URL para a política de privacidade da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="83b90-192">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="83b90-193">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="83b90-193">customPrivacyMessage</span></span>|<span data-ttu-id="83b90-194">String</span><span class="sxs-lookup"><span data-stu-id="83b90-194">String</span></span>|<span data-ttu-id="83b90-195">Comentários de texto sobre o que o administrador tem acesso ao no dispositivo</span><span class="sxs-lookup"><span data-stu-id="83b90-195">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="83b90-196">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="83b90-196">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="83b90-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b90-197">Boolean</span></span>|<span data-ttu-id="83b90-198">Booliano que indica se o adminsistrator desabilitou a ação "remover dispositivo" em dispositivos corporativos de propriedade.</span><span class="sxs-lookup"><span data-stu-id="83b90-198">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="83b90-199">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="83b90-199">isFactoryResetDisabled</span></span>|<span data-ttu-id="83b90-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b90-200">Boolean</span></span>|<span data-ttu-id="83b90-201">Booliano que indica se o adminsistrator desabilitou a ação "redefinição de fábrica" em dispositivos corporativos de propriedade.</span><span class="sxs-lookup"><span data-stu-id="83b90-201">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="83b90-202">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="83b90-202">companyPortalBlockedActions</span></span>|<span data-ttu-id="83b90-203">coleção [companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="83b90-203">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="83b90-204">Conjunto de ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83b90-204">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="83b90-205">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="83b90-205">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="83b90-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b90-206">Boolean</span></span>|<span data-ttu-id="83b90-207">Booliano que indica se os aplicativos empresariais do AzureAD serão mostrados no portal da empresa</span><span class="sxs-lookup"><span data-stu-id="83b90-207">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="83b90-208">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="83b90-208">showOfficeWebApps</span></span>|<span data-ttu-id="83b90-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b90-209">Boolean</span></span>|<span data-ttu-id="83b90-210">Booliano que indica se o Office webapps será mostrado no portal da empresa</span><span class="sxs-lookup"><span data-stu-id="83b90-210">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="83b90-211">sendDeviceOwnershipChangePushNotification</span><span class="sxs-lookup"><span data-stu-id="83b90-211">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="83b90-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b90-212">Boolean</span></span>|<span data-ttu-id="83b90-213">Booliano que indica se uma notificação por push é enviada aos usuários quando o tipo de Propriedade do dispositivo muda de pessoal para corporativo</span><span class="sxs-lookup"><span data-stu-id="83b90-213">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="83b90-214">enrollmentAvailability</span><span class="sxs-lookup"><span data-stu-id="83b90-214">enrollmentAvailability</span></span>|[<span data-ttu-id="83b90-215">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="83b90-215">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="83b90-216">Fluxo de registro de dispositivo personalizado exibido para o usuário final.</span><span class="sxs-lookup"><span data-stu-id="83b90-216">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="83b90-217">Os valores possíveis são: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="83b90-217">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="83b90-218">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83b90-218">roleScopeTagIds</span></span>|<span data-ttu-id="83b90-219">String collection</span><span class="sxs-lookup"><span data-stu-id="83b90-219">String collection</span></span>|<span data-ttu-id="83b90-220">Lista de marcas de escopo atribuídas ao perfil de identidade visual</span><span class="sxs-lookup"><span data-stu-id="83b90-220">List of scope tags assigned to the branding profile</span></span>|



## <a name="response"></a><span data-ttu-id="83b90-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="83b90-221">Response</span></span>
<span data-ttu-id="83b90-222">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83b90-222">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83b90-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83b90-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="83b90-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83b90-224">Request</span></span>
<span data-ttu-id="83b90-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83b90-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
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

### <a name="response"></a><span data-ttu-id="83b90-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="83b90-226">Response</span></span>
<span data-ttu-id="83b90-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83b90-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





