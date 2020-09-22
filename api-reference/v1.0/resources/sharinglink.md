---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
description: O recurso SharingLink agrupa itens de dados relacionados ao link em uma única estrutura.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 679e1f749a8e6be3ed0be055118c25a6d585b5d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037049"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="3b96b-103">Tipo de recurso SharingLink</span><span class="sxs-lookup"><span data-stu-id="3b96b-103">SharingLink resource type</span></span>

<span data-ttu-id="3b96b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b96b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3b96b-105">O recurso **SharingLink** agrupa itens de dados relacionados ao link em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="3b96b-105">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="3b96b-106">Se um recurso [**Permission**](permission.md) tiver uma faceta **sharingLink** não nula, a permissão representará um link de compartilhamento (em vez de permissões concedidas a uma pessoa ou um grupo).</span><span class="sxs-lookup"><span data-stu-id="3b96b-106">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b96b-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b96b-107">JSON representation</span></span>

<span data-ttu-id="3b96b-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3b96b-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": { "@odata.type": "microsoft.graph.identity" },
  "preventsDownload": false,
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="3b96b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b96b-109">Properties</span></span>

| <span data-ttu-id="3b96b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b96b-110">Property</span></span>    | <span data-ttu-id="3b96b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b96b-111">Type</span></span>          | <span data-ttu-id="3b96b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b96b-112">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="3b96b-113">aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b96b-113">application</span></span> | <span data-ttu-id="3b96b-114">[identity][]</span><span class="sxs-lookup"><span data-stu-id="3b96b-114">[identity][]</span></span>  | <span data-ttu-id="3b96b-115">O aplicativo ao qual o link está associado.</span><span class="sxs-lookup"><span data-stu-id="3b96b-115">The app the link is associated with.</span></span>
| <span data-ttu-id="3b96b-116">tipo</span><span class="sxs-lookup"><span data-stu-id="3b96b-116">type</span></span>        | <span data-ttu-id="3b96b-117">String</span><span class="sxs-lookup"><span data-stu-id="3b96b-117">String</span></span>        | <span data-ttu-id="3b96b-118">O tipo do link criado.</span><span class="sxs-lookup"><span data-stu-id="3b96b-118">The type of the link created.</span></span>
| <span data-ttu-id="3b96b-119">scope</span><span class="sxs-lookup"><span data-stu-id="3b96b-119">scope</span></span>       | <span data-ttu-id="3b96b-120">String</span><span class="sxs-lookup"><span data-stu-id="3b96b-120">String</span></span>        | <span data-ttu-id="3b96b-p101">O escopo do link representado por esta permissão. O valor `anonymous` indica que o link é utilizável por qualquer pessoa; `organization` indica que o link só é útil para usuários conectados ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="3b96b-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="3b96b-123">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="3b96b-123">preventsDownload</span></span> | <span data-ttu-id="3b96b-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b96b-124">Boolean</span></span>       | <span data-ttu-id="3b96b-125">Se true, o usuário só pode usar este link para exibir o item na Web e não pode usá-lo para baixar o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="3b96b-125">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="3b96b-126">Somente para o OneDrive for Business e o SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3b96b-126">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="3b96b-127">webHtml</span><span class="sxs-lookup"><span data-stu-id="3b96b-127">webHtml</span></span>     | <span data-ttu-id="3b96b-128">String</span><span class="sxs-lookup"><span data-stu-id="3b96b-128">String</span></span>        | <span data-ttu-id="3b96b-129">Para links `embed`, essa propriedade contém o código HTML para um elemento `<iframe>` que inserirá o item em uma página da Web.</span><span class="sxs-lookup"><span data-stu-id="3b96b-129">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="3b96b-130">webUrl</span><span class="sxs-lookup"><span data-stu-id="3b96b-130">webUrl</span></span>      | <span data-ttu-id="3b96b-131">String</span><span class="sxs-lookup"><span data-stu-id="3b96b-131">String</span></span>        | <span data-ttu-id="3b96b-132">Uma URL que abre o item no navegador no site do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3b96b-132">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-options"></a><span data-ttu-id="3b96b-134">Opções de tipo</span><span class="sxs-lookup"><span data-stu-id="3b96b-134">Type options</span></span>

<span data-ttu-id="3b96b-135">Esta tabela define os valores possíveis para a propriedade **type**:</span><span class="sxs-lookup"><span data-stu-id="3b96b-135">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="3b96b-136">Valor</span><span class="sxs-lookup"><span data-stu-id="3b96b-136">Value</span></span>   | <span data-ttu-id="3b96b-137">Role</span><span class="sxs-lookup"><span data-stu-id="3b96b-137">Role</span></span>    | <span data-ttu-id="3b96b-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b96b-138">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="3b96b-139">Um link somente de compartilhamento para exibição, permitindo o acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3b96b-139">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="3b96b-140">Um link de compartilhamento de edição, permitindo o acesso de leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="3b96b-140">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="3b96b-p103">Um link de compartilhamento somente exibição que pode ser usado para inserir o conteúdo em uma página da Web de hospedagem. Os links de compartilhamento não estão disponíveis para OneDrive for Business ou SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3b96b-p103">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-options"></a><span data-ttu-id="3b96b-143">Opções de escopo</span><span class="sxs-lookup"><span data-stu-id="3b96b-143">Scope options</span></span>

| <span data-ttu-id="3b96b-144">Valor</span><span class="sxs-lookup"><span data-stu-id="3b96b-144">Value</span></span>          | <span data-ttu-id="3b96b-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b96b-145">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="3b96b-146">Qualquer pessoa com o link tem acesso, sem precisar fazer logon.</span><span class="sxs-lookup"><span data-stu-id="3b96b-146">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="3b96b-147">Isso pode incluir pessoas de fora da organização.</span><span class="sxs-lookup"><span data-stu-id="3b96b-147">This may include people outside of your organization.</span></span>
| `organization` | <span data-ttu-id="3b96b-148">Qualquer pessoa que tenha feito logon em sua organização (locatário) pode usar o link para obter acesso.</span><span class="sxs-lookup"><span data-stu-id="3b96b-148">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="3b96b-149">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3b96b-149">Only available in OneDrive for Business and SharePoint.</span></span>

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

