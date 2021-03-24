---
title: Criar intuneBrandingProfile
description: Crie um novo objeto intuneBrandingProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e6b8d89b2575402cc38b5f86ecd8a872fd666b3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133847"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="ecb18-103">Criar intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="ecb18-103">Create intuneBrandingProfile</span></span>

<span data-ttu-id="ecb18-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecb18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ecb18-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ecb18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecb18-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ecb18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecb18-107">Crie um novo [objeto intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ecb18-107">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecb18-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ecb18-108">Prerequisites</span></span>
<span data-ttu-id="ecb18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecb18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecb18-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecb18-111">Permission type</span></span>|<span data-ttu-id="ecb18-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ecb18-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecb18-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecb18-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ecb18-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecb18-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ecb18-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ecb18-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecb18-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecb18-116">Not supported.</span></span>|
|<span data-ttu-id="ecb18-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ecb18-117">Application</span></span>|<span data-ttu-id="ecb18-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecb18-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecb18-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecb18-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="ecb18-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecb18-120">Request headers</span></span>
|<span data-ttu-id="ecb18-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ecb18-121">Header</span></span>|<span data-ttu-id="ecb18-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ecb18-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecb18-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecb18-123">Authorization</span></span>|<span data-ttu-id="ecb18-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecb18-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecb18-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ecb18-125">Accept</span></span>|<span data-ttu-id="ecb18-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ecb18-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecb18-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecb18-127">Request body</span></span>
<span data-ttu-id="ecb18-128">No corpo da solicitação, fornece uma representação JSON para o objeto intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="ecb18-128">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="ecb18-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o intuneBrandingProfile.</span><span class="sxs-lookup"><span data-stu-id="ecb18-129">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="ecb18-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ecb18-130">Property</span></span>|<span data-ttu-id="ecb18-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecb18-131">Type</span></span>|<span data-ttu-id="ecb18-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecb18-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecb18-133">id</span><span class="sxs-lookup"><span data-stu-id="ecb18-133">id</span></span>|<span data-ttu-id="ecb18-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecb18-134">String</span></span>|<span data-ttu-id="ecb18-135">Chave de Perfil</span><span class="sxs-lookup"><span data-stu-id="ecb18-135">Profile Key</span></span>|
|<span data-ttu-id="ecb18-136">profileName</span><span class="sxs-lookup"><span data-stu-id="ecb18-136">profileName</span></span>|<span data-ttu-id="ecb18-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecb18-137">String</span></span>|<span data-ttu-id="ecb18-138">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="ecb18-138">Name of the profile</span></span>|
|<span data-ttu-id="ecb18-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="ecb18-139">profileDescription</span></span>|<span data-ttu-id="ecb18-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecb18-140">String</span></span>|<span data-ttu-id="ecb18-141">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="ecb18-141">Description of the profile</span></span>|
|<span data-ttu-id="ecb18-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="ecb18-142">isDefaultProfile</span></span>|<span data-ttu-id="ecb18-143">Booleano</span><span class="sxs-lookup"><span data-stu-id="ecb18-143">Boolean</span></span>|<span data-ttu-id="ecb18-144">Boolean que representa se o perfil é usado como padrão ou não</span><span class="sxs-lookup"><span data-stu-id="ecb18-144">Boolean that represents whether the profile is used as default or not</span></span>|
|<span data-ttu-id="ecb18-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ecb18-145">createdDateTime</span></span>|<span data-ttu-id="ecb18-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecb18-146">DateTimeOffset</span></span>|<span data-ttu-id="ecb18-147">Hora em que o BrandingProfile foi criado</span><span class="sxs-lookup"><span data-stu-id="ecb18-147">Time when the BrandingProfile was created</span></span>|
|<span data-ttu-id="ecb18-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ecb18-148">lastModifiedDateTime</span></span>|<span data-ttu-id="ecb18-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecb18-149">DateTimeOffset</span></span>|<span data-ttu-id="ecb18-150">Hora em que o BrandingProfile foi modificado pela última vez</span><span class="sxs-lookup"><span data-stu-id="ecb18-150">Time when the BrandingProfile was last modified</span></span>|
|<span data-ttu-id="ecb18-151">displayName</span><span class="sxs-lookup"><span data-stu-id="ecb18-151">displayName</span></span>|<span data-ttu-id="ecb18-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecb18-152">String</span></span>|<span data-ttu-id="ecb18-153">Nome da empresa/organização exibido para usuários finais</span><span class="sxs-lookup"><span data-stu-id="ecb18-153">Company/organization name that is displayed to end users</span></span>|
|<span data-ttu-id="ecb18-154">themeColor</span><span class="sxs-lookup"><span data-stu-id="ecb18-154">themeColor</span></span>|[<span data-ttu-id="ecb18-155">rgbColor</span><span class="sxs-lookup"><span data-stu-id="ecb18-155">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="ecb18-156">Cor de tema principal usada nos aplicativos do Portal da Empresa e no portal da Web</span><span class="sxs-lookup"><span data-stu-id="ecb18-156">Primary theme color used in the Company Portal applications and web portal</span></span>|
|<span data-ttu-id="ecb18-157">showLogo</span><span class="sxs-lookup"><span data-stu-id="ecb18-157">showLogo</span></span>|<span data-ttu-id="ecb18-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="ecb18-158">Boolean</span></span>|<span data-ttu-id="ecb18-159">Boolean que representa se as imagens de logotipo fornecidas pelo administrador são mostradas ou não</span><span class="sxs-lookup"><span data-stu-id="ecb18-159">Boolean that represents whether the administrator-supplied logo images are shown or not</span></span>|
|<span data-ttu-id="ecb18-160">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="ecb18-160">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="ecb18-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="ecb18-161">Boolean</span></span>|<span data-ttu-id="ecb18-162">Boolean que representa se o nome de exibição fornecido pelo administrador será mostrado ao lado da imagem de logotipo ou não</span><span class="sxs-lookup"><span data-stu-id="ecb18-162">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not</span></span>|
|<span data-ttu-id="ecb18-163">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="ecb18-163">themeColorLogo</span></span>|[<span data-ttu-id="ecb18-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ecb18-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ecb18-165">Imagem de logotipo exibida em aplicativos do Portal da Empresa que têm um plano de fundo de cor de tema atrás do logotipo</span><span class="sxs-lookup"><span data-stu-id="ecb18-165">Logo image displayed in Company Portal apps which have a theme color background behind the logo</span></span>|
|<span data-ttu-id="ecb18-166">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="ecb18-166">lightBackgroundLogo</span></span>|[<span data-ttu-id="ecb18-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ecb18-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ecb18-168">Imagem de logotipo exibida em aplicativos do Portal da Empresa que têm um plano de fundo claro atrás do logotipo</span><span class="sxs-lookup"><span data-stu-id="ecb18-168">Logo image displayed in Company Portal apps which have a light background behind the logo</span></span>|
|<span data-ttu-id="ecb18-169">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="ecb18-169">landingPageCustomizedImage</span></span>|[<span data-ttu-id="ecb18-170">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ecb18-170">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ecb18-171">Imagem personalizada exibida na página inicial de aplicativos do Portal da Empresa</span><span class="sxs-lookup"><span data-stu-id="ecb18-171">Customized image displayed in Company Portal apps landing page</span></span>|
|<span data-ttu-id="ecb18-172">contactITName</span><span class="sxs-lookup"><span data-stu-id="ecb18-172">contactITName</span></span>|<span data-ttu-id="ecb18-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecb18-173">String</span></span>|<span data-ttu-id="ecb18-174">Nome da pessoa/organização responsável pelo suporte a IT</span><span class="sxs-lookup"><span data-stu-id="ecb18-174">Name of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="ecb18-175">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="ecb18-175">contactITPhoneNumber</span></span>|<span data-ttu-id="ecb18-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecb18-176">String</span></span>|<span data-ttu-id="ecb18-177">Número de telefone da pessoa/organização responsável pelo suporte a IT</span><span class="sxs-lookup"><span data-stu-id="ecb18-177">Phone number of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="ecb18-178">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="ecb18-178">contactITEmailAddress</span></span>|<span data-ttu-id="ecb18-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecb18-179">String</span></span>|<span data-ttu-id="ecb18-180">Endereço de email da pessoa/organização responsável pelo suporte a IT</span><span class="sxs-lookup"><span data-stu-id="ecb18-180">E-mail address of the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="ecb18-181">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="ecb18-181">contactITNotes</span></span>|<span data-ttu-id="ecb18-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecb18-182">String</span></span>|<span data-ttu-id="ecb18-183">Comentários de texto sobre a pessoa/organização responsável pelo suporte a IT</span><span class="sxs-lookup"><span data-stu-id="ecb18-183">Text comments regarding the person/organization responsible for IT support</span></span>|
|<span data-ttu-id="ecb18-184">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="ecb18-184">onlineSupportSiteUrl</span></span>|<span data-ttu-id="ecb18-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecb18-185">String</span></span>|<span data-ttu-id="ecb18-186">URL para o site de ajuda de IT da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="ecb18-186">URL to the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="ecb18-187">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="ecb18-187">onlineSupportSiteName</span></span>|<span data-ttu-id="ecb18-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecb18-188">String</span></span>|<span data-ttu-id="ecb18-189">Nome de exibição do site de ajuda de IT da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="ecb18-189">Display name of the company/organization’s IT helpdesk site</span></span>|
|<span data-ttu-id="ecb18-190">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="ecb18-190">privacyUrl</span></span>|<span data-ttu-id="ecb18-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecb18-191">String</span></span>|<span data-ttu-id="ecb18-192">URL para a política de privacidade da empresa/organização</span><span class="sxs-lookup"><span data-stu-id="ecb18-192">URL to the company/organization’s privacy policy</span></span>|
|<span data-ttu-id="ecb18-193">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="ecb18-193">customPrivacyMessage</span></span>|<span data-ttu-id="ecb18-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecb18-194">String</span></span>|<span data-ttu-id="ecb18-195">Comentários de texto sobre o que o administrador não tem acesso no dispositivo</span><span class="sxs-lookup"><span data-stu-id="ecb18-195">Text comments regarding what the admin doesn't have access to on the device</span></span>|
|<span data-ttu-id="ecb18-196">customCanSeePrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="ecb18-196">customCanSeePrivacyMessage</span></span>|<span data-ttu-id="ecb18-197">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecb18-197">String</span></span>|<span data-ttu-id="ecb18-198">Comentários de texto sobre o que o administrador tem acesso no dispositivo</span><span class="sxs-lookup"><span data-stu-id="ecb18-198">Text comments regarding what the admin has access to on the device</span></span>|
|<span data-ttu-id="ecb18-199">customCantSeePrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="ecb18-199">customCantSeePrivacyMessage</span></span>|<span data-ttu-id="ecb18-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecb18-200">String</span></span>|<span data-ttu-id="ecb18-201">Comentários de texto sobre o que o administrador não tem acesso no dispositivo</span><span class="sxs-lookup"><span data-stu-id="ecb18-201">Text comments regarding what the admin doesn't have access to on the device</span></span>|
|<span data-ttu-id="ecb18-202">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="ecb18-202">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="ecb18-203">Booleano</span><span class="sxs-lookup"><span data-stu-id="ecb18-203">Boolean</span></span>|<span data-ttu-id="ecb18-204">Boolean que representa se o administrador desabilitou a ação "Remover Dispositivo" em dispositivos de propriedade corporativa.</span><span class="sxs-lookup"><span data-stu-id="ecb18-204">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="ecb18-205">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="ecb18-205">isFactoryResetDisabled</span></span>|<span data-ttu-id="ecb18-206">Booleano</span><span class="sxs-lookup"><span data-stu-id="ecb18-206">Boolean</span></span>|<span data-ttu-id="ecb18-207">Boolean que representa se o administrador desabilitou a ação 'Redefinição de Fábrica' em dispositivos de propriedade corporativa.</span><span class="sxs-lookup"><span data-stu-id="ecb18-207">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="ecb18-208">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="ecb18-208">companyPortalBlockedActions</span></span>|<span data-ttu-id="ecb18-209">[Coleção companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="ecb18-209">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="ecb18-210">Coleção de ações bloqueadas no portal da empresa de acordo com os tipos de propriedade da plataforma e do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ecb18-210">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="ecb18-211">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="ecb18-211">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="ecb18-212">Booleano</span><span class="sxs-lookup"><span data-stu-id="ecb18-212">Boolean</span></span>|<span data-ttu-id="ecb18-213">Boolean que indica se os aplicativos corporativos do AzureAD serão mostrados no Portal da Empresa</span><span class="sxs-lookup"><span data-stu-id="ecb18-213">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="ecb18-214">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="ecb18-214">showOfficeWebApps</span></span>|<span data-ttu-id="ecb18-215">Booleano</span><span class="sxs-lookup"><span data-stu-id="ecb18-215">Boolean</span></span>|<span data-ttu-id="ecb18-216">Boolean que indica se o Office WebApps será mostrado no Portal da Empresa</span><span class="sxs-lookup"><span data-stu-id="ecb18-216">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="ecb18-217">sendDeviceOwnershipChangePushNotification</span><span class="sxs-lookup"><span data-stu-id="ecb18-217">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="ecb18-218">Booleano</span><span class="sxs-lookup"><span data-stu-id="ecb18-218">Boolean</span></span>|<span data-ttu-id="ecb18-219">Boolean que indica se uma notificação por push é enviada aos usuários quando o tipo de propriedade do dispositivo muda de pessoal para corporativo</span><span class="sxs-lookup"><span data-stu-id="ecb18-219">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="ecb18-220">enrollmentAvailability</span><span class="sxs-lookup"><span data-stu-id="ecb18-220">enrollmentAvailability</span></span>|[<span data-ttu-id="ecb18-221">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="ecb18-221">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="ecb18-222">Fluxo de registro de dispositivo personalizado exibido para o usuário final .</span><span class="sxs-lookup"><span data-stu-id="ecb18-222">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="ecb18-223">Os valores possíveis são: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="ecb18-223">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="ecb18-224">disableClientTelemetry</span><span class="sxs-lookup"><span data-stu-id="ecb18-224">disableClientTelemetry</span></span>|<span data-ttu-id="ecb18-225">Booleano</span><span class="sxs-lookup"><span data-stu-id="ecb18-225">Boolean</span></span>|<span data-ttu-id="ecb18-226">Aplica-se à telemetria enviada de todos os clientes para o serviço do Intune.</span><span class="sxs-lookup"><span data-stu-id="ecb18-226">Applies to telemetry sent from all clients to the Intune service.</span></span> <span data-ttu-id="ecb18-227">Quando desabilitado, todos os avisos de solução de problemas e problemas proativos dentro do cliente são desativados, e as configurações de telemetria aparecem inativas ou ocultas para o usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ecb18-227">When disabled, all proactive troubleshooting and issue warnings within the client are turned off, and telemetry settings appear inactive or hidden to the device user.</span></span>|
|<span data-ttu-id="ecb18-228">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ecb18-228">roleScopeTagIds</span></span>|<span data-ttu-id="ecb18-229">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecb18-229">String collection</span></span>|<span data-ttu-id="ecb18-230">Lista de marcas de escopo atribuídas ao perfil de identidade visual</span><span class="sxs-lookup"><span data-stu-id="ecb18-230">List of scope tags assigned to the branding profile</span></span>|



## <a name="response"></a><span data-ttu-id="ecb18-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecb18-231">Response</span></span>
<span data-ttu-id="ecb18-232">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ecb18-232">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecb18-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecb18-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecb18-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecb18-234">Request</span></span>
<span data-ttu-id="ecb18-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecb18-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ecb18-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecb18-236">Response</span></span>
<span data-ttu-id="ecb18-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ecb18-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




