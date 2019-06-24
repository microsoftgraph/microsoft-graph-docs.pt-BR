---
title: tipo de recurso applicationtemplate
description: Representa um aplicativo na Galeria de aplicativos do Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4a8e1f4cb365f86df32e32ed568aa3a96d1c090f
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147887"
---
# <a name="applicationtemplate-resource-type"></a><span data-ttu-id="9dd19-103">tipo de recurso applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="9dd19-103">applicationTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dd19-104">Representa um aplicativo na [Galeria de aplicativos do Azure ad](https://docs.microsoft.com/en-us/azure/active-directory/saas-apps/tutorial-list).</span><span class="sxs-lookup"><span data-stu-id="9dd19-104">Represents an application in the [Azure AD application gallery](https://docs.microsoft.com/en-us/azure/active-directory/saas-apps/tutorial-list).</span></span>

## <a name="methods"></a><span data-ttu-id="9dd19-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="9dd19-105">Methods</span></span>

| <span data-ttu-id="9dd19-106">Método</span><span class="sxs-lookup"><span data-stu-id="9dd19-106">Method</span></span>       | <span data-ttu-id="9dd19-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9dd19-107">Return Type</span></span> | <span data-ttu-id="9dd19-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9dd19-108">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="9dd19-109">Listar aplicativo</span><span class="sxs-lookup"><span data-stu-id="9dd19-109">List applicationTemplate</span></span>](../api/applicationtemplate-list.md)|[<span data-ttu-id="9dd19-110">applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="9dd19-110">applicationTemplate</span></span>](applicationtemplate.md)|<span data-ttu-id="9dd19-111">Recupere uma lista de objetos applicationtemplate.</span><span class="sxs-lookup"><span data-stu-id="9dd19-111">Retrieve a list of applicationTemplate objects.</span></span>|
| [<span data-ttu-id="9dd19-112">Obter applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="9dd19-112">Get applicationTemplate</span></span>](../api/applicationtemplate-get.md) | [<span data-ttu-id="9dd19-113">applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="9dd19-113">applicationTemplate</span></span>](applicationtemplate.md) | <span data-ttu-id="9dd19-114">Leia as propriedades e as relações do objeto applicationtemplate.</span><span class="sxs-lookup"><span data-stu-id="9dd19-114">Read properties and relationships of applicationTemplate object.</span></span> |
|[<span data-ttu-id="9dd19-115">Instanciar applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="9dd19-115">Instantiate applicationTemplate</span></span>](../api/applicationtemplate-instantiate.md)|[<span data-ttu-id="9dd19-116">applicationServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="9dd19-116">applicationServicePrincipal</span></span>](applicationserviceprincipal.md)| <span data-ttu-id="9dd19-117">Adicione uma instância de um aplicativo da Galeria de aplicativos do Azure AD ao seu diretório.</span><span class="sxs-lookup"><span data-stu-id="9dd19-117">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>|


## <a name="properties"></a><span data-ttu-id="9dd19-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9dd19-118">Properties</span></span>

