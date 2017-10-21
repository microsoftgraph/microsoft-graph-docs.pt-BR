---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
ms.openlocfilehash: 7b7729899d134fa1d5de7debb1f209ec5aadd70d
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="48698-102">Tipo de recurso SharingLink</span><span class="sxs-lookup"><span data-stu-id="48698-102">SharingLink resource type</span></span>

<span data-ttu-id="48698-103">O recurso **SharingLink** agrupa itens de dados relacionados ao link em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="48698-103">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="48698-104">Se um recurso [**Permission**](permission.md) tiver uma faceta **sharingLink** não nula, a permissão representará um link de compartilhamento (em vez de permissões concedidas a uma pessoa ou um grupo).</span><span class="sxs-lookup"><span data-stu-id="48698-104">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="48698-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48698-105">JSON representation</span></span>

<span data-ttu-id="48698-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48698-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="48698-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48698-107">Properties</span></span>

| <span data-ttu-id="48698-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48698-108">Property</span></span>    | <span data-ttu-id="48698-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="48698-109">Type</span></span>          | <span data-ttu-id="48698-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="48698-110">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="48698-111">aplicativo</span><span class="sxs-lookup"><span data-stu-id="48698-111">application</span></span> | <span data-ttu-id="48698-112">[identity][]</span><span class="sxs-lookup"><span data-stu-id="48698-112">[identity][]</span></span>  | <span data-ttu-id="48698-113">O aplicativo ao qual o link está associado.</span><span class="sxs-lookup"><span data-stu-id="48698-113">The app the link is associated with.</span></span>
| <span data-ttu-id="48698-114">type</span><span class="sxs-lookup"><span data-stu-id="48698-114">type</span></span>        | <span data-ttu-id="48698-115">String</span><span class="sxs-lookup"><span data-stu-id="48698-115">String</span></span>        | <span data-ttu-id="48698-116">O tipo do link criado.</span><span class="sxs-lookup"><span data-stu-id="48698-116">The type of the link created.</span></span>
| <span data-ttu-id="48698-117">scope</span><span class="sxs-lookup"><span data-stu-id="48698-117">scope</span></span>       | <span data-ttu-id="48698-118">String</span><span class="sxs-lookup"><span data-stu-id="48698-118">String</span></span>        | <span data-ttu-id="48698-p101">O escopo do link representado por esta permissão. O valor `anonymous` indica que o link é utilizável por qualquer pessoa; `organization` indica que o link só é útil para usuários conectados ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="48698-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="48698-121">webHtml</span><span class="sxs-lookup"><span data-stu-id="48698-121">webHtml</span></span>     | <span data-ttu-id="48698-122">String</span><span class="sxs-lookup"><span data-stu-id="48698-122">String</span></span>        | <span data-ttu-id="48698-123">Para links `embed`, essa propriedade contém o código HTML para um elemento `<iframe>` que inserirá o item em uma página da Web.</span><span class="sxs-lookup"><span data-stu-id="48698-123">For embeddable links, this property contains the HTML code for an  element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="48698-124">webUrl</span><span class="sxs-lookup"><span data-stu-id="48698-124">webUrl</span></span>      | <span data-ttu-id="48698-125">String</span><span class="sxs-lookup"><span data-stu-id="48698-125">String</span></span>        | <span data-ttu-id="48698-126">Uma URL que abre o item no navegador no site do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="48698-126">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-enumeration"></a><span data-ttu-id="48698-128">Enumeração Type</span><span class="sxs-lookup"><span data-stu-id="48698-128">Type enumeration</span></span>

<span data-ttu-id="48698-129">Esta tabela define os valores possíveis para a propriedade **type**:</span><span class="sxs-lookup"><span data-stu-id="48698-129">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="48698-130">Valor</span><span class="sxs-lookup"><span data-stu-id="48698-130">Value</span></span>   | <span data-ttu-id="48698-131">Função</span><span class="sxs-lookup"><span data-stu-id="48698-131">Role</span></span>    | <span data-ttu-id="48698-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="48698-132">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="48698-133">Um link somente de compartilhamento para exibição, permitindo o acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="48698-133">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="48698-134">Um link de compartilhamento de edição, permitindo o acesso de leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="48698-134">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="48698-135">Um link de compartilhamento somente exibição que pode ser usado para inserir o conteúdo em uma página da Web de hospedagem.</span><span class="sxs-lookup"><span data-stu-id="48698-135">A view-only sharing link that can be used to embed content into a host webpage.</span></span> <span data-ttu-id="48698-136">Os links de compartilhamento não estão disponíveis para OneDrive for Business ou SharePoint.</span><span class="sxs-lookup"><span data-stu-id="48698-136">Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-enumeration"></a><span data-ttu-id="48698-137">Enumeração de escopo</span><span class="sxs-lookup"><span data-stu-id="48698-137">Scope enumeration</span></span>

| <span data-ttu-id="48698-138">Valor</span><span class="sxs-lookup"><span data-stu-id="48698-138">Value</span></span>          | <span data-ttu-id="48698-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="48698-139">Description</span></span>                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="48698-140">O link de compartilhamento está disponível para uso por qualquer pessoa.</span><span class="sxs-lookup"><span data-stu-id="48698-140">The sharing link is available for anyone to use.</span></span>                                                                            |
| `organization` | <span data-ttu-id="48698-p103">O link de compartilhamento está disponível para uso por qualquer pessoa na mesma organização (locatário). Não disponível para o OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="48698-p103">The sharing link is available for anyone within the same organization (tenant) to use. Not available for OneDrive Personal.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "Facets/SharingLink"
} -->
