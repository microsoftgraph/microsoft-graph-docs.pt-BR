---
title: Tipo de recurso intuneBrand
description: intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 92b706fee0e1b0a6af0d877d040339416d9b78c4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455571"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="df5a0-103">Tipo de recurso intuneBrand</span><span class="sxs-lookup"><span data-stu-id="df5a0-103">intuneBrand resource type</span></span>

<span data-ttu-id="df5a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df5a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df5a0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="df5a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df5a0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df5a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df5a0-107">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="df5a0-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="df5a0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df5a0-108">Properties</span></span>
|<span data-ttu-id="df5a0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df5a0-109">Property</span></span>|<span data-ttu-id="df5a0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="df5a0-110">Type</span></span>|<span data-ttu-id="df5a0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="df5a0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df5a0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="df5a0-112">displayName</span></span>|<span data-ttu-id="df5a0-113">String</span><span class="sxs-lookup"><span data-stu-id="df5a0-113">String</span></span>|<span data-ttu-id="df5a0-114">Nome da empresa/organização exibido para usuários finais.</span><span class="sxs-lookup"><span data-stu-id="df5a0-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="df5a0-115">themeColor</span><span class="sxs-lookup"><span data-stu-id="df5a0-115">themeColor</span></span>|[<span data-ttu-id="df5a0-116">rgbColor</span><span class="sxs-lookup"><span data-stu-id="df5a0-116">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="df5a0-117">Cor de tema principal usado nos aplicativos e no portal da Web do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="df5a0-117">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="df5a0-118">showLogo</span><span class="sxs-lookup"><span data-stu-id="df5a0-118">showLogo</span></span>|<span data-ttu-id="df5a0-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="df5a0-119">Boolean</span></span>|<span data-ttu-id="df5a0-120">Booliano que indica se as imagens de logotipo fornecidas pelo administrador serão exibidas ou não.</span><span class="sxs-lookup"><span data-stu-id="df5a0-120">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="df5a0-121">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="df5a0-121">lightBackgroundLogo</span></span>|[<span data-ttu-id="df5a0-122">mimeContent</span><span class="sxs-lookup"><span data-stu-id="df5a0-122">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="df5a0-123">Imagem do logotipo exibida nos aplicativos do Portal da Empresa que têm um plano de fundo claro atrás do logotipo.</span><span class="sxs-lookup"><span data-stu-id="df5a0-123">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="df5a0-124">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="df5a0-124">darkBackgroundLogo</span></span>|[<span data-ttu-id="df5a0-125">mimeContent</span><span class="sxs-lookup"><span data-stu-id="df5a0-125">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="df5a0-126">Imagem do logotipo exibida nos aplicativos do Portal da Empresa que têm um plano de fundo escuro atrás do logotipo.</span><span class="sxs-lookup"><span data-stu-id="df5a0-126">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="df5a0-127">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="df5a0-127">showNameNextToLogo</span></span>|<span data-ttu-id="df5a0-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="df5a0-128">Boolean</span></span>|<span data-ttu-id="df5a0-129">Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.</span><span class="sxs-lookup"><span data-stu-id="df5a0-129">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="df5a0-130">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="df5a0-130">landingPageCustomizedImage</span></span>|[<span data-ttu-id="df5a0-131">mimeContent</span><span class="sxs-lookup"><span data-stu-id="df5a0-131">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="df5a0-132">Imagem personalizada exibida na página inicial do aplicativo do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="df5a0-132">Customized image displayed in Company Portal app landing page</span></span>|
|<span data-ttu-id="df5a0-133">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="df5a0-133">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="df5a0-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="df5a0-134">Boolean</span></span>|<span data-ttu-id="df5a0-135">Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.</span><span class="sxs-lookup"><span data-stu-id="df5a0-135">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="df5a0-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="df5a0-136">roleScopeTagIds</span></span>|<span data-ttu-id="df5a0-137">Coleção String</span><span class="sxs-lookup"><span data-stu-id="df5a0-137">String collection</span></span>|<span data-ttu-id="df5a0-138">Lista de marcas de escopo atribuídas ao perfil de identidade visual padrão</span><span class="sxs-lookup"><span data-stu-id="df5a0-138">List of scope tags assigned to the default branding profile</span></span>|
|<span data-ttu-id="df5a0-139">contactITName</span><span class="sxs-lookup"><span data-stu-id="df5a0-139">contactITName</span></span>|<span data-ttu-id="df5a0-140">String</span><span class="sxs-lookup"><span data-stu-id="df5a0-140">String</span></span>|<span data-ttu-id="df5a0-141">Nome da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="df5a0-141">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="df5a0-142">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="df5a0-142">contactITPhoneNumber</span></span>|<span data-ttu-id="df5a0-143">String</span><span class="sxs-lookup"><span data-stu-id="df5a0-143">String</span></span>|<span data-ttu-id="df5a0-144">Número de telefone da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="df5a0-144">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="df5a0-145">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="df5a0-145">contactITEmailAddress</span></span>|<span data-ttu-id="df5a0-146">String</span><span class="sxs-lookup"><span data-stu-id="df5a0-146">String</span></span>|<span data-ttu-id="df5a0-147">Endereço de email da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="df5a0-147">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="df5a0-148">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="df5a0-148">contactITNotes</span></span>|<span data-ttu-id="df5a0-149">String</span><span class="sxs-lookup"><span data-stu-id="df5a0-149">String</span></span>|<span data-ttu-id="df5a0-150">Comentários de texto relacionados à pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="df5a0-150">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="df5a0-151">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="df5a0-151">onlineSupportSiteUrl</span></span>|<span data-ttu-id="df5a0-152">String</span><span class="sxs-lookup"><span data-stu-id="df5a0-152">String</span></span>|<span data-ttu-id="df5a0-153">URL do site de assistência técnica de TI da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="df5a0-153">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="df5a0-154">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="df5a0-154">onlineSupportSiteName</span></span>|<span data-ttu-id="df5a0-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df5a0-155">String</span></span>|<span data-ttu-id="df5a0-156">Nome de exibição do site de assistência técnica de TI da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="df5a0-156">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="df5a0-157">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="df5a0-157">privacyUrl</span></span>|<span data-ttu-id="df5a0-158">String</span><span class="sxs-lookup"><span data-stu-id="df5a0-158">String</span></span>|<span data-ttu-id="df5a0-159">URL da política de privacidade da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="df5a0-159">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="df5a0-160">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="df5a0-160">customPrivacyMessage</span></span>|<span data-ttu-id="df5a0-161">String</span><span class="sxs-lookup"><span data-stu-id="df5a0-161">String</span></span>|<span data-ttu-id="df5a0-162">Mensagem de privacidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="df5a0-162">Custom privacy message.</span></span>|
|<span data-ttu-id="df5a0-163">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="df5a0-163">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="df5a0-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="df5a0-164">Boolean</span></span>|<span data-ttu-id="df5a0-165">Booliano que indica se o adminsistrator desabilitou a ação "remover dispositivo" em dispositivos corporativos de propriedade.</span><span class="sxs-lookup"><span data-stu-id="df5a0-165">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="df5a0-166">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="df5a0-166">isFactoryResetDisabled</span></span>|<span data-ttu-id="df5a0-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="df5a0-167">Boolean</span></span>|<span data-ttu-id="df5a0-168">Booliano que indica se o adminsistrator desabilitou a ação "redefinição de fábrica" em dispositivos corporativos de propriedade.</span><span class="sxs-lookup"><span data-stu-id="df5a0-168">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="df5a0-169">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="df5a0-169">companyPortalBlockedActions</span></span>|<span data-ttu-id="df5a0-170">coleção [companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="df5a0-170">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="df5a0-171">Conjunto de ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo.</span><span class="sxs-lookup"><span data-stu-id="df5a0-171">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="df5a0-172">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="df5a0-172">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="df5a0-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="df5a0-173">Boolean</span></span>|<span data-ttu-id="df5a0-174">Booliano que indica se os aplicativos empresariais do AzureAD serão mostrados no portal da empresa</span><span class="sxs-lookup"><span data-stu-id="df5a0-174">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="df5a0-175">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="df5a0-175">showOfficeWebApps</span></span>|<span data-ttu-id="df5a0-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="df5a0-176">Boolean</span></span>|<span data-ttu-id="df5a0-177">Booliano que indica se o Office webapps será mostrado no portal da empresa</span><span class="sxs-lookup"><span data-stu-id="df5a0-177">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="df5a0-178">sendDeviceOwnershipChangePushNotification</span><span class="sxs-lookup"><span data-stu-id="df5a0-178">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="df5a0-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="df5a0-179">Boolean</span></span>|<span data-ttu-id="df5a0-180">Booliano que indica se uma notificação por push é enviada aos usuários quando o tipo de Propriedade do dispositivo muda de pessoal para corporativo</span><span class="sxs-lookup"><span data-stu-id="df5a0-180">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="df5a0-181">enrollmentAvailability</span><span class="sxs-lookup"><span data-stu-id="df5a0-181">enrollmentAvailability</span></span>|[<span data-ttu-id="df5a0-182">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="df5a0-182">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="df5a0-183">Fluxo de registro de dispositivo personalizado exibido para o usuário final.</span><span class="sxs-lookup"><span data-stu-id="df5a0-183">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="df5a0-184">Os valores possíveis são: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span><span class="sxs-lookup"><span data-stu-id="df5a0-184">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df5a0-185">Relações</span><span class="sxs-lookup"><span data-stu-id="df5a0-185">Relationships</span></span>
<span data-ttu-id="df5a0-186">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df5a0-186">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df5a0-187">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df5a0-187">JSON Representation</span></span>
<span data-ttu-id="df5a0-188">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df5a0-188">Here is a JSON representation of the resource.</span></span>
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
  "enrollmentAvailability": "String"
}
```