| <span data-ttu-id="9dd19-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9dd19-119">Property</span></span>     | <span data-ttu-id="9dd19-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9dd19-120">Type</span></span>        | <span data-ttu-id="9dd19-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9dd19-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9dd19-122">categories</span><span class="sxs-lookup"><span data-stu-id="9dd19-122">categories</span></span>|<span data-ttu-id="9dd19-123">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9dd19-123">String collection</span></span>|<span data-ttu-id="9dd19-124">A lista de categorias para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9dd19-124">The list of categories for the application.</span></span> <span data-ttu-id="9dd19-125">Os valores com suporte podem `Collaboration`ser `Business Management`: `Consumer`,`Content management`, `CRM`, `Data services` `Developer services`,, `E-commerce`, `Education`, `ERP`, `Finance`, `Health`, `Human resources`, `IT infrastructure`, `Mail`, `Management`, `Marketing`, `Media`, `Productivity` ,,,,, , `Project management`, `Telecommunications`, `Tools, Travel`, e `Web design & hosting`.</span><span class="sxs-lookup"><span data-stu-id="9dd19-125">Supported values can be: `Collaboration`, `Business Management`, `Consumer`,`Content management`, `CRM`, `Data services`, `Developer services`, `E-commerce`, `Education`, `ERP`, `Finance`, `Health`, `Human resources`, `IT infrastructure`, `Mail`, `Management`, `Marketing`, `Media`, `Productivity`, `Project management`, `Telecommunications`, `Tools, Travel`, and `Web design & hosting`.</span></span>|
|<span data-ttu-id="9dd19-126">descrição</span><span class="sxs-lookup"><span data-stu-id="9dd19-126">description</span></span>|<span data-ttu-id="9dd19-127">String</span><span class="sxs-lookup"><span data-stu-id="9dd19-127">String</span></span>|<span data-ttu-id="9dd19-128">Uma descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9dd19-128">A description of the application.</span></span>|
|<span data-ttu-id="9dd19-129">displayName</span><span class="sxs-lookup"><span data-stu-id="9dd19-129">displayName</span></span>|<span data-ttu-id="9dd19-130">String</span><span class="sxs-lookup"><span data-stu-id="9dd19-130">String</span></span>|<span data-ttu-id="9dd19-131">O nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9dd19-131">The name of the application.</span></span>|
|<span data-ttu-id="9dd19-132">homePageUrl</span><span class="sxs-lookup"><span data-stu-id="9dd19-132">homePageUrl</span></span>|<span data-ttu-id="9dd19-133">String</span><span class="sxs-lookup"><span data-stu-id="9dd19-133">String</span></span>|<span data-ttu-id="9dd19-134">A URL da home page do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9dd19-134">The home page URL of the application.</span></span>|
|<span data-ttu-id="9dd19-135">id</span><span class="sxs-lookup"><span data-stu-id="9dd19-135">id</span></span>|<span data-ttu-id="9dd19-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9dd19-136">String</span></span>| <span data-ttu-id="9dd19-137">Identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9dd19-137">Unique identifier for the application.</span></span> <span data-ttu-id="9dd19-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9dd19-138">Read-only.</span></span>|
|<span data-ttu-id="9dd19-139">logoUrl</span><span class="sxs-lookup"><span data-stu-id="9dd19-139">logoUrl</span></span>|<span data-ttu-id="9dd19-140">String</span><span class="sxs-lookup"><span data-stu-id="9dd19-140">String</span></span>|<span data-ttu-id="9dd19-141">A URL para obter o logotipo para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9dd19-141">The URL to get the logo for this application.</span></span>|
|<span data-ttu-id="9dd19-142">publicador</span><span class="sxs-lookup"><span data-stu-id="9dd19-142">publisher</span></span>|<span data-ttu-id="9dd19-143">String</span><span class="sxs-lookup"><span data-stu-id="9dd19-143">String</span></span>|<span data-ttu-id="9dd19-144">O nome do editor para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9dd19-144">The name of the publisher for this application.</span></span>|
|<span data-ttu-id="9dd19-145">supportedProvisioningTypes</span><span class="sxs-lookup"><span data-stu-id="9dd19-145">supportedProvisioningTypes</span></span>|<span data-ttu-id="9dd19-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9dd19-146">String collection</span></span>|<span data-ttu-id="9dd19-147">A lista de modos de provisionamento compatíveis com este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9dd19-147">The list of provisioning modes supported by this application.</span></span> <span data-ttu-id="9dd19-148">O único valor válido é `sync`.</span><span class="sxs-lookup"><span data-stu-id="9dd19-148">The only valid value is `sync`.</span></span>|
|<span data-ttu-id="9dd19-149">supportedSingleSignOnModes</span><span class="sxs-lookup"><span data-stu-id="9dd19-149">supportedSingleSignOnModes</span></span>|<span data-ttu-id="9dd19-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9dd19-150">String collection</span></span>|<span data-ttu-id="9dd19-151">A lista de modos de logon único suportados por este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9dd19-151">The list of single sign-on modes supported by this application.</span></span> <span data-ttu-id="9dd19-152">Os valores com suporte `password`são `saml`, `external`, e `oidc`.</span><span class="sxs-lookup"><span data-stu-id="9dd19-152">The supported values are `password`, `saml`, `external`, and `oidc`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9dd19-153">Relações</span><span class="sxs-lookup"><span data-stu-id="9dd19-153">Relationships</span></span>

<span data-ttu-id="9dd19-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9dd19-154">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9dd19-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9dd19-155">JSON representation</span></span>

<span data-ttu-id="9dd19-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9dd19-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationTemplate",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id" : "id-value",
    "displayName" : "displayName-value",
    "homePageUrl" : "homePageUrl-value",
    "supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
    "logoUrl" : "logoUrl-value",
    "categories" : ["categories-value"],
    "publisher" : "publisher-value",
    "description" : "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
