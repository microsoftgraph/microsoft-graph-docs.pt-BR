---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
description: O recurso SharingLink agrupa itens de dados relacionados ao link em uma única estrutura.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 01d27971cd04ff91333d25240e4d1d517e05cec5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034248"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="65dea-103">Tipo de recurso SharingLink</span><span class="sxs-lookup"><span data-stu-id="65dea-103">SharingLink resource type</span></span>

<span data-ttu-id="65dea-104">O recurso **SharingLink** agrupa itens de dados relacionados ao link em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="65dea-104">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="65dea-105">Se um recurso [**Permission**](permission.md) tiver uma faceta **sharingLink** não nula, a permissão representará um link de compartilhamento (em vez de permissões concedidas a uma pessoa ou um grupo).</span><span class="sxs-lookup"><span data-stu-id="65dea-105">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="65dea-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65dea-106">JSON representation</span></span>

<span data-ttu-id="65dea-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65dea-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": { "@odata.type": "microsoft.graph.identity" },
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="65dea-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65dea-108">Properties</span></span>

| <span data-ttu-id="65dea-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65dea-109">Property</span></span>    | <span data-ttu-id="65dea-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="65dea-110">Type</span></span>          | <span data-ttu-id="65dea-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="65dea-111">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="65dea-112">aplicativo</span><span class="sxs-lookup"><span data-stu-id="65dea-112">application</span></span> | <span data-ttu-id="65dea-113">[identity][]</span><span class="sxs-lookup"><span data-stu-id="65dea-113">[identity][]</span></span>  | <span data-ttu-id="65dea-114">O aplicativo ao qual o link está associado.</span><span class="sxs-lookup"><span data-stu-id="65dea-114">The app the link is associated with.</span></span>
| <span data-ttu-id="65dea-115">type</span><span class="sxs-lookup"><span data-stu-id="65dea-115">type</span></span>        | <span data-ttu-id="65dea-116">String</span><span class="sxs-lookup"><span data-stu-id="65dea-116">String</span></span>        | <span data-ttu-id="65dea-117">O tipo do link criado.</span><span class="sxs-lookup"><span data-stu-id="65dea-117">The type of the link created.</span></span>
| <span data-ttu-id="65dea-118">scope</span><span class="sxs-lookup"><span data-stu-id="65dea-118">scope</span></span>       | <span data-ttu-id="65dea-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65dea-119">String</span></span>        | <span data-ttu-id="65dea-p101">O escopo do link representado por esta permissão. O valor `anonymous` indica que o link é utilizável por qualquer pessoa; `organization` indica que o link só é útil para usuários conectados ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="65dea-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="65dea-122">webHtml</span><span class="sxs-lookup"><span data-stu-id="65dea-122">webHtml</span></span>     | <span data-ttu-id="65dea-123">String</span><span class="sxs-lookup"><span data-stu-id="65dea-123">String</span></span>        | <span data-ttu-id="65dea-124">Para links `embed`, essa propriedade contém o código HTML para um elemento `<iframe>` que inserirá o item em uma página da Web.</span><span class="sxs-lookup"><span data-stu-id="65dea-124">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="65dea-125">webUrl</span><span class="sxs-lookup"><span data-stu-id="65dea-125">webUrl</span></span>      | <span data-ttu-id="65dea-126">String</span><span class="sxs-lookup"><span data-stu-id="65dea-126">String</span></span>        | <span data-ttu-id="65dea-127">Uma URL que abre o item no navegador no site do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="65dea-127">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-options"></a><span data-ttu-id="65dea-129">Opções de tipo</span><span class="sxs-lookup"><span data-stu-id="65dea-129">Type options</span></span>

<span data-ttu-id="65dea-130">Esta tabela define os valores possíveis para a propriedade **type**:</span><span class="sxs-lookup"><span data-stu-id="65dea-130">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="65dea-131">Valor</span><span class="sxs-lookup"><span data-stu-id="65dea-131">Value</span></span>   | <span data-ttu-id="65dea-132">Função</span><span class="sxs-lookup"><span data-stu-id="65dea-132">Role</span></span>    | <span data-ttu-id="65dea-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="65dea-133">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="65dea-134">Um link somente de compartilhamento para exibição, permitindo o acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="65dea-134">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="65dea-135">Um link de compartilhamento de edição, permitindo o acesso de leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="65dea-135">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="65dea-p102">Um link de compartilhamento somente exibição que pode ser usado para inserir o conteúdo em uma página da Web de hospedagem. Os links de compartilhamento não estão disponíveis para OneDrive for Business ou SharePoint.</span><span class="sxs-lookup"><span data-stu-id="65dea-p102">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-options"></a><span data-ttu-id="65dea-138">Opções de escopo</span><span class="sxs-lookup"><span data-stu-id="65dea-138">Scope options</span></span>

| <span data-ttu-id="65dea-139">Valor</span><span class="sxs-lookup"><span data-stu-id="65dea-139">Value</span></span>          | <span data-ttu-id="65dea-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="65dea-140">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="65dea-141">Qualquer pessoa com o link tem acesso, sem a necessidade de fazer logon.</span><span class="sxs-lookup"><span data-stu-id="65dea-141">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="65dea-142">Isso pode incluir pessoas de fora da sua organização.</span><span class="sxs-lookup"><span data-stu-id="65dea-142">This may include people outside of your organization.</span></span>
| `organization` | <span data-ttu-id="65dea-143">Qualquer pessoa que se inscreveu em sua organização (locatário) pode usar o link para obter acesso.</span><span class="sxs-lookup"><span data-stu-id="65dea-143">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="65dea-144">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="65dea-144">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(view,edit,embed) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(anonymous,organization) are in resource, but () are in table"
  ],
  "tocPath": "Facets/SharingLink"
} -->
