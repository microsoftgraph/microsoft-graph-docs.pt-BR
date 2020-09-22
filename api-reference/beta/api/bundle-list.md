---
author: JeremyKelley
ms.author: jeremyke
title: Listar pacotes
description: Listar os pacotes na unidade de um usuário
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: dac031d7bd14cf72932248341740989881529cb2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987740"
---
# <a name="list-bundles"></a><span data-ttu-id="10bab-103">Listar pacotes</span><span class="sxs-lookup"><span data-stu-id="10bab-103">List bundles</span></span>

<span data-ttu-id="10bab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10bab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10bab-105">Obter uma lista de todos os pacotes de [pacote][na unidade] de um usuário.</span><span class="sxs-lookup"><span data-stu-id="10bab-105">Get a list of all the [bundles][bundle] in a user's drive.</span></span>

## <a name="permissions"></a><span data-ttu-id="10bab-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="10bab-106">Permissions</span></span>

<span data-ttu-id="10bab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10bab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10bab-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10bab-109">Permission type</span></span>      | <span data-ttu-id="10bab-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10bab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10bab-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10bab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="10bab-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10bab-112">Not supported.</span></span>                             |
|<span data-ttu-id="10bab-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10bab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10bab-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10bab-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="10bab-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10bab-115">Application</span></span>          | <span data-ttu-id="10bab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10bab-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="10bab-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10bab-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/bundles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10bab-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="10bab-118">Optional query parameters</span></span>

<span data-ttu-id="10bab-119">Esse método dá suporte a [Parâmetros de consulta OData][] para filtrar e dar forma à resposta.</span><span class="sxs-lookup"><span data-stu-id="10bab-119">This method supports the [OData Query Parameters][] to filter and shape the response.</span></span>

<span data-ttu-id="10bab-120">Você não pode usar o `expand=children` parâmetro de consulta ao enumerar os pacotes.</span><span class="sxs-lookup"><span data-stu-id="10bab-120">You can't use the `expand=children` query parameter when enumerating bundles.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10bab-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10bab-121">Request headers</span></span>

| <span data-ttu-id="10bab-122">Nome</span><span class="sxs-lookup"><span data-stu-id="10bab-122">Name</span></span>          | <span data-ttu-id="10bab-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="10bab-123">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="10bab-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="10bab-124">Authorization</span></span> | <span data-ttu-id="10bab-125">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="10bab-125">Bearer \{token\}.</span></span> <span data-ttu-id="10bab-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10bab-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10bab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10bab-127">Request body</span></span>

<span data-ttu-id="10bab-128">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="10bab-128">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="10bab-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="10bab-129">Response</span></span>

<span data-ttu-id="10bab-130">Se tiver êxito, essa solicitação retornará a lista de itens de pacote definidos para a unidade.</span><span class="sxs-lookup"><span data-stu-id="10bab-130">If successful, this request returns the list of bundle items defined for the drive.</span></span>

<span data-ttu-id="10bab-131">Leia o tópico [respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="10bab-131">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="10bab-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="10bab-132">Examples</span></span>

### <a name="example-1-list-all-bundles-in-a-drive"></a><span data-ttu-id="10bab-133">Exemplo 1: listar todos os pacotes em uma unidade</span><span class="sxs-lookup"><span data-stu-id="10bab-133">Example 1: List all bundles in a drive</span></span>

<span data-ttu-id="10bab-134">Para solicitar uma enumeração de todos os pacotes definidos na unidade, você pode fazer uma solicitação para a coleção de **pacotes** sem qualquer parâmetro.</span><span class="sxs-lookup"><span data-stu-id="10bab-134">To request an enumeration of all bundles defined in the drive, you can make a request to the **bundles** collection without any parameters.</span></span>

#### <a name="request"></a><span data-ttu-id="10bab-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10bab-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="10bab-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="10bab-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-all-bundles", "tags": "service.onedrive" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles
```
# <a name="c"></a>[<span data-ttu-id="10bab-137">C#</span><span class="sxs-lookup"><span data-stu-id="10bab-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-all-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10bab-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10bab-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-all-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10bab-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10bab-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-all-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="10bab-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="10bab-140">Response</span></span>

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

<span data-ttu-id="10bab-141">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="10bab-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="10bab-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10bab-142">All the properties will be returned from an actual call.</span></span>


### <a name="example-2-list-all-photo-albums-in-a-drive"></a><span data-ttu-id="10bab-143">Exemplo 2: listar todos os álbuns de fotos em uma unidade</span><span class="sxs-lookup"><span data-stu-id="10bab-143">Example 2: List all photo albums in a drive</span></span>

<span data-ttu-id="10bab-144">Para filtrar a lista de pacotes retornados de uma solicitação para a coleção de pacotes, você pode usar o `filter` parâmetro de cadeia de caracteres de consulta para especificar o tipo de pacote a ser retornado verificando a existência de uma faceta no pacote:</span><span class="sxs-lookup"><span data-stu-id="10bab-144">To filter the list of bundles returned from a request to the bundles collection, you can use the `filter` query string parameter to specify the type of bundle to return by checking for the existence of a facet on the bundle:</span></span>

#### <a name="request"></a><span data-ttu-id="10bab-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10bab-145">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="10bab-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="10bab-146">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "list-album-bundles", "tags": "service.onedrive" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles?filter=bundle/album%20ne%20null
```
# <a name="c"></a>[<span data-ttu-id="10bab-147">C#</span><span class="sxs-lookup"><span data-stu-id="10bab-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-album-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10bab-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10bab-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-album-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10bab-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10bab-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-album-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="10bab-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="10bab-150">Response</span></span>

<span data-ttu-id="10bab-151">A resposta para um GET para o ponto de extremidade de pacotes é uma matriz de recursos do [driveItem][] com o [pacote][].</span><span class="sxs-lookup"><span data-stu-id="10bab-151">The response to a GET to the bundles endpoint is an array of [driveItem][] resources with the [bundle][].</span></span>
<span data-ttu-id="10bab-152">Como todos os pacotes são itens, você pode usar todas as operações de item padrão neles.</span><span class="sxs-lookup"><span data-stu-id="10bab-152">Because all bundles are items, you can use use all the standard item operations on them.</span></span>

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

<span data-ttu-id="10bab-153">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="10bab-153">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="10bab-154">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10bab-154">All the properties will be returned from an actual call.</span></span>


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


