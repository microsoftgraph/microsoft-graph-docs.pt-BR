---
title: Tipo de recurso intuneBrand
description: intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4550fa46df5db366342495491f1e4207f1a1bffc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029488"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="1a3ba-103">Tipo de recurso intuneBrand</span><span class="sxs-lookup"><span data-stu-id="1a3ba-103">intuneBrand resource type</span></span>

<span data-ttu-id="1a3ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a3ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a3ba-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a3ba-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a3ba-107">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="1a3ba-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a3ba-108">Properties</span></span>
|<span data-ttu-id="1a3ba-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a3ba-109">Property</span></span>|<span data-ttu-id="1a3ba-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a3ba-110">Type</span></span>|<span data-ttu-id="1a3ba-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a3ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a3ba-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1a3ba-112">displayName</span></span>|<span data-ttu-id="1a3ba-113">String</span><span class="sxs-lookup"><span data-stu-id="1a3ba-113">String</span></span>|<span data-ttu-id="1a3ba-114">Nome da empresa/organização exibido para usuários finais.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="1a3ba-115">themeColor</span><span class="sxs-lookup"><span data-stu-id="1a3ba-115">themeColor</span></span>|[<span data-ttu-id="1a3ba-116">rgbColor</span><span class="sxs-lookup"><span data-stu-id="1a3ba-116">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="1a3ba-117">Cor de tema principal usado nos aplicativos e no portal da Web do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-117">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="1a3ba-118">showLogo</span><span class="sxs-lookup"><span data-stu-id="1a3ba-118">showLogo</span></span>|<span data-ttu-id="1a3ba-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a3ba-119">Boolean</span></span>|<span data-ttu-id="1a3ba-120">Booliano que indica se as imagens de logotipo fornecidas pelo administrador serão exibidas ou não.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-120">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="1a3ba-121">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="1a3ba-121">lightBackgroundLogo</span></span>|[<span data-ttu-id="1a3ba-122">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1a3ba-122">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1a3ba-123">Imagem do logotipo exibida nos aplicativos do Portal da Empresa que têm um plano de fundo claro atrás do logotipo.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-123">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="1a3ba-124">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="1a3ba-124">darkBackgroundLogo</span></span>|[<span data-ttu-id="1a3ba-125">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1a3ba-125">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1a3ba-126">Imagem do logotipo exibida nos aplicativos do Portal da Empresa que têm um plano de fundo escuro atrás do logotipo.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-126">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="1a3ba-127">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="1a3ba-127">showNameNextToLogo</span></span>|<span data-ttu-id="1a3ba-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a3ba-128">Boolean</span></span>|<span data-ttu-id="1a3ba-129">Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-129">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="1a3ba-130">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="1a3ba-130">landingPageCustomizedImage</span></span>|[<span data-ttu-id="1a3ba-131">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1a3ba-131">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1a3ba-132">Imagem personalizada exibida na página inicial do aplicativo do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="1a3ba-132">Customized image displayed in Company Portal app landing page</span></span>|
|<span data-ttu-id="1a3ba-133">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="1a3ba-133">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="1a3ba-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a3ba-134">Boolean</span></span>|<span data-ttu-id="1a3ba-135">Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-135">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="1a3ba-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1a3ba-136">roleScopeTagIds</span></span>|<span data-ttu-id="1a3ba-137">Coleção String</span><span class="sxs-lookup"><span data-stu-id="1a3ba-137">String collection</span></span>|<span data-ttu-id="1a3ba-138">Lista de marcas de escopo atribuídas ao perfil de identidade visual padrão</span><span class="sxs-lookup"><span data-stu-id="1a3ba-138">List of scope tags assigned to the default branding profile</span></span>|
|<span data-ttu-id="1a3ba-139">contactITName</span><span class="sxs-lookup"><span data-stu-id="1a3ba-139">contactITName</span></span>|<span data-ttu-id="1a3ba-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a3ba-140">String</span></span>|<span data-ttu-id="1a3ba-141">Nome da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-141">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="1a3ba-142">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="1a3ba-142">contactITPhoneNumber</span></span>|<span data-ttu-id="1a3ba-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a3ba-143">String</span></span>|<span data-ttu-id="1a3ba-144">Número de telefone da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-144">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="1a3ba-145">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="1a3ba-145">contactITEmailAddress</span></span>|<span data-ttu-id="1a3ba-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a3ba-146">String</span></span>|<span data-ttu-id="1a3ba-147">Endereço de email da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-147">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="1a3ba-148">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="1a3ba-148">contactITNotes</span></span>|<span data-ttu-id="1a3ba-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a3ba-149">String</span></span>|<span data-ttu-id="1a3ba-150">Comentários de texto relacionados à pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-150">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="1a3ba-151">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="1a3ba-151">onlineSupportSiteUrl</span></span>|<span data-ttu-id="1a3ba-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a3ba-152">String</span></span>|<span data-ttu-id="1a3ba-153">URL do site de assistência técnica de TI da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-153">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="1a3ba-154">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="1a3ba-154">onlineSupportSiteName</span></span>|<span data-ttu-id="1a3ba-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a3ba-155">String</span></span>|<span data-ttu-id="1a3ba-156">Nome de exibição do site de assistência técnica de TI da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-156">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="1a3ba-157">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="1a3ba-157">privacyUrl</span></span>|<span data-ttu-id="1a3ba-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a3ba-158">String</span></span>|<span data-ttu-id="1a3ba-159">URL da política de privacidade da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-159">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="1a3ba-160">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="1a3ba-160">customPrivacyMessage</span></span>|<span data-ttu-id="1a3ba-161">String</span><span class="sxs-lookup"><span data-stu-id="1a3ba-161">String</span></span>|<span data-ttu-id="1a3ba-162">A mensagem de privacidade personalizada usada para explicar o que a organização não pode ver ou fazer em dispositivos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-162">The custom privacy message used to explain what the organization can’t see or do on managed devices.</span></span>|
|<span data-ttu-id="1a3ba-163">customCantSeePrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="1a3ba-163">customCantSeePrivacyMessage</span></span>|<span data-ttu-id="1a3ba-164">String</span><span class="sxs-lookup"><span data-stu-id="1a3ba-164">String</span></span>|<span data-ttu-id="1a3ba-165">A mensagem de privacidade personalizada usada para explicar o que a organização não pode ver ou fazer em dispositivos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-165">The custom privacy message used to explain what the organization can’t see or do on managed devices.</span></span>|
|<span data-ttu-id="1a3ba-166">customCanSeePrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="1a3ba-166">customCanSeePrivacyMessage</span></span>|<span data-ttu-id="1a3ba-167">String</span><span class="sxs-lookup"><span data-stu-id="1a3ba-167">String</span></span>|<span data-ttu-id="1a3ba-168">A mensagem de privacidade personalizada usada para explicar o que a organização pode ver e fazer em dispositivos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-168">The custom privacy message used to explain what the organization can see and do on managed devices.</span></span>|
|<span data-ttu-id="1a3ba-169">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="1a3ba-169">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="1a3ba-170">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a3ba-170">Boolean</span></span>|<span data-ttu-id="1a3ba-171">Booliano que indica se o adminsistrator desabilitou a ação "remover dispositivo" em dispositivos corporativos de propriedade.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-171">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="1a3ba-172">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="1a3ba-172">isFactoryResetDisabled</span></span>|<span data-ttu-id="1a3ba-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a3ba-173">Boolean</span></span>|<span data-ttu-id="1a3ba-174">Booliano que indica se o adminsistrator desabilitou a ação "redefinição de fábrica" em dispositivos corporativos de propriedade.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-174">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="1a3ba-175">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="1a3ba-175">companyPortalBlockedActions</span></span>|<span data-ttu-id="1a3ba-176">coleção [companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="1a3ba-176">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="1a3ba-177">Conjunto de ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-177">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="1a3ba-178">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="1a3ba-178">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="1a3ba-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a3ba-179">Boolean</span></span>|<span data-ttu-id="1a3ba-180">Booliano que indica se os aplicativos empresariais do AzureAD serão mostrados no portal da empresa</span><span class="sxs-lookup"><span data-stu-id="1a3ba-180">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="1a3ba-181">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="1a3ba-181">showOfficeWebApps</span></span>|<span data-ttu-id="1a3ba-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a3ba-182">Boolean</span></span>|<span data-ttu-id="1a3ba-183">Booliano que indica se o Office webapps será mostrado no portal da empresa</span><span class="sxs-lookup"><span data-stu-id="1a3ba-183">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="1a3ba-184">sendDeviceOwnershipChangePushNotification</span><span class="sxs-lookup"><span data-stu-id="1a3ba-184">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="1a3ba-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a3ba-185">Boolean</span></span>|<span data-ttu-id="1a3ba-186">Booliano que indica se uma notificação por push é enviada aos usuários quando o tipo de Propriedade do dispositivo muda de pessoal para corporativo</span><span class="sxs-lookup"><span data-stu-id="1a3ba-186">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="1a3ba-187">enrollmentAvailability</span><span class="sxs-lookup"><span data-stu-id="1a3ba-187">enrollmentAvailability</span></span>|[<span data-ttu-id="1a3ba-188">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="1a3ba-188">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="1a3ba-189">Fluxo de registro de dispositivo personalizado exibido para o usuário final.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-189">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="1a3ba-190">Os valores possíveis são: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-190">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="1a3ba-191">disableClientTelemetry</span><span class="sxs-lookup"><span data-stu-id="1a3ba-191">disableClientTelemetry</span></span>|<span data-ttu-id="1a3ba-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a3ba-192">Boolean</span></span>|<span data-ttu-id="1a3ba-193">Aplica-se à telemetria enviada de todos os clientes para o serviço do Intune.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-193">Applies to telemetry sent from all clients to the Intune service.</span></span> <span data-ttu-id="1a3ba-194">Quando desabilitado, todos os avisos proativos de solução de problemas e emissão dentro do cliente estão desativados, e as configurações de telemetria aparecem inativas ou ocultas para o usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-194">When disabled, all proactive troubleshooting and issue warnings within the client are turned off, and telemetry settings appear inactive or hidden to the device user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a3ba-195">Relações</span><span class="sxs-lookup"><span data-stu-id="1a3ba-195">Relationships</span></span>
<span data-ttu-id="1a3ba-196">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a3ba-196">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a3ba-197">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a3ba-197">JSON Representation</span></span>
<span data-ttu-id="1a3ba-198">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a3ba-198">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showNameNextToLogo": true,
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showDisplayNameNextToLogo": true,
  "roleScopeTagIds": [
    "String"
  ],
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "privacyUrl": "String",
  "customPrivacyMessage": "String",
  "customCantSeePrivacyMessage": "String",
  "customCanSeePrivacyMessage": "String",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "String",
      "ownerType": "String",
      "action": "String"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "String",
  "disableClientTelemetry": true
}
```






