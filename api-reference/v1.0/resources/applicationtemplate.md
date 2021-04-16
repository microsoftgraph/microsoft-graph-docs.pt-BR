---
title: Tipo de recurso applicationTemplate
description: Representa um aplicativo na galeria de aplicativos do Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 1ee619c53d083a4d1ccc91e904b4158643e8ca5b
ms.sourcegitcommit: be09568fa07ab793cd1db500f537ca94ca9e5b4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836868"
---
# <a name="applicationtemplate-resource-type"></a><span data-ttu-id="7ffef-103">Tipo de recurso applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="7ffef-103">applicationTemplate resource type</span></span>

<span data-ttu-id="7ffef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ffef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ffef-105">Representa um aplicativo na galeria de [aplicativos do Azure AD.](/azure/active-directory/saas-apps/tutorial-list)</span><span class="sxs-lookup"><span data-stu-id="7ffef-105">Represents an application in the [Azure AD application gallery](/azure/active-directory/saas-apps/tutorial-list).</span></span>

## <a name="methods"></a><span data-ttu-id="7ffef-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="7ffef-106">Methods</span></span>

| <span data-ttu-id="7ffef-107">Método</span><span class="sxs-lookup"><span data-stu-id="7ffef-107">Method</span></span>                                                                       | <span data-ttu-id="7ffef-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7ffef-108">Return Type</span></span>                                                   | <span data-ttu-id="7ffef-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ffef-109">Description</span></span>                                                                                  |
| :--------------------------------------------------------------------------- | :------------------------------------------------------------ | :------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="7ffef-110">Lista applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="7ffef-110">List applicationTemplate</span></span>](../api/applicationtemplate-list.md)               | [<span data-ttu-id="7ffef-111">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="7ffef-111">applicationTemplate</span></span>](applicationtemplate.md)                 | <span data-ttu-id="7ffef-112">Recupere uma lista de objetos applicationTemplate.</span><span class="sxs-lookup"><span data-stu-id="7ffef-112">Retrieve a list of applicationTemplate objects.</span></span>                                              |
| [<span data-ttu-id="7ffef-113">Obter applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="7ffef-113">Get applicationTemplate</span></span>](../api/applicationtemplate-get.md)                 | [<span data-ttu-id="7ffef-114">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="7ffef-114">applicationTemplate</span></span>](applicationtemplate.md)                 | <span data-ttu-id="7ffef-115">Ler propriedades e relações do objeto applicationTemplate.</span><span class="sxs-lookup"><span data-stu-id="7ffef-115">Read properties and relationships of applicationTemplate object.</span></span>                             |
| [<span data-ttu-id="7ffef-116">Instanciar o applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="7ffef-116">Instantiate applicationTemplate</span></span>](../api/applicationtemplate-instantiate.md) | [<span data-ttu-id="7ffef-117">applicationServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="7ffef-117">applicationServicePrincipal</span></span>](applicationserviceprincipal.md) | <span data-ttu-id="7ffef-118">Adicione uma instância de um aplicativo da galeria de aplicativos do Azure AD ao diretório.</span><span class="sxs-lookup"><span data-stu-id="7ffef-118">Add an instance of an application from the Azure AD application gallery into your directory.</span></span> |

## <a name="properties"></a><span data-ttu-id="7ffef-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ffef-119">Properties</span></span>

