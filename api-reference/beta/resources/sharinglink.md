---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: c5a08ca3a1a7b91d5cd2277a71f1301adf5edc93
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343070"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="8db67-102">tipo de recurso sharingLink</span><span class="sxs-lookup"><span data-stu-id="8db67-102">sharingLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8db67-103">O recurso **sharingLink** agrupa itens de dados relacionados ao link em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="8db67-103">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="8db67-104">Se um recurso de [**permissão**](permission.md) tiver uma faceta **sharingLink** não nula, a permissão representa um link de compartilhamento (em oposição às permissões concedidas a uma pessoa ou grupo).</span><span class="sxs-lookup"><span data-stu-id="8db67-104">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="8db67-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8db67-105">JSON representation</span></span>

<span data-ttu-id="8db67-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8db67-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="8db67-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8db67-107">Properties</span></span>

| <span data-ttu-id="8db67-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8db67-108">Property</span></span>       | <span data-ttu-id="8db67-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8db67-109">Type</span></span>          | <span data-ttu-id="8db67-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8db67-110">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="8db67-111">aplicativo</span><span class="sxs-lookup"><span data-stu-id="8db67-111">application</span></span>    | <span data-ttu-id="8db67-112">[identity][]</span><span class="sxs-lookup"><span data-stu-id="8db67-112">[identity][]</span></span>  | <span data-ttu-id="8db67-113">O aplicativo ao qual o link está associado.</span><span class="sxs-lookup"><span data-stu-id="8db67-113">The app the link is associated with.</span></span>
| <span data-ttu-id="8db67-114">type</span><span class="sxs-lookup"><span data-stu-id="8db67-114">type</span></span>           | <span data-ttu-id="8db67-115">String</span><span class="sxs-lookup"><span data-stu-id="8db67-115">String</span></span>        | <span data-ttu-id="8db67-116">O tipo do link criado.</span><span class="sxs-lookup"><span data-stu-id="8db67-116">The type of the link created.</span></span>
| <span data-ttu-id="8db67-117">scope</span><span class="sxs-lookup"><span data-stu-id="8db67-117">scope</span></span>          | <span data-ttu-id="8db67-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8db67-118">String</span></span>        | <span data-ttu-id="8db67-p101">O escopo do link representado por esta permissão. O valor `anonymous` indica que o link é utilizável por qualquer pessoa; `organization` indica que o link só é útil para usuários conectados ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="8db67-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="8db67-121">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="8db67-121">preventsDownload</span></span> | <span data-ttu-id="8db67-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="8db67-122">Boolean</span></span>       | <span data-ttu-id="8db67-123">Se true, o usuário só pode usar este link para exibir o item na Web e não pode usá-lo para baixar o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="8db67-123">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="8db67-124">Somente para o OneDrive for Business e o SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8db67-124">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="8db67-125">webHtml</span><span class="sxs-lookup"><span data-stu-id="8db67-125">webHtml</span></span>        | <span data-ttu-id="8db67-126">String</span><span class="sxs-lookup"><span data-stu-id="8db67-126">String</span></span>        | <span data-ttu-id="8db67-127">Para links `embed`, essa propriedade contém o código HTML para um elemento `<iframe>` que inserirá o item em uma página da Web.</span><span class="sxs-lookup"><span data-stu-id="8db67-127">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="8db67-128">webUrl</span><span class="sxs-lookup"><span data-stu-id="8db67-128">webUrl</span></span>         | <span data-ttu-id="8db67-129">String</span><span class="sxs-lookup"><span data-stu-id="8db67-129">String</span></span>        | <span data-ttu-id="8db67-130">Uma URL que abre o item no navegador no site do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8db67-130">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="8db67-132">Opções de tipo</span><span class="sxs-lookup"><span data-stu-id="8db67-132">Type options</span></span>

<span data-ttu-id="8db67-133">A tabela a seguir define os valores possíveis para a propriedade **Type** .</span><span class="sxs-lookup"><span data-stu-id="8db67-133">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="8db67-134">Valor</span><span class="sxs-lookup"><span data-stu-id="8db67-134">Value</span></span>    | <span data-ttu-id="8db67-135">Função</span><span class="sxs-lookup"><span data-stu-id="8db67-135">Role</span></span>     | <span data-ttu-id="8db67-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="8db67-136">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="8db67-137">Um link somente de compartilhamento para exibição, permitindo o acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8db67-137">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="8db67-138">Um link de compartilhamento de edição, permitindo o acesso de leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="8db67-138">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="8db67-p103">Um link de compartilhamento somente exibição que pode ser usado para inserir o conteúdo em uma página da Web de hospedagem. Os links de compartilhamento não estão disponíveis para OneDrive for Business ou SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8db67-p103">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="8db67-141">Opções de escopo</span><span class="sxs-lookup"><span data-stu-id="8db67-141">Scope options</span></span>

<span data-ttu-id="8db67-142">A tabela a seguir define os valores possíveis para a propriedade **Scope** .</span><span class="sxs-lookup"><span data-stu-id="8db67-142">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="8db67-143">Valor</span><span class="sxs-lookup"><span data-stu-id="8db67-143">Value</span></span>            | <span data-ttu-id="8db67-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="8db67-144">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="8db67-145">Qualquer pessoa com o link tem acesso, sem a necessidade de fazer logon.</span><span class="sxs-lookup"><span data-stu-id="8db67-145">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="8db67-146">Isso pode incluir pessoas de fora da sua organização.</span><span class="sxs-lookup"><span data-stu-id="8db67-146">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="8db67-147">Qualquer pessoa que se inscreveu em sua organização (locatário) pode usar o link para obter acesso.</span><span class="sxs-lookup"><span data-stu-id="8db67-147">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="8db67-148">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8db67-148">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="8db67-149">Somente as pessoas que já receberam acesso ao item por meio de outros meios podem acessar o item usando este link.</span><span class="sxs-lookup"><span data-stu-id="8db67-149">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="8db67-150">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8db67-150">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="8db67-151">O link concede acesso somente a uma lista específica de pessoas.</span><span class="sxs-lookup"><span data-stu-id="8db67-151">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="8db67-152">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8db67-152">Only available in OneDrive for Business and SharePoint.</span></span>

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
