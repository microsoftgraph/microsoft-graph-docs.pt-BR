---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: f16f8240800be4b9c1780a4057583381b736f079
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481423"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="1d7a4-102">Tipo de recurso SharingLink</span><span class="sxs-lookup"><span data-stu-id="1d7a4-102">SharingLink resource type</span></span>

<span data-ttu-id="1d7a4-103">O recurso **SharingLink** agrupa itens de dados relacionados ao link em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="1d7a4-103">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="1d7a4-104">Se um recurso [**Permission**](permission.md) tiver uma faceta **sharingLink** não nula, a permissão representará um link de compartilhamento (em vez de permissões concedidas a uma pessoa ou um grupo).</span><span class="sxs-lookup"><span data-stu-id="1d7a4-104">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d7a4-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d7a4-105">JSON representation</span></span>

<span data-ttu-id="1d7a4-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d7a4-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="1d7a4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d7a4-107">Properties</span></span>

| <span data-ttu-id="1d7a4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d7a4-108">Property</span></span>    | <span data-ttu-id="1d7a4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d7a4-109">Type</span></span>          | <span data-ttu-id="1d7a4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d7a4-110">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="1d7a4-111">aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d7a4-111">application</span></span> | <span data-ttu-id="1d7a4-112">[identity][]</span><span class="sxs-lookup"><span data-stu-id="1d7a4-112">[identity][]</span></span>  | <span data-ttu-id="1d7a4-113">O aplicativo ao qual o link está associado.</span><span class="sxs-lookup"><span data-stu-id="1d7a4-113">The app the link is associated with.</span></span>
| <span data-ttu-id="1d7a4-114">type</span><span class="sxs-lookup"><span data-stu-id="1d7a4-114">type</span></span>        | <span data-ttu-id="1d7a4-115">String</span><span class="sxs-lookup"><span data-stu-id="1d7a4-115">String</span></span>        | <span data-ttu-id="1d7a4-116">O tipo do link criado.</span><span class="sxs-lookup"><span data-stu-id="1d7a4-116">The type of the link created.</span></span>
| <span data-ttu-id="1d7a4-117">scope</span><span class="sxs-lookup"><span data-stu-id="1d7a4-117">scope</span></span>       | <span data-ttu-id="1d7a4-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d7a4-118">String</span></span>        | <span data-ttu-id="1d7a4-p101">O escopo do link representado por esta permissão. O valor `anonymous` indica que o link é utilizável por qualquer pessoa; `organization` indica que o link só é útil para usuários conectados ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="1d7a4-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="1d7a4-121">webHtml</span><span class="sxs-lookup"><span data-stu-id="1d7a4-121">webHtml</span></span>     | <span data-ttu-id="1d7a4-122">String</span><span class="sxs-lookup"><span data-stu-id="1d7a4-122">String</span></span>        | <span data-ttu-id="1d7a4-123">Para links `embed`, essa propriedade contém o código HTML para um elemento `<iframe>` que inserirá o item em uma página da Web.</span><span class="sxs-lookup"><span data-stu-id="1d7a4-123">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="1d7a4-124">webUrl</span><span class="sxs-lookup"><span data-stu-id="1d7a4-124">webUrl</span></span>      | <span data-ttu-id="1d7a4-125">String</span><span class="sxs-lookup"><span data-stu-id="1d7a4-125">String</span></span>        | <span data-ttu-id="1d7a4-126">Uma URL que abre o item no navegador no site do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1d7a4-126">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-options"></a><span data-ttu-id="1d7a4-128">Opções de tipo</span><span class="sxs-lookup"><span data-stu-id="1d7a4-128">Type options</span></span>

<span data-ttu-id="1d7a4-129">Esta tabela define os valores possíveis para a propriedade **type**:</span><span class="sxs-lookup"><span data-stu-id="1d7a4-129">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="1d7a4-130">Valor</span><span class="sxs-lookup"><span data-stu-id="1d7a4-130">Value</span></span>   | <span data-ttu-id="1d7a4-131">Função</span><span class="sxs-lookup"><span data-stu-id="1d7a4-131">Role</span></span>    | <span data-ttu-id="1d7a4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d7a4-132">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="1d7a4-133">Um link somente de compartilhamento para exibição, permitindo o acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1d7a4-133">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="1d7a4-134">Um link de compartilhamento de edição, permitindo o acesso de leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="1d7a4-134">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="1d7a4-p102">Um link de compartilhamento somente exibição que pode ser usado para inserir o conteúdo em uma página da Web de hospedagem. Os links de compartilhamento não estão disponíveis para OneDrive for Business ou SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1d7a4-p102">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-options"></a><span data-ttu-id="1d7a4-137">Opções de escopo</span><span class="sxs-lookup"><span data-stu-id="1d7a4-137">Scope options</span></span>

| <span data-ttu-id="1d7a4-138">Valor</span><span class="sxs-lookup"><span data-stu-id="1d7a4-138">Value</span></span>          | <span data-ttu-id="1d7a4-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d7a4-139">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="1d7a4-140">Qualquer pessoa com o link tem acesso, sem a necessidade de fazer logon.</span><span class="sxs-lookup"><span data-stu-id="1d7a4-140">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="1d7a4-141">Isso pode incluir pessoas de fora da sua organização.</span><span class="sxs-lookup"><span data-stu-id="1d7a4-141">This may include people outside of your organization.</span></span>
| `organization` | <span data-ttu-id="1d7a4-142">Qualquer pessoa que se inscreveu em sua organização (locatário) pode usar o link para obter acesso.</span><span class="sxs-lookup"><span data-stu-id="1d7a4-142">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="1d7a4-143">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1d7a4-143">Only available in OneDrive for Business and SharePoint.</span></span>

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
