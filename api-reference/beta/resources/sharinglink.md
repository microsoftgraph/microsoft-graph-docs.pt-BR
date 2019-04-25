---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: 7f0ecdbb498ee75133ec9499027f7cfdc6191327
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583820"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="0b5aa-102">tipo de recurso sharingLink</span><span class="sxs-lookup"><span data-stu-id="0b5aa-102">sharingLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b5aa-103">O recurso **sharingLink** agrupa itens de dados relacionados ao link em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-103">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="0b5aa-104">Se um recurso de [**permissão**](permission.md) tiver uma faceta **sharingLink** não nula, a permissão representa um link de compartilhamento (em oposição às permissões concedidas a uma pessoa ou grupo).</span><span class="sxs-lookup"><span data-stu-id="0b5aa-104">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b5aa-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b5aa-105">JSON representation</span></span>

<span data-ttu-id="0b5aa-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="0b5aa-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b5aa-107">Properties</span></span>

| <span data-ttu-id="0b5aa-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b5aa-108">Property</span></span>       | <span data-ttu-id="0b5aa-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b5aa-109">Type</span></span>          | <span data-ttu-id="0b5aa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b5aa-110">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="0b5aa-111">aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b5aa-111">application</span></span>    | <span data-ttu-id="0b5aa-112">[identity][]</span><span class="sxs-lookup"><span data-stu-id="0b5aa-112">[identity][]</span></span>  | <span data-ttu-id="0b5aa-113">O aplicativo ao qual o link está associado.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-113">The app the link is associated with.</span></span>
| <span data-ttu-id="0b5aa-114">type</span><span class="sxs-lookup"><span data-stu-id="0b5aa-114">type</span></span>           | <span data-ttu-id="0b5aa-115">String</span><span class="sxs-lookup"><span data-stu-id="0b5aa-115">String</span></span>        | <span data-ttu-id="0b5aa-116">O tipo do link criado.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-116">The type of the link created.</span></span>
| <span data-ttu-id="0b5aa-117">scope</span><span class="sxs-lookup"><span data-stu-id="0b5aa-117">scope</span></span>          | <span data-ttu-id="0b5aa-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b5aa-118">String</span></span>        | <span data-ttu-id="0b5aa-p101">O escopo do link representado por esta permissão. O valor `anonymous` indica que o link é utilizável por qualquer pessoa; `organization` indica que o link só é útil para usuários conectados ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="0b5aa-121">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="0b5aa-121">preventsDownload</span></span> | <span data-ttu-id="0b5aa-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b5aa-122">Boolean</span></span>       | <span data-ttu-id="0b5aa-123">Se true, o usuário só pode usar este link para exibir o item na Web e não pode usá-lo para baixar o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-123">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="0b5aa-124">Somente para o OneDrive for Business e o SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-124">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="0b5aa-125">webHtml</span><span class="sxs-lookup"><span data-stu-id="0b5aa-125">webHtml</span></span>        | <span data-ttu-id="0b5aa-126">String</span><span class="sxs-lookup"><span data-stu-id="0b5aa-126">String</span></span>        | <span data-ttu-id="0b5aa-127">Para links `embed`, essa propriedade contém o código HTML para um elemento `<iframe>` que inserirá o item em uma página da Web.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-127">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="0b5aa-128">webUrl</span><span class="sxs-lookup"><span data-stu-id="0b5aa-128">webUrl</span></span>         | <span data-ttu-id="0b5aa-129">String</span><span class="sxs-lookup"><span data-stu-id="0b5aa-129">String</span></span>        | <span data-ttu-id="0b5aa-130">Uma URL que abre o item no navegador no site do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-130">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="0b5aa-132">Opções de tipo</span><span class="sxs-lookup"><span data-stu-id="0b5aa-132">Type options</span></span>

<span data-ttu-id="0b5aa-133">A tabela a seguir define os valores possíveis para a propriedade **Type** .</span><span class="sxs-lookup"><span data-stu-id="0b5aa-133">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="0b5aa-134">Valor</span><span class="sxs-lookup"><span data-stu-id="0b5aa-134">Value</span></span>    | <span data-ttu-id="0b5aa-135">Função</span><span class="sxs-lookup"><span data-stu-id="0b5aa-135">Role</span></span>     | <span data-ttu-id="0b5aa-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b5aa-136">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="0b5aa-137">Um link somente de compartilhamento para exibição, permitindo o acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-137">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="0b5aa-138">Um link de compartilhamento de edição, permitindo o acesso de leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-138">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="0b5aa-p103">Um link de compartilhamento somente exibição que pode ser usado para inserir o conteúdo em uma página da Web de hospedagem. Os links de compartilhamento não estão disponíveis para OneDrive for Business ou SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-p103">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="0b5aa-141">Opções de escopo</span><span class="sxs-lookup"><span data-stu-id="0b5aa-141">Scope options</span></span>

<span data-ttu-id="0b5aa-142">A tabela a seguir define os valores possíveis para a propriedade **Scope** .</span><span class="sxs-lookup"><span data-stu-id="0b5aa-142">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="0b5aa-143">Valor</span><span class="sxs-lookup"><span data-stu-id="0b5aa-143">Value</span></span>            | <span data-ttu-id="0b5aa-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b5aa-144">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="0b5aa-145">Qualquer pessoa com o link tem acesso, sem a necessidade de fazer logon.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-145">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="0b5aa-146">Isso pode incluir pessoas de fora da sua organização.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-146">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="0b5aa-147">Qualquer pessoa que se inscreveu em sua organização (locatário) pode usar o link para obter acesso.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-147">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="0b5aa-148">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-148">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="0b5aa-149">Somente as pessoas que já receberam acesso ao item por meio de outros meios podem acessar o item usando este link.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-149">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="0b5aa-150">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-150">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="0b5aa-151">O link concede acesso somente a uma lista específica de pessoas.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-151">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="0b5aa-152">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0b5aa-152">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharinglink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
