---
author: JeremyKelley
ms.author: jeremyke
title: Listar pacotes
description: Listar os pacotes na unidade de um usuário
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8a58417be4b582c81c772d045a1bf6867a7d3f9f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419261"
---
# <a name="list-bundles"></a><span data-ttu-id="e7fea-103">Listar pacotes</span><span class="sxs-lookup"><span data-stu-id="e7fea-103">List bundles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7fea-104">Obter uma lista de todos os pacotes de [pacote][] na unidade de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e7fea-104">Get a list of all the [bundles][bundle] in a user's drive.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7fea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7fea-105">Permissions</span></span>

<span data-ttu-id="e7fea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7fea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7fea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7fea-108">Permission type</span></span>      | <span data-ttu-id="e7fea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7fea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7fea-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7fea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e7fea-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7fea-111">Not supported.</span></span>                             |
|<span data-ttu-id="e7fea-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7fea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7fea-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7fea-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e7fea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7fea-114">Application</span></span>          | <span data-ttu-id="e7fea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7fea-115">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="e7fea-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7fea-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/bundles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7fea-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e7fea-117">Optional query parameters</span></span>

<span data-ttu-id="e7fea-118">Esse método dá suporte a [Parâmetros de consulta OData][] para filtrar e dar forma à resposta.</span><span class="sxs-lookup"><span data-stu-id="e7fea-118">This method supports the [OData Query Parameters][] to filter and shape the response.</span></span>

<span data-ttu-id="e7fea-119">Você não pode usar `expand=children` o parâmetro de consulta ao enumerar os pacotes.</span><span class="sxs-lookup"><span data-stu-id="e7fea-119">You can't use the `expand=children` query parameter when enumerating bundles.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7fea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7fea-120">Request headers</span></span>

| <span data-ttu-id="e7fea-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e7fea-121">Name</span></span>          | <span data-ttu-id="e7fea-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7fea-122">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="e7fea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7fea-123">Authorization</span></span> | <span data-ttu-id="e7fea-124">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="e7fea-124">Bearer \{token\}.</span></span> <span data-ttu-id="e7fea-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7fea-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7fea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7fea-126">Request body</span></span>

<span data-ttu-id="e7fea-127">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="e7fea-127">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7fea-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7fea-128">Response</span></span>

<span data-ttu-id="e7fea-129">Se tiver êxito, essa solicitação retornará a lista de itens de pacote definidos para a unidade.</span><span class="sxs-lookup"><span data-stu-id="e7fea-129">If successful, this request returns the list of bundle items defined for the drive.</span></span>

<span data-ttu-id="e7fea-130">Leia o tópico [respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="e7fea-130">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="e7fea-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e7fea-131">Examples</span></span>

### <a name="example-1-list-all-bundles-in-a-drive"></a><span data-ttu-id="e7fea-132">Exemplo 1: listar todos os pacotes em uma unidade</span><span class="sxs-lookup"><span data-stu-id="e7fea-132">Example 1: List all bundles in a drive</span></span>

<span data-ttu-id="e7fea-133">Para solicitar uma enumeração de todos os pacotes definidos na unidade, você pode fazer uma solicitação para a coleção de **pacotes** sem qualquer parâmetro.</span><span class="sxs-lookup"><span data-stu-id="e7fea-133">To request an enumeration of all bundles defined in the drive, you can make a request to the **bundles** collection without any parameters.</span></span>

#### <a name="request"></a><span data-ttu-id="e7fea-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7fea-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e7fea-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7fea-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-all-bundles", "tags": "service.onedrive" } -->

```http
GET https://graph.microsoft.com/beta/drive/bundles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7fea-136">C#</span><span class="sxs-lookup"><span data-stu-id="e7fea-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-all-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7fea-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7fea-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-all-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7fea-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e7fea-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-all-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e7fea-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7fea-139">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true, "isCollection": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0123456789abc",
      "name": "Vacation photo album",
      "bundle": {
        "childCount": 1,
        "album": { }
      }
    },
    {
      "id": "0120310201abd",
      "name": "Family shared files",
      "bundle": {
        "childCount": 1
      }
    }
  ],
  "@odata.nextLink": "https://..."
}
```

<span data-ttu-id="e7fea-140">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e7fea-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e7fea-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7fea-141">All the properties will be returned from an actual call.</span></span>


### <a name="example-2-list-all-photo-albums-in-a-drive"></a><span data-ttu-id="e7fea-142">Exemplo 2: listar todos os álbuns de fotos em uma unidade</span><span class="sxs-lookup"><span data-stu-id="e7fea-142">Example 2: List all photo albums in a drive</span></span>

<span data-ttu-id="e7fea-143">Para filtrar a lista de pacotes retornados de uma solicitação para a coleção de pacotes, você pode usar o `filter` parâmetro de cadeia de caracteres de consulta para especificar o tipo de pacote a ser retornado verificando a existência de uma faceta no pacote:</span><span class="sxs-lookup"><span data-stu-id="e7fea-143">To filter the list of bundles returned from a request to the bundles collection, you can use the `filter` query string parameter to specify the type of bundle to return by checking for the existence of a facet on the bundle:</span></span>

#### <a name="request"></a><span data-ttu-id="e7fea-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7fea-144">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e7fea-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7fea-145">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "list-album-bundles", "tags": "service.onedrive" } -->

```http
GET https://graph.microsoft.com/beta/drive/bundles?filter=bundle/album%20ne%20null
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7fea-146">C#</span><span class="sxs-lookup"><span data-stu-id="e7fea-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-album-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7fea-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7fea-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-album-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7fea-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e7fea-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-album-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e7fea-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7fea-149">Response</span></span>

<span data-ttu-id="e7fea-150">A resposta para um GET para o ponto de extremidade de pacotes é uma matriz de recursos do [driveItem][] com o [pacote][].</span><span class="sxs-lookup"><span data-stu-id="e7fea-150">The response to a GET to the bundles endpoint is an array of [driveItem][] resources with the [bundle][].</span></span>
<span data-ttu-id="e7fea-151">Como todos os pacotes são itens, você pode usar todas as operações de item padrão neles.</span><span class="sxs-lookup"><span data-stu-id="e7fea-151">Because all bundles are items, you can use use all the standard item operations on them.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true, "isCollection": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0123456789abc",
      "name": "Vacation photo album",
      "bundle": {
        "childCount": 1,
        "album": { }
      }
    },
    {
      "id": "120301010abcd",
      "name": "Seattle Center event",
      "bundle": {
        "childCount": 4,
        "album": { }
      },
      "tags": [
        {
          "name": "outside",
          "autoTagged": { }
        }
      ]
    }
  ]
}
```

<span data-ttu-id="e7fea-152">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e7fea-152">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e7fea-153">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7fea-153">All the properties will be returned from an actual call.</span></span>


[pacote]: ../resources/bundle.md
[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors
[Parâmetros de consulta OData]: /graph/query-parameters
[OData Query Parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "List the bundles in a drive.",
  "keywords": "list,bundle,collection",
  "section": "documentation",
  "tocPath": "Bundles/List"
} -->
