---
author: JeremyKelley
description: O recurso sharingLink agrupa itens de dados relacionados ao link em uma única estrutura.
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f1ebff332227410bcb67d87de50a97dd2e078660
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965128"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="abe69-103">tipo de recurso sharingLink</span><span class="sxs-lookup"><span data-stu-id="abe69-103">sharingLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abe69-104">O recurso **sharingLink** agrupa itens de dados relacionados ao link em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="abe69-104">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="abe69-105">Se um recurso de [**permissão**](permission.md) tiver uma faceta **sharingLink** não nula, a permissão representa um link de compartilhamento (em oposição às permissões concedidas a uma pessoa ou grupo).</span><span class="sxs-lookup"><span data-stu-id="abe69-105">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="abe69-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="abe69-106">JSON representation</span></span>

<span data-ttu-id="abe69-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="abe69-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="abe69-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="abe69-108">Properties</span></span>

| <span data-ttu-id="abe69-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abe69-109">Property</span></span>       | <span data-ttu-id="abe69-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="abe69-110">Type</span></span>          | <span data-ttu-id="abe69-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="abe69-111">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="abe69-112">aplicativo</span><span class="sxs-lookup"><span data-stu-id="abe69-112">application</span></span>    | <span data-ttu-id="abe69-113">[identity][]</span><span class="sxs-lookup"><span data-stu-id="abe69-113">[identity][]</span></span>  | <span data-ttu-id="abe69-114">O aplicativo ao qual o link está associado.</span><span class="sxs-lookup"><span data-stu-id="abe69-114">The app the link is associated with.</span></span>
| <span data-ttu-id="abe69-115">type</span><span class="sxs-lookup"><span data-stu-id="abe69-115">type</span></span>           | <span data-ttu-id="abe69-116">String</span><span class="sxs-lookup"><span data-stu-id="abe69-116">String</span></span>        | <span data-ttu-id="abe69-117">O tipo do link criado.</span><span class="sxs-lookup"><span data-stu-id="abe69-117">The type of the link created.</span></span>
| <span data-ttu-id="abe69-118">scope</span><span class="sxs-lookup"><span data-stu-id="abe69-118">scope</span></span>          | <span data-ttu-id="abe69-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abe69-119">String</span></span>        | <span data-ttu-id="abe69-p101">O escopo do link representado por esta permissão. O valor `anonymous` indica que o link é utilizável por qualquer pessoa; `organization` indica que o link só é útil para usuários conectados ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="abe69-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="abe69-122">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="abe69-122">preventsDownload</span></span> | <span data-ttu-id="abe69-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="abe69-123">Boolean</span></span>       | <span data-ttu-id="abe69-124">Se true, o usuário só pode usar este link para exibir o item na Web e não pode usá-lo para baixar o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="abe69-124">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="abe69-125">Somente para o OneDrive for Business e o SharePoint.</span><span class="sxs-lookup"><span data-stu-id="abe69-125">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="abe69-126">webHtml</span><span class="sxs-lookup"><span data-stu-id="abe69-126">webHtml</span></span>        | <span data-ttu-id="abe69-127">String</span><span class="sxs-lookup"><span data-stu-id="abe69-127">String</span></span>        | <span data-ttu-id="abe69-128">Para links `embed`, essa propriedade contém o código HTML para um elemento `<iframe>` que inserirá o item em uma página da Web.</span><span class="sxs-lookup"><span data-stu-id="abe69-128">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="abe69-129">webUrl</span><span class="sxs-lookup"><span data-stu-id="abe69-129">webUrl</span></span>         | <span data-ttu-id="abe69-130">String</span><span class="sxs-lookup"><span data-stu-id="abe69-130">String</span></span>        | <span data-ttu-id="abe69-131">Uma URL que abre o item no navegador no site do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="abe69-131">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="abe69-133">Opções de tipo</span><span class="sxs-lookup"><span data-stu-id="abe69-133">Type options</span></span>

<span data-ttu-id="abe69-134">A tabela a seguir define os valores possíveis para a propriedade **Type** .</span><span class="sxs-lookup"><span data-stu-id="abe69-134">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="abe69-135">Valor</span><span class="sxs-lookup"><span data-stu-id="abe69-135">Value</span></span>    | <span data-ttu-id="abe69-136">Função</span><span class="sxs-lookup"><span data-stu-id="abe69-136">Role</span></span>     | <span data-ttu-id="abe69-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="abe69-137">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="abe69-138">Um link somente de compartilhamento para exibição, permitindo o acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="abe69-138">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="abe69-139">Um link de compartilhamento de edição, permitindo o acesso de leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="abe69-139">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="abe69-p103">Um link de compartilhamento somente exibição que pode ser usado para inserir o conteúdo em uma página da Web de hospedagem. Os links de compartilhamento não estão disponíveis para OneDrive for Business ou SharePoint.</span><span class="sxs-lookup"><span data-stu-id="abe69-p103">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="abe69-142">Opções de escopo</span><span class="sxs-lookup"><span data-stu-id="abe69-142">Scope options</span></span>

<span data-ttu-id="abe69-143">A tabela a seguir define os valores possíveis para a propriedade **Scope** .</span><span class="sxs-lookup"><span data-stu-id="abe69-143">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="abe69-144">Valor</span><span class="sxs-lookup"><span data-stu-id="abe69-144">Value</span></span>            | <span data-ttu-id="abe69-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="abe69-145">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="abe69-146">Qualquer pessoa com o link tem acesso, sem a necessidade de fazer logon.</span><span class="sxs-lookup"><span data-stu-id="abe69-146">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="abe69-147">Isso pode incluir pessoas de fora da sua organização.</span><span class="sxs-lookup"><span data-stu-id="abe69-147">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="abe69-148">Qualquer pessoa que se inscreveu em sua organização (locatário) pode usar o link para obter acesso.</span><span class="sxs-lookup"><span data-stu-id="abe69-148">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="abe69-149">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="abe69-149">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="abe69-150">Somente as pessoas que já receberam acesso ao item por meio de outros meios podem acessar o item usando este link.</span><span class="sxs-lookup"><span data-stu-id="abe69-150">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="abe69-151">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="abe69-151">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="abe69-152">O link concede acesso somente a uma lista específica de pessoas.</span><span class="sxs-lookup"><span data-stu-id="abe69-152">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="abe69-153">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="abe69-153">Only available in OneDrive for Business and SharePoint.</span></span>

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
