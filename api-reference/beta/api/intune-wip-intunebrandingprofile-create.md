---
title: Criar intuneBrandingProfile
description: Criar um novo objeto intuneBrandingProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a3f9f77f964d26b753d4e634ea0db830490f3fba
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702688"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="891bb-103">Criar intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="891bb-103">Create intuneBrandingProfile</span></span>

<span data-ttu-id="891bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="891bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="891bb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="891bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="891bb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="891bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="891bb-107">Criar um novo objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="891bb-107">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="891bb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="891bb-108">Prerequisites</span></span>
<span data-ttu-id="891bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="891bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="891bb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="891bb-111">Permission type</span></span>|<span data-ttu-id="891bb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="891bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="891bb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="891bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="891bb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="891bb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="891bb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="891bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="891bb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="891bb-116">Not supported.</span></span>|
|<span data-ttu-id="891bb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="891bb-117">Application</span></span>|<span data-ttu-id="891bb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="891bb-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="891bb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="891bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="891bb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="891bb-120">Request headers</span></span>
|<span data-ttu-id="891bb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="891bb-121">Header</span></span>|<span data-ttu-id="891bb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="891bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="891bb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="891bb-123">Authorization</span></span>|<span data-ttu-id="891bb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="891bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="891bb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="891bb-125">Accept</span></span>|<span data-ttu-id="891bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="891bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="891bb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="891bb-127">Request body</span></span>
<span data-ttu-id="891bb-128">No corpo da solicitação, forneça uma representação JSON do objeto intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="891bb-128">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="891bb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="891bb-129">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="891bb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="891bb-130">Property</span></span>|<span data-ttu-id="891bb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="891bb-131">Type</span></span>|<span data-ttu-id="891bb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="891bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="891bb-133">id</span><span class="sxs-lookup"><span data-stu-id="891bb-133">id</span></span>|<span data-ttu-id="891bb-134">String</span><span class="sxs-lookup"><span data-stu-id="891bb-134">String</span></span>|<span data-ttu-id="891bb-135">Chave de perfil</span><span class="sxs-lookup"><span data-stu-id="891bb-135">Profile Key</span></span>|
|<span data-ttu-id="891bb-136">ProfileName</span><span class="sxs-lookup"><span data-stu-id="891bb-136">profileName</span></span>|<span data-ttu-id="891bb-137">String</span><span class="sxs-lookup"><span data-stu-id="891bb-137">String</span></span>|<span data-ttu-id="891bb-138">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="891bb-138">Name of the profile</span></span>|
|<span data-ttu-id="891bb-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="891bb-139">profileDescription</span></span>|<span data-ttu-id="891bb-140">String</span><span class="sxs-lookup"><span data-stu-id="891bb-140">String</span></span>|<span data-ttu-id="891bb-141">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="891bb-141">Description of the profile</span></span>|
|<span data-ttu-id="891bb-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="891bb-142">isDefaultProfile</span></span>|<span data-ttu-id="891bb-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="891bb-143">Boolean</span></span>|<span data-ttu-id="891bb-144">Booliano que indica se o perfil é usado como padrão ou não</span><span class="sxs-lookup"><span data-stu-id="891bb-144">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="891bb-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="891bb-145">createdDateTime</span></span>|<span data-ttu-id="891bb-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="891bb-146">DateTimeOffset</span></span>|<span data-ttu-id="891bb-147">Hora em que o BrandingProfile foi criado</span><span class="sxs-lookup"><span data-stu-id="891bb-147">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="891bb-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="891bb-148">lastModifiedDateTime</span></span>|<span data-ttu-id="891bb-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="891bb-149">DateTimeOffset</span></span>|<span data-ttu-id="891bb-150">Hora em que a BrandingProfile foi modificada pela última vez</span><span class="sxs-lookup"><span data-stu-id="891bb-150">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="891bb-151">displayName</span><span class="sxs-lookup"><span data-stu-id="891bb-151">displayName</span></span>|<span data-ttu-id="891bb-152">String</span><span class="sxs-lookup"><span data-stu-id="891bb-152">String</span></span>|<span data-ttu-id="891bb-153">Nome da empresa/organização que é exibido para os usuários finais</span><span class="sxs-lookup"><span data-stu-id="891bb-153">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="891bb-154">themeColor</span><span class="sxs-lookup"><span data-stu-id="891bb-154">themeColor</span></span>|[<span data-ttu-id="891bb-155">rgbColor</span><span class="sxs-lookup"><span data-stu-id="891bb-155">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="891bb-156">Cor do tema principal usada nos aplicativos do portal da empresa e no portal da Web</span><span class="sxs-lookup"><span data-stu-id="891bb-156">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="891bb-157">showLogo</span><span class="sxs-lookup"><span data-stu-id="891bb-157">showLogo</span></span>|<span data-ttu-id="891bb-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="891bb-158">Boolean</span></span>|<span data-ttu-id="891bb-159">Booliano que indica se as imagens de logotipo fornecidas pelo administrador são mostradas ou não</span><span class="sxs-lookup"><span data-stu-id="891bb-159">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="891bb-160">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="891bb-160">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="891bb-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="891bb-161">Boolean</span></span>|<span data-ttu-id="891bb-162">Booliano que indica se o nome de exibição fornecido pelo administrador será mostrado ao lado da imagem de logotipo ou não</span><span class="sxs-lookup"><span data-stu-id="891bb-162">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="891bb-163">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="891bb-163">themeColorLogo</span></span>|[<span data-ttu-id="891bb-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="891bb-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="891bb-165">Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo de cor de tema atrás do logotipo</span><span class="sxs-lookup"><span data-stu-id="891bb-165">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="891bb-166">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="891bb-166">lightBackgroundLogo</span></span>|[<span data-ttu-id="891bb-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="891bb-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="891bb-168">Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo claro atrás do logotipo</span><span class="sxs-lookup"><span data-stu-id="891bb-168">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="891bb-169">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="891bb-169">landingPageCustomizedImage</span></span>|[<span data-ttu-id="891bb-170">mimeContent</span><span class="sxs-lookup"><span data-stu-id="891bb-170">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="891bb-171">Imagem personalizada exibida na página inicial dos aplicativos do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="891bb-171">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="891bb-172">contactITName</span><span class="sxs-lookup"><span data-stu-id="891bb-172">contactITName</span></span>|<span data-ttu-id="891bb-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="891bb-173">String</span></span>|<span data-ttu-id="891bb-174">Nome da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="891bb-174">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="891bb-175">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="891bb-175">contactITPhoneNumber</span></span>|<span data-ttu-id="891bb-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="891bb-176">String</span></span>|<span data-ttu-id="891bb-177">Número de telefone da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="891bb-177">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="891bb-178">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="891bb-178">contactITEmailAddress</span></span>|<span data-ttu-id="891bb-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="891bb-179">String</span></span>|<span data-ttu-id="891bb-180">Endereço de email da pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="891bb-180">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="891bb-181">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="891bb-181">contactITNotes</span></span>|<span data-ttu-id="891bb-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="891bb-182">String</span></span>|<span data-ttu-id="891bb-183">Comentários de texto sobre a pessoa/organização responsável pelo suporte de ti</span><span class="sxs-lookup"><span data-stu-id="891bb-183">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="891bb-184">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="891bb-184">onlineSupportSiteUrl</span></span>|<span data-ttu-id="891bb-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="891bb-185">String</span></span>|<span data-ttu-id="891bb-186">URL para o site de assistência técnica de ti da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="891bb-186">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="891bb-187">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="891bb-187">onlineSupportSiteName</span></span>|<span data-ttu-id="891bb-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="891bb-188">String</span></span>|<span data-ttu-id="891bb-189">Nome para exibição do site de assistência técnica de ti da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="891bb-189">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="891bb-190">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="891bb-190">privacyUrl</span></span>|<span data-ttu-id="891bb-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="891bb-191">String</span></span>|<span data-ttu-id="891bb-192">URL para a política de privacidade da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="891bb-192">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="891bb-193">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="891bb-193">customPrivacyMessage</span></span>|<span data-ttu-id="891bb-194">String</span><span class="sxs-lookup"><span data-stu-id="891bb-194">String</span></span>|<span data-ttu-id="891bb-195">Comentários de texto sobre o que o administrador não tem acesso ao no dispositivo</span><span class="sxs-lookup"><span data-stu-id="891bb-195">Text comments regarding what the admin doesn't have access to on the device</span></span>|
|<span data-ttu-id="891bb-196">customCanSeePrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="891bb-196">customCanSeePrivacyMessage</span></span>|<span data-ttu-id="891bb-197">String</span><span class="sxs-lookup"><span data-stu-id="891bb-197">String</span></span>|<span data-ttu-id="891bb-198">Comentários de texto sobre o que o administrador tem acesso ao no dispositivo</span><span class="sxs-lookup"><span data-stu-id="891bb-198">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="891bb-199">customCantSeePrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="891bb-199">customCantSeePrivacyMessage</span></span>|<span data-ttu-id="891bb-200">String</span><span class="sxs-lookup"><span data-stu-id="891bb-200">String</span></span>|<span data-ttu-id="891bb-201">Comentários de texto sobre o que o administrador não tem acesso ao no dispositivo</span><span class="sxs-lookup"><span data-stu-id="891bb-201">Text comments regarding what the admin doesn't have access to on the device</span></span>|
|<span data-ttu-id="891bb-202">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="891bb-202">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="891bb-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="891bb-203">Boolean</span></span>|<span data-ttu-id="891bb-204">Booliano que indica se o adminsistrator desabilitou a ação "remover dispositivo" em dispositivos corporativos de propriedade.</span><span class="sxs-lookup"><span data-stu-id="891bb-204">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="891bb-205">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="891bb-205">isFactoryResetDisabled</span></span>|<span data-ttu-id="891bb-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="891bb-206">Boolean</span></span>|<span data-ttu-id="891bb-207">Booliano que indica se o adminsistrator desabilitou a ação "redefinição de fábrica" em dispositivos corporativos de propriedade.</span><span class="sxs-lookup"><span data-stu-id="891bb-207">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="891bb-208">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="891bb-208">companyPortalBlockedActions</span></span>|<span data-ttu-id="891bb-209">coleção [companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="891bb-209">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="891bb-210">Conjunto de ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo.</span><span class="sxs-lookup"><span data-stu-id="891bb-210">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="891bb-211">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="891bb-211">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="891bb-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="891bb-212">Boolean</span></span>|<span data-ttu-id="891bb-213">Booliano que indica se os aplicativos empresariais do AzureAD serão mostrados no portal da empresa</span><span class="sxs-lookup"><span data-stu-id="891bb-213">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="891bb-214">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="891bb-214">showOfficeWebApps</span></span>|<span data-ttu-id="891bb-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="891bb-215">Boolean</span></span>|<span data-ttu-id="891bb-216">Booliano que indica se o Office webapps será mostrado no portal da empresa</span><span class="sxs-lookup"><span data-stu-id="891bb-216">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="891bb-217">sendDeviceOwnershipChangePushNotification</span><span class="sxs-lookup"><span data-stu-id="891bb-217">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="891bb-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="891bb-218">Boolean</span></span>|<span data-ttu-id="891bb-219">Booliano que indica se uma notificação por push é enviada aos usuários quando o tipo de Propriedade do dispositivo muda de pessoal para corporativo</span><span class="sxs-lookup"><span data-stu-id="891bb-219">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="891bb-220">enrollmentAvailability</span><span class="sxs-lookup"><span data-stu-id="891bb-220">enrollmentAvailability</span></span>|[<span data-ttu-id="891bb-221">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="891bb-221">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="891bb-222">Fluxo de registro de dispositivo personalizado exibido para o usuário final.</span><span class="sxs-lookup"><span data-stu-id="891bb-222">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="891bb-223">Os valores possíveis são: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="891bb-223">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="891bb-224">disableClientTelemetry</span><span class="sxs-lookup"><span data-stu-id="891bb-224">disableClientTelemetry</span></span>|<span data-ttu-id="891bb-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="891bb-225">Boolean</span></span>|<span data-ttu-id="891bb-226">Aplica-se à telemetria enviada de todos os clientes para o serviço do Intune.</span><span class="sxs-lookup"><span data-stu-id="891bb-226">Applies to telemetry sent from all clients to the Intune service.</span></span> <span data-ttu-id="891bb-227">Quando desabilitado, todos os avisos proativos de solução de problemas e emissão dentro do cliente estão desativados, e as configurações de telemetria aparecem inativas ou ocultas para o usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="891bb-227">When disabled, all proactive troubleshooting and issue warnings within the client are turned off, and telemetry settings appear inactive or hidden to the device user.</span></span>|
|<span data-ttu-id="891bb-228">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="891bb-228">roleScopeTagIds</span></span>|<span data-ttu-id="891bb-229">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="891bb-229">String collection</span></span>|<span data-ttu-id="891bb-230">Lista de marcas de escopo atribuídas ao perfil de identidade visual</span><span class="sxs-lookup"><span data-stu-id="891bb-230">List of scope tags assigned to the branding profile</span></span>|



## <a name="response"></a><span data-ttu-id="891bb-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="891bb-231">Response</span></span>
<span data-ttu-id="891bb-232">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="891bb-232">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="891bb-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="891bb-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="891bb-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="891bb-234">Request</span></span>
<span data-ttu-id="891bb-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="891bb-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1975

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
  "customCanSeePrivacyMessage": "Custom Can See Privacy Message value",
  "customCantSeePrivacyMessage": "Custom Cant See Privacy Message value",
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
  "disableClientTelemetry": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="891bb-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="891bb-236">Response</span></span>
<span data-ttu-id="891bb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="891bb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2147

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
  "customCanSeePrivacyMessage": "Custom Can See Privacy Message value",
  "customCantSeePrivacyMessage": "Custom Cant See Privacy Message value",
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
  "disableClientTelemetry": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





