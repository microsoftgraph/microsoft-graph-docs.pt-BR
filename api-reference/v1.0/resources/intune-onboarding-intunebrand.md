---
title: Tipo de recurso intuneBrand
description: intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 346966fdcb3cfc8b3c4c24e55f4a07e46c97a612
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751269"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="b2ca3-103">Tipo de recurso intuneBrand</span><span class="sxs-lookup"><span data-stu-id="b2ca3-103">intuneBrand resource type</span></span>

<span data-ttu-id="b2ca3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2ca3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2ca3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2ca3-106">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-106">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="b2ca3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2ca3-107">Properties</span></span>
|<span data-ttu-id="b2ca3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2ca3-108">Property</span></span>|<span data-ttu-id="b2ca3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2ca3-109">Type</span></span>|<span data-ttu-id="b2ca3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2ca3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2ca3-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b2ca3-111">displayName</span></span>|<span data-ttu-id="b2ca3-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2ca3-112">String</span></span>|<span data-ttu-id="b2ca3-113">Nome da empresa/organização exibido para usuários finais.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-113">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="b2ca3-114">themeColor</span><span class="sxs-lookup"><span data-stu-id="b2ca3-114">themeColor</span></span>|[<span data-ttu-id="b2ca3-115">rgbColor</span><span class="sxs-lookup"><span data-stu-id="b2ca3-115">rgbColor</span></span>](../resources/intune-onboarding-rgbcolor.md)|<span data-ttu-id="b2ca3-116">Cor de tema principal usado nos aplicativos e no portal da Web do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-116">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="b2ca3-117">showLogo</span><span class="sxs-lookup"><span data-stu-id="b2ca3-117">showLogo</span></span>|<span data-ttu-id="b2ca3-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2ca3-118">Boolean</span></span>|<span data-ttu-id="b2ca3-119">Booliano que indica se as imagens de logotipo fornecidas pelo administrador serão exibidas ou não.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-119">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="b2ca3-120">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="b2ca3-120">lightBackgroundLogo</span></span>|[<span data-ttu-id="b2ca3-121">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b2ca3-121">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b2ca3-122">Imagem do logotipo exibida nos aplicativos do Portal da Empresa que têm um plano de fundo claro atrás do logotipo.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-122">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="b2ca3-123">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="b2ca3-123">darkBackgroundLogo</span></span>|[<span data-ttu-id="b2ca3-124">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b2ca3-124">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b2ca3-125">Imagem do logotipo exibida nos aplicativos do Portal da Empresa que têm um plano de fundo escuro atrás do logotipo.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-125">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="b2ca3-126">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="b2ca3-126">showNameNextToLogo</span></span>|<span data-ttu-id="b2ca3-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2ca3-127">Boolean</span></span>|<span data-ttu-id="b2ca3-128">Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-128">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="b2ca3-129">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="b2ca3-129">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="b2ca3-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2ca3-130">Boolean</span></span>|<span data-ttu-id="b2ca3-131">Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-131">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="b2ca3-132">contactITName</span><span class="sxs-lookup"><span data-stu-id="b2ca3-132">contactITName</span></span>|<span data-ttu-id="b2ca3-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2ca3-133">String</span></span>|<span data-ttu-id="b2ca3-134">Nome da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-134">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="b2ca3-135">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="b2ca3-135">contactITPhoneNumber</span></span>|<span data-ttu-id="b2ca3-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2ca3-136">String</span></span>|<span data-ttu-id="b2ca3-137">Número de telefone da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-137">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="b2ca3-138">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="b2ca3-138">contactITEmailAddress</span></span>|<span data-ttu-id="b2ca3-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2ca3-139">String</span></span>|<span data-ttu-id="b2ca3-140">Endereço de email da pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-140">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="b2ca3-141">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="b2ca3-141">contactITNotes</span></span>|<span data-ttu-id="b2ca3-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2ca3-142">String</span></span>|<span data-ttu-id="b2ca3-143">Comentários de texto relacionados à pessoa/organização responsável pelo suporte de TI.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-143">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="b2ca3-144">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="b2ca3-144">onlineSupportSiteUrl</span></span>|<span data-ttu-id="b2ca3-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2ca3-145">String</span></span>|<span data-ttu-id="b2ca3-146">URL do site de assistência técnica de TI da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-146">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="b2ca3-147">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="b2ca3-147">onlineSupportSiteName</span></span>|<span data-ttu-id="b2ca3-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2ca3-148">String</span></span>|<span data-ttu-id="b2ca3-149">Nome de exibição do site de assistência técnica de TI da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-149">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="b2ca3-150">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="b2ca3-150">privacyUrl</span></span>|<span data-ttu-id="b2ca3-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2ca3-151">String</span></span>|<span data-ttu-id="b2ca3-152">URL da política de privacidade da empresa/organização.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-152">URL to the company/organization’s privacy policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2ca3-153">Relações</span><span class="sxs-lookup"><span data-stu-id="b2ca3-153">Relationships</span></span>
<span data-ttu-id="b2ca3-154">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b2ca3-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2ca3-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2ca3-155">JSON Representation</span></span>
<span data-ttu-id="b2ca3-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b2ca3-156">Here is a JSON representation of the resource.</span></span>
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
  "showDisplayNameNextToLogo": true,
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "privacyUrl": "String"
}
```




