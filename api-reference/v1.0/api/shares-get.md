---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Acessar itens compartilhados
localization_priority: Normal
description: Acesse um DriveItem compartilhado ou uma coleção de itens compartilhados usando um shareId ou uma URL de compartilhamento.
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: f8ca26b4e226212186f3e2716b5d4ff4c250b44f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013031"
---
# <a name="accessing-shared-driveitems"></a><span data-ttu-id="46f1e-103">Acessar DriveItems compartilhados</span><span class="sxs-lookup"><span data-stu-id="46f1e-103">Accessing shared DriveItems</span></span>

<span data-ttu-id="46f1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46f1e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="46f1e-105">Acesse um [DriveItem](../resources/driveitem.md) compartilhado ou uma coleção de itens compartilhados usando um **shareId** ou uma URL de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="46f1e-105">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="46f1e-106">Para usar uma URL de compartilhamento com esta API, seu aplicativo precisa [transformar a URL em um token de compartilhamento](#encoding-sharing-urls).</span><span class="sxs-lookup"><span data-stu-id="46f1e-106">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#encoding-sharing-urls).</span></span>

## <a name="permissions"></a><span data-ttu-id="46f1e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="46f1e-107">Permissions</span></span>

<span data-ttu-id="46f1e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46f1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46f1e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46f1e-110">Permission type</span></span>      | <span data-ttu-id="46f1e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46f1e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46f1e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46f1e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="46f1e-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46f1e-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="46f1e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46f1e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46f1e-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46f1e-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="46f1e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46f1e-116">Application</span></span> | <span data-ttu-id="46f1e-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46f1e-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46f1e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46f1e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a><span data-ttu-id="46f1e-119">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="46f1e-119">Path parameters</span></span>

| <span data-ttu-id="46f1e-120">Nome do Parâmetro</span><span class="sxs-lookup"><span data-stu-id="46f1e-120">Parameter Name</span></span>                 | <span data-ttu-id="46f1e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="46f1e-121">Value</span></span>    | <span data-ttu-id="46f1e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="46f1e-122">Description</span></span>                                                                         |
|:-------------------------------|:---------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="46f1e-123">**shareIdOrEncodedSharingUrl**</span><span class="sxs-lookup"><span data-stu-id="46f1e-123">**shareIdOrEncodedSharingUrl**</span></span> | `string` | <span data-ttu-id="46f1e-p102">Obrigatório. Um token de compartilhamento retornado pela API ou uma URL de compartilhamento corretamente codificada.</span><span class="sxs-lookup"><span data-stu-id="46f1e-p102">Required. A sharing token as returned by the API or a properly encoded sharing URL.</span></span> |

### <a name="encoding-sharing-urls"></a><span data-ttu-id="46f1e-126">Codificação de URLs de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="46f1e-126">Encoding sharing URLs</span></span>

<span data-ttu-id="46f1e-127">Para codificar uma URL de compartilhamento, use a seguinte lógica:</span><span class="sxs-lookup"><span data-stu-id="46f1e-127">To encode a sharing URL, use the following logic:</span></span>

