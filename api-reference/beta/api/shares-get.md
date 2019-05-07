---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Acessar itens compartilhados
localization_priority: Normal
ms.openlocfilehash: 1204239bf2e1a6f5fca271d115169c8f06852a33
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638659"
---
# <a name="accessing-shared-driveitems"></a><span data-ttu-id="3bc67-102">Acessar DriveItems compartilhados</span><span class="sxs-lookup"><span data-stu-id="3bc67-102">Accessing shared DriveItems</span></span>

<span data-ttu-id="3bc67-103">Acesse um [DriveItem](../resources/driveitem.md) compartilhado ou uma coleção de itens compartilhados usando um **shareId** ou uma URL de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="3bc67-103">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="3bc67-104">Para usar uma URL de compartilhamento com esta API, seu aplicativo precisa [transformar a URL em um token de compartilhamento](#encoding-sharing-urls).</span><span class="sxs-lookup"><span data-stu-id="3bc67-104">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#encoding-sharing-urls).</span></span>

## <a name="permissions"></a><span data-ttu-id="3bc67-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3bc67-105">Permissions</span></span>

<span data-ttu-id="3bc67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bc67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bc67-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3bc67-108">Permission type</span></span>      | <span data-ttu-id="3bc67-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3bc67-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bc67-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3bc67-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3bc67-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bc67-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3bc67-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3bc67-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bc67-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bc67-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3bc67-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3bc67-114">Application</span></span> | <span data-ttu-id="3bc67-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bc67-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bc67-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3bc67-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a><span data-ttu-id="3bc67-117">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="3bc67-117">Path parameters</span></span>

| <span data-ttu-id="3bc67-118">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3bc67-118">Parameter Name</span></span>                 | <span data-ttu-id="3bc67-119">Valor</span><span class="sxs-lookup"><span data-stu-id="3bc67-119">Value</span></span>    | <span data-ttu-id="3bc67-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bc67-120">Description</span></span>                                                                         |
|:-------------------------------|:---------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="3bc67-121">**shareIdOrEncodedSharingUrl**</span><span class="sxs-lookup"><span data-stu-id="3bc67-121">**shareIdOrEncodedSharingUrl**</span></span> | `string` | <span data-ttu-id="3bc67-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3bc67-122">Required.</span></span> <span data-ttu-id="3bc67-123">Um token de compartilhamento retornado pela API ou uma URL de compartilhamento corretamente codificada.</span><span class="sxs-lookup"><span data-stu-id="3bc67-123">A sharing token as returned by the API or a properly encoded sharing URL.</span></span> |

### <a name="encoding-sharing-urls"></a><span data-ttu-id="3bc67-124">Codificação de URLs de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="3bc67-124">Encoding sharing URLs</span></span>

<span data-ttu-id="3bc67-125">Para codificar uma URL de compartilhamento, use a seguinte lógica:</span><span class="sxs-lookup"><span data-stu-id="3bc67-125">To encode a sharing URL, use the following logic:</span></span>

1. <span data-ttu-id="3bc67-126">Primeiro, use base64 para codificar a URL.</span><span class="sxs-lookup"><span data-stu-id="3bc67-126">First, use base64 encode the URL.</span></span>
2. <span data-ttu-id="3bc67-127">Converta o resultado codificado na base64 para o [formato base64url sem preenchimento](https://en.wikipedia.org/wiki/Base64) removendo caracteres `=` do final do valor, substituindo `/` por `_` e `+` por `-`.)</span><span class="sxs-lookup"><span data-stu-id="3bc67-127">Convert the base64 encoded result to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by removing `=` characters from the end of the value, replacing `/` with `_` and `+` with `-`.)</span></span>
3. <span data-ttu-id="3bc67-128">Acrescente `u!` ao início da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="3bc67-128">Append `u!` to be beginning of the string.</span></span>

<span data-ttu-id="3bc67-129">Por exemplo, para codificar uma URL em C#:</span><span class="sxs-lookup"><span data-stu-id="3bc67-129">As an example, to encode a URL in C#:</span></span>

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="optional-request-headers"></a><span data-ttu-id="3bc67-130">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="3bc67-130">Optional request headers</span></span>

| <span data-ttu-id="3bc67-131">Nome</span><span class="sxs-lookup"><span data-stu-id="3bc67-131">Name</span></span>       | <span data-ttu-id="3bc67-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bc67-132">Type</span></span>   | <span data-ttu-id="3bc67-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bc67-133">Description</span></span>                                                    |
|:-----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="3bc67-134">**Prefer**</span><span class="sxs-lookup"><span data-stu-id="3bc67-134">**Prefer**</span></span> | <span data-ttu-id="3bc67-135">string</span><span class="sxs-lookup"><span data-stu-id="3bc67-135">string</span></span> | <span data-ttu-id="3bc67-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3bc67-136">Optional.</span></span> <span data-ttu-id="3bc67-137">Defina como um dos `prefer` valores documentados abaixo.</span><span class="sxs-lookup"><span data-stu-id="3bc67-137">Set to one of the `prefer` values documented below.</span></span>  |

### <a name="prefer-header-values"></a><span data-ttu-id="3bc67-138">Preferir valores de cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3bc67-138">Prefer header values</span></span>

| <span data-ttu-id="3bc67-139">Nome</span><span class="sxs-lookup"><span data-stu-id="3bc67-139">Name</span></span>                          | <span data-ttu-id="3bc67-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bc67-140">Description</span></span>                                                                                             |
|:------------------------------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3bc67-141">redeemSharingLink</span><span class="sxs-lookup"><span data-stu-id="3bc67-141">redeemSharingLink</span></span>             | <span data-ttu-id="3bc67-142">Se o **shareIdOrEncodedSharingUrl** for um link de compartilhamento, conceda ao chamador acesso durável ao item</span><span class="sxs-lookup"><span data-stu-id="3bc67-142">If the **shareIdOrEncodedSharingUrl** is a sharing link, grant the caller durable access to the item</span></span>    |
| <span data-ttu-id="3bc67-143">redeemSharingLinkIfNecessary</span><span class="sxs-lookup"><span data-stu-id="3bc67-143">redeemSharingLinkIfNecessary</span></span>  | <span data-ttu-id="3bc67-144">O mesmo que redeemSharingLink, mas o acesso só é garantido para a duração da solicitação</span><span class="sxs-lookup"><span data-stu-id="3bc67-144">Same as redeemSharingLink, but access is only guaranteed to be granted for the duration of this request</span></span> |

<span data-ttu-id="3bc67-145">redeemSharingLink deve ser considerado equivalente ao chamador navegando para o link de compartilhamento do navegador (aceitando o gesto de compartilhamento), enquanto o redeemSharingLinkIfNecessary se destina a cenários em que a intenção é simplesmente exibir o link do los.</span><span class="sxs-lookup"><span data-stu-id="3bc67-145">redeemSharingLink should be considered equivalent to the caller navigating to the sharing link the browser (accepting the sharing gesture), whereas redeemSharingLinkIfNecessary is intended for scenarios where the intention is simply to peek at the link's metadata.</span></span>

## <a name="response"></a><span data-ttu-id="3bc67-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bc67-146">Response</span></span>

<span data-ttu-id="3bc67-147">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [sharedDriveItem](../resources/shareddriveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3bc67-147">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bc67-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3bc67-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bc67-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bc67-149">Request</span></span>

<span data-ttu-id="3bc67-150">Veja a seguir um exemplo da solicitação para recuperar um item compartilhado:</span><span class="sxs-lookup"><span data-stu-id="3bc67-150">Here is an example of the request to retrieve a shared item:</span></span>

<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="response"></a><span data-ttu-id="3bc67-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bc67-151">Response</span></span>

<span data-ttu-id="3bc67-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3bc67-152">Here is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3bc67-153">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3bc67-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3bc67-154">Basic</span><span class="sxs-lookup"><span data-stu-id="3bc67-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-shared-root-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3bc67-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bc67-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-shared-root-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="3bc67-156">Acessar diretamente o item compartilhado</span><span class="sxs-lookup"><span data-stu-id="3bc67-156">Access the shared item directly</span></span>

<span data-ttu-id="3bc67-p104">Embora [**SharedDriveItem**](../resources/shareddriveitem.md) contenha algumas informações úteis, a maioria dos aplicativos acessará diretamente o [DriveItem](../resources/driveitem.md) compartilhado. O recurso **SharedDriveItem** inclui **root** e relações **itens** que podem acessar o conteúdo no escopo do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="3bc67-p104">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="3bc67-159">Exemplo (arquivo único)</span><span class="sxs-lookup"><span data-stu-id="3bc67-159">Example (single file)</span></span>

### <a name="request"></a><span data-ttu-id="3bc67-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bc67-160">Request</span></span>

<span data-ttu-id="3bc67-161">Ao solicitar a relação **driveItem**, o **DriveItem** compartilhado será retornado.</span><span class="sxs-lookup"><span data-stu-id="3bc67-161">By requesting the **driveItem** relationship, the **DriveItem** that was shared will be returned.</span></span>

<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```

### <a name="response"></a><span data-ttu-id="3bc67-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bc67-162">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3bc67-163">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3bc67-163">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3bc67-164">Basic</span><span class="sxs-lookup"><span data-stu-id="3bc67-164">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3bc67-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bc67-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-shared-folder"></a><span data-ttu-id="3bc67-166">Exemplo (pasta compartilhada)</span><span class="sxs-lookup"><span data-stu-id="3bc67-166">Example (shared folder)</span></span>

### <a name="request"></a><span data-ttu-id="3bc67-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bc67-167">Request</span></span>

<span data-ttu-id="3bc67-168">Solicitando a relação **driveItem** e expandindo a coleção **children**, o **DriveItem** que foi compartilhado será retornado junto com os arquivos da pasta compartilhada.</span><span class="sxs-lookup"><span data-stu-id="3bc67-168">By requesting the **driveItem** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>

<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```

### <a name="response"></a><span data-ttu-id="3bc67-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bc67-169">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3bc67-170">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3bc67-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3bc67-171">Basic</span><span class="sxs-lookup"><span data-stu-id="3bc67-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-expand-children-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3bc67-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bc67-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-expand-children-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="error-responses"></a><span data-ttu-id="3bc67-173">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="3bc67-173">Error Responses</span></span>

<span data-ttu-id="3bc67-174">Saiba mais sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="3bc67-174">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="remarks"></a><span data-ttu-id="3bc67-175">Comentários</span><span class="sxs-lookup"><span data-stu-id="3bc67-175">Remarks</span></span>

* <span data-ttu-id="3bc67-176">Para o OneDrive for Business e o SharePoint, a API Shares sempre requer autenticação e não pode ser usada para acessar conteúdo compartilhado anonimamente sem um contexto de usuário.</span><span class="sxs-lookup"><span data-stu-id="3bc67-176">For OneDrive for Business and SharePoint, the Shares API always requires authentication and cannot be used to access anonymously shared content without a user context.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Access the contents of a sharing link with the OneDrive API.",
  "keywords": "shares,shared,sharing,share link, sharing link, share id, share token",
  "section": "documentation",
  "tocPath": "Sharing/Use a link",
  "suppressions": [
    "Error: /api-reference/beta/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
