---
title: Tipo de recurso intuneBrand
description: intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 478f087b4a7998a8c90bd429e0a0d3173d9b8e3c
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088032"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="9ea12-103">Tipo de recurso intuneBrand</span><span class="sxs-lookup"><span data-stu-id="9ea12-103">intuneBrand resource type</span></span>

> <span data-ttu-id="9ea12-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ea12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ea12-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ea12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ea12-106">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="9ea12-106">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="9ea12-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ea12-107">Properties</span></span>
|<span data-ttu-id="9ea12-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ea12-108">Property</span></span>|<span data-ttu-id="9ea12-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ea12-109">Type</span></span>|<span data-ttu-id="9ea12-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ea12-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ea12-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9ea12-111">displayName</span></span>|<span data-ttu-id="9ea12-112">String</span><span class="sxs-lookup"><span data-stu-id="9ea12-112">String</span></span>|<span data-ttu-id="9ea12-113">Nome da empresa/organização exibido para usuários finais.</span><span class="sxs-lookup"><span data-stu-id="9ea12-113">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="9ea12-114">themeColor</span><span class="sxs-lookup"><span data-stu-id="9ea12-114">themeColor</span></span>|[<span data-ttu-id="9ea12-115">rgbColor</span><span class="sxs-lookup"><span data-stu-id="9ea12-115">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="9ea12-116">Cor de tema principal usado nos aplicativos e no portal da Web do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="9ea12-116">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="9ea12-117">showLogo</span><span class="sxs-lookup"><span data-stu-id="9ea12-117">showLogo</span></span>|<span data-ttu-id="9ea12-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ea12-118">Boolean</span></span>|<span data-ttu-id="9ea12-119">Booliano que indica se as imagens de logotipo fornecidas pelo administrador serão exibidas ou não.</span><span class="sxs-lookup"><span data-stu-id="9ea12-119">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="9ea12-120">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="9ea12-120">lightBackgroundLogo</span></span>|[<span data-ttu-id="9ea12-121">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9ea12-121">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9ea12-122">Imagem do logotipo exibida nos aplicativos do Portal da Empresa que têm um plano de fundo claro atrás do logotipo.</span><span class="sxs-lookup"><span data-stu-id="9ea12-122">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="9ea12-123">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="9ea12-123">darkBackgroundLogo</span></span>|[<span data-ttu-id="9ea12-124">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9ea12-124">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9ea12-125">Imagem do logotipo exibida nos aplicativos do Portal da Empresa que têm um plano de fundo escuro atrás do logotipo.</span><span class="sxs-lookup"><span data-stu-id="9ea12-125">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="9ea12-126">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="9ea12-126">showNameNextToLogo</span></span>|<span data-ttu-id="9ea12-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ea12-127">Boolean</span></span>|<span data-ttu-id="9ea12-128">Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.</span><span class="sxs-lookup"><span data-stu-id="9ea12-128">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="9ea12-129">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="9ea12-129">landingPageCustomizedImage</span></span>|[<span data-ttu-id="9ea12-130">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9ea12-130">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9ea12-131">Imagem personalizada exibida na página inicial do aplicativo do portal da empresa</span><span class="sxs-lookup"><span data-stu-id="9ea12-131">Customized image displayed in Company Portal app landing page</span></span>|
|<span data-ttu-id="9ea12-132">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="9ea12-132">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="9ea12-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ea12-133">Boolean</span></span>|<span data-ttu-id="9ea12-134">Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.</span><span class="sxs-lookup"><span data-stu-id="9ea12-134">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="9ea12-135">contactITName</span><span class="sxs-lookup"><span data-stu-id="9ea12-135">contactITName</span></span>|<span data-ttu-id="9ea12-136">String</span><span class="sxs-lookup"><span data-stu-id="9ea12-136">String</span></span>|<span data-ttu-id="9ea12-137">Nome da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="9ea12-137">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="9ea12-138">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="9ea12-138">contactITPhoneNumber</span></span>|<span data-ttu-id="9ea12-139">String</span><span class="sxs-lookup"><span data-stu-id="9ea12-139">String</span></span>|<span data-ttu-id="9ea12-140">Número de telefone da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="9ea12-140">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="9ea12-141">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="9ea12-141">contactITEmailAddress</span></span>|<span data-ttu-id="9ea12-142">String</span><span class="sxs-lookup"><span data-stu-id="9ea12-142">String</span></span>|<span data-ttu-id="9ea12-143">Endereço de email da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="9ea12-143">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="9ea12-144">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="9ea12-144">contactITNotes</span></span>|<span data-ttu-id="9ea12-145">String</span><span class="sxs-lookup"><span data-stu-id="9ea12-145">String</span></span>|<span data-ttu-id="9ea12-146">Comentários de texto relacionados à pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="9ea12-146">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="9ea12-147">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="9ea12-147">onlineSupportSiteUrl</span></span>|<span data-ttu-id="9ea12-148">String</span><span class="sxs-lookup"><span data-stu-id="9ea12-148">String</span></span>|<span data-ttu-id="9ea12-149">URL do site de assistência técnica de TI da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="9ea12-149">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="9ea12-150">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="9ea12-150">onlineSupportSiteName</span></span>|<span data-ttu-id="9ea12-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ea12-151">String</span></span>|<span data-ttu-id="9ea12-152">Nome de exibição do site de assistência técnica de TI da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="9ea12-152">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="9ea12-153">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="9ea12-153">privacyUrl</span></span>|<span data-ttu-id="9ea12-154">String</span><span class="sxs-lookup"><span data-stu-id="9ea12-154">String</span></span>|<span data-ttu-id="9ea12-155">URL da política de privacidade da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="9ea12-155">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="9ea12-156">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="9ea12-156">customPrivacyMessage</span></span>|<span data-ttu-id="9ea12-157">String</span><span class="sxs-lookup"><span data-stu-id="9ea12-157">String</span></span>|<span data-ttu-id="9ea12-158">Mensagem de privacidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="9ea12-158">Custom privacy message.</span></span>|
|<span data-ttu-id="9ea12-159">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="9ea12-159">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="9ea12-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ea12-160">Boolean</span></span>|<span data-ttu-id="9ea12-161">Booliano que indica se o adminsistrator desabilitou a ação "remover dispositivo" em dispositivos corporativos de propriedade.</span><span class="sxs-lookup"><span data-stu-id="9ea12-161">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="9ea12-162">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="9ea12-162">isFactoryResetDisabled</span></span>|<span data-ttu-id="9ea12-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ea12-163">Boolean</span></span>|<span data-ttu-id="9ea12-164">Booliano que indica se o adminsistrator desabilitou a ação "redefinição de fábrica" em dispositivos corporativos de propriedade.</span><span class="sxs-lookup"><span data-stu-id="9ea12-164">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="9ea12-165">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="9ea12-165">companyPortalBlockedActions</span></span>|<span data-ttu-id="9ea12-166">coleção [companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)</span><span class="sxs-lookup"><span data-stu-id="9ea12-166">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="9ea12-167">Conjunto de ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ea12-167">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="9ea12-168">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="9ea12-168">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="9ea12-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ea12-169">Boolean</span></span>|<span data-ttu-id="9ea12-170">Booliano que indica se os aplicativos empresariais do AzureAD serão mostrados no portal da empresa</span><span class="sxs-lookup"><span data-stu-id="9ea12-170">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="9ea12-171">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="9ea12-171">showOfficeWebApps</span></span>|<span data-ttu-id="9ea12-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ea12-172">Boolean</span></span>|<span data-ttu-id="9ea12-173">Booliano que indica se o Office webapps será mostrado no portal da empresa</span><span class="sxs-lookup"><span data-stu-id="9ea12-173">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ea12-174">Relações</span><span class="sxs-lookup"><span data-stu-id="9ea12-174">Relationships</span></span>
<span data-ttu-id="9ea12-175">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ea12-175">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ea12-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ea12-176">JSON Representation</span></span>
<span data-ttu-id="9ea12-177">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ea12-177">Here is a JSON representation of the resource.</span></span>
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
  "showOfficeWebApps": true
}
```



