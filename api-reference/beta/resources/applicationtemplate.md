---
title: tipo de recurso applicationtemplate
description: Representa um aplicativo na Galeria de aplicativos do Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1dcb5d1a4f1a86521081487ec66494d76c035b82
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050231"
---
# <a name="applicationtemplate-resource-type"></a><span data-ttu-id="b7b32-103">tipo de recurso applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="b7b32-103">applicationTemplate resource type</span></span>

<span data-ttu-id="b7b32-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7b32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7b32-105">Representa um aplicativo na [Galeria de aplicativos do Azure ad](/azure/active-directory/saas-apps/tutorial-list).</span><span class="sxs-lookup"><span data-stu-id="b7b32-105">Represents an application in the [Azure AD application gallery](/azure/active-directory/saas-apps/tutorial-list).</span></span>

## <a name="methods"></a><span data-ttu-id="b7b32-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b7b32-106">Methods</span></span>

| <span data-ttu-id="b7b32-107">Método</span><span class="sxs-lookup"><span data-stu-id="b7b32-107">Method</span></span>       | <span data-ttu-id="b7b32-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b7b32-108">Return Type</span></span> | <span data-ttu-id="b7b32-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7b32-109">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="b7b32-110">Lista applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="b7b32-110">List applicationTemplate</span></span>](../api/applicationtemplate-list.md)|[<span data-ttu-id="b7b32-111">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="b7b32-111">applicationTemplate</span></span>](applicationtemplate.md)|<span data-ttu-id="b7b32-112">Recupere uma lista de objetos applicationtemplate.</span><span class="sxs-lookup"><span data-stu-id="b7b32-112">Retrieve a list of applicationTemplate objects.</span></span>|
| [<span data-ttu-id="b7b32-113">Obter applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="b7b32-113">Get applicationTemplate</span></span>](../api/applicationtemplate-get.md) | [<span data-ttu-id="b7b32-114">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="b7b32-114">applicationTemplate</span></span>](applicationtemplate.md) | <span data-ttu-id="b7b32-115">Leia as propriedades e as relações do objeto applicationtemplate.</span><span class="sxs-lookup"><span data-stu-id="b7b32-115">Read properties and relationships of applicationTemplate object.</span></span> |
|[<span data-ttu-id="b7b32-116">Instanciar o applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="b7b32-116">Instantiate applicationTemplate</span></span>](../api/applicationtemplate-instantiate.md)|[<span data-ttu-id="b7b32-117">applicationServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="b7b32-117">applicationServicePrincipal</span></span>](applicationserviceprincipal.md)| <span data-ttu-id="b7b32-118">Adicione uma instância de um aplicativo da Galeria de aplicativos do Azure AD ao seu diretório.</span><span class="sxs-lookup"><span data-stu-id="b7b32-118">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>|


## <a name="properties"></a><span data-ttu-id="b7b32-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7b32-119">Properties</span></span>

