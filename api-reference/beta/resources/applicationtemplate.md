---
title: tipo de recurso applicationtemplate
description: Representa um aplicativo na Galeria de aplicativos do Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c707a9010103f4226e62782a83891ff880a245e8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508258"
---
# <a name="applicationtemplate-resource-type"></a><span data-ttu-id="b512d-103">tipo de recurso applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="b512d-103">applicationTemplate resource type</span></span>

<span data-ttu-id="b512d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b512d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b512d-105">Representa um aplicativo na [Galeria de aplicativos do Azure ad](/azure/active-directory/saas-apps/tutorial-list).</span><span class="sxs-lookup"><span data-stu-id="b512d-105">Represents an application in the [Azure AD application gallery](/azure/active-directory/saas-apps/tutorial-list).</span></span>

## <a name="methods"></a><span data-ttu-id="b512d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b512d-106">Methods</span></span>

| <span data-ttu-id="b512d-107">Método</span><span class="sxs-lookup"><span data-stu-id="b512d-107">Method</span></span>       | <span data-ttu-id="b512d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b512d-108">Return Type</span></span> | <span data-ttu-id="b512d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b512d-109">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="b512d-110">Listar aplicativo</span><span class="sxs-lookup"><span data-stu-id="b512d-110">List applicationTemplate</span></span>](../api/applicationtemplate-list.md)|[<span data-ttu-id="b512d-111">applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="b512d-111">applicationTemplate</span></span>](applicationtemplate.md)|<span data-ttu-id="b512d-112">Recupere uma lista de objetos applicationtemplate.</span><span class="sxs-lookup"><span data-stu-id="b512d-112">Retrieve a list of applicationTemplate objects.</span></span>|
| [<span data-ttu-id="b512d-113">Obter applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="b512d-113">Get applicationTemplate</span></span>](../api/applicationtemplate-get.md) | [<span data-ttu-id="b512d-114">applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="b512d-114">applicationTemplate</span></span>](applicationtemplate.md) | <span data-ttu-id="b512d-115">Leia as propriedades e as relações do objeto applicationtemplate.</span><span class="sxs-lookup"><span data-stu-id="b512d-115">Read properties and relationships of applicationTemplate object.</span></span> |
|[<span data-ttu-id="b512d-116">Instanciar applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="b512d-116">Instantiate applicationTemplate</span></span>](../api/applicationtemplate-instantiate.md)|[<span data-ttu-id="b512d-117">applicationServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="b512d-117">applicationServicePrincipal</span></span>](applicationserviceprincipal.md)| <span data-ttu-id="b512d-118">Adicione uma instância de um aplicativo da Galeria de aplicativos do Azure AD ao seu diretório.</span><span class="sxs-lookup"><span data-stu-id="b512d-118">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>|


## <a name="properties"></a><span data-ttu-id="b512d-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b512d-119">Properties</span></span>

