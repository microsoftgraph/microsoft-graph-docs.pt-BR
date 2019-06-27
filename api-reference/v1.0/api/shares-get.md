---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Acessar itens compartilhados
localization_priority: Normal
ms.openlocfilehash: cd2bd6653d12aa3296889147c1b1c78eeaddc676
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279286"
---
# <a name="accessing-shared-driveitems"></a><span data-ttu-id="6bbd7-102">Acessar DriveItems compartilhados</span><span class="sxs-lookup"><span data-stu-id="6bbd7-102">Accessing shared DriveItems</span></span>

<span data-ttu-id="6bbd7-103">Acesse um [DriveItem](../resources/driveitem.md) compartilhado ou uma coleção de itens compartilhados usando um **shareId** ou uma URL de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="6bbd7-103">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="6bbd7-104">Para usar uma URL de compartilhamento com esta API, seu aplicativo precisa [transformar a URL em um token de compartilhamento](#encoding-sharing-urls).</span><span class="sxs-lookup"><span data-stu-id="6bbd7-104">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#encoding-sharing-urls).</span></span>

## <a name="permissions"></a><span data-ttu-id="6bbd7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6bbd7-105">Permissions</span></span>

<span data-ttu-id="6bbd7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bbd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bbd7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bbd7-108">Permission type</span></span>      | <span data-ttu-id="6bbd7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6bbd7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6bbd7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bbd7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6bbd7-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bbd7-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6bbd7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bbd7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bbd7-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bbd7-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6bbd7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bbd7-114">Application</span></span> | <span data-ttu-id="6bbd7-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bbd7-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6bbd7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bbd7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a><span data-ttu-id="6bbd7-117">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="6bbd7-117">Path parameters</span></span>

| <span data-ttu-id="6bbd7-118">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6bbd7-118">Parameter Name</span></span>                 | <span data-ttu-id="6bbd7-119">Valor</span><span class="sxs-lookup"><span data-stu-id="6bbd7-119">Value</span></span>    | <span data-ttu-id="6bbd7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bbd7-120">Description</span></span>                                                                         |
|:-------------------------------|:---------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="6bbd7-121">**shareIdOrEncodedSharingUrl**</span><span class="sxs-lookup"><span data-stu-id="6bbd7-121">**shareIdOrEncodedSharingUrl**</span></span> | `string` | <span data-ttu-id="6bbd7-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bbd7-122">Required.</span></span> <span data-ttu-id="6bbd7-123">Um token de compartilhamento retornado pela API ou uma URL de compartilhamento corretamente codificada.</span><span class="sxs-lookup"><span data-stu-id="6bbd7-123">A sharing token as returned by the API or a properly encoded sharing URL.</span></span> |

### <a name="encoding-sharing-urls"></a><span data-ttu-id="6bbd7-124">Codificação de URLs de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="6bbd7-124">Encoding sharing URLs</span></span>

<span data-ttu-id="6bbd7-125">Para codificar uma URL de compartilhamento, use a seguinte lógica:</span><span class="sxs-lookup"><span data-stu-id="6bbd7-125">To encode a sharing URL, use the following logic:</span></span>

1. <span data-ttu-id="6bbd7-126">Primeiro, use base64 para codificar a URL.</span><span class="sxs-lookup"><span data-stu-id="6bbd7-126">First, use base64 encode the URL.</span></span>
2. <span data-ttu-id="6bbd7-127">Converta o resultado codificado na base64 para o [formato base64url sem preenchimento](https://en.wikipedia.org/wiki/Base64) removendo caracteres `=` do final do valor, substituindo `/` por `_` e `+` por `-`.)</span><span class="sxs-lookup"><span data-stu-id="6bbd7-127">Convert the base64 encoded result to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by removing `=` characters from the end of the value, replacing `/` with `_` and `+` with `-`.)</span></span>
3. <span data-ttu-id="6bbd7-128">Acrescente `u!` ao início da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="6bbd7-128">Append `u!` to be beginning of the string.</span></span>

<span data-ttu-id="6bbd7-129">Por exemplo, para codificar uma URL em C#:</span><span class="sxs-lookup"><span data-stu-id="6bbd7-129">As an example, to encode a URL in C#:</span></span>

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="optional-request-headers"></a><span data-ttu-id="6bbd7-130">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="6bbd7-130">Optional request headers</span></span>

| <span data-ttu-id="6bbd7-131">Nome</span><span class="sxs-lookup"><span data-stu-id="6bbd7-131">Name</span></span>       | <span data-ttu-id="6bbd7-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bbd7-132">Type</span></span>   | <span data-ttu-id="6bbd7-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bbd7-133">Description</span></span>                                                    |
|:-----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="6bbd7-134">**Prefer**</span><span class="sxs-lookup"><span data-stu-id="6bbd7-134">**Prefer**</span></span> | <span data-ttu-id="6bbd7-135">string</span><span class="sxs-lookup"><span data-stu-id="6bbd7-135">string</span></span> | <span data-ttu-id="6bbd7-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6bbd7-136">Optional.</span></span> <span data-ttu-id="6bbd7-137">Defina como um dos `prefer` valores documentados abaixo.</span><span class="sxs-lookup"><span data-stu-id="6bbd7-137">Set to one of the `prefer` values documented below.</span></span>  |

### <a name="prefer-header-values"></a><span data-ttu-id="6bbd7-138">Preferir valores de cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6bbd7-138">Prefer header values</span></span>

| <span data-ttu-id="6bbd7-139">Nome</span><span class="sxs-lookup"><span data-stu-id="6bbd7-139">Name</span></span>                          | <span data-ttu-id="6bbd7-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bbd7-140">Description</span></span>                                                                                             |
|:------------------------------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6bbd7-141">redeemSharingLink</span><span class="sxs-lookup"><span data-stu-id="6bbd7-141">redeemSharingLink</span></span>             | <span data-ttu-id="6bbd7-142">Se o **shareIdOrEncodedSharingUrl** for um link de compartilhamento, conceda ao chamador acesso durável ao item</span><span class="sxs-lookup"><span data-stu-id="6bbd7-142">If the **shareIdOrEncodedSharingUrl** is a sharing link, grant the caller durable access to the item</span></span>    |
| <span data-ttu-id="6bbd7-143">redeemSharingLinkIfNecessary</span><span class="sxs-lookup"><span data-stu-id="6bbd7-143">redeemSharingLinkIfNecessary</span></span>  | <span data-ttu-id="6bbd7-144">O mesmo que redeemSharingLink, mas o acesso só é garantido para a duração da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bbd7-144">Same as redeemSharingLink, but access is only guaranteed to be granted for the duration of this request</span></span> |

<span data-ttu-id="6bbd7-145">redeemSharingLink deve ser considerado equivalente ao chamador navegando para o link de compartilhamento do navegador (aceitando o gesto de compartilhamento), enquanto o redeemSharingLinkIfNecessary se destina a cenários em que a intenção é simplesmente exibir o link do los.</span><span class="sxs-lookup"><span data-stu-id="6bbd7-145">redeemSharingLink should be considered equivalent to the caller navigating to the sharing link the browser (accepting the sharing gesture), whereas redeemSharingLinkIfNecessary is intended for scenarios where the intention is simply to peek at the link's metadata.</span></span>

## <a name="response"></a><span data-ttu-id="6bbd7-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bbd7-146">Response</span></span>

<span data-ttu-id="6bbd7-147">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [sharedDriveItem](../resources/shareddriveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bbd7-147">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bbd7-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6bbd7-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="6bbd7-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bbd7-149">Request</span></span>

<span data-ttu-id="6bbd7-150">Veja a seguir um exemplo da solicitação para recuperar um item compartilhado:</span><span class="sxs-lookup"><span data-stu-id="6bbd7-150">Here is an example of the request to retrieve a shared item:</span></span>

<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="response"></a><span data-ttu-id="6bbd7-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bbd7-151">Response</span></span>

<span data-ttu-id="6bbd7-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bbd7-152">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.sharedDriveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "B64397C8-07AE-43E4-920E-32BFB4331A5B",
  "name": "contoso project.docx",
  "owner": {
    "user": {
      "id": "98E88F1C-F8DC-47CC-A406-C090248B30E5",
      "displayName": "Ryan Gregg"
    }
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6bbd7-153">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6bbd7-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6bbd7-154">C#</span><span class="sxs-lookup"><span data-stu-id="6bbd7-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-shared-root-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6bbd7-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="6bbd7-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-shared-root-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6bbd7-156">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6bbd7-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-shared-root-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="6bbd7-157">Acessar diretamente o item compartilhado</span><span class="sxs-lookup"><span data-stu-id="6bbd7-157">Access the shared item directly</span></span>

<span data-ttu-id="6bbd7-p104">Embora [**SharedDriveItem**](../resources/shareddriveitem.md) contenha algumas informações úteis, a maioria dos aplicativos acessará diretamente o [DriveItem](../resources/driveitem.md) compartilhado. O recurso **SharedDriveItem** inclui **root** e relações **itens** que podem acessar o conteúdo no escopo do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="6bbd7-p104">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="6bbd7-160">Exemplo (arquivo único)</span><span class="sxs-lookup"><span data-stu-id="6bbd7-160">Example (single file)</span></span>

### <a name="request"></a><span data-ttu-id="6bbd7-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bbd7-161">Request</span></span>

<span data-ttu-id="6bbd7-162">Ao solicitar a relação **driveItem**, o **DriveItem** compartilhado será retornado.</span><span class="sxs-lookup"><span data-stu-id="6bbd7-162">By requesting the **driveItem** relationship, the **DriveItem** that was shared will be returned.</span></span>

<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```

### <a name="response"></a><span data-ttu-id="6bbd7-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bbd7-163">Response</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6bbd7-164">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6bbd7-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6bbd7-165">C#</span><span class="sxs-lookup"><span data-stu-id="6bbd7-165">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6bbd7-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="6bbd7-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6bbd7-167">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6bbd7-167">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-shared-folder"></a><span data-ttu-id="6bbd7-168">Exemplo (pasta compartilhada)</span><span class="sxs-lookup"><span data-stu-id="6bbd7-168">Example (shared folder)</span></span>

### <a name="request"></a><span data-ttu-id="6bbd7-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bbd7-169">Request</span></span>

<span data-ttu-id="6bbd7-170">Solicitando a relação **driveItem** e expandindo a coleção **children**, o **DriveItem** que foi compartilhado será retornado junto com os arquivos da pasta compartilhada.</span><span class="sxs-lookup"><span data-stu-id="6bbd7-170">By requesting the **driveItem** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>

<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```

### <a name="response"></a><span data-ttu-id="6bbd7-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bbd7-171">Response</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {},
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6bbd7-172">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6bbd7-172">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6bbd7-173">C#</span><span class="sxs-lookup"><span data-stu-id="6bbd7-173">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-expand-children-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6bbd7-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="6bbd7-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-expand-children-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6bbd7-175">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6bbd7-175">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-expand-children-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="error-responses"></a><span data-ttu-id="6bbd7-176">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="6bbd7-176">Error Responses</span></span>

<span data-ttu-id="6bbd7-177">Saiba mais sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="6bbd7-177">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="remarks"></a><span data-ttu-id="6bbd7-178">Comentários</span><span class="sxs-lookup"><span data-stu-id="6bbd7-178">Remarks</span></span>

* <span data-ttu-id="6bbd7-179">Para o OneDrive for Business e o SharePoint, a API Shares sempre requer autenticação e não pode ser usada para acessar conteúdo compartilhado anonimamente sem um contexto de usuário.</span><span class="sxs-lookup"><span data-stu-id="6bbd7-179">For OneDrive for Business and SharePoint, the Shares API always requires authentication and cannot be used to access anonymously shared content without a user context.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Access the contents of a sharing link with the OneDrive API.",
  "keywords": "shares,shared,sharing,share link, sharing link, share id, share token",
  "section": "documentation",
  "tocPath": "Sharing/Use a link",
  "suppressions": [
    "Error: /api-reference/v1.0/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