| <span data-ttu-id="7ffef-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ffef-120">Property</span></span>                   | <span data-ttu-id="7ffef-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ffef-121">Type</span></span>              | <span data-ttu-id="7ffef-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ffef-122">Description</span></span>                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| :------------------------- | :---------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7ffef-123">categories</span><span class="sxs-lookup"><span data-stu-id="7ffef-123">categories</span></span>                 | <span data-ttu-id="7ffef-124">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ffef-124">String collection</span></span> | <span data-ttu-id="7ffef-125">A lista de categorias do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ffef-125">The list of categories for the application.</span></span> <span data-ttu-id="7ffef-126">Os valores suportados podem ser: `Collaboration` , , , , , , , `Business Management` `Consumer` `Content management` `CRM` `Data services` `Developer services` `E-commerce` `Education` `ERP` `Finance` `Health` , `Human resources` `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Project management` `Telecommunications` `Tools` `Travel` `Web design & hosting`</span><span class="sxs-lookup"><span data-stu-id="7ffef-126">Supported values can be: `Collaboration`, `Business Management`, `Consumer`, `Content management`, `CRM`, `Data services`, `Developer services`, `E-commerce`, `Education`, `ERP`, `Finance`, `Health`, `Human resources`, `IT infrastructure`, `Mail`, `Management`, `Marketing`, `Media`, `Productivity`, `Project management`, `Telecommunications`, `Tools`, `Travel`, and `Web design & hosting`.</span></span> |
| <span data-ttu-id="7ffef-127">description</span><span class="sxs-lookup"><span data-stu-id="7ffef-127">description</span></span>                | <span data-ttu-id="7ffef-128">String</span><span class="sxs-lookup"><span data-stu-id="7ffef-128">String</span></span>            | <span data-ttu-id="7ffef-129">Uma descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ffef-129">A description of the application.</span></span>                                                                                                                                                                                                                                                                                                                                                                                                               |
| <span data-ttu-id="7ffef-130">displayName</span><span class="sxs-lookup"><span data-stu-id="7ffef-130">displayName</span></span>                | <span data-ttu-id="7ffef-131">String</span><span class="sxs-lookup"><span data-stu-id="7ffef-131">String</span></span>            | <span data-ttu-id="7ffef-132">O nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ffef-132">The name of the application.</span></span>                                                                                                                                                                                                                                                                                                                                                                                                                    |
| <span data-ttu-id="7ffef-133">homePageUrl</span><span class="sxs-lookup"><span data-stu-id="7ffef-133">homePageUrl</span></span>                | <span data-ttu-id="7ffef-134">String</span><span class="sxs-lookup"><span data-stu-id="7ffef-134">String</span></span>            | <span data-ttu-id="7ffef-135">A URL da home page do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ffef-135">The home page URL of the application.</span></span>                                                                                                                                                                                                                                                                                                                                                                                                           |
| <span data-ttu-id="7ffef-136">id</span><span class="sxs-lookup"><span data-stu-id="7ffef-136">id</span></span>                         | <span data-ttu-id="7ffef-137">String</span><span class="sxs-lookup"><span data-stu-id="7ffef-137">String</span></span>            | <span data-ttu-id="7ffef-138">Identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ffef-138">Unique identifier for the application.</span></span> <span data-ttu-id="7ffef-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7ffef-139">Read-only.</span></span>                                                                                                                                                                                                                                                                                                                                                                                               |
| <span data-ttu-id="7ffef-140">logoUrl</span><span class="sxs-lookup"><span data-stu-id="7ffef-140">logoUrl</span></span>                    | <span data-ttu-id="7ffef-141">String</span><span class="sxs-lookup"><span data-stu-id="7ffef-141">String</span></span>            | <span data-ttu-id="7ffef-142">A URL para obter o logotipo desse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ffef-142">The URL to get the logo for this application.</span></span>                                                                                                                                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="7ffef-143">publicador</span><span class="sxs-lookup"><span data-stu-id="7ffef-143">publisher</span></span>                  | <span data-ttu-id="7ffef-144">String</span><span class="sxs-lookup"><span data-stu-id="7ffef-144">String</span></span>            | <span data-ttu-id="7ffef-145">O nome do editor deste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ffef-145">The name of the publisher for this application.</span></span>                                                                                                                                                                                                                                                                                                                                                                                                 |
| <span data-ttu-id="7ffef-146">supportedProvisioningTypes</span><span class="sxs-lookup"><span data-stu-id="7ffef-146">supportedProvisioningTypes</span></span> | <span data-ttu-id="7ffef-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ffef-147">String collection</span></span> | <span data-ttu-id="7ffef-148">A lista de modos de provisionamento suportados por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ffef-148">The list of provisioning modes supported by this application.</span></span> <span data-ttu-id="7ffef-149">O único valor válido é `sync` .</span><span class="sxs-lookup"><span data-stu-id="7ffef-149">The only valid value is `sync`.</span></span>                                                                                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="7ffef-150">supportedSingleSignOnModes</span><span class="sxs-lookup"><span data-stu-id="7ffef-150">supportedSingleSignOnModes</span></span> | <span data-ttu-id="7ffef-151">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ffef-151">String collection</span></span> | <span data-ttu-id="7ffef-152">A lista de modos de login único suportados por este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ffef-152">The list of single sign-on modes supported by this application.</span></span> <span data-ttu-id="7ffef-153">Os valores com suporte são: `oidc`, `password`, `saml`, e `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="7ffef-153">The supported values are `oidc`, `password`, `saml`, and `notSupported`.</span></span>                                                                                                                                                                                                                                                                                                            |

## <a name="relationships"></a><span data-ttu-id="7ffef-154">Relações</span><span class="sxs-lookup"><span data-stu-id="7ffef-154">Relationships</span></span>

<span data-ttu-id="7ffef-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ffef-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ffef-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ffef-156">JSON representation</span></span>

<span data-ttu-id="7ffef-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ffef-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationTemplate",
  "keyProperty": "id"
}-->

```json
{
  "id": "id-value",
  "displayName": "displayName-value",
  "homePageUrl": "homePageUrl-value",
  "supportedSingleSignOnModes": ["supportedSingleSignOnModes-value"],
  "logoUrl": "logoUrl-value",
  "categories": ["categories-value"],
  "publisher": "publisher-value",
  "description": "description-value"
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
