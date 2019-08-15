---
author: JeremyKelley
description: Acesse um DriveItem compartilhado ou uma coleção de itens compartilhados usando um shareId ou uma URL de compartilhamento.
ms.date: 09/10/2017
title: Acessar itens compartilhados
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 705c7033309fe383ac0649609e783caa4c6acb63
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410119"
---
# <a name="accessing-shared-driveitems"></a><span data-ttu-id="a8e90-103">Acessar DriveItems compartilhados</span><span class="sxs-lookup"><span data-stu-id="a8e90-103">Accessing shared DriveItems</span></span>

<span data-ttu-id="a8e90-104">Acesse um [DriveItem](../resources/driveitem.md) compartilhado ou uma coleção de itens compartilhados usando um **shareId** ou uma URL de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="a8e90-104">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="a8e90-105">Para usar uma URL de compartilhamento com esta API, seu aplicativo precisa [transformar a URL em um token de compartilhamento](#encoding-sharing-urls).</span><span class="sxs-lookup"><span data-stu-id="a8e90-105">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#encoding-sharing-urls).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8e90-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8e90-106">Permissions</span></span>

<span data-ttu-id="a8e90-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8e90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8e90-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8e90-109">Permission type</span></span>      | <span data-ttu-id="a8e90-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8e90-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8e90-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8e90-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a8e90-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8e90-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a8e90-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8e90-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8e90-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8e90-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a8e90-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8e90-115">Application</span></span> | <span data-ttu-id="a8e90-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8e90-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8e90-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8e90-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a><span data-ttu-id="a8e90-118">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="a8e90-118">Path parameters</span></span>

| <span data-ttu-id="a8e90-119">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a8e90-119">Parameter Name</span></span>                 | <span data-ttu-id="a8e90-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a8e90-120">Value</span></span>    | <span data-ttu-id="a8e90-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8e90-121">Description</span></span>                                                                         |
|:-------------------------------|:---------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="a8e90-122">**shareIdOrEncodedSharingUrl**</span><span class="sxs-lookup"><span data-stu-id="a8e90-122">**shareIdOrEncodedSharingUrl**</span></span> | `string` | <span data-ttu-id="a8e90-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8e90-123">Required.</span></span> <span data-ttu-id="a8e90-124">Um token de compartilhamento retornado pela API ou uma URL de compartilhamento corretamente codificada.</span><span class="sxs-lookup"><span data-stu-id="a8e90-124">A sharing token as returned by the API or a properly encoded sharing URL.</span></span> |

### <a name="encoding-sharing-urls"></a><span data-ttu-id="a8e90-125">Codificação de URLs de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="a8e90-125">Encoding sharing URLs</span></span>

<span data-ttu-id="a8e90-126">Para codificar uma URL de compartilhamento, use a seguinte lógica:</span><span class="sxs-lookup"><span data-stu-id="a8e90-126">To encode a sharing URL, use the following logic:</span></span>

1. <span data-ttu-id="a8e90-127">Primeiro, use base64 para codificar a URL.</span><span class="sxs-lookup"><span data-stu-id="a8e90-127">First, use base64 encode the URL.</span></span>
2. <span data-ttu-id="a8e90-128">Converta o resultado codificado na base64 para o [formato base64url sem preenchimento](https://en.wikipedia.org/wiki/Base64) removendo caracteres `=` do final do valor, substituindo `/` por `_` e `+` por `-`.)</span><span class="sxs-lookup"><span data-stu-id="a8e90-128">Convert the base64 encoded result to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by removing `=` characters from the end of the value, replacing `/` with `_` and `+` with `-`.)</span></span>
3. <span data-ttu-id="a8e90-129">Acrescente `u!` ao início da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="a8e90-129">Append `u!` to be beginning of the string.</span></span>

<span data-ttu-id="a8e90-130">Por exemplo, para codificar uma URL em C#:</span><span class="sxs-lookup"><span data-stu-id="a8e90-130">As an example, to encode a URL in C#:</span></span>

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="optional-request-headers"></a><span data-ttu-id="a8e90-131">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="a8e90-131">Optional request headers</span></span>

| <span data-ttu-id="a8e90-132">Nome</span><span class="sxs-lookup"><span data-stu-id="a8e90-132">Name</span></span>       | <span data-ttu-id="a8e90-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8e90-133">Type</span></span>   | <span data-ttu-id="a8e90-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8e90-134">Description</span></span>                                                    |
|:-----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="a8e90-135">**Prefer**</span><span class="sxs-lookup"><span data-stu-id="a8e90-135">**Prefer**</span></span> | <span data-ttu-id="a8e90-136">string</span><span class="sxs-lookup"><span data-stu-id="a8e90-136">string</span></span> | <span data-ttu-id="a8e90-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a8e90-137">Optional.</span></span> <span data-ttu-id="a8e90-138">Defina como um dos `prefer` valores documentados abaixo.</span><span class="sxs-lookup"><span data-stu-id="a8e90-138">Set to one of the `prefer` values documented below.</span></span>  |

### <a name="prefer-header-values"></a><span data-ttu-id="a8e90-139">Preferir valores de cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8e90-139">Prefer header values</span></span>

| <span data-ttu-id="a8e90-140">Nome</span><span class="sxs-lookup"><span data-stu-id="a8e90-140">Name</span></span>                          | <span data-ttu-id="a8e90-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8e90-141">Description</span></span>                                                                                             |
|:------------------------------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a8e90-142">redeemSharingLink</span><span class="sxs-lookup"><span data-stu-id="a8e90-142">redeemSharingLink</span></span>             | <span data-ttu-id="a8e90-143">Se o **shareIdOrEncodedSharingUrl** for um link de compartilhamento, conceda ao chamador acesso durável ao item</span><span class="sxs-lookup"><span data-stu-id="a8e90-143">If the **shareIdOrEncodedSharingUrl** is a sharing link, grant the caller durable access to the item</span></span>    |
| <span data-ttu-id="a8e90-144">redeemSharingLinkIfNecessary</span><span class="sxs-lookup"><span data-stu-id="a8e90-144">redeemSharingLinkIfNecessary</span></span>  | <span data-ttu-id="a8e90-145">O mesmo que redeemSharingLink, mas o acesso só é garantido para a duração da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8e90-145">Same as redeemSharingLink, but access is only guaranteed to be granted for the duration of this request</span></span> |

<span data-ttu-id="a8e90-146">redeemSharingLink deve ser considerado equivalente ao chamador navegando para o link de compartilhamento do navegador (aceitando o gesto de compartilhamento), enquanto o redeemSharingLinkIfNecessary se destina a cenários em que a intenção é simplesmente exibir o link do los.</span><span class="sxs-lookup"><span data-stu-id="a8e90-146">redeemSharingLink should be considered equivalent to the caller navigating to the sharing link the browser (accepting the sharing gesture), whereas redeemSharingLinkIfNecessary is intended for scenarios where the intention is simply to peek at the link's metadata.</span></span>

## <a name="response"></a><span data-ttu-id="a8e90-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8e90-147">Response</span></span>

<span data-ttu-id="a8e90-148">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [sharedDriveItem](../resources/shareddriveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8e90-148">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8e90-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8e90-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8e90-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8e90-150">Request</span></span>

<span data-ttu-id="a8e90-151">Veja a seguir um exemplo da solicitação para recuperar um item compartilhado:</span><span class="sxs-lookup"><span data-stu-id="a8e90-151">Here is an example of the request to retrieve a shared item:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a8e90-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8e90-152">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a8e90-153">C#</span><span class="sxs-lookup"><span data-stu-id="a8e90-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8e90-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8e90-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a8e90-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a8e90-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8e90-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8e90-156">Response</span></span>

<span data-ttu-id="a8e90-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8e90-157">Here is an example of the response.</span></span>

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

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="a8e90-158">Acessar diretamente o item compartilhado</span><span class="sxs-lookup"><span data-stu-id="a8e90-158">Access the shared item directly</span></span>

<span data-ttu-id="a8e90-p104">Embora [**SharedDriveItem**](../resources/shareddriveitem.md) contenha algumas informações úteis, a maioria dos aplicativos acessará diretamente o [DriveItem](../resources/driveitem.md) compartilhado. O recurso **SharedDriveItem** inclui **root** e relações **itens** que podem acessar o conteúdo no escopo do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="a8e90-p104">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="a8e90-161">Exemplo (arquivo único)</span><span class="sxs-lookup"><span data-stu-id="a8e90-161">Example (single file)</span></span>

### <a name="request"></a><span data-ttu-id="a8e90-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8e90-162">Request</span></span>

<span data-ttu-id="a8e90-163">Ao solicitar a relação **driveItem**, o **DriveItem** compartilhado será retornado.</span><span class="sxs-lookup"><span data-stu-id="a8e90-163">By requesting the **driveItem** relationship, the **DriveItem** that was shared will be returned.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a8e90-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8e90-164">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a8e90-165">C#</span><span class="sxs-lookup"><span data-stu-id="a8e90-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-driveitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8e90-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8e90-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-driveitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a8e90-167">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a8e90-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-driveitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8e90-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8e90-168">Response</span></span>

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

## <a name="example-shared-folder"></a><span data-ttu-id="a8e90-169">Exemplo (pasta compartilhada)</span><span class="sxs-lookup"><span data-stu-id="a8e90-169">Example (shared folder)</span></span>

### <a name="request"></a><span data-ttu-id="a8e90-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8e90-170">Request</span></span>

<span data-ttu-id="a8e90-171">Solicitando a relação **driveItem** e expandindo a coleção **children**, o **DriveItem** que foi compartilhado será retornado junto com os arquivos da pasta compartilhada.</span><span class="sxs-lookup"><span data-stu-id="a8e90-171">By requesting the **driveItem** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a8e90-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8e90-172">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a8e90-173">C#</span><span class="sxs-lookup"><span data-stu-id="a8e90-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-driveitem-expand-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8e90-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8e90-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-driveitem-expand-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a8e90-175">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a8e90-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-driveitem-expand-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8e90-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8e90-176">Response</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="a8e90-177">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="a8e90-177">Error Responses</span></span>

<span data-ttu-id="a8e90-178">Saiba mais sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="a8e90-178">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="remarks"></a><span data-ttu-id="a8e90-179">Comentários</span><span class="sxs-lookup"><span data-stu-id="a8e90-179">Remarks</span></span>

* <span data-ttu-id="a8e90-180">Para o OneDrive for Business e o SharePoint, a API Shares sempre requer autenticação e não pode ser usada para acessar conteúdo compartilhado anonimamente sem um contexto de usuário.</span><span class="sxs-lookup"><span data-stu-id="a8e90-180">For OneDrive for Business and SharePoint, the Shares API always requires authentication and cannot be used to access anonymously shared content without a user context.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Access the contents of a sharing link with the OneDrive API.",
  "keywords": "shares,shared,sharing,share link, sharing link, share id, share token",
  "section": "documentation",
  "tocPath": "Sharing/Use a link",
  "suppressions": [
  ]
} -->