| <span data-ttu-id="b512d-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b512d-120">Property</span></span>     | <span data-ttu-id="b512d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b512d-121">Type</span></span>        | <span data-ttu-id="b512d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b512d-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b512d-123">categories</span><span class="sxs-lookup"><span data-stu-id="b512d-123">categories</span></span>|<span data-ttu-id="b512d-124">String collection</span><span class="sxs-lookup"><span data-stu-id="b512d-124">String collection</span></span>|<span data-ttu-id="b512d-125">A lista de categorias para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b512d-125">The list of categories for the application.</span></span> <span data-ttu-id="b512d-126">Os valores com suporte podem `Collaboration`ser `Business Management`: `Consumer`,`Content management`, `CRM`, `Data services` `Developer services` `E-commerce` `Education` `ERP` `Finance` `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Project management` `Telecommunications` `Tools, Travel`,,,,,,,,,,,,,,,,,,,,,,,,,, e `Web design & hosting` `Health` `Human resources`</span><span class="sxs-lookup"><span data-stu-id="b512d-126">Supported values can be: `Collaboration`, `Business Management`, `Consumer`,`Content management`, `CRM`, `Data services`, `Developer services`, `E-commerce`, `Education`, `ERP`, `Finance`, `Health`, `Human resources`, `IT infrastructure`, `Mail`, `Management`, `Marketing`, `Media`, `Productivity`, `Project management`, `Telecommunications`, `Tools, Travel`, and `Web design & hosting`.</span></span>|
|<span data-ttu-id="b512d-127">description</span><span class="sxs-lookup"><span data-stu-id="b512d-127">description</span></span>|<span data-ttu-id="b512d-128">String</span><span class="sxs-lookup"><span data-stu-id="b512d-128">String</span></span>|<span data-ttu-id="b512d-129">Uma descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b512d-129">A description of the application.</span></span>|
|<span data-ttu-id="b512d-130">displayName</span><span class="sxs-lookup"><span data-stu-id="b512d-130">displayName</span></span>|<span data-ttu-id="b512d-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b512d-131">String</span></span>|<span data-ttu-id="b512d-132">O nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b512d-132">The name of the application.</span></span>|
|<span data-ttu-id="b512d-133">homePageUrl</span><span class="sxs-lookup"><span data-stu-id="b512d-133">homePageUrl</span></span>|<span data-ttu-id="b512d-134">String</span><span class="sxs-lookup"><span data-stu-id="b512d-134">String</span></span>|<span data-ttu-id="b512d-135">A URL da home page do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b512d-135">The home page URL of the application.</span></span>|
|<span data-ttu-id="b512d-136">id</span><span class="sxs-lookup"><span data-stu-id="b512d-136">id</span></span>|<span data-ttu-id="b512d-137">String</span><span class="sxs-lookup"><span data-stu-id="b512d-137">String</span></span>| <span data-ttu-id="b512d-138">Identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b512d-138">Unique identifier for the application.</span></span> <span data-ttu-id="b512d-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b512d-139">Read-only.</span></span>|
|<span data-ttu-id="b512d-140">logoUrl</span><span class="sxs-lookup"><span data-stu-id="b512d-140">logoUrl</span></span>|<span data-ttu-id="b512d-141">String</span><span class="sxs-lookup"><span data-stu-id="b512d-141">String</span></span>|<span data-ttu-id="b512d-142">A URL para obter o logotipo para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b512d-142">The URL to get the logo for this application.</span></span>|
|<span data-ttu-id="b512d-143">publicador</span><span class="sxs-lookup"><span data-stu-id="b512d-143">publisher</span></span>|<span data-ttu-id="b512d-144">String</span><span class="sxs-lookup"><span data-stu-id="b512d-144">String</span></span>|<span data-ttu-id="b512d-145">O nome do editor para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b512d-145">The name of the publisher for this application.</span></span>|
|<span data-ttu-id="b512d-146">supportedProvisioningTypes</span><span class="sxs-lookup"><span data-stu-id="b512d-146">supportedProvisioningTypes</span></span>|<span data-ttu-id="b512d-147">String collection</span><span class="sxs-lookup"><span data-stu-id="b512d-147">String collection</span></span>|<span data-ttu-id="b512d-148">A lista de modos de provisionamento compatíveis com este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b512d-148">The list of provisioning modes supported by this application.</span></span> <span data-ttu-id="b512d-149">O único valor válido é `sync`.</span><span class="sxs-lookup"><span data-stu-id="b512d-149">The only valid value is `sync`.</span></span>|
|<span data-ttu-id="b512d-150">supportedSingleSignOnModes</span><span class="sxs-lookup"><span data-stu-id="b512d-150">supportedSingleSignOnModes</span></span>|<span data-ttu-id="b512d-151">String collection</span><span class="sxs-lookup"><span data-stu-id="b512d-151">String collection</span></span>|<span data-ttu-id="b512d-152">A lista de modos de logon único suportados por este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b512d-152">The list of single sign-on modes supported by this application.</span></span> <span data-ttu-id="b512d-153">Os valores com suporte `password`são `saml`, `external`, e `oidc`.</span><span class="sxs-lookup"><span data-stu-id="b512d-153">The supported values are `password`, `saml`, `external`, and `oidc`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b512d-154">Relações</span><span class="sxs-lookup"><span data-stu-id="b512d-154">Relationships</span></span>

<span data-ttu-id="b512d-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b512d-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b512d-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b512d-156">JSON representation</span></span>

<span data-ttu-id="b512d-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b512d-157">The following is a JSON representation of the resource.</span></span>

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