| <span data-ttu-id="b7b32-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7b32-120">Property</span></span>     | <span data-ttu-id="b7b32-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7b32-121">Type</span></span>        | <span data-ttu-id="b7b32-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7b32-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b7b32-123">Categorias</span><span class="sxs-lookup"><span data-stu-id="b7b32-123">categories</span></span>|<span data-ttu-id="b7b32-124">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7b32-124">String collection</span></span>|<span data-ttu-id="b7b32-125">A lista de categorias para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b7b32-125">The list of categories for the application.</span></span> <span data-ttu-id="b7b32-126">Os valores com suporte podem ser:,,,,,,,,,,,,,,,,,,,,,,,,,,,,, `Collaboration` `Business Management` `Consumer` `Content management` `CRM` `Data services` `Developer services` `E-commerce` `Education` `ERP` `Finance` `Health` `Human resources` `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Project management` `Telecommunications` `Tools, Travel` e `Web design & hosting` .</span><span class="sxs-lookup"><span data-stu-id="b7b32-126">Supported values can be: `Collaboration`, `Business Management`, `Consumer`,`Content management`, `CRM`, `Data services`, `Developer services`, `E-commerce`, `Education`, `ERP`, `Finance`, `Health`, `Human resources`, `IT infrastructure`, `Mail`, `Management`, `Marketing`, `Media`, `Productivity`, `Project management`, `Telecommunications`, `Tools, Travel`, and `Web design & hosting`.</span></span>|
|<span data-ttu-id="b7b32-127">description</span><span class="sxs-lookup"><span data-stu-id="b7b32-127">description</span></span>|<span data-ttu-id="b7b32-128">String</span><span class="sxs-lookup"><span data-stu-id="b7b32-128">String</span></span>|<span data-ttu-id="b7b32-129">Uma descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b7b32-129">A description of the application.</span></span>|
|<span data-ttu-id="b7b32-130">displayName</span><span class="sxs-lookup"><span data-stu-id="b7b32-130">displayName</span></span>|<span data-ttu-id="b7b32-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7b32-131">String</span></span>|<span data-ttu-id="b7b32-132">O nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b7b32-132">The name of the application.</span></span>|
|<span data-ttu-id="b7b32-133">homePageUrl</span><span class="sxs-lookup"><span data-stu-id="b7b32-133">homePageUrl</span></span>|<span data-ttu-id="b7b32-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7b32-134">String</span></span>|<span data-ttu-id="b7b32-135">A URL da home page do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b7b32-135">The home page URL of the application.</span></span>|
|<span data-ttu-id="b7b32-136">id</span><span class="sxs-lookup"><span data-stu-id="b7b32-136">id</span></span>|<span data-ttu-id="b7b32-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7b32-137">String</span></span>| <span data-ttu-id="b7b32-138">Identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b7b32-138">Unique identifier for the application.</span></span> <span data-ttu-id="b7b32-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b7b32-139">Read-only.</span></span>|
|<span data-ttu-id="b7b32-140">logoUrl</span><span class="sxs-lookup"><span data-stu-id="b7b32-140">logoUrl</span></span>|<span data-ttu-id="b7b32-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7b32-141">String</span></span>|<span data-ttu-id="b7b32-142">A URL para obter o logotipo para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b7b32-142">The URL to get the logo for this application.</span></span>|
|<span data-ttu-id="b7b32-143">publicador</span><span class="sxs-lookup"><span data-stu-id="b7b32-143">publisher</span></span>|<span data-ttu-id="b7b32-144">String</span><span class="sxs-lookup"><span data-stu-id="b7b32-144">String</span></span>|<span data-ttu-id="b7b32-145">O nome do editor para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b7b32-145">The name of the publisher for this application.</span></span>|
|<span data-ttu-id="b7b32-146">supportedProvisioningTypes</span><span class="sxs-lookup"><span data-stu-id="b7b32-146">supportedProvisioningTypes</span></span>|<span data-ttu-id="b7b32-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7b32-147">String collection</span></span>|<span data-ttu-id="b7b32-148">A lista de modos de provisionamento compatíveis com este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b7b32-148">The list of provisioning modes supported by this application.</span></span> <span data-ttu-id="b7b32-149">O único valor válido é `sync` .</span><span class="sxs-lookup"><span data-stu-id="b7b32-149">The only valid value is `sync`.</span></span>|
|<span data-ttu-id="b7b32-150">supportedSingleSignOnModes</span><span class="sxs-lookup"><span data-stu-id="b7b32-150">supportedSingleSignOnModes</span></span>|<span data-ttu-id="b7b32-151">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7b32-151">String collection</span></span>|<span data-ttu-id="b7b32-152">A lista de modos de logon único suportados por este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b7b32-152">The list of single sign-on modes supported by this application.</span></span> <span data-ttu-id="b7b32-153">Os valores com suporte são `password` , `saml` , `external` e `oidc` .</span><span class="sxs-lookup"><span data-stu-id="b7b32-153">The supported values are `password`, `saml`, `external`, and `oidc`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7b32-154">Relações</span><span class="sxs-lookup"><span data-stu-id="b7b32-154">Relationships</span></span>

<span data-ttu-id="b7b32-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b7b32-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7b32-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7b32-156">JSON representation</span></span>

<span data-ttu-id="b7b32-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b7b32-157">The following is a JSON representation of the resource.</span></span>

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


