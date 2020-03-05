---
author: JeremyKelley
description: O recurso sharingLink agrupa itens de dados relacionados ao link em uma única estrutura.
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e96164b636866637a30f733cb46da5124d90fa49
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520643"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="52ba8-103">tipo de recurso sharingLink</span><span class="sxs-lookup"><span data-stu-id="52ba8-103">sharingLink resource type</span></span>

<span data-ttu-id="52ba8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="52ba8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52ba8-105">O recurso **sharingLink** agrupa itens de dados relacionados ao link em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="52ba8-105">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="52ba8-106">Se um recurso de [**permissão**](permission.md) tiver uma faceta **sharingLink** não nula, a permissão representa um link de compartilhamento (em oposição às permissões concedidas a uma pessoa ou grupo).</span><span class="sxs-lookup"><span data-stu-id="52ba8-106">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="52ba8-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52ba8-107">JSON representation</span></span>

<span data-ttu-id="52ba8-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52ba8-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="52ba8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52ba8-109">Properties</span></span>

| <span data-ttu-id="52ba8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52ba8-110">Property</span></span>       | <span data-ttu-id="52ba8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="52ba8-111">Type</span></span>          | <span data-ttu-id="52ba8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="52ba8-112">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="52ba8-113">aplicativo</span><span class="sxs-lookup"><span data-stu-id="52ba8-113">application</span></span>    | <span data-ttu-id="52ba8-114">[identity][]</span><span class="sxs-lookup"><span data-stu-id="52ba8-114">[identity][]</span></span>  | <span data-ttu-id="52ba8-115">O aplicativo ao qual o link está associado.</span><span class="sxs-lookup"><span data-stu-id="52ba8-115">The app the link is associated with.</span></span>
| <span data-ttu-id="52ba8-116">type</span><span class="sxs-lookup"><span data-stu-id="52ba8-116">type</span></span>           | <span data-ttu-id="52ba8-117">String</span><span class="sxs-lookup"><span data-stu-id="52ba8-117">String</span></span>        | <span data-ttu-id="52ba8-118">O tipo do link criado.</span><span class="sxs-lookup"><span data-stu-id="52ba8-118">The type of the link created.</span></span>
| <span data-ttu-id="52ba8-119">scope</span><span class="sxs-lookup"><span data-stu-id="52ba8-119">scope</span></span>          | <span data-ttu-id="52ba8-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52ba8-120">String</span></span>        | <span data-ttu-id="52ba8-p101">O escopo do link representado por esta permissão. O valor `anonymous` indica que o link é utilizável por qualquer pessoa; `organization` indica que o link só é útil para usuários conectados ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="52ba8-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="52ba8-123">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="52ba8-123">preventsDownload</span></span> | <span data-ttu-id="52ba8-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="52ba8-124">Boolean</span></span>       | <span data-ttu-id="52ba8-125">Se true, o usuário só pode usar este link para exibir o item na Web e não pode usá-lo para baixar o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="52ba8-125">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="52ba8-126">Somente para o OneDrive for Business e o SharePoint.</span><span class="sxs-lookup"><span data-stu-id="52ba8-126">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="52ba8-127">webHtml</span><span class="sxs-lookup"><span data-stu-id="52ba8-127">webHtml</span></span>        | <span data-ttu-id="52ba8-128">String</span><span class="sxs-lookup"><span data-stu-id="52ba8-128">String</span></span>        | <span data-ttu-id="52ba8-129">Para links `embed`, essa propriedade contém o código HTML para um elemento `<iframe>` que inserirá o item em uma página da Web.</span><span class="sxs-lookup"><span data-stu-id="52ba8-129">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="52ba8-130">webUrl</span><span class="sxs-lookup"><span data-stu-id="52ba8-130">webUrl</span></span>         | <span data-ttu-id="52ba8-131">String</span><span class="sxs-lookup"><span data-stu-id="52ba8-131">String</span></span>        | <span data-ttu-id="52ba8-132">Uma URL que abre o item no navegador no site do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="52ba8-132">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="52ba8-134">Opções de tipo</span><span class="sxs-lookup"><span data-stu-id="52ba8-134">Type options</span></span>

<span data-ttu-id="52ba8-135">A tabela a seguir define os valores possíveis para a propriedade **Type** .</span><span class="sxs-lookup"><span data-stu-id="52ba8-135">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="52ba8-136">Valor</span><span class="sxs-lookup"><span data-stu-id="52ba8-136">Value</span></span>    | <span data-ttu-id="52ba8-137">Role</span><span class="sxs-lookup"><span data-stu-id="52ba8-137">Role</span></span>     | <span data-ttu-id="52ba8-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="52ba8-138">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="52ba8-139">Um link somente de compartilhamento para exibição, permitindo o acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52ba8-139">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="52ba8-140">Um link de compartilhamento de edição, permitindo o acesso de leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="52ba8-140">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="52ba8-p103">Um link de compartilhamento somente exibição que pode ser usado para inserir o conteúdo em uma página da Web de hospedagem. Os links de compartilhamento não estão disponíveis para OneDrive for Business ou SharePoint.</span><span class="sxs-lookup"><span data-stu-id="52ba8-p103">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="52ba8-143">Opções de escopo</span><span class="sxs-lookup"><span data-stu-id="52ba8-143">Scope options</span></span>

<span data-ttu-id="52ba8-144">A tabela a seguir define os valores possíveis para a propriedade **Scope** .</span><span class="sxs-lookup"><span data-stu-id="52ba8-144">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="52ba8-145">Valor</span><span class="sxs-lookup"><span data-stu-id="52ba8-145">Value</span></span>            | <span data-ttu-id="52ba8-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="52ba8-146">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="52ba8-147">Qualquer pessoa com o link tem acesso, sem precisar fazer logon.</span><span class="sxs-lookup"><span data-stu-id="52ba8-147">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="52ba8-148">Isso pode incluir pessoas de fora da organização.</span><span class="sxs-lookup"><span data-stu-id="52ba8-148">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="52ba8-149">Qualquer pessoa que tenha feito logon em sua organização (locatário) pode usar o link para obter acesso.</span><span class="sxs-lookup"><span data-stu-id="52ba8-149">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="52ba8-150">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="52ba8-150">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="52ba8-151">Somente as pessoas que já receberam acesso ao item por meio de outros meios podem acessar o item usando este link.</span><span class="sxs-lookup"><span data-stu-id="52ba8-151">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="52ba8-152">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="52ba8-152">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="52ba8-153">O link concede acesso somente a uma lista específica de pessoas.</span><span class="sxs-lookup"><span data-stu-id="52ba8-153">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="52ba8-154">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="52ba8-154">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
