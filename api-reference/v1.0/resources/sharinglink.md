---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
description: O recurso SharingLink agrupa itens de dados relacionados ao link em uma única estrutura.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3195207588061840c4e1394e1460f74d3728510c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446860"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="84691-103">Tipo de recurso SharingLink</span><span class="sxs-lookup"><span data-stu-id="84691-103">SharingLink resource type</span></span>

<span data-ttu-id="84691-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="84691-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="84691-105">O recurso **SharingLink** agrupa itens de dados relacionados ao link em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="84691-105">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="84691-106">Se um recurso [**Permission**](permission.md) tiver uma faceta **sharingLink** não nula, a permissão representará um link de compartilhamento (em vez de permissões concedidas a uma pessoa ou um grupo).</span><span class="sxs-lookup"><span data-stu-id="84691-106">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="84691-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84691-107">JSON representation</span></span>

<span data-ttu-id="84691-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84691-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="84691-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84691-109">Properties</span></span>

| <span data-ttu-id="84691-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84691-110">Property</span></span>    | <span data-ttu-id="84691-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="84691-111">Type</span></span>          | <span data-ttu-id="84691-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="84691-112">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="84691-113">aplicativo</span><span class="sxs-lookup"><span data-stu-id="84691-113">application</span></span> | <span data-ttu-id="84691-114">[identity][]</span><span class="sxs-lookup"><span data-stu-id="84691-114">[identity][]</span></span>  | <span data-ttu-id="84691-115">O aplicativo ao qual o link está associado.</span><span class="sxs-lookup"><span data-stu-id="84691-115">The app the link is associated with.</span></span>
| <span data-ttu-id="84691-116">type</span><span class="sxs-lookup"><span data-stu-id="84691-116">type</span></span>        | <span data-ttu-id="84691-117">String</span><span class="sxs-lookup"><span data-stu-id="84691-117">String</span></span>        | <span data-ttu-id="84691-118">O tipo do link criado.</span><span class="sxs-lookup"><span data-stu-id="84691-118">The type of the link created.</span></span>
| <span data-ttu-id="84691-119">scope</span><span class="sxs-lookup"><span data-stu-id="84691-119">scope</span></span>       | <span data-ttu-id="84691-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84691-120">String</span></span>        | <span data-ttu-id="84691-p101">O escopo do link representado por esta permissão. O valor `anonymous` indica que o link é utilizável por qualquer pessoa; `organization` indica que o link só é útil para usuários conectados ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="84691-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="84691-123">webHtml</span><span class="sxs-lookup"><span data-stu-id="84691-123">webHtml</span></span>     | <span data-ttu-id="84691-124">String</span><span class="sxs-lookup"><span data-stu-id="84691-124">String</span></span>        | <span data-ttu-id="84691-125">Para links `embed`, essa propriedade contém o código HTML para um elemento `<iframe>` que inserirá o item em uma página da Web.</span><span class="sxs-lookup"><span data-stu-id="84691-125">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="84691-126">webUrl</span><span class="sxs-lookup"><span data-stu-id="84691-126">webUrl</span></span>      | <span data-ttu-id="84691-127">String</span><span class="sxs-lookup"><span data-stu-id="84691-127">String</span></span>        | <span data-ttu-id="84691-128">Uma URL que abre o item no navegador no site do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="84691-128">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-options"></a><span data-ttu-id="84691-130">Opções de tipo</span><span class="sxs-lookup"><span data-stu-id="84691-130">Type options</span></span>

<span data-ttu-id="84691-131">Esta tabela define os valores possíveis para a propriedade **type**:</span><span class="sxs-lookup"><span data-stu-id="84691-131">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="84691-132">Valor</span><span class="sxs-lookup"><span data-stu-id="84691-132">Value</span></span>   | <span data-ttu-id="84691-133">Role</span><span class="sxs-lookup"><span data-stu-id="84691-133">Role</span></span>    | <span data-ttu-id="84691-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="84691-134">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="84691-135">Um link somente de compartilhamento para exibição, permitindo o acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="84691-135">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="84691-136">Um link de compartilhamento de edição, permitindo o acesso de leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="84691-136">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="84691-p102">Um link de compartilhamento somente exibição que pode ser usado para inserir o conteúdo em uma página da Web de hospedagem. Os links de compartilhamento não estão disponíveis para OneDrive for Business ou SharePoint.</span><span class="sxs-lookup"><span data-stu-id="84691-p102">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-options"></a><span data-ttu-id="84691-139">Opções de escopo</span><span class="sxs-lookup"><span data-stu-id="84691-139">Scope options</span></span>

| <span data-ttu-id="84691-140">Valor</span><span class="sxs-lookup"><span data-stu-id="84691-140">Value</span></span>          | <span data-ttu-id="84691-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="84691-141">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="84691-142">Qualquer pessoa com o link tem acesso, sem precisar fazer logon.</span><span class="sxs-lookup"><span data-stu-id="84691-142">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="84691-143">Isso pode incluir pessoas de fora da organização.</span><span class="sxs-lookup"><span data-stu-id="84691-143">This may include people outside of your organization.</span></span>
| `organization` | <span data-ttu-id="84691-144">Qualquer pessoa que tenha feito logon em sua organização (locatário) pode usar o link para obter acesso.</span><span class="sxs-lookup"><span data-stu-id="84691-144">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="84691-145">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="84691-145">Only available in OneDrive for Business and SharePoint.</span></span>

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