1. <span data-ttu-id="46f1e-128">Primeiro, use base64 para codificar a URL.</span><span class="sxs-lookup"><span data-stu-id="46f1e-128">First, use base64 encode the URL.</span></span>
2. <span data-ttu-id="46f1e-129">Converta o resultado codificado na base64 para o [formato base64url sem preenchimento](https://en.wikipedia.org/wiki/Base64) removendo caracteres `=` do final do valor, substituindo `/` por `_` e `+` por `-`.)</span><span class="sxs-lookup"><span data-stu-id="46f1e-129">Convert the base64 encoded result to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by removing `=` characters from the end of the value, replacing `/` with `_` and `+` with `-`.)</span></span>
3. <span data-ttu-id="46f1e-130">Acrescente `u!` ao início da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="46f1e-130">Append `u!` to be beginning of the string.</span></span>

<span data-ttu-id="46f1e-131">Por exemplo, para codificar uma URL em C#:</span><span class="sxs-lookup"><span data-stu-id="46f1e-131">As an example, to encode a URL in C#:</span></span>

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="optional-request-headers"></a><span data-ttu-id="46f1e-132">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="46f1e-132">Optional request headers</span></span>

| <span data-ttu-id="46f1e-133">Nome</span><span class="sxs-lookup"><span data-stu-id="46f1e-133">Name</span></span>       | <span data-ttu-id="46f1e-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="46f1e-134">Type</span></span>   | <span data-ttu-id="46f1e-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="46f1e-135">Description</span></span>                                                    |
|:-----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="46f1e-136">**Prefer**</span><span class="sxs-lookup"><span data-stu-id="46f1e-136">**Prefer**</span></span> | <span data-ttu-id="46f1e-137">string</span><span class="sxs-lookup"><span data-stu-id="46f1e-137">string</span></span> | <span data-ttu-id="46f1e-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="46f1e-138">Optional.</span></span> <span data-ttu-id="46f1e-139">Defina como um dos `prefer` valores documentados abaixo.</span><span class="sxs-lookup"><span data-stu-id="46f1e-139">Set to one of the `prefer` values documented below.</span></span>  |

### <a name="prefer-header-values"></a><span data-ttu-id="46f1e-140">Preferir valores de cabeçalho</span><span class="sxs-lookup"><span data-stu-id="46f1e-140">Prefer header values</span></span>

| <span data-ttu-id="46f1e-141">Nome</span><span class="sxs-lookup"><span data-stu-id="46f1e-141">Name</span></span>                          | <span data-ttu-id="46f1e-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="46f1e-142">Description</span></span>                                                                                             |
|:------------------------------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="46f1e-143">redeemSharingLink</span><span class="sxs-lookup"><span data-stu-id="46f1e-143">redeemSharingLink</span></span>             | <span data-ttu-id="46f1e-144">Se o **shareIdOrEncodedSharingUrl** for um link de compartilhamento, conceda ao chamador acesso durável ao item</span><span class="sxs-lookup"><span data-stu-id="46f1e-144">If the **shareIdOrEncodedSharingUrl** is a sharing link, grant the caller durable access to the item</span></span>    |
| <span data-ttu-id="46f1e-145">redeemSharingLinkIfNecessary</span><span class="sxs-lookup"><span data-stu-id="46f1e-145">redeemSharingLinkIfNecessary</span></span>  | <span data-ttu-id="46f1e-146">O mesmo que redeemSharingLink, mas o acesso só é garantido para a duração da solicitação</span><span class="sxs-lookup"><span data-stu-id="46f1e-146">Same as redeemSharingLink, but access is only guaranteed to be granted for the duration of this request</span></span> |

<span data-ttu-id="46f1e-147">redeemSharingLink deve ser considerado equivalente ao chamador navegando para o link de compartilhamento do navegador (aceitando o gesto de compartilhamento), enquanto o redeemSharingLinkIfNecessary se destina a cenários em que a intenção é simplesmente inspecionar os metadados do link.</span><span class="sxs-lookup"><span data-stu-id="46f1e-147">redeemSharingLink should be considered equivalent to the caller navigating to the sharing link the browser (accepting the sharing gesture), whereas redeemSharingLinkIfNecessary is intended for scenarios where the intention is simply to peek at the link's metadata.</span></span>

## <a name="response"></a><span data-ttu-id="46f1e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="46f1e-148">Response</span></span>

<span data-ttu-id="46f1e-149">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [sharedDriveItem](../resources/shareddriveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46f1e-149">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46f1e-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46f1e-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="46f1e-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46f1e-151">Request</span></span>

<span data-ttu-id="46f1e-152">Veja a seguir um exemplo da solicitação para recuperar um item compartilhado:</span><span class="sxs-lookup"><span data-stu-id="46f1e-152">Here is an example of the request to retrieve a shared item:</span></span>


# <a name="http"></a>[<span data-ttu-id="46f1e-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="46f1e-153">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-root" } -->

```msgraph-interactive
GET /shares/{shareIdOrEncodedSharingUrl}
```
# <a name="c"></a>[<span data-ttu-id="46f1e-154">C#</span><span class="sxs-lookup"><span data-stu-id="46f1e-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46f1e-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46f1e-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46f1e-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46f1e-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46f1e-157">Java</span><span class="sxs-lookup"><span data-stu-id="46f1e-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shared-root-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="46f1e-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="46f1e-158">Response</span></span>

<span data-ttu-id="46f1e-159">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46f1e-159">Here is an example of the response.</span></span>

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

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="46f1e-160">Acessar diretamente o item compartilhado</span><span class="sxs-lookup"><span data-stu-id="46f1e-160">Access the shared item directly</span></span>

<span data-ttu-id="46f1e-p104">Embora [**SharedDriveItem**](../resources/shareddriveitem.md) contenha algumas informações úteis, a maioria dos aplicativos acessará diretamente o [DriveItem](../resources/driveitem.md) compartilhado. O recurso **SharedDriveItem** inclui **root** e relações **itens** que podem acessar o conteúdo no escopo do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="46f1e-p104">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="46f1e-163">Exemplo (arquivo único)</span><span class="sxs-lookup"><span data-stu-id="46f1e-163">Example (single file)</span></span>

### <a name="request"></a><span data-ttu-id="46f1e-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46f1e-164">Request</span></span>

<span data-ttu-id="46f1e-165">Ao solicitar a relação **driveItem**, o **DriveItem** compartilhado será retornado.</span><span class="sxs-lookup"><span data-stu-id="46f1e-165">By requesting the **driveItem** relationship, the **DriveItem** that was shared will be returned.</span></span>


# <a name="http"></a>[<span data-ttu-id="46f1e-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="46f1e-166">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```msgraph-interactive
GET /shares/{shareIdOrUrl}/driveItem
```
# <a name="c"></a>[<span data-ttu-id="46f1e-167">C#</span><span class="sxs-lookup"><span data-stu-id="46f1e-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-driveitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46f1e-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46f1e-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-driveitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46f1e-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46f1e-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-driveitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46f1e-170">Java</span><span class="sxs-lookup"><span data-stu-id="46f1e-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shared-driveitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="46f1e-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="46f1e-171">Response</span></span>

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

## <a name="example-shared-folder"></a><span data-ttu-id="46f1e-172">Exemplo (pasta compartilhada)</span><span class="sxs-lookup"><span data-stu-id="46f1e-172">Example (shared folder)</span></span>

### <a name="request"></a><span data-ttu-id="46f1e-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46f1e-173">Request</span></span>

<span data-ttu-id="46f1e-174">Solicitando a relação **driveItem** e expandindo a coleção **children**, o **DriveItem** que foi compartilhado será retornado junto com os arquivos da pasta compartilhada.</span><span class="sxs-lookup"><span data-stu-id="46f1e-174">By requesting the **driveItem** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>


# <a name="http"></a>[<span data-ttu-id="46f1e-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="46f1e-175">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```msgraph-interactive
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```
# <a name="c"></a>[<span data-ttu-id="46f1e-176">C#</span><span class="sxs-lookup"><span data-stu-id="46f1e-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-driveitem-expand-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46f1e-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46f1e-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-driveitem-expand-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46f1e-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46f1e-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-driveitem-expand-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46f1e-179">Java</span><span class="sxs-lookup"><span data-stu-id="46f1e-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shared-driveitem-expand-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="46f1e-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="46f1e-180">Response</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="46f1e-181">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="46f1e-181">Error Responses</span></span>

<span data-ttu-id="46f1e-182">Veja mais informações sobre como os erros são retornados no tópico [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="46f1e-182">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="remarks"></a><span data-ttu-id="46f1e-183">Comentários</span><span class="sxs-lookup"><span data-stu-id="46f1e-183">Remarks</span></span>

* <span data-ttu-id="46f1e-184">Para o OneDrive for Business e o SharePoint, a API Shares sempre requer autenticação e não pode ser usada para acessar conteúdo compartilhado anonimamente sem um contexto de usuário.</span><span class="sxs-lookup"><span data-stu-id="46f1e-184">For OneDrive for Business and SharePoint, the Shares API always requires authentication and cannot be used to access anonymously shared content without a user context.</span></span>

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

