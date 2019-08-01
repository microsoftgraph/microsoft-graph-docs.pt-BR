---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Acessar itens compartilhados
localization_priority: Normal
description: Acesse um DriveItem compartilhado ou uma coleção de itens compartilhados usando um shareId ou uma URL de compartilhamento.
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: d1080c42d3dd6471b2c09ac5a6d013f8e0c4986b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021512"
---
# <a name="accessing-shared-driveitems"></a><span data-ttu-id="c3bac-103">Acessar DriveItems compartilhados</span><span class="sxs-lookup"><span data-stu-id="c3bac-103">Accessing shared DriveItems</span></span>

<span data-ttu-id="c3bac-104">Acesse um [DriveItem](../resources/driveitem.md) compartilhado ou uma coleção de itens compartilhados usando um **shareId** ou uma URL de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="c3bac-104">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="c3bac-105">Para usar uma URL de compartilhamento com esta API, seu aplicativo precisa [transformar a URL em um token de compartilhamento](#encoding-sharing-urls).</span><span class="sxs-lookup"><span data-stu-id="c3bac-105">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#encoding-sharing-urls).</span></span>

## <a name="permissions"></a><span data-ttu-id="c3bac-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3bac-106">Permissions</span></span>

<span data-ttu-id="c3bac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3bac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3bac-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3bac-109">Permission type</span></span>      | <span data-ttu-id="c3bac-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3bac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3bac-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3bac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c3bac-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3bac-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c3bac-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3bac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3bac-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3bac-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c3bac-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3bac-115">Application</span></span> | <span data-ttu-id="c3bac-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3bac-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3bac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3bac-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a><span data-ttu-id="c3bac-118">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="c3bac-118">Path parameters</span></span>

| <span data-ttu-id="c3bac-119">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c3bac-119">Parameter Name</span></span>                 | <span data-ttu-id="c3bac-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c3bac-120">Value</span></span>    | <span data-ttu-id="c3bac-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3bac-121">Description</span></span>                                                                         |
|:-------------------------------|:---------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="c3bac-122">**shareIdOrEncodedSharingUrl**</span><span class="sxs-lookup"><span data-stu-id="c3bac-122">**shareIdOrEncodedSharingUrl**</span></span> | `string` | <span data-ttu-id="c3bac-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3bac-123">Required.</span></span> <span data-ttu-id="c3bac-124">Um token de compartilhamento retornado pela API ou uma URL de compartilhamento corretamente codificada.</span><span class="sxs-lookup"><span data-stu-id="c3bac-124">A sharing token as returned by the API or a properly encoded sharing URL.</span></span> |

### <a name="encoding-sharing-urls"></a><span data-ttu-id="c3bac-125">Codificação de URLs de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="c3bac-125">Encoding sharing URLs</span></span>

<span data-ttu-id="c3bac-126">Para codificar uma URL de compartilhamento, use a seguinte lógica:</span><span class="sxs-lookup"><span data-stu-id="c3bac-126">To encode a sharing URL, use the following logic:</span></span>

1. <span data-ttu-id="c3bac-127">Primeiro, use base64 para codificar a URL.</span><span class="sxs-lookup"><span data-stu-id="c3bac-127">First, use base64 encode the URL.</span></span>
2. <span data-ttu-id="c3bac-128">Converta o resultado codificado na base64 para o [formato base64url sem preenchimento](https://en.wikipedia.org/wiki/Base64) removendo caracteres `=` do final do valor, substituindo `/` por `_` e `+` por `-`.)</span><span class="sxs-lookup"><span data-stu-id="c3bac-128">Convert the base64 encoded result to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by removing `=` characters from the end of the value, replacing `/` with `_` and `+` with `-`.)</span></span>
3. <span data-ttu-id="c3bac-129">Acrescente `u!` ao início da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="c3bac-129">Append `u!` to be beginning of the string.</span></span>

<span data-ttu-id="c3bac-130">Por exemplo, para codificar uma URL em C#:</span><span class="sxs-lookup"><span data-stu-id="c3bac-130">As an example, to encode a URL in C#:</span></span>

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="optional-request-headers"></a><span data-ttu-id="c3bac-131">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c3bac-131">Optional request headers</span></span>

| <span data-ttu-id="c3bac-132">Nome</span><span class="sxs-lookup"><span data-stu-id="c3bac-132">Name</span></span>       | <span data-ttu-id="c3bac-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3bac-133">Type</span></span>   | <span data-ttu-id="c3bac-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3bac-134">Description</span></span>                                                    |
|:-----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="c3bac-135">**Prefer**</span><span class="sxs-lookup"><span data-stu-id="c3bac-135">**Prefer**</span></span> | <span data-ttu-id="c3bac-136">string</span><span class="sxs-lookup"><span data-stu-id="c3bac-136">string</span></span> | <span data-ttu-id="c3bac-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c3bac-137">Optional.</span></span> <span data-ttu-id="c3bac-138">Defina como um dos `prefer` valores documentados abaixo.</span><span class="sxs-lookup"><span data-stu-id="c3bac-138">Set to one of the `prefer` values documented below.</span></span>  |

### <a name="prefer-header-values"></a><span data-ttu-id="c3bac-139">Preferir valores de cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c3bac-139">Prefer header values</span></span>

| <span data-ttu-id="c3bac-140">Nome</span><span class="sxs-lookup"><span data-stu-id="c3bac-140">Name</span></span>                          | <span data-ttu-id="c3bac-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3bac-141">Description</span></span>                                                                                             |
|:------------------------------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c3bac-142">redeemSharingLink</span><span class="sxs-lookup"><span data-stu-id="c3bac-142">redeemSharingLink</span></span>             | <span data-ttu-id="c3bac-143">Se o **shareIdOrEncodedSharingUrl** for um link de compartilhamento, conceda ao chamador acesso durável ao item</span><span class="sxs-lookup"><span data-stu-id="c3bac-143">If the **shareIdOrEncodedSharingUrl** is a sharing link, grant the caller durable access to the item</span></span>    |
| <span data-ttu-id="c3bac-144">redeemSharingLinkIfNecessary</span><span class="sxs-lookup"><span data-stu-id="c3bac-144">redeemSharingLinkIfNecessary</span></span>  | <span data-ttu-id="c3bac-145">O mesmo que redeemSharingLink, mas o acesso só é garantido para a duração da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3bac-145">Same as redeemSharingLink, but access is only guaranteed to be granted for the duration of this request</span></span> |

<span data-ttu-id="c3bac-146">redeemSharingLink deve ser considerado equivalente ao chamador navegando para o link de compartilhamento do navegador (aceitando o gesto de compartilhamento), enquanto o redeemSharingLinkIfNecessary se destina a cenários em que a intenção é simplesmente exibir o link do los.</span><span class="sxs-lookup"><span data-stu-id="c3bac-146">redeemSharingLink should be considered equivalent to the caller navigating to the sharing link the browser (accepting the sharing gesture), whereas redeemSharingLinkIfNecessary is intended for scenarios where the intention is simply to peek at the link's metadata.</span></span>

## <a name="response"></a><span data-ttu-id="c3bac-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3bac-147">Response</span></span>

<span data-ttu-id="c3bac-148">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [sharedDriveItem](../resources/shareddriveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3bac-148">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3bac-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3bac-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3bac-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3bac-150">Request</span></span>

<span data-ttu-id="c3bac-151">Veja a seguir um exemplo da solicitação para recuperar um item compartilhado:</span><span class="sxs-lookup"><span data-stu-id="c3bac-151">Here is an example of the request to retrieve a shared item:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c3bac-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3bac-152">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3bac-153">C#</span><span class="sxs-lookup"><span data-stu-id="c3bac-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3bac-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="c3bac-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3bac-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c3bac-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c3bac-156">Java</span><span class="sxs-lookup"><span data-stu-id="c3bac-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shared-root-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c3bac-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3bac-157">Response</span></span>

<span data-ttu-id="c3bac-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3bac-158">Here is an example of the response.</span></span>

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

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="c3bac-159">Acessar diretamente o item compartilhado</span><span class="sxs-lookup"><span data-stu-id="c3bac-159">Access the shared item directly</span></span>

<span data-ttu-id="c3bac-p104">Embora [**SharedDriveItem**](../resources/shareddriveitem.md) contenha algumas informações úteis, a maioria dos aplicativos acessará diretamente o [DriveItem](../resources/driveitem.md) compartilhado. O recurso **SharedDriveItem** inclui **root** e relações **itens** que podem acessar o conteúdo no escopo do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="c3bac-p104">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="c3bac-162">Exemplo (arquivo único)</span><span class="sxs-lookup"><span data-stu-id="c3bac-162">Example (single file)</span></span>

### <a name="request"></a><span data-ttu-id="c3bac-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3bac-163">Request</span></span>

<span data-ttu-id="c3bac-164">Ao solicitar a relação **driveItem**, o **DriveItem** compartilhado será retornado.</span><span class="sxs-lookup"><span data-stu-id="c3bac-164">By requesting the **driveItem** relationship, the **DriveItem** that was shared will be returned.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c3bac-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3bac-165">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3bac-166">C#</span><span class="sxs-lookup"><span data-stu-id="c3bac-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-driveitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3bac-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="c3bac-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-driveitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3bac-168">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c3bac-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-driveitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c3bac-169">Java</span><span class="sxs-lookup"><span data-stu-id="c3bac-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shared-driveitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c3bac-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3bac-170">Response</span></span>

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

## <a name="example-shared-folder"></a><span data-ttu-id="c3bac-171">Exemplo (pasta compartilhada)</span><span class="sxs-lookup"><span data-stu-id="c3bac-171">Example (shared folder)</span></span>

### <a name="request"></a><span data-ttu-id="c3bac-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3bac-172">Request</span></span>

<span data-ttu-id="c3bac-173">Solicitando a relação **driveItem** e expandindo a coleção **children**, o **DriveItem** que foi compartilhado será retornado junto com os arquivos da pasta compartilhada.</span><span class="sxs-lookup"><span data-stu-id="c3bac-173">By requesting the **driveItem** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c3bac-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3bac-174">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3bac-175">C#</span><span class="sxs-lookup"><span data-stu-id="c3bac-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-driveitem-expand-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3bac-176">Javascript</span><span class="sxs-lookup"><span data-stu-id="c3bac-176">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-driveitem-expand-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3bac-177">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c3bac-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-driveitem-expand-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c3bac-178">Java</span><span class="sxs-lookup"><span data-stu-id="c3bac-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shared-driveitem-expand-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c3bac-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3bac-179">Response</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="c3bac-180">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="c3bac-180">Error Responses</span></span>

<span data-ttu-id="c3bac-181">Saiba mais sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="c3bac-181">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="remarks"></a><span data-ttu-id="c3bac-182">Comentários</span><span class="sxs-lookup"><span data-stu-id="c3bac-182">Remarks</span></span>

* <span data-ttu-id="c3bac-183">Para o OneDrive for Business e o SharePoint, a API Shares sempre requer autenticação e não pode ser usada para acessar conteúdo compartilhado anonimamente sem um contexto de usuário.</span><span class="sxs-lookup"><span data-stu-id="c3bac-183">For OneDrive for Business and SharePoint, the Shares API always requires authentication and cannot be used to access anonymously shared content without a user context.</span></span>

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
